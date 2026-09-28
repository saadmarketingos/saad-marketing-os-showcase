# Saad Marketing OS — Public Showcase

> AI-native marketing decision and execution system for SMEs.

Saad Marketing OS turns fragmented business context into a structured operating loop for marketing: understand the situation, identify priorities, build an actionable 90-day plan, execute, measure outcomes, and learn.

This repository is a **sanitized public showcase**. The production codebase, internal AI methods, prompts, decision logic, customer data, infrastructure configuration, and security controls are intentionally private.

## The problem

Many SMEs run marketing through disconnected briefs, agencies, spreadsheets, social channels, dashboards and ad-hoc decisions. The result is often fragmented execution, unclear accountability, weak measurement and repeated decisions without a learning loop.

## The product

Saad Marketing OS provides a single operating workflow:

`Business Context → Evidence → Diagnosis → Priorities → 90-Day Plan → Human Review → Execution → Measurement → Learning`

The system is designed to support business owners and marketing teams with structured, evidence-aware decision support rather than generic content generation.

## What the private beta currently validates

- structured business onboarding and workspace separation;
- brief and evidence capture;
- AI-assisted diagnosis and planning;
- evidence/assumption separation and confidence handling;
- human review before recommendations become approved actions;
- 30/60/90-day execution planning;
- action ownership, KPI tracking and outcome logging;
- persistence and recovery across AI or workflow failures.

## Public demo

Open [`demo/index.html`](demo/index.html) locally in a browser. The demo uses **synthetic data only** and does not call any external service.

## Architecture — intentionally high level

```mermaid
flowchart LR
    A[Business Brief & Data] --> B[Evidence Layer]
    B --> C[AI Decision Layer]
    C --> D[Diagnosis & Priorities]
    D --> E[90-Day Plan]
    E --> F[Human Review]
    F --> G[Actions & KPIs]
    G --> H[Outcomes]
    H --> I[Learning Loop]
    I --> B
```

The public architecture deliberately omits proprietary orchestration, prompting, validation rules and production data models.

## Product principles

1. **Evidence before certainty** — missing information stays visible instead of being invented.
2. **Human approval for consequential decisions** — AI drafts do not automatically become approved business decisions.
3. **Execution over reports** — recommendations are converted into owned actions, KPIs and decision rules.
4. **Learning loop** — outcomes feed future decisions instead of disappearing into static reports.
5. **Tenant and data separation** — each business workspace is isolated in the production system.

## Technology profile

The private product uses a modern TypeScript/React web stack, managed authentication/data infrastructure and an LLM provider abstraction. Exact production configuration and integration details are private by design.

## Current stage

**Private beta / pilot validation.** The focus is validating one complete end-to-end workflow with real business use cases before broader rollout.

## Business model

Subscription software with optional assisted-execution service levels for businesses that need additional operational support.

## Repository disclosure policy

This repository does **not** contain:

- production source code;
- internal prompts or AI orchestration logic;
- proprietary evaluation/quality rules;
- production schemas, migrations or access policies;
- API keys, credentials or private endpoints;
- customer names, briefs, documents or metrics;
- internal pricing experiments or confidential commercial terms.

See [`docs/PUBLIC_DISCLOSURE.md`](docs/PUBLIC_DISCLOSURE.md) and [`SECURITY.md`](SECURITY.md).

## Private technical review

The production repository is private. Limited technical review can be provided to qualified reviewers or investors when appropriate, without making proprietary implementation public.

## Ownership

Copyright © 2026 Saad Marketing OS. All rights reserved. This repository is provided for evaluation and demonstration only. See [`LICENSE.md`](LICENSE.md).
