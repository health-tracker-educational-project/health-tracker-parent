# Health Tracker parent library.

## Version
Current version: `v1.0.4`

## Dependencies

This library uses the following dependencies:

| Dependency                            | Group ID                       | Artifact ID                           | Notes           |
|----------------------------------------|--------------------------------|---------------------------------------|-----------------|
| Auth0 Java JWT                        | `com.auth0`                    | `java-jwt`                            |                 |
| HealthTracker Common                  | `com.healthtracker`            | `healthtracker-common`                |                 |
| Database Rider Spring                 | `com.github.database-rider`    | `rider-spring`                        | Test scope      |
| Preliquibase Spring Boot Starter      | `net.lbruun.springboot`        | `preliquibase-spring-boot-starter`    |                 |
| MapStruct                             | `org.mapstruct`                | `mapstruct`                           |                 |
| MapStruct Processor                   | `org.mapstruct`                | `mapstruct-processor`                 |                 |
| Lombok MapStruct Binding              | `org.projectlombok`            | `lombok-mapstruct-binding`            |                 |
| SpringDoc OpenAPI WebMVC UI Starter   | `org.springdoc`                | `springdoc-openapi-starter-webmvc-ui` |                 |

## How to connect ?
### 1. Pull this library and build it with next command:

`mvn clean install`
### 2. Add this parent to your pom instead of default.
#### pom.xml:
```
    <parent>
        <groupId>com.healthtracker</groupId>
        <artifactId>healthtracker-parent</artifactId>
        <version>1.0.4</version>
    </parent>
```
### 3. If you have dependencies that exists in parent, version can be deleted.
Like this:
```
<dependencies>
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-actuator</artifactId>
            // dependency exists in parent, thus it's not needed)
        </dependency>
</dependencies>
```
### 3. Group id also can be deleted, cuz it inherits from parent.
`<groupId>com.healthtracker</groupId>`
