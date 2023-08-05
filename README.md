# Build

```
docker pull bellsoft/liberica-openjre-alpine-musl:20.0.2-10
mvn clean package
```

# Run

```
# run from jar file
mvn exec:java

# run from docker image
cd ${project-home-dir}/target
docker load -i jib-image.tar
docker run batzorigt.rentsen.rest-api-template
```
