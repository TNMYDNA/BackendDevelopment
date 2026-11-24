# Docker Bind Mount Example

This folder demonstrates how to share a file from the host machine with a Docker container using a bind mount.

## Files

- `test.txt` — a host file containing `Hello from Mac`.

## Run the example

From this directory, run:

```bash
docker run --rm \
  --mount type=bind,source="$(pwd)",target=/app,readonly \
  ubuntu:latest \
  cat /app/test.txt
```

Expected output:

```text
Hello from Mac
```

The folder is mounted at `/app` inside a temporary Ubuntu container. The `readonly` option prevents the container from modifying the host files, and `--rm` removes the container after the command finishes.
