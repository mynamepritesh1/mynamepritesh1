<h1 align="center">Pritesh Ingale</h1>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1200&color=2F81F7&center=true&vCenter=true&width=720&lines=Java+Backend+Engineer;Distributed+Systems+%26+Microservices;Solo+architect+of+ZenWorks+HRMS;Spring+Boot+%C2%B7+Kafka+%C2%B7+Redis+%C2%B7+AWS" alt="Typing intro" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/pritesh-ingale-1902b6105/"><img src="https://img.shields.io/badge/LinkedIn-Pritesh_Ingale-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:pritesh1272@gmail.com"><img src="https://img.shields.io/badge/Email-Get_in_touch-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <img src="https://img.shields.io/badge/Thane,_Mumbai-India-555555?style=for-the-badge&logo=googlemaps&logoColor=white" alt="Location" />
</p>

---

## 👋 About me

Java backend engineer with **5+ years** building REST APIs, event-driven microservices and distributed systems on **Spring Boot, Kafka, Redis and AWS**.

- 🛫 **Today:** SDE-II at **Accelya**, working on **ONO**, an offer-and-order airline commerce platform for Finnair: order lifecycle, ticketing, ancillaries, 24×7 production, strict SLAs.
- 🏗️ **On the side:** founder and sole architect of **ZenWorks HRMS**, a multi-tenant SaaS platform with an LLM-powered resume-matching pipeline.
- ⚡ **What I'm good at:** finding why an API is slow and fixing it (N+1 queries, caching, indexing, pagination), and owning services end to end, from schema design to deployment.
- 🤖 **How I work:** I use AI-assisted tools (Cursor, Copilot, Windsurf) to move faster, and I keep full ownership of architecture and code quality.

---

## 🛠️ Tech stack

**Languages & frameworks**

<img src="https://skillicons.dev/icons?i=java,spring,hibernate,ts&perline=8" alt="Languages and frameworks" />

**Data, messaging & caching**

<img src="https://skillicons.dev/icons?i=mysql,postgres,redis,kafka,rabbitmq&perline=8" alt="Data and messaging" />

**Cloud & DevOps**

<img src="https://skillicons.dev/icons?i=aws,docker,jenkins,linux,maven,gradle,git&perline=8" alt="Cloud and DevOps" />

**Observability**

<img src="https://skillicons.dev/icons?i=grafana,prometheus&perline=8" alt="Observability" />

<details>
<summary><b>Full skill list</b></summary>

| Area | Details |
|---|---|
| Backend | Spring Boot 2.x/3.x, Spring MVC, Spring Security, Spring Cloud Gateway, Hibernate/JPA, QueryDSL, MapStruct, Resilience4j |
| Architecture | Microservices, event-driven architecture, API gateway, DDD, multi-tenancy, system design |
| Security | OAuth 2.0, JWT (RS256), RBAC, TOTP MFA, WebAuthn, SCIM 2.0 |
| Migrations | Liquibase, Flyway |
| Quality & perf | JMeter, SonarQube, Swagger/OpenAPI 3.0, TDD, code review |
| AI engineering | LangChain4j, OpenAI GPT-4 APIs, prompt engineering |

</details>

---

## 🚀 Featured project: ZenWorks HRMS

A multi-tenant SaaS HRMS backend that I'm designing and building solo from scratch.

```mermaid
flowchart LR
  C[Clients] --> G[Spring Cloud Gateway]
  G --> A["zen-auth<br/>RS256 JWT · MFA · WebAuthn · SCIM"]
  G --> E[Employee Service]
  G --> AI["AI Module<br/>LangChain4j"]
  A --> R[(Redis)]
  E --> P[(PostgreSQL)]
  E --> S3[(AWS S3)]
  E -- events --> K{{Kafka}}
  AI --> L[OpenAI GPT-4]
```

