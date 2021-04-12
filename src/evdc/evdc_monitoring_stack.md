# Monitor Kubernetes Clusters using Monitoring Stack

<!--- TODO 
- intro: what is monitoring stack what are included in monitoring stack
- explain what is prometheus, what's the use / what can it monitor
- explain what is grafana , what can it monitor, what's the use / what can it monitor
- requirements: explain requirements
- getting started explain deployment steps
- use case: give 1 example of monitoring on the deployed  grafana / prometheus
-------------->
You can monitor the health of the VDC you deploy. A stack has been prepared that offers monitoring through Prometheus and Grafana. A Helm chart `kube-prometheus-stack` is available, which offers Prometheus and Grafana as tooling to monitor your VDC. 

## What is Prometheus

[Prometheus](https://prometheus.io/) is a free software application used for event monitoring and alerting. It records real-time metrics in a time series database (allowing for high dimensionality).

## What is Grafana

[Grafana](https://grafana.com) has become the world’s most popular technology used to compose observability dashboards with everything from Prometheus & Graphite metrics to logs and application data to power plants and beehives.

## Getting Started

The monitoring stack is available as a solution in the marketplace. 

![](img/evdc_k8s_monitoring_01_mktpl.png ':size=200')

Click `Deploy` and go through a simple chat flow to configure the monitoring on your cluster. 

![](img/evdc_k8s_monitoring_02_mktpl2.png ':size=200')

A few elements need to be provided. 
First, give your monitoring the name you want (it will be part of the url).

![](img/evdc_k8s_monitoring_03_name.png ':size=600')

You can configure the URL to be auto-generated or part of your domain. 

![](img/evdc_k8s_monitoring_04_subdomain.png ':size=600')

This information is enough to prepare the Monitoring Stack. 

![](img/evdc_k8s_monitoring_05_deploying.png ':size=600')

Choose the size of the hardware to be reserved for your monitoring solution. 

![](img/evdc_k8s_monitoring_06_flavour.png ':size=600')

Now there is enough information to set up the monitoring stack on your Kubernetes cluster. 

![](img/evdc_k8s_monitoring_07_init.png ':size=600')

And that's it: the URLs are available to access your monitoring solution, with both UIs on Prometheus and Grafana. 

![](img/evdc_k8s_monitoring_08_success.png ':size=600')

![](img/evdc_k8s_monitoring_09_prometheus.png)

![](img/evdc_k8s_monitoring_09_grafana1.png)

![](img/evdc_k8s_monitoring_11_grafana3.png)

> For the installation of Kubernetes monitoring on your local machine, please read [__Local Monitoring__](evdc_monitoring_local)).

