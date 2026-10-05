# Hi, I'm Nithin 👋

**Java backend developer** · Spring Boot · Spring Security · Microservices<br>
📍 Greater Toronto Area · Open to Java backend and application support roles

I build secure, well-tested Spring services and like understanding *why* the framework behaves the way it does, from the filter chain down to the bean lifecycle.

---

## 🔐 Featured project: [SecurePay — Payment Security Journey](https://github.com/Nithin900/PaymentSecurityJourney)

A payment system split into four Spring Boot services, secured end to end with OAuth 2.0 and JWT.

```
Client ──login──► Auth Server :9000 ──JWT──► Client
Client ──Bearer JWT──► Gateway (A) :8080 ──token relay──► Payment (B) :8081 ──► DB
                                                   │ client_credentials JWT
                                                   ▼
                                     Notification :8082 ──► SMTP
```

- **Spring Authorization Server** issues RS256-signed JWTs (authorization code + client credentials flows)
- **Scope-based access** per HTTP method; **ownership enforced** from the token's `sub` (other users get 404)
- **Zero-trust between services** — B re-validates every token instead of trusting the gateway
- **Resilience** — WebClient timeouts, 503 when downstream is unreachable, email failure never fails a payment
- **Consistent error contract** (400 / 404 / 409 / 502 / 503) via `GlobalExceptionHandler`
- **25+ automated end-to-end checks** plus unit tests with `@MockitoBean`

`Java 17` `Spring Boot 3.5` `Spring Security 6.5` `Spring Authorization Server` `JPA / H2` `WebClient` `Maven` `GitHub Actions`

🌐 [Interactive explainer site](https://nithin900.github.io/PaymentSecurityJourney/) — a request traced hop by hop through the real code

---

## 🧩 Also worth a look

| Project | What it shows |
|---|---|
| [Spring Core Fundamentals](https://github.com/Nithin900/Fundementals-spring-core) | DI (XML / Java / annotations), bean scopes and lifecycle, and an AOP module with custom aspects for timing, security, audit, retry and per-invocation trace IDs |
| [Health Care Price Tool](https://github.com/Nithin900/Health-Care-Price-Tool) | Python + Flask app serving a scikit-learn insurance price model |

---

## 🛠 Tech

**Backend:** Java (8–21) · Spring Boot · Spring Security · OAuth 2.0 / JWT · JPA / Hibernate · REST · Kafka<br>
**Data:** Oracle · MySQL · SQL Server · H2<br>
**Ops & debugging:** OpenShift · Kibana · JVM thread dumps · Maven · Git · GitHub Actions<br>
**Also:** Python · Pandas · scikit-learn · Tableau · Power BI

---

## 📫 Reach me

[LinkedIn](https://www.linkedin.com/in/nithinarumbakam)
