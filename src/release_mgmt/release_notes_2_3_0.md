# ThreeFold Cloud 2.3.0 Release Notes

New in this release:

- 3Bot, your virtual system administrator
  - 3bot deployer got serious upgrade (faster, prefunded wallet, easier to use)
  - more performance of deployment
  - auto topup for capacity pools (if capacity pools run out of capacity, they can be autofunded)
  - SSH access into the 3bot, advanced users can now SSH into their 3bot and have full functionality access from the root shell.
- Zero-OS = expanded manageability on TFGrid
  - integrated monitoring hooks for the grid workloads like containers, which can be consulted by means of our SDK inside the 3bot
  - logging hooks, which can be consulted by means of our SDK inside the 3bot
- Explorer
  - shows devnet, testnet and mainnet in 1 interface
- TFGrid capabilities
  - Automatic SSL test certificates can be given out for web workloads
  - More capacity on Testnet.
- Demo for Marketplace
  - see https://marketplace.threefold.io

And of course lots of bugfixes and small improvements.

## Details

### 3Bot

- package management
  - 3Bot Packages can be installed from a github repo directly.
  - reload of packages without restart of 3bot
- auto topup of capacity pools
  - You can now automatically extend your capacity pools when they are expiring; that way it will minimize workload downtime due to lacking resources. 
  - An escalation email will also be sent automatically as a reminder to extend your capacity pool.
- SSH access capability is added
- backup has been improved:
  - downloaded packages
  - .ssh directory (so your access key is remembered)
  - your personal code directories (to keep your code changes you made for your own 3Bot)

### 3Bot Deployer

- simplifactions & faster
- can select where to deploy your 3bot (more decentralization possibility)
- pre-funded wallet during deployment makes it easier to get started (was 2 steps before)

### ThreeFold Now Demo

- see [ThreeFold Now Marketplace](https://marketplace.threefold.io/marketplace/#/).

<!-- - Along with new categories, this release introduces a new ThreeFold Now solution: you can now use a decentralized video calling solution deployable via ThreeFold Now Marketplace on [this link](https://marketplace.threefold.io/marketplace/#/solutions/meetings).  -->

### Jumpscale Framework 

We have a new version of our jumpscale framework which is our automation framework and the foundation of the autonomous layer.

- releases: 
  - https://github.com/threefoldtech/js-ng/releases/tag/v11.0-b7
  - https://github.com/threefoldtech/js-sdk/releases/tag/11.0-b11

