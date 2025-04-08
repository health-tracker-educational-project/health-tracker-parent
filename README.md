# Health Tracker parent library.
## How to connect ?
### 1. Add this parent to your pom instead of default.
#### pom.xml:
```
    <parent>
        <groupId>com.healthtracker</groupId>
        <artifactId>healthtracker-parent</artifactId>
        <version>1.0.0</version>
    </parent>
```
### 2. If you have dependencies that exists in parent, version can be deleted.
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