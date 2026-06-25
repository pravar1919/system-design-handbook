# System Design Handbook

> An open-source, production-quality handbook for learning system design — from computer fundamentals to designing real distributed systems. Written for everyone, from beginners taking their first steps to senior engineers preparing for interviews or sharpening their architecture skills.

[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## Why this handbook exists

Most system design resources fall into one of two traps: they are either shallow "interview cheat sheets" that teach you to pattern-match buzzwords, or dense academic papers that assume you already know everything. This handbook aims for the middle path that working engineers actually need:

- **First principles, not memorization.** Every concept is explained from the ground up, with the *why* behind the *what*.
- **Self-contained chapters.** Each file stands on its own. You can start anywhere. No chapter assumes you read another one first.
- **Production-grounded.** Real examples from how companies like Google, Amazon, Netflix, Uber, and Stripe actually build systems.
- **Honest about tradeoffs.** There are no silver bullets in distributed systems. Every chapter documents disadvantages and tradeoffs, not just benefits.

## How to use this handbook

- **New to the field?** Start with [Computer Fundamentals](00-computer-fundamentals/) and work through the numbered sections in order.
- **Preparing for interviews?** Jump to [Interviews](24-interviews/), and use the topic chapters as deep-dive references when you hit a gap.
- **Looking something up?** Use the table of contents below. Every chapter is a standalone reference.

Each chapter follows a [consistent template](TEMPLATE.md): difficulty, reading time, prerequisites, learning objectives, detailed explanations, ASCII + Mermaid diagrams, real production examples, advantages, disadvantages, tradeoffs, interview questions, misconceptions, implementation advice, and references.

### Difficulty legend

| Badge | Meaning |
|-------|---------|
| 🟢 Beginner | No prior system design knowledge assumed. |
| 🟡 Intermediate | Assumes comfort with the fundamentals (networking basics, databases, a programming language). |
| 🔴 Advanced | Assumes solid distributed systems grounding. Deep tradeoffs and edge cases. |

---

## Table of Contents

### Part I — Foundations

#### 00. Computer Fundamentals
- How computers execute programs, memory hierarchy, concurrency vs parallelism, latency numbers every engineer should know.

#### 01. Networking
- The OSI & TCP/IP models, TCP vs UDP, DNS, HTTP/1.1·2·3, TLS, WebSockets, gRPC.

#### 02. Operating Systems
- Processes & threads, scheduling, virtual memory, file systems, I/O models (blocking, non-blocking, epoll/io_uring).

### Part II — Storage & Data

#### 03. Databases
- Relational vs NoSQL, ACID, indexing, the transaction isolation levels, query planning, B-trees vs LSM-trees.

#### 04. Caching
- Cache strategies (cache-aside, read/write-through, write-behind), eviction policies, invalidation, CDNs.

#### 10. Replication
- Leader-follower, multi-leader, leaderless, synchronous vs asynchronous, replication lag.

#### 11. Sharding
- Partitioning strategies, consistent hashing, rebalancing, hotspots, the cross-shard query problem.

### Part III — Traffic & Edge

#### 05. Load Balancing
- L4 vs L7, algorithms, health checks, sticky sessions, global server load balancing.

#### 06. Reverse Proxies
- What they are, Nginx/Envoy/HAProxy, TLS termination, the proxy vs load balancer distinction.

#### 07. API Gateways
- Routing, authn/authz, rate limiting, the BFF pattern, gateway vs service mesh.

### Part IV — Distributed Systems

#### 08. Distributed Systems
- Fallacies of distributed computing, failure modes, time & clocks, idempotency, consensus (Paxos/Raft).

#### 09. Consistency & Consensus
- CAP theorem, PACELC, consistency models (linearizable → eventual), quorums.

#### 12. Event-Driven Architecture
- Events vs commands, pub/sub, event sourcing, choreography vs orchestration.

#### 13. CQRS & Saga
- Command/query separation, the saga pattern for distributed transactions, compensating actions.

#### 14. Messaging Systems
- Message queues vs logs, Kafka deep-dive, RabbitMQ deep-dive, delivery guarantees, backpressure.

#### 15. Redis
- Data structures, persistence (RDB/AOF), Redis as cache vs database, Cluster, common patterns.

### Part V — Infrastructure & Operations

#### 16. Containers & Orchestration
- Docker internals, Kubernetes architecture, pods/services/deployments, autoscaling.

#### 17. Cloud
- IaaS/PaaS/SaaS, regions & availability zones, object storage, serverless, multi-cloud tradeoffs.

#### 18. Security
- Authentication vs authorization, OAuth2/OIDC, JWT, encryption in transit & at rest, common attacks.

#### 19. Observability
- The three pillars (metrics, logs, traces), SLI/SLO/SLA, alerting, distributed tracing.

#### 20. Scaling
- Vertical vs horizontal, stateless design, capacity planning, back-of-the-envelope estimation.

### Part VI — Design Craft

#### 21. Design Patterns
- GoF patterns that matter for systems, plus distributed patterns (circuit breaker, bulkhead, retry/backoff).

#### 22. High-Level Design (HLD)
- The end-to-end design process, requirements → estimation → API → data model → architecture.

#### 23. Low-Level Design (LLD)
- Class design, SOLID, designing for testability, concurrency-safe components.

#### 24. Interviews
- A repeatable framework, worked examples (URL shortener, news feed, rate limiter, chat, etc.), evaluation rubrics.

---

## Status

This handbook is being built incrementally. Chapters are added and refined over time. See [CONTRIBUTING.md](CONTRIBUTING.md) if you'd like to help.

See [ROADMAP.md](ROADMAP.md) for the full file manifest, dependency graph, learning order, and milestones.

| Section | Status |
|---------|--------|
| 09. Consistency & Consensus → [CAP Theorem](09-consistency-and-consensus/01-cap-theorem.md) | ✅ Published |
| Everything else | 🚧 In progress |

## License

This work is licensed under [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](LICENSE). You are free to share and adapt the material, even commercially, as long as you give credit and share alike.

## Contributing

Contributions are welcome and encouraged. Please read [CONTRIBUTING.md](CONTRIBUTING.md) and follow the [chapter template](TEMPLATE.md).
