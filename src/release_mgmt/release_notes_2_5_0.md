 ThreeFold Cloud 2.5

## Component Upgrades

### JS-SDK V11.2.0
    -   Consists of elements:
        - [3Bot Deployer](https://github.com/threefoldtech/js-sdk/tree/development/jumpscale/packages/threebot_deployer)
        - [Solution Marketplace](https://github.com/threefoldtech/js-sdk/tree/development/jumpscale/packages/marketplace)
        - [Virtual Datacenter VDC](https://github.com/threefoldtech/js-sdk/tree/development/jumpscale/packages/vdc)

#### VDC v2.5.0 
- Marketplace is now the default view for the VDC dashboard 
- 'Update Dashboard' button 
- Blockchain solution: Digibyte and Presearch 
- 'Transaction History': 'List Transaction' button 
- TF Connect sign-in for most solutions on the Marketplace: done
        - gitea 
        - peertube
        - cryptpad
        - zeroci
        - mattermost (still issues to be finished by then )
- Back up/restore feature on the VDC in progress
- Updates Notification for new updates
- QR Scan Top up PR ready
- ZDBs expose over public IPv4
- Kubernetes autoscaling
- External etcd datasource for kubernetes (config manager support, solution / cluster support.)

#### 3Bot SDK v2.5.0
- New chatflows on network management and capacity pool
- Farmmgmt custom prices support and 3Bot deal
- New K8s support for public IPs
- More sizes support for K8s deployment
- Email notification for expiring pools and empty wallets
- Rebrand 3Bot Marketplace as 3Bot Apps


### JS-NG v11.2.0
- ETCD backend support
- Mongo backend support

### JS-Ansible v0.1.0
- Ansible modules that creates an IT automation capability.
- One-to-one mapping with the grid
- Added on generic modules
 identity, wallet, pool, network, volume, container, ipv4, k8s, zdb, subdomain, tcp reverse proxy, 4to6, workloads
- Add to helper modules: node selection scheduler, IP management, and metadata management

### TFGateway v0.3.9
- Nameservers validations 
- Domains validation
- Ownership validation

### ZOS 0.4.9
- Major ZOS network refactoring
- Single ZOS binary
- Elevated containers support

### O-stor v2 v0.1.1
- Revert to the original way to do namespace authentication

### TF Explorer 0.4.9
- Improvements on the escrow and payments
- Retries capability on error
- Drop support for TFTA and FreeTFT
- Use stellar production network for all three Threefold networks
- Store cause of payment cancellation on payment object
- Added ability on clients to check the status of payments
- Set Different prices for different networks
- Validate gateway registration to ensure the gateway manages the domains it claims
- Faster pool expiration checks
- Validation for farmer ID on both node and gateway registration

### 0-DB-FS V0.1.2
- Add autons fuse option to create required namespace on initialization


