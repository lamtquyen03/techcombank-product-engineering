# Techcombank — Product Engineering Playbook

Concise, production-ready artifacts a Senior Product Owner at Techcombank would use. Visual-first, decision-focused, ready for handoff to PMs, EMs and stakeholders.

Quick links

- Docs: [docs/product-spec.md](docs/product-spec.md)
- Roadmap: [docs/roadmap.md](docs/roadmap.md)
- Templates: [templates/REQ_TEMPLATE.md](templates/REQ_TEMPLATE.md)

---

## Portfolio (visual)

```mermaid
flowchart LR
	style P fill:#0b75bd,stroke:#034f84,color:#fff
	P[Techcombank Portfolio]
	subgraph Retail
		direction TB
		CA[Current Account]
		SV[Savings]
		CD[Cards]
		LN[Loans]
	end
	subgraph SME
		direction TB
		SA[SME Account]
		SL[SME Loans]
		EI[E-invoicing]
	end
	subgraph Wealth
		direction TB
		IV[Investments]
		MM[Mutual Funds]
	end
	P --> Retail
	P --> SME
	P --> Wealth
	classDef bank fill:#f3f6fb,stroke:#0b75bd;
	class Retail,SME,Wealth bank;
```

## Short product catalog (concise)

- Current Account — core transactional product for retail customers (digital-first onboarding, debit + e-statements).
- Savings — tiered accounts and goal-based savings tools.
- Cards — credit/debit products with rewards + installment plans.
- Loans — consumer & mortgage; fast decisioning for salaried customers.
- SME Account — business banking for micro / small businesses (payments, cash mgmt).
- SME Loans — working capital and trade finance for SMEs.
- E-invoicing — SME automation & partner integrations (AP/AR).
- Investments — brokerage and funds for retail investors.

---

## User journey — account opening (visual)

```mermaid
journey
	title Account opening (digital)
	section Discover
		User learns product: 5: Customer
	section Apply
		Submit docs & eKYC: 4: Customer
		System checks & scoring: 3: System
	section Approve
		Manual review (if needed): 2: Ops
		Create account & issue token: 4: System
	section Activate
		Card delivery / in-app activation: 3: Customer

```

## Roadmap snapshot

```mermaid
gantt
	title Q3–Q4 Roadmap
	dateFormat  YYYY-MM-DD
	section Onboarding
	Research       :done, des1, 2026-07-01, 2026-07-31
	Alpha          :active, des2, 2026-08-01, 30d
	Beta           :des3, 2026-10-01, 30d
	Launch         :des4, 2026-11-01, 15d

```

## Stakeholders & outputs

- **Outputs in this repo:** `docs/product-spec.md`, `templates/REQ_TEMPLATE.md`, `templates/PR_TEMPLATE.md`, `docs/monitoring-checklist.md`, diagrams in `/diagrams`.
- **Stakeholders:** Business, Engineering, Compliance, Ops, Marketing.

---

If you want more visuals (colored swimlanes, persona cards, or export-ready PNGs), tell me which diagram to expand and I will commit & push updates.
