# How to Build Docker Images

## `Dockerfile`

Building an image:

```
docker build -t php ./php
docker run php
```

```
docker build -t node ./node
docker run node
```

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
