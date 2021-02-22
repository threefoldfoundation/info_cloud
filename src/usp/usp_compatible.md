# IT-Standard Compatibility

The IT industry is used to standard tooling for the deployment of their IT workload.

## Docker

![](img/docker.png)

Docker is the standard and most widely used container system. 
Docker is supported on the ThreeFold grid, either through the Kubernetes orchestrator layer, or directly through conversion into a flist on the [ThreeFold Hub](https://hub.grid.tf). 
Extensive Docker documentation can be found [here](https://docs.docker.com).

## Kubernetes 

![](img/ips-kubernetes.png)


Kubernetes is the standard for container orchestration.

On the TF grid a Kubernetes orchestrator can be deployed out of the box. We have implemented the [K3S](https://k3s.io) implementation, which is full-blown Kubernetes offering, but using only half of the memory footprint, packaged as a single binary and made more lightweight so that it can run in resource-constrained locations (so fit for IoT, edge, ARM etc).

## Helm

![](img/helm.jpg)

The process for deploying workloads on a Kubernetes cluster can be made easy through the use of Helm templates. These templates are YAML-formatted resource descriptions tyhat Kubernetes can understand. 
A [nice guide](https://helm.sh/docs/chart_template_guide/) describes all ins and outs of this widely used way of defining workload fit for Kubernetes. 

# Filesystem

For storage, any file system will be supported, see our [planetary_filesystem](threefold:threefold_fs) for more detail.