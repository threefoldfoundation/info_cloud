# Deploy an ETCD key-value database in your eVDC

[etcd](https://etcd.io/) is a distributed, reliable key-value store for the most critical data of a distributed system, with a focus on being :

- Simple: well-defined, user-facing API (gRPC)
- Secure: automatic TLS with optional client cert authentication
- Fast: benchmarked 10,000 writes/sec
- Reliable: properly distributed using Raft

## Getting Started

Once you're logged in the eVDC, find the __etcd__ marketplace widget on your admin panel and click on __Deploy__ button.

![](img/02_evdc_etcd_widget.png ':size=200')

Create a name for your ETCD instance. You will use this name to identify your deployment on your 'Deployed Solutions' list.

![](img/03_evdc_etcd_name.png ':size=600')

Select the domain for your website. For deployment with a random subdomain, select 'Choose subdomain for me on a gateway',. For deployment with a particular available subdomain, select 'Choose a custom subdomain on a gateway. To host a website using your domain, select 'choose a custom domain'.

![](img/04_evdc_etcd_subdomain.png ':size=600')

Select the vdc capacity plan for your ETCD.

![](img/05_evdc_etcd_config.png ':size=600')

Congratulations! you just successfully hosted an ETCD instance ThreeFold Grid!

![](img/06_evdc_etcd_success.png ':size=600')

