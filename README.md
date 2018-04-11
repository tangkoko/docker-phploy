# docker-phploy
[![](https://badge.imagelayers.io/tangkoko/phploy:latest.svg)](https://imagelayers.io/?images=tangkoko/phploy:latest) [![Docker Pulls](https://img.shields.io/docker/pulls/tangkoko/phploy.svg)](https://hub.docker.com/r/tangkoko/phploy/)

A Docker container for [PHPloy](https://github.com/banago/PHPloy) that can be used as-is or as a Gitlab-CI docker runner.
[PHPloy](https://github.com/banago/PHPloy) is a command-line tool for deploying a Git Repository over (S)FTP.

How to Build
--------------------

Build from `Dockerfile`:

```sh
docker build --no-cache -t tangkoko/phploy .
```

Verify build:

```sh
docker run --rm -it tangkoko/phploy phploy
```

Usage
--------------------

1. Install the `tangkoko/phploy` container (optional - this step is performed by Docker automatically when running the container):

```sh
docker pull tangkoko/phploy
```

2. Run the docker container like this:

```sh
docker run --rm -it -v $(pwd):/app tangkoko/phploy phploy
```
