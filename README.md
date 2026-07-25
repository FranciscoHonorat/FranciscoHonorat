# Francisco Honorat | Full Stack Developer

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=28&duration=3000&pause=1000&color=5B8CFF&center=true&vCenter=true&width=620&height=60&lines=Full+Stack+Developer;Go+%26+Node.js+Backends;Clean+%26+Hexagonal+Architecture;Production-Ready+Code" alt="Typing SVG" />

## About Me

Backend-focused full stack developer building services in **Go** and **Node.js / TypeScript**. I like taking a fuzzy requirement, drawing the boundaries, and shipping something maintainable on the other side.

Most of my recent work lives on the backend: Go microservices talking over **gRPC**, event-driven flows with **RabbitMQ**, and a full observability pipeline built on **Redis Streams** and **TimescaleDB**. I model data with PostgreSQL, MongoDB and Redis, and build the front when a project needs one, usually **React**.

I care about the fundamentals that don't show up in a demo but decide whether a system survives contact with production: clear architecture boundaries, validation, idempotency, and observability. When it matters, I go down to the metal, profiling Go allocations with escape analysis to keep the hot path off the heap.

## Tech Stack

**Backend**
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Gin](https://img.shields.io/badge/Gin-008ECF?style=for-the-badge&logo=gin&logoColor=white)
![gRPC](https://img.shields.io/badge/gRPC-244c5a?style=for-the-badge&logo=google&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)

**Frontend**
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)

**Data & Messaging**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white)

**DevOps & Tools**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

## GitHub Stats

<img height="180em" src="https://github-readme-stats.vercel.app/api?username=FranciscoHonorat&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true" alt="GitHub Stats"/>
<img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=FranciscoHonorat&layout=compact&theme=tokyonight&hide_border=true" alt="Top Languages"/>

> *"Quod est superius est sicut quod est inferius."*
> As above, so below. — Hermes Trismegistus, *The Emerald Tablet*

## Featured Projects

### OrderFlow, Analytics Platform *(in progress)*

Order-management platform with a real-time analytics pipeline, built to apply high-performance distributed-systems concepts in practice: Clean Architecture, DDD, the OLTP vs OLAP split, and modern orchestration. Current focus is the domain core, including a hands-on Escape Analysis study of the `Money` value object, measuring heap vs stack allocation and GC impact with Go's native benchmarking tools.

Stack: `Go` · `PostgreSQL` · `ClickHouse` · `Apache Kafka` · `Redis` · `Kubernetes`
[Repository »](https://github.com/FranciscoHonorat/Hermes-OrderFlow-Analytics-Platform)

### Movies API, Go Microservices

Movie REST API split into two services: an HTTP API Gateway (Gin) and a gRPC Movies Service, communicating over Protobuf. Hexagonal architecture with swappable MongoDB / DynamoDB (LocalStack) adapters, event-driven creation via RabbitMQ (async POST returning 202 Accepted), Swagger docs, seven Kubernetes manifests and 20 unit tests. Organized as a Go workspace.

Stack: `Go` · `gRPC` · `RabbitMQ` · `MongoDB` · `DynamoDB` · `Kubernetes`
[Repository »](https://github.com/FranciscoHonorat/Hermes-Movies)

### Hermes Observability Platform

Observability for Node.js apps: an instrumentation agent SDK, collector, processor and a React dashboard. Metrics flow through Redis Streams and persist in TimescaleDB, with threshold-based email alerts. Counter, Gauge and Histogram metric types, auto-instrumentation of runtime signals, and a clearly bounded MVP scope. Built as an npm-workspaces monorepo.

Stack: `Node.js` · `TypeScript` · `Redis Streams` · `TimescaleDB` · `React`
[Repository »](https://github.com/FranciscoHonorat/Hermes-Observability-Platform)

### Books API, Go REST

REST API in Go for managing a book collection, with filtering, pagination and sorting. Clean handler / service / repository layering, PostgreSQL with sqlc, Prometheus metrics, rate limiting, TLS, CORS, structured logging (slog) and graceful shutdown. Ships with a Postman collection and full Docker setup.

Stack: `Go` · `Gin` · `PostgreSQL` · `sqlc` · `Prometheus` · `Docker`
[Repository »](https://github.com/FranciscoHonorat/Hermes-Books-API)

### Mundo Invest, Go Backend

Customer-management REST API in Go with a simulated Pipefy integration over GraphQL. Hexagonal architecture (ports & adapters), async event publishing to RabbitMQ, idempotent webhooks, SQLite persistence and Kubernetes manifests. Includes a production-design section mapping the stack to AWS (Lambda, SQS, RDS / DynamoDB) and a NoopPublisher for graceful degradation without a broker.

Stack: `Go` · `GraphQL` · `RabbitMQ` · `SQLite` · `Kubernetes`
[Repository »](https://github.com/FranciscoHonorat/Hermes-Customers)

## Expertise

**Go Backends.** Microservices, gRPC + Protobuf, hexagonal architecture, event-driven design, allocation profiling with escape analysis.

**Node.js & TS.** REST APIs, validation, rate limiting, Swagger docs, SDK design.

**Architecture.** Clean & Hexagonal Architecture, SOLID, DDD, testability.

**Data & Messaging.** PostgreSQL, MongoDB, Redis Streams, TimescaleDB, RabbitMQ, caching strategy.

**Security.** Input validation, rate limiting, TLS, CORS, idempotency, graceful shutdown.

**DevOps.** Docker, Kubernetes, Prometheus, CI/CD, Git workflows.

## Let's Connect

[LinkedIn](https://www.linkedin.com/in/francisco-jefferson-batista-honorato/) · [GitHub](https://github.com/FranciscoHonorat) · [jeffhonorato230@gmail.com](mailto:jeffhonorato230@gmail.com)

---

*Always learning, always building.*
