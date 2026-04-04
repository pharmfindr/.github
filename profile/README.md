# PharmFindr

### The Intelligence Platform for Pharmaceutical Outsourcing

*Find, evaluate, and compare CDMOs — all in one place.*

[![Platform Status](https://img.shields.io/badge/Status-Building%20MVP-yellow?style=flat-square)](https://github.com/PharmFindr)
[![License](https://img.shields.io/badge/License-Proprietary-red?style=flat-square)](./LICENSE)
[![Frontend](https://img.shields.io/badge/Frontend-v0.1.3-blue?style=flat-square)]()
[![API Gateway](https://img.shields.io/badge/API%20Gateway-v0.0.4-blue?style=flat-square)]()
[![Auth Service](https://img.shields.io/badge/Auth%20Service-v0.0.4-blue?style=flat-square)]()
[![User Service](https://img.shields.io/badge/User%20Service-v0.0.2-blue?style=flat-square)]()
[![Company Service](https://img.shields.io/badge/Company%20Service-v0.0.3-blue?style=flat-square)]()
[![Admin Service](https://img.shields.io/badge/Admin%20Service-v0.0.3-blue?style=flat-square)]()
[![Company Enrichment Worker](https://img.shields.io/badge/Company%20Enrichment%20Worker-v0.0.2-blue?style=flat-square)]()
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-v0.1.2-blue?style=flat-square)]()
[![Redis](https://img.shields.io/badge/Redis-v0.0.1-blue?style=flat-square)]()

---

## What is PharmFindr?

PharmFindr is a **pharmaceutical outsourcing intelligence platform** — think *Yelp meets G2 for CDMOs*. We're solving a critical gap in the industry: pharma companies currently rely on scattered directories and expensive consultants to find and evaluate Contract Development and Manufacturing Organizations (CDMOs).

We centralize **FDA compliance data**, **verified peer reviews**, and **capability-based filtering** into one searchable platform — giving drug developers the transparency they need to make confident outsourcing decisions.

---

## Core Features

| Feature | Description |
|---|---|
| **Smart Search** | Filter CDMOs by molecule type, dosage form, country, and service stage |
| **FDA Compliance Data** | Integrated 483 inspection history, cGMP status, and regulatory flags |
| **Verified Reviews** | Confidentiality-aware peer reviews built around NDA/CDA constraints |
| **Side-by-Side Comparison** | Compare up to 3 CDMOs simultaneously across capability and compliance metrics |
| **Global Coverage** | CDMOs across USA, EU, India, China, and more |

---

## Platform Architecture

PharmFindr is built on a **7-microservice backend** designed for flexibility and scale:

```
┌─────────────────────────────────────────────────────┐
│                    API Gateway                      │
├─────────────────────────────────────────────────────┤
│                   Auth Service                      │
│         (Login · Logout · Registration · OAuth)     │
├──────────┬──────────┬──────────┬────────────────────┤
│  User    │ Company  │  Review  │  Discovery Service │
│ Service  │ Service  │ Service  │  (Search + Compare)│
├──────────┴──────────┴──────────┴────────────────────┤
│        Notification Service  │  Admin Service       │
└─────────────────────────────────────────────────────┘
```

**Tech Stack**

- **Frontend:** React.js + shadcn/ui
- **Backend:** Golang microservices
- **Databases:** PostgreSQL · MongoDB · Redis
- **Auth:** JWT dual-token system with Google & LinkedIn OAuth

---

## Platform Scope

**Molecule Types**
- Small Molecules (Solid oral, Soft gel, Parenteral, Formulation platforms)
- Large Molecules / Biologics

**Service Coverage**
- Drug Substance (API) manufacturing
- Drug Product manufacturing
- Early clinical → Late phase → Commercial scale
- Analytical & testing services

**Geographic Reach**
- 🇺🇸 USA · 🇨🇦 Canada · 🇲🇽 Mexico
- 🇬🇧 UK · 🇫🇷 France · 🇮🇪 Ireland · 🇵🇱 Poland · 🇪🇸 Spain · 🇮🇹 Italy · 🇵🇹 Portugal
- 🇵🇷 Puerto Rico · 🇮🇳 India · 🇨🇳 China

---

## Roadmap

- [x] Core platform architecture defined
- [x] MVP wireframes & requirements
- [ ] 150–200 CDMO profiles onboarded
- [ ] 100–200 verified users
- [ ] 50+ peer reviews collected
- [ ] CRO & analytical lab expansion
- [ ] RFP management module
- [ ] Full compliance monitoring dashboard

---

## Contributing & Partnerships

We're actively looking for:

- **CDMO partners** to join as founding listed organizations
- **Pharma professionals** to beta test and submit verified reviews
- **Industry advisors** with outsourcing or regulatory expertise

Interested? Reach out via [GitHub Discussions](../../discussions) or open an issue.

---

<div align="center">

*PharmFindr — Bringing transparency to pharmaceutical outsourcing.*

</div>
