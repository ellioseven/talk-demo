# How to Build Docker Images

## `Dockerfile`

Building an image:

```
docker build -t talk-demo-php ./php
docker run php
```

```
docker build -t talk-demo-node ./node
docker run node
```

## Registries

- https://hub.docker.com/r/ellioseven/node/

## `docker-compose.yml`

```
docker-compose up
```

## Sharing Docker Builds

```
git clone https://github.com/ellioseven/talk-demo
cd talk-demo
docker-compose up
```
