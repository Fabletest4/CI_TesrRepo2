# Backend Coding Standards

## Java Standards

- Use Java 21
- Use constructor injection
- Avoid field injection
- Prefer immutable DTOs

---

## Logging

Use structured logging:

```java
log.info("Fraud alert generated for transaction {}", transactionId);
