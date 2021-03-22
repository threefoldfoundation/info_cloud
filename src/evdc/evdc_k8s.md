# Docker and Kubernetes
<!-- TO DO geert
- intro: explain in short what is kubernetes cluster and how it relates to TF evdc Compute nodes. 
- intro: show when you upgrade a computer node, it means youre deploying kubernetes cluster. 
- explains the sizes of kubernetes cluster,  
- add link on how to add compute nodes at the end. (evdc_compute) -->

The IT industry is used to standard tooling for the deployment of their IT workload: 
- Docker is the standard for containers
- Kubernetes is the standard for container orchestration

On the TF Grid, you can deploy a Kubernetes orchestrator out of the box. We have implemented the [K3S](https://k3s.io) implementation, which is a full-blown Kubernetes offering.  It uses only half of the memory footprint while being packaged as a single binary and made more lightweight to run in resource-constrained locations (so fit for IoT, edge, ARM etc). 

#### More info on K3S 

The deployed Kubernetes instance is a lightweight K3S Kubernetes implementation in Zero-OS.

  ![](img/evdck3slogo.png)

- K3S is full conformant production-ready Kubernetes distribution with the following changes:   
   - It is packaged as a single binary
   - It adds support to sqlite3 as default storage. Etcd3, MySQL and Postgres are also supported
   - It wraps Kubernetes and other components in a single, simple launcher
   - It is secure by default with reasonable defa&ults for lightweight environments
   - It eliminates the need to expose a port on Kubernetes worker nodes fopr the kubelet API by exposing this API to the Kubernetes control plain nodes over a websocket tunnel. 
   
   You can find more info [here](https://github.com/rancher/k3s)
   
### VDC Compute: a Kubernetes Cluster

The Compute part of the VDC is in essence, a Kubernetes cluster with a master node and different worker nodes. It comes with an IP address to expose the workloads to the public internet. 

In the below screenshot, the VDC contains one master node and 2 worker nodes. 

![](img/evdc_compute_nodes.png)

Any tooling for managing your Kubernetes cluster, both for workload provisioning and monitoring, can be provided with the offering in the marketplace. 

> Please read [__Kubeapps__](evdc_kubeapps) section to deploy and manage applications in your Kubernetes cluster. 

> Please read [__Monitoring__](evdc_monitoring_k8s) to deploy monitoring tools on your Kubernetes cluster. 

The process for deploying workloads has been made easy as many Helm templates have been made available, ready for usage on the grid. The `Marketplace` widget are created with the help of Helm Charts, which can be found [here](https://github.com/threefoldtech/vdc-solutions-charts), but evidently you can also create your own Helm Charts and deploy them onto your Kubernetes cluster. 
