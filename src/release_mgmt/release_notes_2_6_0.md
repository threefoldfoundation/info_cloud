
 # ThreeFold Cloud 2.6


## JS-SDK v11.4.0

### Component Upgrades
- [3Bot Deployer](https://github.com/threefoldtech/js-sdk/tree/development/jumpscale/packages/threebot_deployer)
- [Solution Marketplace](https://github.com/threefoldtech/js-sdk/tree/development/jumpscale/packages/marketplace)
- [Virtual Datacenter VDC](https://github.com/threefoldtech/js-sdk/tree/development/jumpscale/packages/vdc)

#### VDC v2.6.0 
- VDC Backup feature: manual and auto back up, enable switching between back ups.
- Auto rediirect to VDC solution deployment page via Marketplace website
- Auto balance-check feature before deploying vdc to ensure sufficient tokens
- Added user notification for new vdc updates
- Reenabled external etcd usage for VDC
- Allow VDC Deployment using chosen farm
- Transaction fee reduction to 0.01 TFT
- Payment: Added Transaction History page
- Payment: Added Wallet QR Scan for balance top up
- Marketplace solution: Presearch node deployment improvement
- Marketplace solution: Taiga SSO using TF Connect Authentication
- Marketplace solution: Discourse SSO using TF Connect Authentication
- Marketplace solution: Added Matic (Full/Sentry Node) solution deployment

#### 3Bot SDK v2.6.0
- New chatflows on network management and capacity pool
- Farm management custom prices support
- New Kubernetes support for public IPs
- More sizes support for Kubernetes deployment
- Email notification for expiring pools empty wallets
- Rebranded 3Bot Marketplace as 3Bot Apps

## Quantum FileSystem (QSFS) V0.2.0

### Component Upgrades
- [0-DB](https://github.com/threefoldtech/0-db)
- [0-DB-FS](https://github.com/threefoldtech/0-db-fs)
- [0-Stor](https://github.com/threefoldtech/0-stor)


### New on QSFS V0.2.0

- Integrated etcd redundant backend
- Time-based upload using z-stor for all storage containers
- Support index dirty detection in 0-DB
- Upload changed (dirty) index, use ETCD to keep required metadata
- Multi level ZDB stor to support millions of backend files
- Retreive and Restore: easily recreate and restore data by retreiving it as metadata stor 
- Added rust-based monitoring / repair tool to check backend health and prevent data loss

### 0-stor Gen2 v0.2
- Use build time optimization to reduce the size of the final binaries
- Implement real error types, improving feedback to users
- Better handling of some code paths
- Test connectivity to the metadata cluster before starting
- Add a Test subcommand to verify the configuration file, metadata cluster connectivity, and 0-db backend connectivity
- Zstor.log. :Add a logfile for operations.
- Verify 0-db namespace for sufficient capacity before writing and sharding attempt
- Support unhealthy backends when writing

## ZOS 0.5.0
- added ZOS capacity collecting and reporting feature
- Made ZOS do flist cache periodic clean up
- added optional Yggdrasil ip inside ZOS containers
- Periodical billing info handling
- Support small memory containers (100MB)

## Digital Twin v0.2.0 (Demo)
- Full chat and messaging features: Add gifs, block contact, send files
- Responsive Mobile layout
- TF connect SSO for quick sign up
- Integrated meeting feature (video chat feature)
- Integrated File manager (file cloud and storage)
- Decentralized and private connection with Planetary network on the backend
- Full redesign with Modern ThreeFold Branding
