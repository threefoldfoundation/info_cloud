
 # ThreeFold Cloud 2.7.1
 
Live on testnet - May 14, 2021.

## JS-SDK v11.2.1

### Component Upgrades
- [3Bot Deployer](https://github.com/threefoldtech/js-sdk/tree/development/jumpscale/packages/threebot_deployer)
- [Solution Marketplace](https://github.com/threefoldtech/js-sdk/tree/development/jumpscale/packages/marketplace)
- [Virtual Datacenter VDC](https://github.com/threefoldtech/js-sdk/tree/development/jumpscale/packages/vdc)

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


### ThreeFold Connect App 2.7.1
- Added TFT Vesting feature
- Added BTC deposit and withdrawal feature
- Added BTC - TFT Exchange feature
- Added auto notifications for new terms and conditions

### TFT v1.0
- Added TFT - Binance Smart Chain Bridge integration
- Added Vesting Wallet feature
- Improved Tokenstats on wiki.threefold.io

## ZOS 0.4.11
-
