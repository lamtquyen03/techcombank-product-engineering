# Techcombank — Product Engineering Playbook

![Techcombank hero](assets/hero-personal.webp)

## Quick links

- Docs: [docs/product-spec.md](docs/product-spec.md)
- Roadmap: [docs/roadmap.md](docs/roadmap.md)
- Templates: [templates/REQ_TEMPLATE.md](templates/REQ_TEMPLATE.md)
- Monitoring: [docs/monitoring-checklist.md](docs/monitoring-checklist.md)

---

## Techcombank product landscape

![Techcombank mobile](assets/hero-mobile.webp)

```mermaid
flowchart LR
  style P fill:#0b75bd,stroke:#034f84,color:#fff
  P[Techcombank Product Universe]
  subgraph Retail
    RC[Current Account]
    RS[Savings]
    RD[Cards]
    RL[Loans]
  end
  subgraph Business
    BS[SME Account]
    BL[SME Loans]
    BE[E-invoicing]
    BP[Payments & POS]
  end
  subgraph Wealth
    WI[Investments]
    WF[Wealth & Funds]
  end
  P --> Retail
  P --> Business
  P --> Wealth
  classDef area fill:#f4f8fc,stroke:#0b75bd;
  class Retail,Business,Wealth area;
```

### Customer segments

- Retail: personal banking, cards, savings, loans, mobile banking.
- Business: SME accounts, merchant payments, digital invoicing, working capital.
- Wealth / Investors: investments, funds, investor communications.

---

## Product lines by customer type

![Merchant banner](assets/hero-merchant.webp)

```mermaid
mindmap
  root((Techcombank Products))
    Retail
      Current Account
      Savings
      Cards
      Personal Loans
      Mobile Banking
    Business
      SME Accounts
      SME Loans
      Merchant Payments
      SoftPOS / SmartPOS
      E-invoicing
    Investors
      Securities / Wealth
      Investor Relations
      Fund & Deposit Products
```

---

## Core product themes

![Savings product](assets/product-savings.webp)

- Savings & deposit products — growth, liquidity, automatic interest features.
- Payments & transaction rails — card, QR, merchant, and account transfers.
- Credit & lending — personal loans, SME working capital, installment offers.
- Digital banking — onboarding, self-service, mobile-first experience.
- Enterprise / merchant tools — POS, merchant onboarding, business cash management.

---

## Customer journey: digital onboarding

```mermaid
journey
  title Digital account opening
  section Discover
    Learn about product: 5: Customer
  section Apply
    Submit eKYC docs: 4: Customer
    Run checks & scoring: 3: System
  section Approve
    Review / verify: 2: Ops
    Open account: 4: System
  section Activate
    Activate card / app: 3: Customer
```

---

## Roadmap snapshot

```mermaid
gantt
  title Q3–Q4 delivery rhythm
  dateFormat  YYYY-MM-DD
  section Onboarding
  Discovery      :done, a1, 2026-07-01, 2026-07-31
  Alpha          :active, a2, 2026-08-01, 30d
  Beta           :a3, 2026-10-01, 30d
  Launch         :a4, 2026-11-01, 15d
```

---

## Internal-ready structure

- Product spec: [docs/product-spec.md](docs/product-spec.md)
- Requirement template: [templates/REQ_TEMPLATE.md](templates/REQ_TEMPLATE.md)
- PR template: [templates/PR_TEMPLATE.md](templates/PR_TEMPLATE.md)
- Monitoring checklist: [docs/monitoring-checklist.md](docs/monitoring-checklist.md)
- Stakeholder map: [docs/stakeholder-map.md](docs/stakeholder-map.md)

![Investor banner](assets/hero-investor.webp)

 