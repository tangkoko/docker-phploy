# docker-phploy
[![](https://badge.imagelayers.io/remyvv/phploy:latest.svg)](https://imagelayers.io/?images=remyvv/phploy:latest) [![Docker Pulls](https://img.shields.io/docker/pulls/remyvv/phploy.svg)](https://hub.docker.com/r/remyvv/phploy/)

A Docker container for [PHPloy](https://github.com/banago/PHPloy) that can be used as-is or as a Gitlab-CI docker runner.
[PHPloy](https://github.com/banago/PHPloy) is a command-line tool for deploying a Git Repository over (S)FTP.

How to Build
--------------------

Build from `Dockerfile`:

```sh
docker build --no-cache -t remyvv/phploy .
```

Verify build:

```sh
docker run --rm -it remyvv/phploy phploy
```

Usage
--------------------

1. Install the `remyvv/phploy` container (optional - this step is performed by Docker automatically when running the container):

```sh
docker pull remyvv/phploy
```

2. Run the docker container like this:

```sh
docker run --rm -it -v $(pwd):/app remyvv/phploy phploy
```
