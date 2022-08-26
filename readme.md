# AdGuard Home

Dockerized instance of AdGuard Home to be used on Raspbian OS arm64 on novapi.

Based on official [AdGuard Home image](https://hub.docker.com/r/adguard/adguardhome).


## Installation

Clone the repository to the local:
```bash
git clone https://github.com/n0vi/AdGuardHome adguardhome

```

Create conf and work folders for adguard container volumes
```bash
mkdir conf work
```

## Usage

Start AdGuard Home:
```bash
sudo docker-compose up -d adguardhome
```

Logs to check:

```bash
sudo docker-compose logs -f adguardhome
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
