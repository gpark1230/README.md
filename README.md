# Hi there 👋 I'm Gavin 🏀
Backend Engineer | Python · FastAPI · PostgreSQL | APIs, Data Pipelines & Distributed Services

I build backend services in Python — REST APIs with real authentication, normalized relational
schemas, ETL pipelines, and async services that talk to each other over queues.

I came into backend engineering from the security side. While running an access review at an
accounting firm, I found a service credential ten people were sharing. Instead of rotating it,
I replaced the integration with an authenticated internal API — and that project is what moved
me from IT into software engineering.

## 🙋🏻‍♂️ About Me
🎓 B.A. in Computer Science, Business Minor, Boston University
💻 Software Engineer, Internal Applications at KLCP LLP
🔒 CompTIA Security+
☁️ Microsoft Certified: Azure Fundamentals (AZ-900)
📍 New York
🔍 **Open to backend engineering roles — NYC or remote**

I'm interested in the parts of backend work where correctness actually matters: authentication
and access control, transactional integrity, idempotent retries, and knowing what your system
does when a dependency is down. My security background is why I care about getting those right.

## 🚀 Projects

### 🛡️ [IncidentDesk](https://github.com/gpark1230/incidentdesk) — Security Incident Tracking API
A REST API for tracking security incidents, with a full audit trail.
- 10+ endpoints in FastAPI with JWT authentication
- 3-tier RBAC (viewer / analyst / admin) enforced server-side
- Append-only audit logging with diff-based change tracking
- Alembic migrations verified upgrade *and* downgrade in CI
- PostgreSQL · SQLAlchemy · Docker · pytest · GitHub Actions · Railway

### 📡 [IncidentRelay](https://github.com/gpark1230/incidentrelay) — Async Notification Service
A separately deployed worker service that consumes IncidentDesk events over a Redis queue.
- Exponential-backoff retries (3 attempts, 10s/30s/90s) with idempotent attempt records
- Token-bucket rate limiter implemented as an atomic Redis Lua script — no check-then-set race
- Read-through cache with event-driven invalidation, measured at a 91.4% hit rate
- Service-to-service auth with a least-privilege service account and cached JWTs
- FastAPI · Redis · RQ · PostgreSQL · Docker · GitHub Actions · Railway

## 🛠️ Technical Skills

### Backend
- Python
- FastAPI
- REST API design
- SQLAlchemy
- Alembic
- Pydantic
- ETL pipeline design
- Redis
- RQ / task queues
- Caching
- Rate limiting

### Databases
- PostgreSQL
- Schema design
- Relational modeling
- Migrations
- Indexing

### Testing & Infrastructure
- pytest
- Fixtures & parametrized tests
- Integration testing against live databases
- Docker
- Docker Compose
- GitHub Actions
- CI/CD
- Linux
- Git

### Authentication & Security
- OAuth2
- JSON Web Tokens (JWT)
- Role-based access control (RBAC)
- Audit logging
- Least privilege
- MFA / SSO
- Microsoft Entra ID
- Secrets management

### Languages
- Python
- SQL
- Bash

📬 Contact
Email: [gpark1230@gmail.com](mailto:gpark1230@gmail.com)
LinkedIn: [My LinkedIn](https://www.linkedin.com/in/gavinpark123/)
