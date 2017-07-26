# System Monitoring

### Info:

This template deploys a collection of monitoring services based upon the technologies listed below, once deployed you will have a monitoring platform capable of querying a wide variety of metrics that represent your environment, also included are somehandy pre-configured dashboards to get you started.

In this catalog item, the following technologies are utilised to make this as useful as possible;

* [Prometheus](https://github.com/prometheus/prometheus) - Used to scrape and store metrics from our data sources.
* [Prometheus Node Exporter](https://github.com/prometheus/node_exporter) - Gets host level metrics and exposes them to Prometheus.
* [cAdvisor](https://github.com/google/cadvisor) - Deploys and Exposes the cadvsior stats used by Rancher's agent container, to Prometheus.
* [Grafana](https://github.com/grafana/grafana/) - Used to visualise the data from Prometheus and InfluxDB.
* Scheduler Exporter - Allows Prometheus to access the Scheduler API and return the status of any stack or service in one environment.

### Future enhancements:
* zabbix for deeper system monitoring 
* eventing/notification


All components in this stack are open source tools available in the community. All this template does is to bound them together in an easy to use package. 
 
### Deployment:
1. Select 'System Monitoring' from catalog.
2. Enter the IP Address of your scheduler server (optional)
3. Click deploy.

### Usage
* Grafana will now be available on, running on port 3000. I've added a number of dashboards to help get you started. Authentication is with the default `admin/admin`.
* Prometheus will now be available, running on port 9090. Have a play around with some of the data. For more information on Prometheus, check out their [documentation](https://prometheus.io/docs/introduction/overview/).
