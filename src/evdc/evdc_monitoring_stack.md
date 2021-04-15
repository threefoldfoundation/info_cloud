# Monitor Kubernetes Clusters using Monitoring Stack

## What is Prometheus

[Prometheus](https://prometheus.io/) is a free software application used for event monitoring and alerting. It records real-time metrics in a time series database, allowing for high dimensionality.

## What is Grafana

[Grafana](https://grafana.com) has become the world’s most popular technology used to compose observability dashboards with everything from Prometheus & Graphite metrics to logs and application to data power plants and beehives.

## Getting Started

The monitoring stack is available as a solution in the Marketplace. 

![](img/evdc_k8s_monitoring_01_mktpl.png ':size=200')

Click `Deploy` and go through a simple chat flow to configure the monitoring of your cluster. 

![](img/evdc_k8s_monitoring_02_mktpl2.png ':size=200')

A few elements need to be provided. First, give your monitoring the name you want (it will be part of the url).

![](img/evdc_k8s_monitoring_03_name.png ':size=600')

You can configure the URL to be auto-generated or part of your domain. 

![](img/evdc_k8s_monitoring_04_subdomain.png ':size=600')

After setting up the name of your monitoring and configuring the URL, the Monitoring Stack will be deployed. 

![](img/evdc_k8s_monitoring_05_deploying.png ':size=600')

Choose the size of the hardware to be reserved for your monitoring solution. 

![](img/evdc_k8s_monitoring_06_flavour.png ':size=600')

Once the package is selected, the montiroing stack will be initialized on your Kubernetes cluster. 

![](img/evdc_k8s_monitoring_07_init.png ':size=600')

You will be provided with URLs to access your monitoring solution, with both UIs on Prometheus and Grafana. 

![](img/evdc_k8s_monitoring_08_success.png ':size=600')

![](img/evdc_k8s_monitoring_09_prometheus.png)

![](img/evdc_k8s_monitoring_09_grafana1.png)

![](img/evdc_k8s_monitoring_11_grafana3.png)

More Info:
- For the installation of Kubernetes monitoring on your local machine, see [Local Monitoring](evdc_monitoring_local).
- Go back to [Kubernetes Actions](kubernetes_deploy).


