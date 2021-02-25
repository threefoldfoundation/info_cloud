![](img/planet_fs.png)

# ThreeFold Planetary Filesystem

Part of the VDC is a set of Storage Nodes, which can be used as storage infrastructure for your Planetary Filesystem. 

## Mount Any Storage Anywhere

The Planetary Filesystem is a mechanism to mount any file system (in any format) on the grid. 
It is currently available as a Docker file, and is meant to be integrated into the workload you run in the Kubernetes cluster. 
The Planetary Filesystem relies relies on 3 primitives of the ThreeFold technology : 

- [0-db](https://github.com/threefoldtech/0-db) is the storage engine.
It is an always append database, which stores objects in an immutable format. It allows to
have history out-of-the-box, good performance on disk, low overhead, easy data structure and easy backup (linear copy and immutable files).

- [0-stor-v2](https://github.com/threefoldtech/0-stor_v2) is used to disperse the data into chunks by performing 'forward looking error correcting code' (FLECC) on it and send the chunks to a safe location.
It takes files in any format as input, encrypts this file in AES based on a key user-defined, then FLECC-encodes the file and spreads out the result
to multiple 0-db's. The number of generated chunks is configurable, to make it more or less robust against loss of data through unavailable chunks. Even if some 0-db's are unreachable, the original data can still
retrieved and missing 0-db's can even be rebuilt to keep full consistency. It's an essential element of the operational backup. 

- [0-db-fs](https://github.com/threefoldtech/0-db-fs) is the filesystem driver which uses 0-db as primary storage engine.  It manages the storage of directories and metadata in a dedicated namespace, and file payloads in another dedicated namespace.


## Getting Started

### Back-up your Local Machine

Please find below a walkthrough on how to use the Planetary File System to backup your local machine on the ThreeFold Grid. 

First download the ZDB config file. This file can be found in the upper right corner of the `VDC Storage Nodes` screen. 2 configurations are available: an IPv4 and an IPv6 version. 

![](img/planetaryfs_zdbconfig.png)

Then download the Quantum Storage container onto your local machine, through the following instructions on your terminal: 

`git clone https://github.com/threefoldtech/quantum-storage.git`
`docker build -t tf/quantum .`

This will download, compile and prepare all what is needed to get a working container. 

> Remark: On MacOS only a configuration with IPv4 and on Docker is available. On Ubuntu both IPv4 and IPv6 configurations are supported. 

For running the container, execute the following command :

`docker run --rm -it --device /dev/fuse --cap-add CAP_SYS_ADMIN tf/quantum`

For MacOS users and if port forwarding needed, execute : 

`docker run --rm -it --device /dev/fuse --cap-add CAP_SYS_ADMIN -p 9000:9000 tf/quantum`

As soon as the container is up and running, you can reach it via it's IP. In-built is also a Minio interface, on port 9000. 

A UI for Minio S3 storage is available on the provided IP address. 

![](img/planetaryfs_minio_ui.png)

