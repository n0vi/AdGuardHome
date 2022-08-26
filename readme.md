# AdGuard Home

Dockerized instance of AdGuard Home to be used on Raspbian OS arm64 on novapi.

Based on [Install AdGuard Home with Docker on a Raspberry Pi 4](https://samuelsson.dev/install-adguard-home-with-docker-on-a-raspberry-pi-4/) using official [AdGuard Home image](https://hub.docker.com/r/adguard/adguardhome).


## Installation

TBD


## Usage

Start AdGuard Home:
```bash
sudo docker-compose up -d adguardhome
```

Logs to check:

```bash
sudo docker-compose logs -f adguard
```

## Update To A Newer Version

Pull the new version from Docker Hub:
```bash
docker pull adguard/adguardhome
```

Stop and remove the container:

```bash
docker stop adguardhome
docker rm adguardhome
```

Start AdGuard Home
```bash
sudo docker-compose up -d adguardhome
```
