# How to Build Docker Images

## `Dockerfile`

Building an image:

```
docker build -t talk-demo-php ./php
docker run --rm talk-demo-php
```

```
docker build -t talk-demo-node ./node
docker run --rm talk-demo-node
```

### Tags

You can tag versions with:

```
docker tag talk-demo-node talk-demo-node:10
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
