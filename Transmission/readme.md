# Transmission 

[Transmission](Transmission/readme.md) - Dockerized instance of Transmission torrent client, based on [LinuxServer Transmission image](https://hub.docker.com/r/linuxserver/transmission)

## Installation

Clone the repository to the local:
```bash
git clone https://github.com/n0vi/HomeAutomation HomeAutomation

```

Create config, downloads, watch folders for transmission container volumes
```bash
mkdir config downloads watch
```

Symlink downloads and watch to a proper location
```bash
ln -s downloads /path/to/downloads 
ln -s watch /path/to/downloads 
```

## Usage

Start Transmission:
```bash
sudo docker-compose up -d transmission
```

Logs to check:

```bash
sudo docker-compose logs -f transmission
```

## Update To A Newer Version

Pull the new version from Docker Hub:
```bash
docker pull transmission
```

Stop and remove the container:

```bash
docker stop transmission
docker rm transmission
```

Start Transmission
```bash
sudo docker-compose up -d transmission
```
