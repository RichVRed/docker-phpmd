## PHPMD
[![Docker Pulls](https://img.shields.io/docker/pulls/rvannauker/phpmd.svg)](https://hub.docker.com/r/rvannauker/phpmd/) [![Docker Stars](https://img.shields.io/docker/stars/rvannauker/phpmd.svg)](https://hub.docker.com/r/rvannauker/phpmd/) [![](https://images.microbadger.com/badges/image/rvannauker/phpmd:latest.svg)](https://microbadger.com/images/rvannauker/phpmd:latest) [![GitHub issues](https://img.shields.io/github/issues/RichVRed/docker-phpmd.svg)](https://github.com/RichVRed/docker-phpmd) [![license](https://img.shields.io/github/license/RichVRed/docker-phpmd.svg)](https://tldrlegal.com/license/mit-license)

Docker container to install and run phpmd

### Installation / Usage
1. Install the rvannauker/phpmd container:
```bash
docker pull rvannauker/phpmd
```
2. Run phpmd through the phpmd container:
```bash
sudo docker run --rm --volume $(pwd):/workspace --name="phpmd" "rvannauker/phpmd" {destination} text cleancode,codesize,controversial,design,naming,unusedcode
```

### Download the source:
To run, test and develop the PHPMD Dockerfile itself, you must use the source directly:
1. Download the source:
```bash
git clone https://github.com/RichVRed/docker-phpmd.git
```
2. Build the container:
```bash
sudo docker build --force-rm --tag "rvannauker/phpmd" --file phpmd.dockerfile .
```
3. Test running the container:
```bash
 $ docker run rvannauker/phpmd --help
```