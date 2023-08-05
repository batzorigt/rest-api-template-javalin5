# Build

```
docker pull bellsoft/liberica-openjre-alpine-musl:20.0.2-10
mvn package
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

# Eclipse
```
https://projectlombok.org/setup/eclipse
https://ebean.io/docs/getting-started/eclipse-ide
https://mapstruct.org/documentation/ide-support/
```

# IntelliJ IDEA

```
https://projectlombok.org/setup/intellij
https://ebean.io/docs/getting-started/intellij-idea
https://mapstruct.org/documentation/ide-support/
```
