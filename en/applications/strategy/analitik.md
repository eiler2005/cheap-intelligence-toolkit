<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/strategy/analitik
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

# AI strategy: Data analyst

> Prioritized AI adoption map. **Date: 2026-06.** Sources: GDPval, AEI, O*NET, and
> profession automation review (GDPval, AEI, O*NET). ← [Role hub](../analitik.md)

!!! abstract "Context"
    AI can handle a noticeable share of an analyst's weekly tasks, though AEI and O*NET
    estimates are only a guide. The time savings can be substantial. The analyst's value lies
    in choosing the right question and making the result trustworthy.

## 1. Queries and preparation (high priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 1 | Natural language to SQL with reviewable code | time per query · share reviewed | Querio · human SQL review |
| 2 | Data cleaning and normalization | quality · time | automated normalization · comparison with the source of truth |

## 2. Dashboards and monitoring (high priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 3 | Regular dashboards and KPIs | reporting time · metric coverage | automatic updates · metric dictionary |
| 4 | Anomaly detection | deviations found · false positives | alerts · KPI monitoring |

## 3. Interpretation and forecasting (medium priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 5 | Hypotheses and interpretation | % of data-informed decisions | "2 hypotheses + where the evidence does not support them" · defend the conclusion |
| 6 | Baseline forecasts | accuracy | use an AI model as a starting point · test the assumptions |

## 4. Data and trust (foundation)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 7 | Source of truth and data lineage | discrepancies · definition consistency | data dictionary · aggregate checks · keep personal data inside the approved environment |

## 5. The role (foundation)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 8 | Become the "metric owner" | whose judgment the decision relies on | move from producing reports to owning the conclusion |

## Where to start: the first round

The tables are a map of what is possible, not your plan. Build the plan with the
[process scoring tool](../../playbooks/process-scoring.md). Ask: Does the task repeat? Is there
enough volume? Can you check the result? Can you afford the cost of an error? Do you have the
data? For most analysts, the first round looks like this:

1. **No. 3, regular dashboards and KPIs.** The work repeats every week and has enough volume.
   You can verify it by comparing metric definitions with the dictionary and sampling figures
   against the source.
2. **No. 1, natural language to editable SQL.** An error is visible. Read the SQL for logic and
   compare the result with the source of truth instead of accepting it on faith.
3. **No. 4, anomaly detection and alerts.** The task repeats, and the cost of an error is
   manageable. A false alert costs a few minutes of review, not a decision made in the dark.

**Not in the first round:** No. 6, "baseline forecasts," because the assumptions are not yet
calibrated and a forecast can drive a costly decision. No. 5, "hypotheses and interpretation,"
already calls for the metric owner's judgment from No. 8. Earn trust on more mechanical tasks
first. Do not send user or customer data to third-party services without an approved environment.
See the red flags in the [role hub](../analitik.md). That is a boundary, not a scheduling choice.

## Keep these parts of data analysis human

- **Deciding what question to ask of the data.** This is the analyst's work, and it cannot be automated.
- **Checking an aggregate against the source of truth.** A result that sounds statistical is not necessarily correct.
- **The metric owner's judgment.** A person must remain accountable for the view used in a decision.
- **Metric definitions.** Check them against the dictionary, not against a definition supplied by the model.
- **The business's trust in the conclusion.** This is the analyst's reputation, and it cannot be delegated.

## Review points and stop thresholds

Give every first-round initiative its own review point in the
[Human Review Matrix](../../playbooks/human-review-matrix.md) and set a threshold in advance in
the [agent contract](../../playbooks/agent-contract.md):

| Initiative | What a person checks | Stop threshold (example, replace with your own) |
|---|---|---|
| No. 3 dashboards | compare metric definitions with the dictionary and sample figures against the source | a discrepancy in a core metric means returning to manual calculation until the cause is understood |
| No. 1 natural language to SQL | read the SQL for logic and edge cases | one logic error in every N queries means quarantining the tool and rechecking recent reports |
| No. 4 anomalies | review every alert before anyone acts | a false-positive rate above your threshold means revising the alert rules |

Before you increase the workload, build a [reference set of 20 cases](../../playbooks/eval-set-builder.md).
For an analyst, this means 20 queries or dashboards with known correct results. Run every new tool
or prompt against this set first.

## Two paths from here

- **You are an analyst:** open the [role hub](../analitik.md), map your week, and build a personal
  plan in the [Volume 1 workbook](../../playbooks/tom1-workbook.md).
- **You lead the function:** use [process scoring](../../playbooks/process-scoring.md), write the
  [first agent contract](../../playbooks/agent-contract.md), and complete the full path in the
  [Volume 2 workbook](../../playbooks/tom2-workbook.md).

!!! danger "Discipline"
    A result that sounds statistical is not necessarily correct. Check aggregates against the
    source. Review the SQL and the definitions.

→ [Role hub](../analitik.md) · [audit](../../playbooks/profession-audit-integrated.md) · [plan](../../playbooks/personal-90-day-plan.md).

---
**Sources:** profession automation review (GDPval, AEI, O*NET); book, Chapters 2, 3, and 5.
