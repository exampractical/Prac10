
# Practical 10 - Monolithic Application Using Spring Boot

## MonolithDemoApplication.java

```java
import org.springframework.boot.*;
import org.springframework.boot.autoconfigure.*;
import org.springframework.web.bind.annotation.*;

@SpringBootApplication
@RestController
public class MonolithDemoApplication {

    public static void main(String[] args) {
        SpringApplication.run(MonolithDemoApplication.class, args);
    }

    @GetMapping("/")
    public String home() {
        return "Hello Monolithic World!";
    }
}
```
