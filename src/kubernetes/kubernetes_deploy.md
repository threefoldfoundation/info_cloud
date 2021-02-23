# Kubernetes Cluster Actions

#### Pre-required 
- You'll need to log in through Threefold Connect, an authenticator for the ThreeFold ecosystem.
- You can find more on ThreeFold Connect [here](https://manual.threefold.io/#/3botconnect_install).

#### Getting Started 
The Kubernetes cluster comes with the creation of your VDC.

You can create this VDC with a deployed Kubernetes Cluster on the VDC deployment website : 
- on testnet [here](https://vdc.testnet.grid.tf)
- mainnet coming soon

#### Upgrade

- [Add a Node](evdc_upgrade)

#### Downgrade 

- [Remove a Node](evdc_downgrade)

#### Manage
- [Manage your Kubernetes Cluster](evdc_k8s)

## Where to ask questions

- Feel free to ask us any questions you might have on [our forum](https://forum.threefold.io) in the feedback category.
- We also have a Telegram Group for TF Grid testers [here](https://t.me/joinchat/BwOvOxxgK59GmRoZ2_sM0w).

*Please keep in mind that eVDC is currently running on testnet. Mainnet is planned for early 2021.*

*Please forgive any instability you might encounter while our developers continue to work to bring you the best solutions possible and keep in mind the forum (linked directly above) is there for you to bring questions or report any issues.*

---- 

#### More info : K3S 

The deployed Kubernetes instance  is a lightweight K3S Kubernetes implementation in Zero-OS

  ![](evdck3slogo.png)

- K3S is full conformant production-ready Kubernetes distribution with the following changes:   
   - It is packaged as a single binary
   - It adds support to sqlite3 as default storage. Etcd3, MySQL and Postgres are also supported
   - It wraps Kubernetes and other components in a single, simple launcher
   - It is secure by default with reasonable defa&ults for lightweight environments
   - It eliminates the need to expose a port on Kubernetes worker nodes fopr the kubelet API by exposing this API to the Kubernetes control plain nodes over a websocket tunnel. 
   
   More info can be found [here](https://github.com/rancher/k3s)
   
