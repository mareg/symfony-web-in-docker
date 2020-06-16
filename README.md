# symfony-web-in-docker

This set up comes with pre-configured database and yarn watch running continuously in the docker container.

## Installation

Install composer dependencies:
```bash
$  docker run --rm -it -v `pwd`:/app -w /app composer install
```

Install front-end dependencies:
```bash
$ docker run --rm -it -v `pwd`:/app -w /app node yarn install
```

Build docker container:
```bash
$ docker-compose build
```

## Running docker env

Start docker env:
```bash
$ docker-compose up -d
```

Stop docker env:
```bash
$ docker-compose down
```
