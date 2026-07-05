# Biswaranjan Samal

**Senior Backend Engineer · Distributed Systems · Platform Engineering**

Building high-throughput, event-driven backend platforms for commerce, payments, and identity at scale.

---

## About Me

I design and operate production backend systems that power revenue-critical commerce, payments, and acquisition flows. My work sits at the intersection of distributed systems, API platforms, and reliability engineering — building services that stay fast and correct under real production load.

Currently focused on scalable microservices architecture, event-driven pipelines, API gateway design, and platform standardization that reduces cross-team engineering overhead.

- 4+ years building production backend systems across commerce, payments, notifications, and identity
- Led the first organization-wide Kong API Gateway rollout, standardizing auth, CORS, and rate limiting into shared plugins
- Owned auth infrastructure sustaining 500K+ requests/min at p99 under 100ms
- Architected omnichannel notification platform processing 1M+ messages/day

---

## Technology Stack

**Languages** — TypeScript, JavaScript, Node.js, Go, SQL, Python

**Backend** — NestJS, Express.js, HyperExpress, REST APIs, gRPC concepts, Clean Architecture, DDD

**Datastores** — MongoDB, PostgreSQL, Redis, ClickHouse

**Messaging & Data** — Kafka, KafkaJS, SQS, Trino, Airflow, dbt

**Cloud & Infra** — AWS, Kubernetes, Docker, Kong API Gateway, CAST AI, CI/CD, canary deployments

**Observability** — Datadog, Elastic APM, OpenTelemetry, Pino, structured logging

---

## Featured Projects

**[api-gateway](#)** — Plugin-based API gateway inspired by Kong. Reusable auth, CORS, and rate-limiting plugins with dynamic route configuration.

**[auth-service](#)** — Scalable authentication microservice with JWT rotation, OTP flows, Redis-backed sessions, and RBAC — modeled after 500K req/min production systems.

**[payment-gateway-abstraction](#)** — Multi-provider payment orchestration using the strategy pattern, idempotency keys, webhook reconciliation, and a PostgreSQL transaction ledger.

**[notification-platform](#)** — Kafka-driven omnichannel notification system with retries, DLQs, vendor failover, and delivery observability across email, SMS, and push.

**[distributed-rate-limiter](#)** — Redis-backed sliding window and token bucket rate limiter, deployable as a NestJS middleware or standalone service.

**[event-analytics-pipeline](#)** — Kafka to ClickHouse ingestion with Airflow-orchestrated reconciliation and Trino-based analytical queries.

---

## Engineering Philosophy

- **Design for failure.** Retries, idempotency, timeouts, and circuit breakers are not optional.
- **Own the system, not just the code.** Alerts, dashboards, and runbooks belong to the author.
- **Keep the boring parts sharp.** Clean logs, clear contracts, and small, reversible changes.
- **Optimize the platform, not the feature.** Reusable primitives compound across teams.
- **Trade-offs over trends.** Every choice has a cost — write it down in an ADR.

---

## System Design Interests

- Event-driven architecture, sagas, and the outbox pattern
- API gateway and service mesh design trade-offs
- Idempotency and exactly-once semantics in payment systems
- High-throughput authentication and session management
- OLTP/OLAP separation with Kafka, ClickHouse, and Trino
- Multi-tenant SaaS backend patterns and rollout strategies

---

## Open Source Interests

Contributing and following work in the NestJS, KafkaJS, ioredis, BullMQ, and Unleash ecosystems. Interested in improving developer experience around observability, resilience patterns, and API gateway plugins.

---

## Currently Learning

- Event sourcing and CQRS in production commerce systems
- OpenTelemetry-based distributed tracing at scale
- Rust for performance-critical backend components
- Advanced Kubernetes patterns: operators, controllers, and progressive delivery

---

## Contact

- Email — biswaranjan6286@gmail.com
- LinkedIn — [linkedin.com/Biswaranjan](https://www.linkedin.com/in/biswaranjan-samal-80b625212)
- GitHub — [github.com/your-username](https://github.com/your-username)
- Location — Noida, India

Open to Senior Backend Engineer and Platform Engineering conversations.
