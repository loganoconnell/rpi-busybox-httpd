# rpi-busybox-httpd

Custom Raspberry Pi compatible Docker image with a minimal `Busybox httpd` web server adapted from [hypriot/rpi-busybox-httpd](https://github.com/hypriot/rpi-busybox-httpd).

## Starting the default web server
```bash
docker run -d -p 8080:80 hypriot/rpi-busybox-httpd
```

## Creating this image
### Install the build dependencies
```bash
./install-deps.sh
```

### Build the Docker image
```bash
make build
```

#### Test the Docker image
```bash
make test
```

#### Push the Docker image to the Docker Hub
First use a `docker login` with username, password and email address

```bash
make push
```