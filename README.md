# Biswaranjan Samal

**Senior Backend Engineer — Distributed Systems · Platform Engineering · Commerce & Payments**

Noida, India

---

## About

Senior Backend Engineer with 4+ years of experience designing and operating large-scale backend platforms and distributed systems. My work spans identity, commerce, payments, notifications, CRM automation, and analytics — with a strong focus on scalability, event-driven architecture, and production reliability.

I care about the parts of engineering that survive scale: clear service boundaries, safe rollouts, idempotent workflows, and observability that makes production debuggable at 2 AM.

- 4+ years of production backend engineering across commerce, payments, identity, and platform systems
- Deep experience with Node.js, TypeScript, NestJS, MongoDB, Redis, Kafka, PostgreSQL, ClickHouse, and Kubernetes
- Led organization-wide platform initiatives including the first Kong API Gateway rollout
- Comfortable owning services end-to-end: design, implementation, deployment, on-call, and iteration

---

## Professional Platform Experience

These platforms were designed and developed as part of my professional experience. Due to intellectual property and confidentiality agreements, the implementation is private. The descriptions below summarize the architecture, engineering challenges, and business impact.

### Ambassador Platform — ₹250Cr+ revenue

Referral-driven acquisition platform with onboarding, KYC, assisted sales, commission calculation, and payout orchestration.

- **Architecture:** NestJS microservices with MongoDB, Redis, Kafka, and S3; event-driven attribution to decouple sales ingestion from commission and payout processing
- **Challenges:** Concurrent sales attribution, commission consistency under peak traffic, and idempotent event handling
- **Impact:** Attributed ₹250Cr+ in revenue and supported 3x MAU growth across acquisition funnels

### Refer & Earn Platform — ₹100Cr+ revenue

Referral, reward, and coupon-attribution system integrated with acquisition, orders, and notifications.

- **Architecture:** Event-driven referral tracking on Kafka with Redis-backed dedup and cache layers
- **Challenges:** Reliable attribution across delayed events, fraud-resistant referral windows, and cross-service consistency
- **Impact:** Contributed ₹100Cr+ in revenue and reduced manual reward operations

### Identity & Authentication Platform — 500K+ req/min

High-throughput authentication platform for login, OTP, registration, and user journeys.

- **Architecture:** Node.js, TypeScript, HyperExpress, MongoDB, Redis, Kafka on Kubernetes (CAST AI spot capacity) with rate limiting and cache-first user lookups
- **Challenges:** Sustaining p99 under 100ms at 500K+ requests/min while balancing cost and reliability
- **Impact:** Stable auth availability across peak traffic events with disciplined incident response

### Omnichannel Notification Platform — 1M+ notifications/day

Multi-channel notification platform spanning push, SMS, WhatsApp, and email.

- **Architecture:** Kafka topics per channel with asynchronous workers, vendor failover, retries, DLQs, template caching in Redis, and delivery tracking in MongoDB
- **Challenges:** Vendor variability, at-least-once delivery, dedup, and reliable observability across channels
- **Impact:** Processed 1M+ notifications/day at greater than 99.9% delivery success

### Payments & Order Management Platform

Modular payment, coupon, wallet, invoice, and order platform integrating multiple payment providers.

- **Architecture:** NestJS services with MongoDB, Redis, PostgreSQL/Prisma, Kafka, and SQS; strategy-based gateway abstraction for Razorpay, Paytm, Juspay, ICICI, Apple IAP, and CSC Wallet
- **Challenges:** Idempotent transactions, webhook reconciliation, distributed locking, and gateway-agnostic checkout flows
- **Impact:** Reliable checkout across providers with reduced gateway-specific coupling and improved reconciliation

### Kong API Gateway — Organization-wide rollout

First Kong API Gateway implementation in the organization, standardizing cross-cutting concerns across microservices.

- **Architecture:** Centralized authentication, CORS, rate limiting, and routing as reusable plugins; declarative route and plugin management
- **Challenges:** Zero-downtime migration, plugin ordering, and coordinated adoption across independent service teams
- **Impact:** Eliminated duplicated cross-cutting logic and standardized API security, governance, and onboarding for all backend services

### Analytics, Reporting & Event Automation Platform

Analytics and reconciliation pipelines for payments, orders, engagement, and acquisition events.

- **Architecture:** Kafka to ClickHouse ingestion with Trino for federated queries and Airflow-orchestrated batch reconciliation
- **Challenges:** Separating OLTP from OLAP paths, ensuring pipeline reliability, and automating fee attribution and CRM triggers across 10M+ user profiles
- **Impact:** Automated reporting and reconciliation while reducing manual operational effort for finance and operations teams

