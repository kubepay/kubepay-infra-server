# kubepay-infra-server

This repository holds a docker-compose file, which will initiate a few infrastructure services for your needs.

## Usage:
 
 * **docker-compose up** Create containers, of configured servers, and expose them for your application.
 
 * **docker-compose down** Stop services, and Destroys containers. States will be persistent in your specified volume.

## Services: 

* **Postgresql** [port: 54320] RDBMS
* **Keycloack**  [port: 10090] OAuth2.0 and OIDC Server (Backed by Postgre)
* **Redis** [port: 63790] In-memory Key-Pair storage, and PUB-SUB provider
* **Elasticsearch** [port: 10080]
* **Fluentd** [port: 24224 (TCP & UDP)]
* **Kibana** [port: 92000]
* **Httpd** [port: 80800]


## TODO
* RabbitMQ
* Kong
* Zookeeper
* SonarQube
* Prometheus
* InfluxDB
* Kafka,
* Grafana,
* Gitlab,
* Logstatsh

## Reference:

* https://github.com/paunin/PostDock

* https://github.com/fuinorg/keycloak-testready

* https://github.com/trajakovic/keycloak-docker-compose
