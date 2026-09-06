<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/strategy/finanalitik
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

# AI strategy: Financial analyst / FP&A

> Prioritized AI adoption map. **Date: 2026-06.** Sources: GDPval, AEI, O*NET, and
> profession automation review (GDPval, AEI, O*NET). ← [Role hub](../finanalitik.md)

!!! abstract "Context"
    Automated data processing can reduce both errors and time, though AEI and O*NET estimates are
    only a guide. Updates, rolling forecasts, and standard reports are good AI tasks. Choosing a
    scenario and turning figures into action remain human work.

## 1. Data (high priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 1 | Collect, clean, and classify data | data quality · preparation time | planning tools · normalization · comparison with the source |

## 2. Forecasting and planning (high priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 2 | Rolling forecasts and drivers | accuracy · cycle time | AI forecast as a starting point · adjust assumptions |
| 3 | Scenario modeling | number of scenarios · speed | calculate options · human chooses the scenario |

## 3. Reporting (medium priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 4 | Standard management reports | time · errors | templates + AI summary · verify the figures |
| 5 | Detect anomalies and trends | deviations found | AI flags · automatic visuals |

## 4. Decisions (foundation)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 6 | Turn figures into business action | % of data-informed decisions · alignment | briefs for sales and operations · defend the figures with management |

## 5. Control (foundation)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 7 | Quality and data control | incidents · compliance | approved environment · model validation |

## Where to start: the first round

The tables are a map of what is possible, not your plan. Start with
[process scoring](../../playbooks/process-scoring.md). Ask whether the task repeats, has enough
volume, produces a checkable result, carries an affordable error cost, and has usable data. For
most FP&A teams, the first round looks like this:

1. **No. 1, data collection, cleaning, and classification.** It repeats in every cycle and has
   enough volume. Compare the result with the source. An error costs a dataset rebuild, not a
   business decision.
2. **No. 4, standard management reports.** They follow a template, and a person checks the figures
   before sending. This uses the same verifiability logic as marketing reports.
3. **No. 5, anomaly and trend detection.** AI only flags a deviation. A person decides whether it
   matters to the business, which keeps the error cost low.

**Not in the first round:** No. 2, "rolling forecasts," can move real business decisions and has a
higher error cost. Use it only with data that has passed No. 1. No. 3, "scenario modeling," is even
more expensive because a scenario based on an unstable forecast multiplies the error. Nos. 6 and
7, turning figures into action and controlling data quality, remain human responsibilities that
run alongside every other initiative.

## Keep these parts of financial analysis human

- **Choosing the scenario and assumptions.** The model calculates options; a person chooses the one closest to reality.
- **Turning figures into business action.** Give sales and operations a useful brief, not a bare table.
- **Defending figures with management.** A person aligns the plan and explains its assumptions.
- **Judging whether a deviation matters.** Not every anomaly is important to the business.
- **Financial and commercial data.** Allow access only through an approved environment.

## Review points and stop thresholds

| Initiative | What a person checks | Stop threshold (example, replace with your own) |
|---|---|---|
| No. 1 data collection and cleaning | compare final figures with the system of record | a discrepancy above your threshold means rebuilding the dataset manually until the cause is understood |
| No. 4 management reports | check figures and interpretation before sending | if a report figure does not match the source, do not send the report until it has been reconciled |
| No. 5 anomaly detection | decide whether the deviation matters to the business | a missed material anomaly or too many false positives means revising the sensitivity threshold |

Before you expand the flow, build a [reference set of 20 cases](../../playbooks/eval-set-builder.md):
20 periods with data and reports that have already been reconciled. Test each new step against them first.

## Two paths from here

- **You are a financial analyst or FP&A specialist:** open the [role hub](../finanalitik.md), then
  use the [Volume 1 workbook](../../playbooks/tom1-workbook.md) to move from your week to an audit
  and a 90-day plan.
- **You lead the FP&A function:** use [process scoring](../../playbooks/process-scoring.md), write
  the [first agent contract](../../playbooks/agent-contract.md), and continue with the
  [Volume 2 workbook](../../playbooks/tom2-workbook.md).

!!! danger "Discipline"
    People own the figures, formulas, and assumptions. A polished forecast is not necessarily
    correct. Keep financial data inside an approved environment.

→ [Role hub](../finanalitik.md) · [audit](../../playbooks/profession-audit-integrated.md) · [plan](../../playbooks/personal-90-day-plan.md).

---
**Sources:** profession automation review (GDPval, AEI, O*NET); book, Chapters 2, 3, and 5.
