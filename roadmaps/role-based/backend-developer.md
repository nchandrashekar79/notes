---
title: Backend Developer Roadmap
---

# Backend Developer

Build reliable APIs and services that store, protect, and move data.

[← Role based roadmaps](README.md) | [All roadmaps](../README.md)

## What a backend developer does

A backend developer designs the server-side systems behind an application: APIs, data models, authentication, business rules, background work, and the infrastructure that keeps them healthy. The work requires both writing code and reasoning about failure.

## Start here

- [ ] Build a small API with at least one persistent resource
- [ ] Validate input and return useful error responses
- [ ] Write tests for the success and failure paths
- [ ] Run the application from a repeatable setup

## Learning stages

### 1. Language and runtime

Pick one backend language and learn it well.

- Types, collections, functions, modules, and error handling
- Concurrency or asynchronous work in your chosen runtime
- Package management, environment variables, and configuration
- Debugging and reading stack traces
- Database and file system access

**Build:** a command-line tool that imports a CSV, validates it, and stores clean records.

### 2. HTTP and API design

- HTTP methods, status codes, headers, and content negotiation
- REST resource modeling and predictable URLs
- Request validation and structured error responses
- Versioning, pagination, filtering, and idempotency
- Authentication and authorization
- OpenAPI descriptions and generated client types

**Build:** a documented API with create, read, update, and delete operations plus pagination.

### 3. Data and persistence

- Relational modelling, keys, indexes, and transactions
- SQL queries and query plans
- Schema migrations and safe changes
- Caching and cache invalidation
- Background jobs, retries, and idempotent processing
- Backups and restore testing

**Build:** add a schema migration and a background job that can safely retry after failure.

### 4. Security and reliability

- Input handling and parameterized queries
- Password hashing and secure session management
- Secrets management and least privilege
- Rate limits, timeouts, and bounded retries
- Structured logging, metrics, and traces
- Health checks and graceful shutdown
- Threat modelling for the service boundary

**Build:** write a failure scenario, such as a slow dependency or invalid request, and show how logs and metrics reveal it.

### 5. Delivery and operations

- Automated tests at the API and integration level
- Continuous integration and reproducible deployments
- Containers and environment configuration
- Database changes during deployment
- Load testing and capacity assumptions
- Alerting based on user-visible symptoms

**Build:** deploy the API with automated tests and document how to roll back a release.

## Definition of done

You can design and ship a tested API with a persistent data model, secure authentication, useful observability, and a deployment process you can explain.

## Related roadmaps

- [Python](../skill-based/python.md)
- [Git and GitHub](../skill-based/git-and-github.md)
- [Portfolio project](../projects/portfolio-project.md)

## FAQ

### SQL or NoSQL?

Learn relational modelling and SQL first. They transfer to many systems and force you to reason about consistency and data shape. Choose a document or key-value store when its access patterns genuinely fit the problem.

[↑ Catalog](README.md) | [← Category index](README.md)
