# Aarch64 Loki and Docker Driver Plugin
You will need to first build Dockerfile-arm64 by using:
```
docker build -t loki-build-image:arm-1.0 .
```

Then you will use this image to build the docker logging driver plugin by using:
```
make docker-driver
```

The plugin will be created in your machine. You might need to enable it using:
```
docker plugin enable loki-driver:arm64
```