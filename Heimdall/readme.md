# Heimdall

[Heimdall](https://heimdall.site/) is a way to organise all those links to your most used web sites and web applications in a simple way. Based on [Heimdall Image](https://hub.docker.com/r/linuxserver/heimdall/).
## Installation

Clone the repository to the local:
```bash
git clone https://github.com/n0vi/HomeAutomation HomeAutomation

```

Create config folders for heimdall container volume
```bash
mkdir config
```

## Usage

Start Heimdall Home:
```bash
sudo docker-compose up -d heimdall
```

Logs to check:

```bash
sudo docker-compose logs -f heimdall
```

## Update To A Newer Version

Pull the new version from Docker Hub:
```bash
docker pull heimdall
```

Stop and remove the container:

```bash
docker stop heimdall
docker rm heimdall
```

Start AdGuard Home
```bash
sudo docker-compose up -d heimdall
```
