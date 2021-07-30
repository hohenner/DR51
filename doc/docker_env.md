# Docker Test/Development Environment

I followed the setup steps from [here](https://grafana.com/grafana/dashboards/893)

## launch instructions

````
cd docker_env
docker-compose up -d
````

## Links

* [Prometheus homepage](http://localhost:9090)
* [Grafana homepage](http://localhost:3000)
  * grafana admin pasword is defined [here](../docker_env/docker-compose.yml#L60)

## configuration

To link Prometheus and Grafana you need to create a Prometheus datasource in Grafana. Follow the steps [here](https://prometheus.io/docs/visualization/grafana/#creating-a-prometheus-data-source). Use `http://prometheus:9090` as the URL.
![prometheus data source in grafana](pictures/grafana_prometheus_configure.png "Prometheus data source in grafana")