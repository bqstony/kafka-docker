# How to build arm32v7 (Raspberry) kafka broker image

## Change docker

change from alpine apk installer to debian apt [see](https://wiki.onap.org/display/DW/Migrating+Dockerfiles+from+Debian+apt+to+Alpine+apk)

use base image of  arm32v7/openjdk:8u212-jre-alpine

##Build on raspberry 3 for kafka broker 2.3.0

```
docker build --build-arg build_date=$(date -u +"%Y-%m-%dT%H:%M:%SZ") -t bqstony/wurstmeister-arm32v7-kafka:2.12-2.3.0 .
```

