
---

# Setting Up Monitoring Tools: ELK (EFK) & Prometheus-Grafana

## Overview
This guide provides detailed instructions for setting up monitoring tools, including the ELK (Elasticsearch, Logstash, Kibana) stack and Prometheus-Grafana. These tools help in monitoring system performance, application logs, and metrics, ensuring a robust and reliable infrastructure.

## Prerequisites
Before you begin, ensure you have the following:

- **Kubernetes Cluster**: A Kubernetes cluster set up on-premise or in the cloud.
- **Docker**: Installed on your build and deployment servers.
- **Helm**: Installed on your local machine and configured with your Kubernetes cluster.
- **Git**: Access to the Git repository where the configuration files are stored.

## Monitoring System
![Monitoring System](https://github.com/user-attachments/assets/ff41ca3f-cd7b-4371-9bee-9fac8a135709)

## Monitoring Application
![Monitoring Application](https://github.com/user-attachments/assets/665551f2-f964-419d-b8d0-2f83971a5da0)

## Setting Up ELK (EFK) Stack
### Step 1: Install Elasticsearch
1. Follow the [Elasticsearch installation guide](https://www.elastic.co/guide/en/elasticsearch/reference/current/install-elasticsearch.html) to set up Elasticsearch.
2. Ensure Elasticsearch is running and accessible.

### Step 2: Install Logstash
1. Follow the [Logstash installation guide](https://www.elastic.co/guide/en/logstash/current/installing-logstash.html) to set up Logstash.
2. Configure Logstash to collect and process logs.

### Step 3: Install Kibana
1. Follow the [Kibana installation guide](https://www.elastic.co/guide/en/kibana/current/install.html) to set up Kibana.
2. Configure Kibana to visualize the data stored in Elasticsearch.

### Step 4: Deploy Fluentd (EFK)
1. Deploy Fluentd to collect logs from your Kubernetes cluster and forward them to Elasticsearch.
2. Follow the [Fluentd installation guide](https://docs.fluentd.org/installation) for detailed instructions.

## Setting Up Prometheus-Grafana
### Step 1: Install Prometheus
1. Follow the [Prometheus installation guide](https://prometheus.io/docs/prometheus/latest/installation/) to set up Prometheus.
2. Configure Prometheus to scrape metrics from your applications and infrastructure.

### Step 2: Install Grafana
1. Follow the [Grafana installation guide](https://grafana.com/docs/grafana/latest/installation/) to set up Grafana.
2. Configure Grafana to visualize the metrics collected by Prometheus.

### Step 3: Configure Dashboards
1. Create and configure Grafana dashboards to visualize the metrics and logs.
2. Use pre-built dashboards from the Grafana community or create custom ones based on your requirements.

## Additional Resources
For more detailed information, check out this [Notion page](https://www.notion.so/All-Required-Things-which-needed-To-Provision-K8S-on-an-on-Premise-1eec48e905f44b53ad0df6d6ee57e3a0).

## Conclusion
You have successfully set up monitoring tools using ELK (EFK) and Prometheus-Grafana. These tools will help you monitor system performance, application logs, and metrics, ensuring a robust and reliable infrastructure. For any issues or further assistance, feel free to reach out.

---
