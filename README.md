# Build

```
docker pull bellsoft/liberica-openjre-alpine-musl:20.0.2-10
# build uber jar and docker image
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

# IntelliJ IDEA

```
https://projectlombok.org/setup/intellij
https://ebean.io/docs/getting-started/intellij-idea
https://mapstruct.org/documentation/ide-support/
```

# Eclipse
```
https://projectlombok.org/setup/eclipse
https://ebean.io/docs/getting-started/eclipse-ide
https://mapstruct.org/documentation/ide-support/
```

# Used Libraries

```
web framework: https://javalin.io/
configuration: https://matteobaccan.github.io/owner/
orm: https://ebean.io/
bean mappings: https://mapstruct.org/
templating: https://jte.gg/
validation: javalin built validators + custom bean validator using hibernate-validator
monitoring: micrometer plugin for prometheus
logging: log4j2
```

# Architecture & layer roles

```
Handlers: Receive http requests and validate request parameters or request body. Call services. Manage database transactions.
Services: Business logics
Domains: Data access layer
```