| Service | What it does |
|---|---|
| **zen-auth** | RS256 JWT with refresh-token rotation, Redis-based token blacklisting, TOTP MFA, OAuth 2.0, WebAuthn, SCIM 2.0 provisioning |
| **Employee Service** | PostgreSQL + Flyway migrations, Kafka event publishing, S3 document storage, MapStruct mapping, JPA Specifications for dynamic filtering |
| **AI Module** | Prompt-orchestrated pipeline for resume parsing and candidate–job matching (LangChain4j + GPT-4); exploring pgvector for embedding-based search |

**Stack:** Java 17 · Spring Boot 3.x · PostgreSQL · Redis · Kafka · Spring Cloud Gateway · Resilience4j · Flyway · AWS · Docker · LangChain4j

> 🔗 [Repo / write-up: add link]

---

## 💼 Experience

| Period | Role | What I did |
|---|---|---|
| Apr 2026 – now | **SDE-II, Accelya** | ONO (offer & order) platform for Finnair; production defect triage in a 24×7 regulated environment; root-cause analysis across a multi-service architecture; legacy modernization |
| Apr 2024 – Apr 2026 | **Software Engineer, Daten & Wissen** (client: Keva Flavours) | Sole backend engineer on a global fragrance-industry SaaS; 40+ REST APIs; performance work; EU regulatory instance with ECHA / IUCLID 6 integration; zero-downtime Jenkins pipelines |
| Nov 2021 – Apr 2024 | **Software Engineer, Job Circle** | Sole backend owner of four microservices (Job Apply, Referral, ATS, Leave Management) on a live recruitment platform; Kafka, Redis, AWS |
| Sep – Nov 2021 | **Freelance Full-Stack Java Developer** | FoodBox ordering platform: Spring Boot + Angular, Razorpay webhooks, Docker + Jenkins |

---

## 🔧 Selected engineering work

<details>
<summary><b>⚡ Fixing N+1 bottlenecks on a global SaaS platform</b></summary>

- **Problem:** high-traffic endpoints on a globally deployed platform were slow because of N+1 queries.
- **Approach:** Redis caching, MySQL composite indexing, cursor-based pagination.
- **Result:** substantially lower API latency across the affected endpoints.
<!-- Add your real before/after numbers here, e.g. p95 from X ms to Y ms. -->

</details>

<details>
<summary><b>🇪🇺 Isolated EU instance with regulatory API integration</b></summary>

- Dedicated European deployment with ECHA / IUCLID 6 integration.
- Isolated schema of 20+ tables, with data separation enforced via Spring Cloud Gateway routing.
- 40+ REST APIs secured with Spring Security RBAC; DEV/UAT/PROD Spring Profiles; Liquibase schema versioning.

</details>

<details>
<summary><b>🧩 Breaking a JSP monolith into microservices (VCMP)</b></summary>

- Decomposed a JSP monolith into two Spring Boot 3.x services.
- Replaced synchronous calls with Kafka event streams.
- Secured access with OAuth 2.0 / JWT through Spring Cloud Gateway.

</details>

<details>
<summary><b>👥 Recruitment platform microservices (Job Circle)</b></summary>

- Four independent services owned end to end, from schema design to deployment on AWS (EC2, RDS, S3).
- Keyword-based job matching, referral workflow, Kafka-driven async notifications, Redis session caching.
- Docker + Jenkins CI/CD; Flutter mobile client for the platform.

</details>

---

## 📊 GitHub stats

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=mynamepritesh1&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub stats" />
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=mynamepritesh1&layout=compact&theme=tokyonight&hide_border=true" alt="Top languages" />
</p>

---

## 📫 Let's connect

- 💼 [LinkedIn](https://www.linkedin.com/in/pritesh-ingale-1902b6105/)
- ✉️ [pritesh1272@gmail.com](mailto:pritesh1272@gmail.com)
- 📍 Thane, Mumbai, India · English, Hindi, Marathi

<p align="center"><sub>Built with Java, caffeine and a lot of Kafka topics.</sub></p>
