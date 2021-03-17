# Secure in all dimensions

## Running on an OS with minimal hacking surface

Zero-OS is a secure operating system that runs on the Threefold nodes.

some benefits:

- It has no shell, means farmers, i.e. owners of the capacity that hosts the OS and the workloads, have no access to the data residing nor the applications running on their hardware.
- It does no allow inboud network connections to the OS for administration and workload deployment activities.
- It is not installed on local (systems based) harddrives.  The OS os booted over the network with cryptographic boot file verification.  Physical disk access or a "man in the middle attack" do not allow hackers to succeed.


## Network security

- All networking in Zero-OS comes is set up as a private overlay network. All nodes have their own IPv6 address and are fully interconnected in the defined network. All traffic on the network is encrypted.
- Linkage for applications to the outside world is managed through the web gateways. These web gateways terminate all incoming traffic pretending to the the server and then initiate a new client service connection to the real application server.  This internal client server connection is initiated by the (real) application server, not from the outside.  This only allows external traffic that is inititiated and accepted from inside.
- There is no TCP/IP traffic allowed coming from the outside. Data is picked up from the inside.

## Quantum save Storage

The quantum save storage solution splits data objects in an intelligent way into different parts, such that only part of the information stored in one place. Moreover, the data is described in a way such that a person aiming to hack into the low-level data (which is almost impossible in itself), will only find non-relevant information on this storage infrastructure.
The fact that no data part can be (re-)created by accessing one location, makes the storage quantum proof: no compute power can ‘imagine’ what the other data parts are by looking at the datapart of a single location.
More info on our quntum safe storage mechanism can be found [here](https://manual.threefold.io/#/quantumsafe_storage_concept?id=dispersed-storage-architecture-design-philosophy).

Quantum safe storage has been completely overhauled and is availabe as a filesystem, inside VDC's, in containers deployed by 3bot's and on local systems that deploy the binaries and use the TF Grid as a backedn storage system.

## Security in the deployment process

Deployment of IT workload using a so-called “Smart Contract for IT” makes the deployment process resilient to human error and hacking. The system is self-driving and self-healing, therefore removing the human requirement for deploying and operating IT infrastructure or services. This represents a breakthrough in IT. 3Bot records all transactions within the blockchain database (BCDB), ensuring an immutable record of any workload and enables the self-healing functionality as any workload can easily be restored if/when needed.

![](img/smartcontractit_intro.png)


## Secure Decentralized access

Access to your virtual data center happens through Threefold Connect App. This app is a fully decentralized multifactor authentication mechanism, based on PKI technology.

![](img/vdc_secure.png)
