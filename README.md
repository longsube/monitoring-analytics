Monitoring Analytics
====================

Limited public demo instance: https://monitoringartist.shinyapps.io/monitoring-analytics/

If you like or use this project, please provide feedback to author - Star it ★.

Yes, monitoring is not a rocket science usually. However your monitoring system keeps a lot of time series data. You can you use science / math / statistics and turn your data into knowledge, which can be used to improve your monitoring systems and settings.
Don't estimate any static thresholds for your metrics. Set them based on your real values. If you don't know, what is normal value, then try to detect anomalies in your series. Remember, your only limitation is your data science imagination:
histograms, linear/polynomial/...  trends, prediction, anomaly detection, correlation, 3d visualization, heat map, ...
 
![Monitoring Analytics](https://raw.githubusercontent.com/monitoringartist/monitoring-analytics/master/doc/monitoring-analytics.gif) 

**Overview of Monitoring Artist Dockerized monitoring ecosystem:**

- **[Zabbix XXL](https://hub.docker.com/r/monitoringartist/zabbix-3.0-xxl/)** - standard Zabbix 3.0 server/proxy/UI/snmpd/java gateway with additional XXL extensions
- **[Zabbix agent XXL](https://hub.docker.com/r/monitoringartist/zabbix-agent-xxl-limited/)** - Zabbix 3.0 agent with [Docker (Mesos/Chronos/Marathon) monitoring](https://github.com/monitoringartist/zabbix-docker-monitoring) and [systemd monitoring](https://github.com/monitoringartist/zabbix-systemd-monitoring)
- **[Zabbix templates](https://hub.docker.com/r/monitoringartist/zabbix-templates/)** - tiny (5MB) image for easy template deployment of selected Zabbix monitoring templates
- **[Zabbix extension - all templates](https://hub.docker.com/r/monitoringartist/zabbix-ext-all-templates/)** - storage image for Zabbix XXL with 200+ [community templates](https://github.com/monitoringartist/zabbix-community-repos)
- **[Kubernetized Zabbix](https://github.com/monitoringartist/kubernetes-zabbix)** - containerized Zabbix cluster based on Kubernetes
- **[Grafana XXL](https://hub.docker.com/r/monitoringartist/grafana-xxl/)** - dockerized Grafana with all community plugins
- **[Monitoring Analytics](https://hub.docker.com/r/monitoringartist/monitoring-analytics/)** - R statistical computing and graphics for monitoring from data scientists
- **[Docker killer](https://hub.docker.com/r/monitoringartist/docker-killer/)** - Docker image for Docker stress and Docker orchestration testing

Please donate to author, so he can continue to publish other awesome projects
for free:

[![Paypal donate button](http://jangaraj.com/img/github-donate-button02.png)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=8LB6J222WRUZ4)

Dockerized Monitoring Analytics
===============================

```
docker run \
  -d \
  --name=shiny \
  -p 3838:3838 \
  monitoringartist/monitoring-analytics:latest
```

Support
=======

Deep monitoring knowledge and science skills are required, so only commercial support is available.

Recommended related articles
============================

- [Dynatrace blog about percentiles](http://apmblog.dynatrace.com/2012/11/14/why-averages-suck-and-percentiles-are-great/)
- [Zabbix white paper about prediction](http://zabbix.org/mw/images/1/18/Prediction_docs.pdf)

# Author

[Devops Monitoring Expert](http://www.jangaraj.com 'DevOps / Docker / Kubernetes / AWS ECS / Google GCP / Zabbix / Zenoss / Terraform / Monitoring'),
who loves monitoring systems and cutting/bleeding edge technologies: Docker,
Kubernetes, ECS, AWS, Google GCP, Terraform, Lambda, Zabbix, Grafana, Elasticsearch,
Kibana, Prometheus, Sysdig, ...

Summary:
* 1000+ [GitHub](https://github.com/monitoringartist/) stars
* 6000+ [Grafana dashboard](https://grafana.net/monitoringartist) downloads
* 800 000+ [Docker image](https://hub.docker.com/u/monitoringartist/) pulls

Professional devops / monitoring / consulting services:

[![Monitoring Artist](http://monitoringartist.com/img/github-monitoring-artist-logo.jpg)](http://www.monitoringartist.com 'DevOps / Docker / Kubernetes / AWS ECS / Google GCP / Zabbix / Zenoss / Terraform / Monitoring')
