---
{
  "title": "Creator Payout & Reconciliation",
  "description": "From earnings to a traceable payment outcome.",
  "weight": 1,
  "category": "Finance systems",
  "status": "Implemented \u00b7 simulated provider",
  "cardimage": "/images/payout.svg",
  "repo": "https://github.com/SherryHuProducts/creator-payout-ops",
  "tags": [
    "Python",
    "FastAPI",
    "SQLite",
    "Financial controls"
  ],
  "showtoc": true,
  "tocopen": false,
  "hidemeta": true
}
---


## The problem
A correct payout calculation is only the beginning. Operations teams also need to know what has already been paid, which amount remains outstanding, whether it was approved, and whether payment was actually confirmed.

## What I built
A controlled workflow connecting transaction validation, agreement rules, reconciliation, obligations, approval, payment initiation, webhook confirmation, and final reconciliation.

- Exact monetary calculations with Python `Decimal`.
- Five REST endpoints through a FastAPI adapter.
- Durable SQLite records connecting obligations, approvals, payment attempts, and confirmation events.
- Payment and webhook idempotency to prevent duplicate financial effects.
- Automated tests and GitHub Actions CI.

## A concrete example
The repository's synthetic CR-D example starts with **$92.73 outstanding**. Payment is blocked until approval. A success webhook confirms the payment; replaying that event does not create a second payment. Final reconciliation shows **$0.00 outstanding**.

## Scope
The workflow, API, controls, persistence, and tests are implemented. The payment provider and webhook delivery are simulated, and the business data is synthetic. This portfolio project does not claim a live payment integration or authenticated segregation of duties.

## What this demonstrates
Translating accounting judgment into explicit rules, system states, acceptance criteria, and evidence that an operations reviewer can trace.


[Explore the repository →](https://github.com/SherryHuProducts/creator-payout-ops)
