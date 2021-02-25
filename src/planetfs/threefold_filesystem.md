![](img/planet_fs.png)

# ThreeFold Planetary Filesystem

## Mount Any Storage Anywhere

The Planetary Filesystem is a mechanism to mount any file system anywhere on the grid. 
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

> To Do !