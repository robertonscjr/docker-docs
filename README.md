## Build image
```bash
$ cd app-dir
$ ls
Dockerfile ...

$ docker build --tag=$IMAGE_NAME .
```

## Save image
```bash
$ docker save --output $IMAGE_FILE $IMAGE_NAME
```

## Load image
```bash
$ docker load --input $IMAGE_FILE
```

## Run image
```bash
$ docker run --rm -v $VOLUME_NAME:$CONTAINER_DIR $IMAGE_NAME
```

or

```bash
$ docker run --rm -v $HOST_DIR:$CONTAINER_DIR $IMAGE_NAME
```

- -v: volume flag
- --rm: remove container after running
