<div align="center">

# Uday Kiran

### Backend Engineer • Systems Builder • Product Developer

Building scalable backend systems, payment infrastructure, and production-grade products.

<img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&size=24&duration=3000&pause=1000&center=true&vCenter=true&width=700&lines=Backend+Engineering;Distributed+Systems;Payment+Infrastructure;Cloud+%26+DevOps;Flutter+%2B+Node.js;Building+Products+That+Scale" />

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge\&logo=linkedin\&logoColor=white)](https://www.linkedin.com/in/uday-kiran-73a727233/)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge\&logo=vercel\&logoColor=white)](https://udaykrn.vercel.app)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge\&logo=gmail\&logoColor=white)](mailto:udaykiran9147@gmail.com)

</div>

---

## Engineering Philosophy

I enjoy building systems that remain reliable under failure, maintainable under growth, and simple to operate in production.

My work focuses on backend engineering, distributed workflows, payment systems, real-time communication, and cloud infrastructure. From designing immutable ledger systems to deploying production applications on AWS, I enjoy taking ownership from architecture to deployment.

---

## Engineering Map

## System Architecture
 
```text
┌─────────────────────────────────────────────────────────────────────┐
│                          CLIENT LAYER                                │
│  ┌───────────────┐   ┌───────────────┐   ┌───────────────┐          │
│  │    Flutter    │   │  React / Next │   │   Admin Web   │          │
│  │  (Riverpod)   │   │   (SSR/CSR)   │   │   Dashboard   │          │
│  └───────┬───────┘   └───────┬───────┘   └───────┬───────┘          │
└──────────┼───────────────────┼───────────────────┼──────────────────┘
           │                   │                   │
           └─────────┬─────────┴─────────┬─────────┘
                      ▼                   ▼
           ┌─────────────────────────────────────┐
           │        API GATEWAY / NGINX           │
           │   Rate Limiting · TLS · Load Balance │
           └───────────────────┬───────────────────┘
                                ▼
           ┌─────────────────────────────────────┐
           │             AUTH LAYER                │
           │   JWT · Refresh Rotation · RBAC       │
           │   Multi-Actor Sessions (3-role)       │
           └───────────────────┬───────────────────┘
                                ▼
     ┌──────────────────────────────────────────────────────────┐
     │                   APPLICATION SERVICES                     │
     │        Node.js · TypeScript · Express (Modular Monolith)   │
     │                                                              │
     │  ┌───────────┐ ┌───────────┐ ┌───────────┐ ┌────────────┐ │
     │  │  Orders    │ │ Payments  │ │ Discovery │ │ Messaging  │ │
     │  │  Service   │ │  Ledger   │ │  GeoSearch│ │  WebSocket │ │
     │  └─────┬──────┘ └─────┬─────┘ └─────┬─────┘ └─────┬──────┘ │
     └────────┼──────────────┼─────────────┼─────────────┼────────┘
              ▼              ▼             ▼             ▼
     ┌──────────────┐ ┌─────────────┐ ┌───────────┐ ┌───────────┐
     │   BullMQ      │ │  Razorpay   │ │  $geoNear │ │ Socket.io │
     │ Queues/Retry  │ │  Route API  │ │  + Cache  │ │  Pub/Sub  │
     └───────┬───────┘ └──────┬──────┘ └─────┬─────┘ └─────┬─────┘
             │                │              │              │
             └────────┬───────┴──────┬───────┴──────┬───────┘
                       ▼              ▼              ▼
           ┌─────────────────┐ ┌─────────────┐ ┌─────────────┐
           │      Redis       │ │  MongoDB /  │ │  Firebase   │
           │  Cache · Streams │ │  PostgreSQL │ │ Auth/FCM/   │
           │  Pub/Sub         │ │  Ledger DB  │ │  Storage    │
           └─────────────────┘ └─────────────┘ └─────────────┘
                       │              │              │
                       └──────┬───────┴──────┬───────┘
                              ▼               ▼
                 ┌─────────────────────────────────────┐
                 │          INFRASTRUCTURE LAYER          │
                 │  Docker · AWS EC2 · Nginx · GitHub CI  │
                 │  Observability · Horizontal Scaling    │
                 └─────────────────────────────────────┘
```
 
---
 
## Current Focus
 
| Area                    | Technologies                                |
| ------------------------ | -------------------------------------------- |
| ⚙️ Backend Engineering  | Node.js, TypeScript, Express                 |
| 🌐 Frontend / Web        | React, Next.js, Tailwind CSS                 |
| ☁️ Infrastructure       | Docker, AWS EC2, Nginx                       |
| 📦 Distributed Systems  | Redis, Queues, Event-Driven Design           |
| 💳 Financial Systems    | Payments, Ledgers, Idempotency               |
| 📱 Mobile Platforms     | Flutter, Riverpod, Offline-First Apps        |
| 🚀 DevOps               | GitHub Actions, CI/CD                        |
 
---

## Tech Stack

### Languages

<p>
<img src="https://skillicons.dev/icons?i=java,typescript,javascript,dart,python,cpp" />
</p>

### Backend

<p>
<img src="https://skillicons.dev/icons?i=nodejs,express,redis" />
</p>

```text
REST APIs
JWT Authentication
RBAC
WebSockets
BullMQ
Event-Driven Architecture
System Design
```

### Databases

<p>
<img src="https://skillicons.dev/icons?i=mongodb,postgresql,mysql,firebase" />
</p>

### Mobile

<p>
<img src="https://skillicons.dev/icons?i=flutter,firebase" />
</p>

```text
Riverpod
Freezed
FCM
Clean Architecture
Offline-First Systems
```

### Infrastructure

<p>
<img src="https://skillicons.dev/icons?i=docker,aws,githubactions,linux,nginx" />
</p>

---

# Featured Systems

## 🏪 Locaura — Hyperlocal Marketplace Infrastructure

A complete marketplace ecosystem connecting consumers, retailers, and delivery riders.

### Architecture

```text
Consumer / Retailer / Rider
            │
            ▼
     JWT Auth Layer
            │
            ▼
      Express APIs
            │
    ┌───────┼────────┐
    ▼       ▼        ▼
 Orders  Payments  Discovery
    │       │         │
    ▼       ▼         ▼
 BullMQ  Ledger   GeoSearch
    │       │         │
    └──► Redis ◄──────┘
            │
            ▼
        MongoDB
```

### Highlights

* Multi-actor authentication architecture
* Razorpay Route split payout engine
* Immutable ledger system
* Redis caching layer
* BullMQ retry queues
* Exactly-once webhook processing
* Geospatial retailer discovery
* AWS deployment pipeline

**Stack:** Node.js • TypeScript • MongoDB • Redis • BullMQ • Docker • AWS

---

## 📝 SmartKalam

Real-time handwriting digitization platform.

### Architecture

```text
Paper Input
      │
      ▼
  Flutter App
      │
      ▼
    IsarDB
      │
      ▼
 Sync Engine
      │
      ▼
 Socket Layer
      │
      ▼
 Backend APIs
```

### Impact

* Reduced peak server load by 30%
* Supported 10,000+ local records
* Offline-first synchronization
* Real-time communication pipeline
* Improved resilience under unstable networks

---

## 🏠 Leazo

Rental marketplace platform.

### Contributions

* Backend architecture ownership
* Authentication and RBAC
* Redis caching strategy
* Payment integrations
* Flutter mobile application
* Production deployment

---

## 👥 Squad

Group planning platform for friends and communities.

### Highlights

* Subscription infrastructure
* Team monetization flows
* PostgreSQL backend design
* Flutter mobile experience
* End-to-end product ownership

---

# Engineering Impact

```text
✓ Built a complete marketplace infrastructure
✓ Designed payment routing and settlement workflows
✓ Implemented immutable ledger systems
✓ Reduced server load by 30%
✓ Supported 10,000+ offline records
✓ Deployed production applications to AWS
✓ Built event-driven backend architectures
✓ Shipped production Flutter applications
```

---

# Interests

```text
Backend Engineering
Distributed Systems
Financial Infrastructure
System Design
Reliability Engineering
Cloud Infrastructure
Developer Tooling
Real-Time Systems
```

---

# Tech Radar

```text
Backend Engineering      ████████████████████
System Design            ██████████████████
Flutter                  ██████████████████
Database Design          █████████████████
DevOps                   ███████████████
Cloud Infrastructure     ██████████████
Distributed Systems      █████████████
```

---

# GitHub Analytics

<div align="center">

<img height="180em" src="https://github-readme-stats.vercel.app/api?username=Uday-kiran9147&show_icons=true&theme=tokyonight&hide_border=true&count_private=true"/>

<img height="180em" src="https://github-readme-streak-stats.herokuapp.com/?user=Uday-kiran9147&theme=tokyonight&hide_border=true"/>

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Uday-kiran9147&layout=compact&theme=tokyonight&hide_border=true"/>

</div>

<div align="center">

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Uday-kiran9147&theme=tokyo-night&hide_border=true"/>

</div>

---

# Currently Learning

```text
Distributed Systems
Cloud Native Infrastructure
Observability
Scaling Patterns
Database Internals
Reliability Engineering
```

---

# Connect

<div align="center">

🌐 Portfolio
https://udaykrn.vercel.app

💼 LinkedIn
https://www.linkedin.com/in/uday-kiran-73a727233/

📧 Email
[udaykiran9147@gmail.com](mailto:udaykiran9147@gmail.com)

</div>

---

<div align="center">

### Building reliable systems, scalable products, and software that lasts.

</div>
