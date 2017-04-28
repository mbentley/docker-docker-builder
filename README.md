docker-docker-builder
=====================

Docker image used to run the `make` commands used to build Docker

Example usage:
```
docker run --rm --name docker-builder \
  -v /var/run/docker.sock:/var/run/docker.sock \
  -v ${PWD}:${PWD} \
  -w ${PWD} \
  mbentley/docker-builder:latest \
  make all
```
