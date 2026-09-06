<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/strategy/buhgalter
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

# AI strategy: Accountant

> Prioritized AI adoption map for accounting, for both an individual and the function.
> **Date: 2026-06.** Sources: GDPval, AEI, O*NET, and profession automation review (GDPval, AEI, O*NET).
> ← [Role hub](../buhgalter.md)

!!! abstract "Context"
    Bank feeds and OCR now handle a substantial share of manual entry, and routine accounting is
    becoming more automated. AEI and O*NET estimates are only a guide. Machines take on production,
    but a person remains responsible for the figure and the signature.

## 1. Data capture and entry (high priority)

| No. | Goals or directions | KPIs | Initiatives |
|---|---|---|---|
| 1 | OCR for source documents | % entered automatically · recognition errors · time | Dext for data capture · sample checks |
| 2 | Automatic reconciliation of bank feeds | % matched automatically · reconciliation time | connect feeds · matching rules · investigate discrepancies |

## 2. Accounting processes (high priority)

| No. | Goals or directions | KPIs | Initiatives |
|---|---|---|---|
| 3 | Transaction categorization | accuracy · % automatically categorized and confirmed | train on journal entries · confirm disputed cases |
| 4 | Month-end close orchestration | time to close · number of manual operations | close workflow · anomaly detection before filing |

## 3. Reporting and explanations (medium priority)

| No. | Goals or directions | KPIs | Initiatives |
|---|---|---|---|
| 5 | Draft variance commentary | time spent on explanations · quality | AI draft based on the data · fact check |
| 6 | Responses to official requests and letters | time · acceptance rate | response structure from AI + facts from a person |

## 4. Control and risk (foundation)

| No. | Goals or directions | KPIs | Initiatives |
|---|---|---|---|
| 7 | Detect anomalies and errors | errors found · false positives | rule-based and AI checks · audit trail |
| 8 | Protect personal and commercial data | incidents · compliance | approved environment · de-identification · policy |

## 5. Skills (foundation)

| No. | Goals or directions | KPIs | Initiatives |
|---|---|---|---|
| 9 | Move from data entry to ownership of the outcome | % of tasks where you are accountable | practice judgment · work with auditors and tax authorities · disputed cases |

## Where to start: the first round

The tables are a map of what is possible, not your plan. Start with
[process scoring](../../playbooks/process-scoring.md). Ask whether the task repeats, has enough
volume, produces a checkable result, carries an affordable error cost, and has usable data. For
most accounting teams, the first round looks like this:

1. **No. 1, OCR for source documents.** It repeats for every document and has the greatest volume.
   A sample can be compared with the original, and an error costs one corrected entry.
2. **No. 2, automatic bank-feed reconciliation.** The process is checkable by design. The system
   flags discrepancies, so a person reviews those cases instead of the full transaction stream.
3. **No. 3, transaction categorization.** The model learns from your journal entries. A person
   confirms every disputed category, which keeps the cost of error under control.

**Not in the first round:** No. 4, "month-end close orchestration," affects the full closing cycle
and carries a higher error cost. Use it only after Nos. 1 to 3 produce reliable data. No. 6,
"responses to official requests and letters," sends a document to an outside authority. Reliable
facts matter more than speed there. Nos. 8 and 9, data protection and ownership of the outcome,
are permanent rules at every stage, not initiatives to schedule later.

## Keep these parts of accounting human

- **Signing and filing reports.** Accountability cannot be delegated at any maturity level.
- **Disputed matters and the tax position.** These require judgment, not a keyword search for a rule.
- **Working with auditors and tax authorities.** A person handles the negotiation and explanation.
- **Advising management or a client on the figures.** Accounting becomes useful when it supports a decision.
- **Final responsibility for every figure.** This remains true even when AI prepares the draft.

## Review points and stop thresholds

| Initiative | What a person checks | Stop threshold (example, replace with your own) |
|---|---|---|
| No. 1 OCR for source documents | compare a sample of recognized data with the original document | an error rate above your threshold means a 100% manual check of the batch until the setup is fixed |
| No. 2 bank-feed reconciliation | investigate discrepancies only, including timing, partial payments, and duplicates | a discrepancy that cannot be explained within a reasonable time means returning to manual reconciliation for the period |
| No. 3 categorization | confirm disputed categories | a recurring error in one category means revising the rules and retraining |

Before you expand the flow, build a [reference set of 20 cases](../../playbooks/eval-set-builder.md):
20 documents or reconciliations that have already been processed and have known correct results.

## Two paths from here

- **You are an accountant:** open the [role hub](../buhgalter.md), then use the
  [Volume 1 workbook](../../playbooks/tom1-workbook.md) to move from your week to an audit and a
  90-day plan.
- **You lead the accounting function:** use [process scoring](../../playbooks/process-scoring.md),
  write the [first agent contract](../../playbooks/agent-contract.md), and continue with the
  [Volume 2 workbook](../../playbooks/tom2-workbook.md).

!!! danger "Discipline"
    Recheck every figure and calculation. Never delegate signing or filing. Keep sensitive data
    inside an approved environment.

→ [Accountant hub](../buhgalter.md) · [audit](../../playbooks/profession-audit-integrated.md) · [90-day plan](../../playbooks/personal-90-day-plan.md).

---
**Sources:** profession automation review (GDPval, AEI, O*NET); book, Chapters 2 and 3.
