# Wordsmith API

Wordsmith is the demo project originally from [dockersamples/wordsmith](https://github.com/dockersamples/wordsmith)

The demo app runs across three containers:

- **[api](Dockerfile)** - a Java REST API which serves words read from the database
- **[web](https://github.com/bretfisher/wordsmith-web)** - a Go web application that calls the API and builds words into sentences
- **db** - a Postgres database that stores words

## Architecture

![Architecture diagram](architecture.excalidraw.png)

## Build and run in Docker Compose

The only requirement to build and run the app from source is Docker. Clone this repo and use Docker Compose to build all the images. You can use the new V2 Compose with `docker compose` or the classic `docker-compose` CLI:

```shell
docker compose up --build
```

Or you can pull pre-built images from Docker Hub using `docker compose pull`.
