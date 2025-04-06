# Podman Commands Cheat Sheet

## Pull syntax

Pulling an image from Docker.io

```Bash
podman pull docker.io/library/postgres
```

###### Note no trailing `/` in the URL; something like $`podman pull docker.io/library/postgres/` will throw an error.   

## Exec syntax

Executing a command in a container. 

### Synopsis

podman exec [options] container command [arg …]

```Bash
podman exec postgres /bin/sh -c 'exit 3'; echo $?
```

The following command opens up the container terminal in iterative mode.
```Bash
podman exec -it postgres
```