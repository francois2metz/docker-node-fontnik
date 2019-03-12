# docker-node-fontnik

Dockerfile for [node-fontnik](https://github.com/mapbox/node-fontnik)

## Build image

You can build a docker image with the following `docker build` command.

```
docker build -t docker-node-fontnik .
```

## Pull image

You can pull a docker image with the following `docker pull` command.

```
docker pull francois2/fontnik
```

Docker Hub page is [here](https://cloud.docker.com/repository/docker/francois2/fontnik).

## Usage

By default the entrypoint use `build-glyphs`.

    docker run --rm --tty --interactive --volume $(pwd):/data --workdir /data francois2/fontnik ./fonts/open-sans/OpenSans-Regular.ttf ./glyphs
