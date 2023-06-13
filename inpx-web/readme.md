# INPX-Web

[INPX-Web](https://github.com/bookpauk/inpx-web) is a Web and OPDS server over INPX library file.

inpx-web is [inpx-web 1.5.5 linux-arm64](https://github.com/bookpauk/inpx-web/releases/download/1.5.5/inpx-web-1.5.5-linux-arm64.zip)


## Installation

Clone the repository to the local:
```bash
git clone https://github.com/n0vi/HomeAutomation HomeAutomation
```

Build docker image
```bash docker build -t inpx-web:latest .
```

Create appdir folder for inpx-web and symlink to the library folder for container volumes appdir and libdir 
```bash
mkdir appdir
ln -s /path/to/library libdir  
```

## Usage

Start inpx-web:
```bash
sudo docker-compose up -d inpx-web
```

Logs to check:

```bash
sudo docker-compose logs -f inpx-web
```

