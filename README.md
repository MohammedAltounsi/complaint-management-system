<div align="center">

**English** · [العربية](README.ar.md)

</div>

# Complaints Management SaaS

A multi-tenant, Arabic-first customer-complaints platform for Saudi e-commerce — from intake to
resolution to monthly reporting, with the critical cases never buried.

**🔗 Live demo:** https://complaints-saas-demo.vercel.app
**Login:** `cs@demo.local` / `demodemo1234`

Built and designed end to end by **Mohammed Altounsi** — [LinkedIn](https://www.linkedin.com/in/mohammed-altounsi/)

---

## Screenshots

| Dashboard | Complaint detail | Reports |
|---|---|---|
| ![Dashboard](screenshots/dashboard.png) | ![Complaint detail](screenshots/complaint.png) | ![Reports](screenshots/reports.png) |

## What it does

- **Emergency queue** — critical complaint types float above everything else
- **SLA tracking** — response deadlines per complaint; overdue cases flagged automatically
- **Smart routing** — each complaint routed to the responsible team (factory / quality / customer service)
- **Compensation log** — every resolution and its compensation recorded and reportable
- **Reporting** — breakdowns by city, type, and product + a live operations dashboard
- **Salla integration** — order data via webhooks, nightly reconcile as backstop

## Stack

`Next.js 16 (App Router, Server Actions)` · `Supabase / Postgres` · `Vercel` · `TypeScript` · `Tailwind` · `PostHog (EU)`

## Security

- Row-Level Security isolates every tenant at the database layer
- Complaint photos via signed, expiring URLs — no public buckets
- Strict CSP; `frame-ancestors 'none'` blocks clickjacking of destructive actions
- Integration tokens encrypted at rest (AES-GCM, per-tenant key)
- No production source maps; framework version header suppressed

---

> Source code is private — this repository is a showcase. For a walkthrough or a demo tailored to your
> store, reach me on [LinkedIn](https://www.linkedin.com/in/mohammed-altounsi/).
