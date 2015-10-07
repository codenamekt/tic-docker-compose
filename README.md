# Docker tic stack

|Service  | Base Image | Port |
|--------:|:----------:|:----:|
|[telegraf](https://github.com/influxdb/telegraf)|[:link:](https://hub.docker.com/r/codenamekt/telegraf/)|None||
|[influxdb](https://influxdb.com/)|[:link:](https://hub.docker.com/r/codenamekt/influxdb/)|8083, 8086||
|[chronograf](https://influxdb.com/chronograf/index.html)|[:link:](https://hub.docker.com/r/codenamekt/chronograf/)|9080||

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

# Screenshot

![Screenshot](screenshot.png?raw=true "Screenshot")

# Thanks

* [InfluxDB](https://influxdb.com/)
