# Docker

Docker is a containerization platform for building, deploying, and managing applications in isolated environments.

---

## Useful commands

Running something inside a container

```bash
docker exec [OPTIONS] command [ARG...]
```

Entering a container shell

```bash
docker exec -it [CONTAINER NAME / ID] sh
```

## [Dockerfile](https://docs.docker.com/engine/reference/builder/)

A Dockerfile is made up by this format

```yaml
# Comment
INSTRUCTION arguments
```

The most important instructions are, FROM, RUN, CMD. The dockerfile starts with a FROM instruction that defines which image to use. It looks like this

```yaml
FROM node:16-alpine
```

The RUN instruction executes some command inside the docker container. By the way, every INSTRUCTION is executed inside the container, and not on the local machine. For example this line

```yaml
RUN npm install
```

will run the command npm install inside the container.
