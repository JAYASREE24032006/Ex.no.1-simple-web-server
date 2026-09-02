# EX No: 01 – Simple Web Server Using Spring Boot

### Name : Jayasree R
### Register Number : 212223040074

## AIM
    <description>Demo project for Spring Boot Web Server</description>

    <parent>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-parent</artifactId>
        <version>3.1.2</version>
        <relativePath/>
    </parent>

    <dependencies>
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-web</artifactId>
        </dependency>
    </dependencies>

    <build>
        <plugins>
            <plugin>
                <groupId>org.springframework.boot</groupId>
                <artifactId>spring-boot-maven-plugin</artifactId>
            </plugin>
        </plugins>
    </build>

</project>
```

### DemoApplication.java

```java
package com.example.demo;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;

@SpringBootApplication
public class DemoApplication {

    public static void main(String[] args) {
        SpringApplication.run(DemoApplication.class, args);
    }
}
```

### HelloController.java

```java
package com.example.demo;

import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;

@RestController
public class HelloController {

    @GetMapping("/hello")
    public String sayHello() {
        return "Hello, Spring Boot!";
    }
}
```

### application.properties

```properties
server.port=8080
```

---

## OUTPUT

 <img width="657" height="444" alt="image" src="https://github.com/user-attachments/assets/95e9b9db-009e-43e3-b82a-7740153a00b6" />

## RESULT

Thus, a Simple Web Server using Spring Boot that can handle basic HTTP requests and return appropriate responses through RESTful endpoints was developed and executed successfully.
