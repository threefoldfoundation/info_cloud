# Secure in all dimensions

## Running on an OS with minimal hacking surface

Zero-OS is a secure operating system that runs on Threefold nodes.

Some benefits:

- Being shell-less, farmers, i.e. owners of the capacity that hosts the OS and the workloads, have no access to the data residing nor the applications running on their hardware.

## Network security

- All networking in Zero-OS happens on a private overlay network. All nodes have their IPv6 address and are fully interconnected in the defined network. All traffic on the network is encrypted.
- The link to the outside world is managed through web gateways. These web gateways filter out incoming traffic, only allowing external traffic that is accepted from the inside.
- There is no TCP/IP traffic allowed coming from the outside. Data is picked up from the inside.

## Quantum-secure Storage

ThreeFold developed the service to have S3 storage smartly split into different shards to store each information piece in a different location. Moreover, data is represented descriptively on the low-level code; therefore, even if someone hacks into the low-level data (which is almost impossible in itself), only non-relevant information on this storage infrastructure will be found.

No data shard can be created by only accessing one location, making the storage quantum-proof - no computing power can ‘imagine’ what these missing data shards are.

You can find more info on our dispersed storage mechanism [here](https://manual.threefold.io/#/quantumsafe_storage_concept?id=dispersed-storage-architecture-design-philosophy).

This secure storage has been implemented into the Minio S3 storage offering, available on the Threefold Grid.

## Security in the deployment process

Deployment of IT workloads is done using a so-called “Smart Contract for IT” that makes the deployment process resilient to human error and hacking. Therefore, the system is self-driving and self-healing, removing the human requirement for deploying and operating IT infrastructure and services. This represents a breakthrough in IT. 3Bots record all transactions within the blockchain database (BCDB), ensuring an immutable record of the workloads and enabling the self-healing functionality as any workload can easily be restored if/when needed.

![](img/smartcontractit_intro.png)


## Secure Decentralized access

Access your virtual data center through Threefold Connect App. This app is a fully decentralized multi-factor authentication mechanism based on PKI technology.

![](img/vdc_secure.png)
