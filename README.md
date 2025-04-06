# Podman Commands Cheat Sheet

## Pull syntax

Pulling an image from Docker.io

```Bash
podman pull docker.io/library/postgres
```

###### Note no trailing `/` in the URL; something like $`podman pull docker.io/library/postgres/` will throw an error.   
