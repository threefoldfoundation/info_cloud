
 # ThreeFold Products and Services 2.7.1
 
Live on testnet - May 17, 2021.

Including upgrades on:
- **JS-SDK v11.4** = Component upgrades for products:
   - [3Bot Deployer](https://github.com/threefoldtech/js-sdk/tree/development/jumpscale/packages/threebot_deployer)
   - [Solution Marketplace](https://github.com/threefoldtech/js-sdk/tree/development/jumpscale/packages/marketplace)
   - [Virtual Datacenter VDC](https://github.com/threefoldtech/js-sdk/tree/development/jumpscale/packages/vdc)
   - [3Bot SDK](https://github.com/threefoldtech/js-sdk/tree/development/jumpscale/packages/tfgrid_solutions)
- **Service Grid v2.7.1** = Lower level component upgrades
- **ThreeFold Connect App v2.7.0** = ThreeFold's mobile authenticator, wallet, news and support app
- **ThreeFold Token v2.7.1** = Service Improvements related to ThreeFold Token

## ThreeFold Cloud 2.7.1
 
### JS-SDK v11.2.1

#### VDC v2.7.1
- Simplified backup and restore mechanism by clicking 'restore' on just one backup item
- Added 'VDC Alerts' on the VDC Dashboard for notifications
- Added services in vdc deployer to check the health of VDC:  containers health, IPs availability, and IPV4 units
- Added eVDC API: Rest based API which containing all features executable via VDC UI
- Enables backup status info on the VDC API
- Added OpenAPI support for vdc Controller
- Allows choosing SSD/HDD for ZDB nodes addons in the chatflow, with eVDC API
- Improved user's email notification system
- Enables soft-delete on VDC Deployer
- Removed fixed price on add-ons worker nodes
- Re-enabled adding worker nodes with public IPs in chatflow and the rest API
- Removed workload deployments on access nodes except for networks
- Enabled Namespace and workload cleanup after a failed deployment
- Improved Node Deployment Capacity Allocation mechanism
- Improved user interactions auditing mechanism on VDC deployer and on VDC controller 
- Enables compute farms configuration
- Improved error messages on deployment failures.

#### 3Bot SDK v2.7.1
- Allows exporting the 3Bot configurations 
- Allows exporting 3Bot logs/alerts from the system


## Service Grid v2.7.1

Live on testnet - May 17, 2021.

### ZOS v0.5.0
- Fixed bugs related to CPU limit for containers
- Replaced Firecracker to Cloud-hypervisor
- Cleaned up stale VMs
- Updated 0-DB to its latest version
- Updated various ZOS basic services to its latest version
- Better memory capacity planning to improve node stability against workload overload
- Exposed node exporter for both testnet and devnet.
- Protected 0-FS processes against OOM
- Overall system stability improvement
- Various bug fixes 

### 0-DB-FS v0.1.4
- Fixed bugs related to incorrectly parsed fuse argument
- Enables fully static binary build
- Enables backtrace when zdbfs crash
- Prepared improvements regarding database header blocks

## ThreeFold Connect App v2.7.1

Live on production - May 17, 2021.

- Implemented TFT Vesting feature
- Implemented BTC deposit, withdrawal and transfer feature
- Implemented the option to Buy TFT with BTC 
- Improvements and bug fixes throughout the app

## ThreeFold Token v2.7.1

Live on production - May 17, 2021.

- TFT implemented as a cross-chain asset (BToken) on the [Binance Smart Chain (BSC)](https://www.binance.org/en/smartChain).
- Implemented support TFT buying with BTC
- Improvements to the token statistics service
- Implemented TFT vesting service

