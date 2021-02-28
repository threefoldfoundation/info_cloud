![](img/planet_fs.png)

# ThreeFold Planetary Secure File System (PSFS)

Part of the VDC is a set of Storage Nodes, which can be used as storage infrastructure for files in any format. 

## Mount Any Files in your Storage Infrastructure

The Planetary Secure Filesystem is a mechanism to mount any file system (in any format) on the grid, in a quantum-secure way. 

This storage layer relies relies on 3 primitives of the ThreeFold technology : 

- [0-db](https://github.com/threefoldtech/0-db) is the storage engine.
It is an always append database, which stores objects in an immutable format. It allows to
have history out-of-the-box, good performance on disk, low overhead, easy data structure and easy backup (linear copy and immutable files).

- [0-stor-v2](https://github.com/threefoldtech/0-stor_v2) is used to disperse the data into chunks by performing 'forward looking error correcting code' (FLECC) on it and send the chunks to a safe location.
It takes files in any format as input, encrypts this file with AES based on a user-defined key, then FLECC-encodes the file and spreads out the result
to multiple 0-dbs. The number of generated chunks is configurable, to make it more or less robust against loss of data through unavailable chunks. Even if some 0-dbs are unreachable, the original data can still
retrieved and missing 0-dbs can even be rebuilt to keep full consistency. It's an essential element of the operational backup. 

- [0-db-fs](https://github.com/threefoldtech/0-db-fs) is the filesystem driver which uses 0-db as primary storage engine. It manages the storage of directories and metadata in a dedicated namespace, and file payloads in another dedicated namespace.

Together they form a storage layer which is quantum secure: even the most powerful computer can't hack the system, because no single node contains all of the information needed to reconstruct the data.

![](img/quantum_safe_storage.png)

This concept scales forever, and any file system can be brought on top of it: 
- S3 storage 
- any backup system
- an ftp-server
- IPFS and Hypercore distributed file sharing protocols 
- ...

![](img/quantum_safe_storage_scale.png)

## Try it Out

### Intro

There is currently a demo of the Planetary Secure File System available, which uses the storage nodes of a ThreeFold VDC to back data up to the ThreeFold Grid. Below you'll find instructions for using a bootstrap executable file that runs on Linux or in a Linux Docker container to set up the complete environment necessary to use the file system. 

Please note that this solution is currently for testing only and some important features are still under development.

### VDC and Z-Stor Config

If you haven't already, go ahead and [deploy a VDC](evdc_deploy). Then download the Z-Stor config file, found in the upper right corner of the `VDC Storage Nodes` screen. Unless you know that IPv6 works on your machine and within Docker, choose the IPv4 version of the file.

![](img/planetaryfs_zdbconfig.png)

As described in [Manage Storage Nodes](evdc_storage), this file contains the necessary information to connect with the 0-dbs running on the storage nodes in your VDC. It also contains an encryption key used to encrypt data that's uploaded as well as a field to specify your etcd endpoints. Using the defaults here is fine.

### Bootstrap Executable

Download now the Planetary FileSystem bootstrap, available [here](https://github.com/threefoldtech/quantum-storage/releases/download/v0.0.1/planetaryfs-bootstrap-linux-amd64).


> __Remark__: 
For now, the bootstrap executable is only available for Linux. We'll cover how to use it within an Ubuntu container in Docker, which will also work on MacOS.

First, we'll start an Ubuntu container with Docker, enabling fuse file system capabilities. In a terminal window, 

`docker run -it --name zdbfs --cap-add SYS_ADMIN --device /dev/fuse ubuntu:20.04`

Next, we'll copy the Z-Stor config file and the bootstrap executable into the running container. In a separate terminal window, navigate to where you downloaded the files and run:

`docker cp planetaryfs-bootstrap-linux-amd64 zdbfs:/root/`
`docker cp <yourzstorconfig.toml> zdbfs:/root/`

Back in the container's terminal window, `cd /root` and confirm that the two files are there with `ls`. Then run the bootstrap executable, specifying your config file:

`chmod u+x planetaryfs-bootstrap-linux-amd64`
`./planetaryfs-bootstrap-linux-amd64 <yourzstorconfig.toml>`

Execution of this bootstrap will start up all necessary components and show you that the back-end is ready for dispersing the data.

![](img/planetaryfs_bootstrap_ready.png)

After that, your Planetary Secure File System will be mounted at `/root/.threefold/mnt/zdbfs`. Files copied there will automatically be stored on the Grid incrementally as chunks of a certain size are filled, by default 32Mb. In a future release, this will no longer be a limitation.

