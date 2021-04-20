
![](img/cloud_node.png)

# ThreeFold P2P Cloud products

- Quantum Safe File System: A peer-to-peer storage solution that can store any file system of any format securely and privately.
- Edge Virtual Data Center: A peer-to-peer compute solution that can run any containerized Unix application at any scale, securely.
- Planetary Network: A private overlay network that connects everything through end-to-end encryption and defines the shortest path.
- P2P Marketplace: A marketplace of peer-to-peer applications (ex: KubeApps, Gitea, Mattermost) ready to be deployed in a few clicks.
- Infrastructure as Code: A way to manage and provision IT workloads autonomously through machine-readable definition files.

## Quantum Safe file System (QSFS) = P2P Storage

A super secure storage system that stores data in an immutable way and that is equipped of operational backup and self-healing capabilities. QSFS can be used independently as well as integrated to the P2P compute solution - Edge Virtual Data Center. 

QSFS uses a dispersed storage algorithm to split the data into shards in a smart way and is stored in different locations, such that only part of the information is stored in one place, making it impossible for anyone besides the data owner to gain access to it. 

The data is described in a way such that a person aiming to hack into the low-level data (which is almost impossible in itself), will only find non-relevant information on this storage infrastructure and the other data shards can't be re-created, making it quantum-proof.

QSFS offers the following storage benefits:
- Any file system of any format can be mounted (dapps, websites, security archives, public datasets, etc..).
- Compatible with IPFS.
- Store Petabytes of data at hyper-competitive pricing.
- Quantum-safe security made possible with the dispersed storage algorythm.
- Unlimited scaleability provided by the ThreeFold P2P infrastructure.
- Self-healing capability of the P2P Cloud ensures your data remains available at all times. 
- Hyper-competitive pricing.

More information on QSFS [here](https://threefold.io/info/cloud#/threefold__threefold_fs)

![](img/evdc.png)

## Edge Virtual Data Center (EVDC) = P2P Compute 

EVDC is the first peer-to-peer compute solution on the market. It provides the agility to create and deploy containers on the edge and allows for micro-services architectures. An EVDC can be deployed in a matter of a few clicks. 

EVDC makes it easy to set-up and manage the execution of containers and the interaction between them. It also offers DNS and IP addresses, automated load balancing at high traffic, automated rollbacks and rollouts and a self-healing architecture.  

It comes with the most widely used tools and frameworks such as Kubernetes and Helm Scripts. It is also fully compatible with industry standards such as Docker and major frameworks such as Grafana snd Prometheus. 

This enables any IT developer working with those standards to deploy their IT workloads on the ThreeFold P2P Cloud in the format they already use today.

EVDC offers the following compute benefits:

- Any containerized Unix IT applications can be deployed.
- Easy to set-up, orchestrate, and manage Kubernetes clusters as well as containers hosted on external clouds (hybrid cloud management).
- Create and scale your development environment easily with autonomous container management, load balancing and web gateways.
- Data is stored in QSFS (see above), offering the highest standard of security. 
- Self-healing and self-driving functionalities to ensure your workloads are always up and running.
- Hyper-competitive prices considering the advanced technology stack

More information on EVDC [here](https://threefold.io/info/cloud#/cloud__evdc)

## Planetary Network = P2P Network

Planetary network is a smart network that enables the true peer-to-peer abilities of EVDC and QSFS. All nodes on the ThreeFold Grid have their own IPv6 address and are securely interconnected in the defined network. All traffic on the network is end-to-end encrypted.

There is no TCP/IP traffic allowed from the outside, data is picked up from the inside, making it an incredibly secure and private environment to build IT workloads on. The link between applications and the outside world is managed through the web gateways. These web gateways terminate all incoming traffic to the server and initiate new client service connections to the real application servers. This internal client server connection is initiated by the real application server, not from the outside. This only allows external traffic that is initiated and accepted from the inside.

Planetary network offers the following benefits:
- Keep your IT workloads secure from TCP/IP connections while still being able to display on the Internet.
- Experience a truly private and owned environment where you are fully in control.

## P2P Marketplace = P2P Applications 

A marketplace of ready-to-deploy peer-to-peer applications. 

You can find:
- A Monitoring stack that comes with Grafana and Prometheus for your EVDC.
- Hosting tools such as Gitea.
- CRM to grow your business.
- Office and publishing (blog, wiki, website) tools
- Open-source applications such as Commento, Mattermost or Discourse. 
- Easy blockchain node deployment for DigiByte, Dash, Polygon, Casper and more.

![](img/iac_intro.png)

## Infrastructure as Code (IaC) = For experts

Infrastructure as code is the process of managing and provisioning computer data centers through machine-readable definition files, rather than physical hardware configuration or interactive configuration tools.

IAC offers three main advantages:
- IaC makes things much more efficient by eliminating all manual processes and the slack in the process. A code-based approach makes it easy to get more done in less time. No need to wait on a task to be manually completed before heading to the next one.
- IaC shifts the power into the developer’s hands. As the infrastructure provisioning becomes more reliable and consistent, developers can start focusing on the application development. They can script once and use that code multiple times, saving time and effort while keeping complete control.
- Automation removes the risk associated with human error, like manual misconfiguration; removing this can decrease downtime and increase reliability. 

## More info:

- [eVDC Get Started](evdc_getting_started) - Start your peer-to-peer cloud journey with eVDC
- [QSFS Get Started](threefold_filesystem) - Learn how to store peer-to-peer with QSFS
- [Marketplace Get Started](evdc_marketplace) - Deploy peer-to-peer apps on top of your eVDC.
- [P2P Cloud Benefits](usp) - A walk through the benefits of using ThreeFold P2P Cloud.
- [Architecture](cloud_architecture) - Dive into the architecture that powers the ThreeFold P2P Cloud.
- [Web 2.0 vs Web 3.0 vs P2P](cloud_compare) - How ThreeFold P2P Cloud compares to a Public Cloud or a Blockchain.