---

## Featured Personal Projects

### LIMS-APP

A modern **Laboratory Information Management System (LIMS)** designed for **Testing, Inspection & Certification (TIC)** laboratories, digitizing the complete lifecycle from client onboarding and sample intake to testing, quality approval, reporting, and invoicing.

Built to replace spreadsheet-driven operations with a scalable, multi-tenant platform supporting ISO/IEC 17025-compliant workflows, audit trails, barcode-based sample tracking, client self-service portals, and configurable testing protocols.

**Technologies**
- Node.js
- TypeScript
- NestJS
- Postgres
- Redis

**Engineering Highlights**
- Multi-tenant SaaS architecture with tenant isolation
- Modular NestJS architecture following Domain-Driven Design principles
- Role-Based Access Control (RBAC) and workflow-driven authorization
- Barcode-enabled sample lifecycle and chain-of-custody tracking
- Template-driven test protocol and report generation
- Audit logging for compliance and traceability
- RESTful APIs with DTO validation and repository pattern
- Redis-backed caching for frequently accessed reference data
- Extensible architecture for future instrument integrations and regulatory rule engines

### uweb-socket

A high-performance real-time WebSocket gateway built with **NestJS** and **uWebSockets.js**, designed to deliver low-latency, event-driven communication for interactive applications.

The gateway consumes Kafka event streams and efficiently broadcasts updates to connected clients, supporting real-time features such as chat, schedules, notifications, reactions, collaborative sessions, and dynamic event subscriptions.

**Technologies**
- Node.js
- TypeScript
- NestJS
- uWebSockets.js
- Kafka
- Redis

**Engineering Highlights**
- High-throughput WebSocket server optimized for low latency
- Kafka-driven event broadcasting
- Topic-based subscription management
- Connection lifecycle and session management
- Horizontal scalability with Redis
- Modular gateway architecture
- Production-ready logging, monitoring, and error handling

### omnichannel-notification

Personal exploration of an omnichannel notification service supporting multiple delivery channels through a pluggable vendor architecture.

- **Technologies:** Node.js, TypeScript, NestJS, Kafka, Redis
- **Concepts:** Event-driven fan-out, vendor strategy pattern, retry and DLQ handling, template management, and delivery observability

---

## Tech Stack

**Languages** — TypeScript, JavaScript, Node.js, Go, SQL, Python

**Backend** — NestJS, Express.js, HyperExpress, REST APIs, Clean Architecture, Domain-Driven Design

**Databases** — MongoDB, PostgreSQL, Redis, ClickHouse

**Messaging** — Kafka, KafkaJS, SQS, BullMQ

**Cloud** — AWS, Kubernetes, Docker, Kong API Gateway, CAST AI, CI/CD, canary deployments

**Observability** — Datadog, Elastic APM, OpenTelemetry, Pino, structured logging, alerting, dashboards

**Architecture** — Distributed Systems, Event-Driven Architecture, API Gateway Design, Caching, Idempotency, Fault Tolerance, High Availability

---

## Engineering Philosophy

- **Design for failure.** Retries, timeouts, idempotency, and circuit breakers are part of the design, not an afterthought.
- **Own the system, not just the code.** Alerts, dashboards, runbooks, and rollout plans belong to the author.
- **Clean architecture.** Clear boundaries between domain, application, and infrastructure — so the system stays changeable.
- **Reusable platforms.** Solve cross-cutting concerns once at the platform layer; every team benefits.
- **Simplicity over unnecessary complexity.** The best system is the smallest one that meets the SLA.

---

## Currently Learning

- Event Sourcing and its application in commerce and payment systems
- CQRS patterns for read/write separation at scale
- Rust for performance-critical backend components
- Advanced Kubernetes: operators, controllers, and progressive delivery
- Distributed tracing and OpenTelemetry-based observability

---

## Open Source Interests

Following and interested in contributing to work across:

- NestJS
- KafkaJS
- BullMQ
- OpenTelemetry
- Redis
- Kubernetes

Focus areas: reliability primitives, observability, and developer experience for backend platforms.

---

## Contact

- **Location** — Noida, India
- **LinkedIn** — [linkedin.com/Biswaranjan](https://www.linkedin.com/in/biswaranjan-samal-80b625212)
- **Email** — biswaranjan6286@gmail.com
- **GitHub** — [github.com/Biswaranjan](https://github.com/MrBiswa)

Open to conversations about Senior Backend Engineer and Platform Engineering roles.
