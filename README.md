# Docker compose template for Elasticsearch, Kibana and plugins

This Docker compose recipe combines the (legacy) Docker images [elasticsearch:2](https://hub.docker.com/_/elasticsearch/) and [kibana:4](https://hub.docker.com/_/kibana/) and can easily be extended with plugins.

## Prerequisites

- Install [Docker Compose](https://docs.docker.com/compose/)

## Run the docker containers

Start the containers from the cloned repository directory with

```docker-compose up```

At first run the images and plugins are downloaded and installed. When finished, navigate to http://localhost:9200 for the Elasticsearch endpoint, http://localhost:9200/_plugin/hq/ for Elastic-HQ and  http://localhost:5601 for Kibana.

The Elasticsearch data directory is located as a sibling of the directory containing the Docker Compose recipe and is called `elasticsearch-data`.

## Included plugins

- [Elastic Sense](https://www.elastic.co/guide/en/sense/current/index.html)
- [Elastic Watcher](https://www.elastic.co/guide/en/watcher/2.4/index.html) and Elastic Licence (Watcher is a commercial plugin, and the license gives a 30-day trial for Watcher)
- [royrusso/elasticsearch-HQ](https://github.com/royrusso/elasticsearch-HQ)
