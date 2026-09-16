# 1. Interview Quick Revision

### Spring Boot

**What is Spring Boot?**

Spring Boot is a Java framework built on Spring that simplifies the development of production-ready applications and REST APIs.

### Architecture

**What is the basic Spring Boot architecture?**

```text
Controller
    ↓
Service
    ↓
Repository
    ↓
Database
```



### Dependency Injection

**What is DI?**

Dependency Injection means providing required dependencies to a class instead of the class creating them itself.

### Bean

**What is a Bean?**

A Bean is an object managed by the Spring Container.

### Controller

**What does Controller do?**

It handles HTTP requests and responses.

### Service

**What does Service do?**

It contains business logic.

### Repository

**What does Repository do?**

It handles database-related operations.

### Configuration

**Where can Spring Boot configuration be stored?**

Commonly in:

```text
application.properties
application.yml
```



### Logging

**Why do we use logging?**

To understand application activity, debugging information, warnings, and errors.

### Monitoring

**Why do we use monitoring?**

To check application health and performance.

### Exception Handling

**Why do we use exception handling?**

To handle errors properly and return meaningful responses to clients.

# 2. Quick Annotation Summary


| Annotation              | Main Purpose                       |
| ----------------------- | ---------------------------------- |
| `@Controller`           | Handles web requests               |
| `@RestController`       | Handles REST APIs                  |
| `@Service`              | Business logic                     |
| `@Repository`           | Database/data access               |
| `@Autowired`            | Dependency Injection               |
| `@Bean`                 | Creates a Spring-managed Bean      |
| `@Configuration`        | Defines configuration              |
| `@ExceptionHandler`     | Handles exceptions                 |
| `@ControllerAdvice`     | Common exception handling          |
| `@RestControllerAdvice` | Common REST API exception handling |


---



# 3. Complete Simple Architecture

```text
                    Client
                      │
                      ↓
               ┌─────────────┐
               │ Controller  │
               │ @RestController
               └──────┬──────┘
                      ↓
               ┌─────────────┐
               │   Service   │
               │   @Service  │
               └──────┬──────┘
                      ↓
               ┌─────────────┐
               │ Repository  │
               │ @Repository │
               └──────┬──────┘
                      ↓
                  Database


         Spring Container
                │
                ↓
        Dependency Injection
                │
        ┌───────┴────────┐
        ↓                ↓
      Beans          Configuration
                       │
                       ↓
              application.properties


Errors
  ↓
Exception Handling
  ↓
@RestControllerAdvice


Application Activity
  ↓
Logging
  ↓
Monitoring / Actuator
```

---

# 4. Main Things to Remember

```text
Spring Boot
    ↓
Build Java Backend Applications
    ↓
Controller
    ↓
Service
    ↓
Repository
    ↓
Database

Spring Container
    ↓
Manages Beans
    ↓
Dependency Injection

Configuration
    ↓
application.properties / application.yml

Logging
    ↓
Application events and errors

Monitoring
    ↓
Application health and performance

Exception Handling
    ↓
Consistent error responses
```

> **For the interview, first understand the responsibility of each layer and annotation. Don't try to memorize all the code.**



