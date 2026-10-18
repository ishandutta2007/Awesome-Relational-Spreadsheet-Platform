# Awesome-Relational-Spreadsheet-Platform

## Top Relational Spreadsheet Platform Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Database-Backed Grids, Python Formulas & Self-Hosted Data Sovereignty*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Relational Spreadsheet Platforms**. These tools combine the familiar grid interface of a spreadsheet with the structural rigor of a relational database — linked records, typed columns, granular permissions, and API access — turning fragile "final_v3_FINAL.xlsx" workflows into load-bearing applications.

**Examples** include Airtable, Smartsheet, Monday.com, SmartSuite, Notion, Coda, Quickbase, ClickUp, Google Tables, and Rows (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, Python-powered automation, and transparent SQLite/Postgres storage — ideal for operations teams prioritizing data ownership, developers building internal tools, and organizations escaping per-seat pricing and record caps.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Airtable](https://www.airtable.com/)**  
  **The reference relational spreadsheet platform** that defined the category. Grid, Kanban, Calendar, Gallery, and Form views over linked tables with a large template ecosystem. **Free tier caps records per base and users**; paid plans scale per-seat with higher record limits. **Limitations**: **No full-database export** — each table must be exported individually as CSV, losing relational structure [citation:8]. Data lives only in Airtable's cloud with no self-hosting path [citation:9].

- **[Smartsheet](https://www.smartsheet.com/)**  
  Enterprise work management with spreadsheet-style grids, Gantt views, and automation. Strong for project and program management with compliance-oriented controls.

- **[Monday.com](https://monday.com/)**  
  Work OS with customizable boards, automations, and dashboards. Broader than pure relational data — focused on workflow and project tracking with database-like structures.

- **[SmartSuite](https://www.smartsuite.com/)**  
  No-code work management platform with relational tables, multiple views, and automation. Positioned between Airtable and project management tools.

- **[Notion](https://www.notion.com/)**  
  All-in-one workspace with databases that support relations, rollups, and multiple views. **Weaker relational integrity than dedicated database tools** — better for lightweight structured content than mission-critical operations.

- **[Coda](https://coda.io/)**  
  Doc-platform with tables, formulas, buttons, and automations. Strong formula language and pack ecosystem, blending document and database paradigms.

- **[Quickbase](https://www.quickbase.com/)**  
  Enterprise no-code platform for building custom business applications with relational databases, forms, and workflow automation.

- **[ClickUp](https://clickup.com/)**  
  Productivity platform with ClickUp Tables providing database-like views over tasks and custom fields. Broader work management than pure relational spreadsheet.

- **[Google Tables](https://tables.google.com/)**  
  Google's structured data workspace with automation and AI-powered features, integrated with Google Workspace.

- **[Rows](https://rows.com/)**  
  Spreadsheet with built-in data integrations and API connectors. Stronger on data pulling than relational modeling.

## Open-Source GitHub Projects

- **[Grist](https://github.com/gristlabs/grist-core)**  
  **The most database-native open-source relational spreadsheet** — Apache 2.0 licensed, self-hostable on-prem, private cloud, or Docker [citation:1]. **Combines spreadsheet flexibility with true relational structure**: linked records across tables, strict column typing, and **full Python formulas including standard library imports** — not just Excel-style functions [citation:1][citation:8]. **Data ownership is exceptional**: every document is a portable **SQLite file**, so backups are simple file copies and migration between hosts is trivial [citation:13][citation:14]. **Granular permissions** down to row and column level, audit trails, and SAML/SSO support [citation:1]. **REST API, webhooks, and custom widgets** for extending with your existing stack [citation:1]. **No vendor lock-in** — export your entire relational structure as a single `.grist` file openable in any SQLite tool [citation:8]. **Best for teams wanting a genuine database with a spreadsheet UI**, especially in regulated or air-gapped environments [citation:1].

- **[NocoDB](https://github.com/nocodb/nocodb)**  
  **The most flexible database-connector approach** — turns **any existing PostgreSQL, MySQL, or SQL Server database into a smart spreadsheet** without migrating data [citation:2][citation:9]. **Grid, form, kanban, calendar, and gallery views** with collaboration, permissions, and comments [citation:2]. **Auto-generated REST API** over your data, plus webhooks and Zapier integration [citation:2]. **Metadata stored in an external PostgreSQL database**; application data stays in your existing database [citation:2]. **Critical differentiator**: even if you remove NocoDB, **the underlying database remains fully usable** — no framework dependency [citation:9]. **Best for teams with existing databases** wanting a spreadsheet UI without data migration. **Note**: dashboard and advanced chart features are cloud-only [citation:9].

- **[Baserow](https://github.com/baserow/baserow)**  
  **The compliance-focused open-core option** — MIT licensed for all non-premium features, with **GDPR, HIPAA, and SOC 2 Type II compliance** and **150,000+ users** [citation:3]. **Spreadsheet-database hybrid** with applications, portals, automations, dashboards, and an **AI Assistant (Kuma)** for natural-language database creation [citation:3]. **Self-hosted with no storage restrictions**, built on Django, Vue.js, and PostgreSQL [citation:3]. **Full data ownership and infinite scalability** without vendor lock-in [citation:3]. **Best for organizations needing compliance certifications** alongside self-hosting.

- **[Teable](https://github.com/teableio/teable)**  
  **The Postgres-native "no-code Postgres"** — AGPL-3.0 licensed, **21,100+ GitHub stars** [citation:4]. **Every workspace runs on real PostgreSQL** — **no row limits, no query slowdowns at scale, and full SQL compatibility** when you need it [citation:4]. **AI database agent** creates tables, relationships, and workflows from plain English [citation:4]. **Real-time collaboration** with live cursor tracking [citation:4]. **Grid, Kanban, Calendar, Gallery, and Form views** included on every plan [citation:4]. **Self-hosting requires 2-4 CPU cores, 4-8 GB RAM** [citation:4]. **Enterprise Edition adds AI, authority matrix, and automation** [citation:10]. **Best for teams wanting Airtable UX with genuine Postgres underneath** for scale beyond 100K rows.

- **[Undb](https://github.com/undb-io/undb)**  
  **The privacy-first, single-file self-hosted option** — **SQLite and local object storage by default**, requiring **just one file** to persist data [citation:6][citation:12]. **Power BI-like record-level security** [citation:6]. **Multiple views**: grid, kanban, gantt, tree, calendar [citation:6]. **OpenAPI, webhooks, real-time subscriptions, and ERD preview** [citation:6]. **Lightweight and self-hosted in seconds** [citation:6]. **Caution**: **early-stage development, not recommended for production use** — demo data clears on redeploy [citation:12]. **Best for experimentation and privacy-focused prototyping** where SQLite portability matters.

- **[Rowy](https://github.com/rowyio/rowy)**  
  **The Firebase/Firestore-native low-code backend** — **Airtable-like UI on top of Google Cloud Firestore** [citation:5][citation:18]. **Cloud Functions in JavaScript/TypeScript** triggered by field changes [citation:18]. **30+ field types** including rich editors, uploaders, and action fields [citation:18]. **Data and functions stay in your own GCP project** — Rowy's Cloud Run instance operates exclusively on your project and does not store your data [citation:18]. **Best for teams already on Firebase/GCP** wanting a spreadsheet interface over Firestore.

### Additional Strong Open-Source Options

- **SeaTable** — Open-source collaborative spreadsheet/database hybrid with self-hosting options. Frequently compared alongside Grist, NocoDB, and Baserow [citation:1].
- **APITable** — Open-source API-first database with spreadsheet UI, self-hostable.
- **Rowy Run** — Backend services (rowy-backend, rowy-hooks) deployed into your GCP project for derivatives, action scripts, and webhooks [citation:5].
- **NocoDB Cloud** — Managed option for teams wanting NocoDB without infrastructure management, with additional dashboard features [citation:9].

**Frameworks for building custom systems**: Combine **Grist** for database-native relational modeling with Python formulas and SQLite portability, **NocoDB** for a spreadsheet UI over existing PostgreSQL/MySQL without migration, **Baserow** for compliance-certified self-hosting with AI assistance, **Teable** for Postgres-native scale beyond Airtable's row limits, and **Undb** for privacy-first single-file prototyping — to build a relational data layer tailored to your existing infrastructure, compliance requirements, and scale targets.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Relational spreadsheet platforms differ significantly in data ownership, formula power, and scale ceiling. **Airtable cannot export full databases** — only per-table CSVs, losing relational structure [citation:8]. **Grist stores documents as portable SQLite files** and supports full Python, not just Excel-style formulas [citation:1][citation:13]. **NocoDB connects to existing databases without migration** — removing NocoDB leaves the database fully usable [citation:9]. **Teable runs on real PostgreSQL** with no row limits, but self-hosting requires 4-8 GB RAM [citation:4]. **Undb is early-stage and not production-ready** — demo data clears on redeploy [citation:12]. **Rowy's data and functions stay in your GCP project**, but it requires Firebase/Firestore [citation:18].
- Self-hosted open-source solutions require proper database backups, TLS configuration, and access control management. Grist's SQLite portability makes backups trivial; Postgres-backed options require standard database backup practices.

---

**Made for operations teams, data managers, no-code builders, and developers building relational data applications.**
Let's make relational spreadsheets more open, data-sovereign, and formula-powerful.
