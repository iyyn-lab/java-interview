# Java 11 + Spring Boot – Basics & Architecture

## 1. What is Java?

Java is a programming language commonly used to build backend applications, enterprise applications, APIs, and microservices.

For our learning:

```text
Java 11
   ↓
Spring Framework
   ↓
Spring Boot
   ↓
Backend Application / REST API
```

### Java 11

Java 11 is an **LTS (Long-Term Support)** version of Java.

Important Java 11 topics to know at a basic interview level:

* OOP concepts
* Classes and Objects
* Interfaces
* Inheritance
* Polymorphism
* Encapsulation
* Exception Handling
* Collections
* Streams
* Lambda Expressions
* Optional
* Generics
* Java 11 features

We can cover these separately.

---

# 2. What is Spring?

Spring is a Java framework used to build backend and enterprise applications.

Spring provides features such as:

* Dependency Injection
* Database integration
* Web/API development
* Security
* Transaction management
* Configuration
* Testing

One of the most important Spring concepts is:

**Dependency Injection (DI)**

---

# 3. What is Spring Boot?

Spring Boot is built on top of the Spring Framework.

It makes it easier to create and run Spring applications with less configuration.

Simple definition:

> **Spring Boot is a Java framework used to build production-ready backend applications and REST APIs quickly using the Spring Framework.**

For example:

```text
Next.js
   ↓
REST API
   ↓
Spring Boot
   ↓
PostgreSQL
```

It is similar to using NestJS as a backend framework in a TypeScript application.

```text
TypeScript → NestJS

Java       → Spring Boot
```

---

# 4. Why do we use Spring Boot?

Spring Boot helps developers build applications without manually configuring everything.

Common features include:

* REST APIs
* Dependency Injection
* Database connectivity
* Configuration management
* Exception handling
* Logging
* Monitoring
* Security
* Validation
* Microservices

---

# 5. Basic Spring Boot Architecture

A common Spring Boot application follows this structure:

```text
              Client / Frontend
                     │
                     │ HTTP Request
                     ↓
              ┌──────────────┐
              │  Controller  │
              └──────┬───────┘
                     │
                     ↓
              ┌──────────────┐
              │   Service    │
              └──────┬───────┘
                     │
                     ↓
              ┌──────────────┐
              │  Repository  │
              └──────┬───────┘
                     │
                     ↓
              ┌──────────────┐
              │   Database   │
              └──────────────┘
```

---