# Docker tic stack

|Service  | Base Image | Port |
|--------:|:----------:|:----:|
|[telegraf](https://collectd.org/)|[:link:](https://hub.docker.com/r/yaronr/collectd/)|25826/udp||
|[influxdb](https://www.elastic.co/products/logstash)|[:link:](https://registry.hub.docker.com/_/logstash/)|5000||
|[chronograf](https://www.elastic.co/products/elasticsearch)|[:link:](https://registry.hub.docker.com/_/elasticsearch/)|9200||

# Setup

1. Install [Docker](http://docker.io).
2. Install [Docker Compose](http://docs.docker.com/compose/install/).
3. `git clone git@github.com:codenamekt/tic-docker-compose.git`

# Usage

Start the stack in the background using *docker-compose*:

```bash
$ docker-compose up -d
```

You will immediately start seeing stats (cpu, memory, load) getting pushed into the tic stack.

Access the Chronograf UI by hitting [http://localhost:9080](http://localhost:9080) with a web browser to view the statistics.

![Kibana](screenshot.png?raw=true "Kibana")

# Thanks

* [Elastic](https://www.elastic.co)
