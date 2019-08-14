# Installation

pull the monitor's source code

```
git clone https://github.com/coolcode/monitor_docker

cd blockchainmonitor
```

build docker images

```
./build.sh
```

cd monitor-docker

setup monitor's configuration. Sample: ./setup.sh 127.0.0.1 5

```
./setup.sh {ip} {number of nodes}
```

run monitor

```
docker-compose up -d
```

The default monitor’s url is http://{ip}, for example: http://localhost

💡It takes about 30 seconds to synchronize all blocks.

# Cleanup

remove the monitor

```
docker-compose down -v
```

remove the monitor's configuration

```
./cleanup.sh
```
