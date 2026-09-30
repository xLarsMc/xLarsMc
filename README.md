# Leandro Henrique Oliveira Neves

**.NET Developer** · C# · ASP.NET Core · SQL Server / PostgreSQL · Angular

Jaboticabal, SP, Brazil · Open to remote work · Portuguese (native) · English (professional, used daily)

---

## About

.NET developer with 2 years of professional experience. I currently work as a consultant on a UK energy-sector SaaS product (ITIX, assigned to POWWR, Manchester), in English, with a predominantly British team. In parallel, I am a full-stack developer at Sanchez & Sanchez, building REST APIs and Angular front ends.

I build and maintain APIs and services in C# and .NET, integrate systems (HTTP, queues, SFTP, Azure services), write automated tests, and investigate production issues with centralised logs. I apply Clean Architecture, SOLID and DDD, and I use AI coding tools (Claude Code, Codex, Cursor) with critical review of everything they generate.

## Experience

| Role | What I do |
|---|---|
| **.NET Developer** · ITIX (consultant at POWWR, UK) | Features and fixes on a white-label energy-contracting portal (C#, ASP.NET, SQL Server), Azure integrations, scheduled and queue jobs, production diagnostics, Git Flow and Azure DevOps Pipelines, Kanban with Jira. |
| **Full-Stack Developer** · Sanchez & Sanchez | REST APIs in .NET 6 (EF Core, PostgreSQL), Angular 16 interfaces, SignalR notifications instead of polling, RPA/automation with Selenium and direct HTTP integrations, xUnit tests in CI (GitHub Actions), Jenkins builds with Kubernetes/Portainer deployments. |

## Tech stack

| Area | Technologies |
|---|---|
| Languages | C#, TypeScript, JavaScript, SQL |
| Back end | .NET / .NET Framework, ASP.NET Core, Entity Framework Core, Node.js, SignalR |
| Front end | Angular, React |
| Data | SQL Server, PostgreSQL, MongoDB, Redis, SQLite |
| Messaging | RabbitMQ |
| Architecture | Clean Architecture, Hexagonal, DDD, CQRS, SOLID, REST |
| Cloud / DevOps | Azure (DevOps, Pipelines, Key Vault, Blob Storage), Docker, GitHub Actions, Jenkins, Kubernetes, Git Flow |
| Testing | xUnit, NUnit, Moq, Playwright, Vitest |

## Projects

> Most of my recent work lives in **private repositories** (client and personal projects), so the code is not public. I am happy to walk through the architecture and the code in an interview.

### Private projects

**WhatsApp broadcast platform for a medical clinic** *(private, delivered to a client)*
A system that lets clinic staff send appointment notices to patients one by one, each with the correct scheduling link for the patient's city.
- Back end in **.NET 8** (Clean Architecture) with PostgreSQL and Redis; **React + TypeScript** front end; WhatsApp delivery through Evolution API, with the architecture ready to switch to the official Meta API.
- Patient import from Excel with a preview (valid, rejected with reason, duplicated); message templates with per-patient fields.
- Anti-ban rules: 50 messages per 24 h, random 47–173 s interval, one message per device, per-topic "already received", automatic opt-out.
- **LGPD** for health data: mandatory login, masked phone numbers, data export/correction/anonymisation/deletion, audit trail, retention policy, encrypted daily backup.
- Docker-based delivery (one script starts everything), unit, integration (real PostgreSQL in Docker) and E2E (Playwright) tests, CI on every pull request.

**Promotions monitor** *(private, personal project)*
A desktop app that watches supermarket flyers and electronics deals, matches them against a wish list and posts the relevant ones to WhatsApp groups. Runs fully local.
- **TypeScript, Electron, Node.js, SQLite**; Google Gemini (vision for flyers and PDFs, plus a relevance judge that removes semantic false positives) and a custom text parser for Telegram deals.
- Design rules: hard daily send limit with atomic quota reservation, AI cost control (post-ID cache, `Last-Modified` cache), store allowlist and anti-SSRF protections, exhaustive audit logging.
- Built with TDD: about **1,130 tests** and **95%+ coverage**.

### Public repositories

| Project | Stack | Highlights |
|---|---|---|
| [**Microsservices-Messageria**](https://github.com/xLarsMc/Microsservices-Messageria) | .NET 8, RabbitMQ, MySQL, JWT | E-commerce microservices (Product, Cart, Coupon, Order, Payment, Email) communicating through RabbitMQ queues. |
| [**HotelBooking**](https://github.com/xLarsMc/HotelBooking) | .NET 8, EF Core, MediatR, NUnit | Hexagonal architecture and DDD, CQRS, booking state machine, payment provider adapters. |
| [**Projeto-FullStack**](https://github.com/xLarsMc/Projeto-FullStack) | .NET 8, PostgreSQL, xUnit, Docker | Layered API with FluentValidation, i18n error messages, unit and integration tests, SonarCloud in CI. |
| [**Desafio-API-simples-de-Clientes**](https://github.com/xLarsMc/Desafio-API-simples-de-Clientes) | .NET 8, EF Core, SQLite | Customer CRUD API built as a time-boxed challenge, with Clean Architecture. |
| [**Projeto-Final-BackEnd**](https://github.com/xLarsMc/Projeto-Final-BackEnd) | Node.js, Express, MongoDB | Blog API with JWT authentication, roles and Swagger docs. |

Earlier academic work (Node.js/React, design patterns, C, Java) is also available in my repositories.

## Education

Associate degree in Systems Analysis and Development, Federal University of Technology – Paraná (UTFPR), 2022–2025. Udemy certifications: Microservices with Hexagonal Architecture, DDD, TDD, CQRS and SOLID (2026); Microservices Architecture with ASP.NET, .NET 6 and C# (2025).

## Contact

- LinkedIn: [linkedin.com/in/leandro-neves-lhoneves](https://www.linkedin.com/in/leandro-neves-lhoneves)
- Email: [leandrohenriquetti@gmail.com](mailto:leandrohenriquetti@gmail.com)
