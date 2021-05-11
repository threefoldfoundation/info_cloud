
 # ThreeFold Cloud 2.7.1
 
Live on testnet - April 2, 2021.

## JS-SDK v11.2.1

### Component Upgrades
- [3Bot Deployer](https://github.com/threefoldtech/js-sdk/tree/development/jumpscale/packages/threebot_deployer)
- [Solution Marketplace](https://github.com/threefoldtech/js-sdk/tree/development/jumpscale/packages/marketplace)
- [Virtual Datacenter VDC](https://github.com/threefoldtech/js-sdk/tree/development/jumpscale/packages/vdc)

#### VDC v2.7.1


#### 3Bot SDK v2.6.0


### New on QSFS V0.4.0

- Add support for Etcd as metadata backend
- Time-based upload using z-stor for all storage containers
- Support index dirty detection in 0-DB
- Upload changed (dirty) index, use ETCD to keep required metadata
- Multi level ZDB stor to support millions of backend files
- Retrieve and restore: esily recreate and restore data by retrieving it from the metadata store
- Added rust-based monitoring / repair tool to check backend health and prevent data loss

### 0-stor-v2 v0.2
- Use build time optimization to reduce the size of the final binaries
- Implement real error types, improving feedback to users
- Better handling of some code paths
- Test connectivity to the metadata cluster before starting
- Added a Test subcommand to verify the configuration file, metadata cluster connectivity, and 0-DB backend connectivity
- Zstor.log. : Add a logfile for operations.
- Verified 0-DB namespace for sufficient capacity before writing and sharding attempt
- Support unhealthy backends when writing

## ZOS 0.4.10
- Made ZOS do flist cache periodic clean up
- Support small memory containers (100MB)
- Replaced Firecracker to Cloud-hypervisor for virtualization
- Support new k8s special size
- Fixed CPU limits on container
- Upgraded the 0-db's running on the grid
- Add support for creating and using macVtap interfaces for public traffic on vms
- Disable COW on vm disk backends
- Better VM cleanup
