# Docker Build Example

**SAP ID:** 590014609

This folder demonstrates two ways to run an Nginx web server with Docker:

- `Dockerfile` builds an Ubuntu-based image and installs Nginx.
- `compose.yaml` starts the official Nginx image with Docker Compose.

## Build and run the Dockerfile image

From this directory, run:

```bash
docker build -t theory-nginx .
docker run --rm -p 8082:80 theory-nginx
```

Open [http://localhost:8082](http://localhost:8082) in a browser.

## Run with Docker Compose

```bash
docker compose up
```

The Compose configuration starts a container named `compose-nginx` and maps port `8082` on the host to port `80` in the container. Stop it with:

```bash
docker compose down
```
