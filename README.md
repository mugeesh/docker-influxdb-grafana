# docker-compose-influxdb-grafana

### Multi-container Docker app built from the following services:

* [InfluxDB](https://github.com/influxdata/influxdb) - time series database
* [Chronograf](https://github.com/influxdata/chronograf) - admin UI for InfluxDB
* [Grafana](https://github.com/grafana/grafana) - visualization UI for InfluxDB

## Quick Start

System Requirement for this project
1. Mac Book/Windows
2. brew install telegraf (for Mac Users)
3. brew services restart telegraf


### To start the app:

1. Install [docker-compose](https://docs.docker.com/compose/install/) on the docker host.
2. Clone this repo on the docker host.
3. cd docker-influxdb-grafana

To stop the app:

```
docker-compose up -d
```

### Check influxdb GUI
1. http://localhost:8086/
2. enter username & password : admin & admin_123
3. go to the data --> telegraf --create configuration -- select bucket_name and system
4. get tocken from above
6. paste in terminal 
7. export INFLUX_TOKEN=a0Zu89UppZ86BaVQcJrqrMSP0ZxT5pBVigpQ
8. export INFLUX_TOKEN=a0Zu89UppZ86BaVQcJrqrMSP0ZxT5pBVigpQ


### Check the result
1. go to bucket "ts" and submit
2. you will see relevent result.

### Shutdown stopped 
```
docker-compose down
```