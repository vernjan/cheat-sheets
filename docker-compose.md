# Docker Compose

## Networking

https://docs.docker.com/compose/networking/

`HOST_PORT:CONTAINER_PORT`

- Containers on the same network: `service name + CONTAINER_PORT`
- Host to container: `localhost/DOCKER_IP + HOST_PORT`
- Container to host: `host.docker.internal`