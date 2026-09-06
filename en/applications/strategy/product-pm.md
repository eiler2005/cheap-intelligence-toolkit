<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/strategy/product-pm
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

# AI strategy: Product manager

> Prioritized AI adoption map. **Date: 2026-06.** Sources: GDPval, AEI, O*NET, and
> profession automation review (GDPval, AEI, O*NET). ← [Role hub](../product-pm.md)

!!! abstract "Context"
    AI is good at synthesizing research and drafting documents. A person still decides what to
    build and why, which is the core of product management.

## 1. Research and synthesis (high priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 1 | Synthesize interviews and feedback | synthesis time · signal coverage | Dovetail/NotebookLM · topic clustering |
| 2 | Competitive and market intelligence | freshness · verifiability | Crayon/Perplexity · verify figures |

## 2. Documentation (high priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 3 | Draft PRDs, user stories, and release notes | document time · quality | ChatPRD/Claude with paid access · human completion |

## 3. Metrics and priorities (medium priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 4 | Answer metric questions in natural language | speed to insight | Mixpanel/PostHog · verify definitions |
| 5 | Prioritization suggestions | decision speed | group ideas · **a person makes the bet** |

## 4. The role (foundation)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 6 | Strategy and team trust | % of time spent on what to build | less documentation, more decisions and time with people |

## Where to start: the first round

The tables are a map of what is possible, not your plan. Start with
[process scoring](../../playbooks/process-scoring.md). Ask whether the task repeats, has enough
volume, produces a checkable result, carries an affordable error cost, and has usable data. For
most product managers, the first round looks like this:

1. **No. 1, interview and feedback synthesis.** It repeats in every research cycle and can involve
   hundreds of responses. Check the clusters against the original transcripts.
2. **No. 3, draft PRDs, user stories, and release notes.** An error is cheap because this is a
   draft. A person still sets priorities and decides what not to do.
3. **No. 4, natural-language answers about metrics.** Verify each answer against the metric
   definition and the source dashboard.

**Not in the first round:** No. 5, "prioritization suggestions," can quietly hand the actual bet
to AI instead of merely grouping ideas. Use it only when the line between suggestion and decision
is firm. Decisions about priorities and trade-offs cannot be delegated. See the
[role hub](../product-pm.md). No. 2, "competitive and market intelligence," requires checking every
figure and quotation against its source for each report. That is a review discipline, not a quick pilot.

## Keep these parts of product management human

- **What to build and why.** The strategic bet cannot be outsourced.
- **Priorities and trade-offs.** Do not delegate them, even as "advice" from the model.
- **What not to do.** This is also a product decision, and it belongs to you.
- **Team trust.** It grows from a person's presence and decisions, not from documents.
- **User data.** De-identify it before any outside AI processing.

## Review points and stop thresholds

Give every first-round initiative its own review point in the
[Human Review Matrix](../../playbooks/human-review-matrix.md) and set a threshold in advance in the
[agent contract](../../playbooks/agent-contract.md):

| Initiative | What a person checks | Stop threshold (example, replace with your own) |
|---|---|---|
| No. 1 interview synthesis | sample clusters against the original transcripts | a cluster that the transcripts do not support means repeating the synthesis manually |
| No. 3 PRDs and stories | a person sets final priorities and "what not to do" | if the draft pushes a priority you did not choose, fix the prompt and manually review the priorities section |
| No. 4 metrics in natural language | compare the metric definition with the dictionary and source dashboard | if the definition differs from the dictionary, do not publish the conclusion and investigate manually |

Before you expand, build a [reference set of 20 cases](../../playbooks/eval-set-builder.md). For a
PM, this means 20 accepted PRDs or interview syntheses with a known correct analysis. Test each new
tool against this set before trusting the live flow.

## Two paths from here

- **You are a product manager:** open the [role hub](../product-pm.md), map your week, and build a
  personal plan in the [Volume 1 workbook](../../playbooks/tom1-workbook.md).
- **You lead the product function:** use [process scoring](../../playbooks/process-scoring.md), write
  the [first agent contract](../../playbooks/agent-contract.md), and complete the full path in the
  [Volume 2 workbook](../../playbooks/tom2-workbook.md).

!!! danger "Discipline"
    Do not set priorities from AI advice because the model lacks your context. Verify market
    figures. De-identify user data.

→ [Role hub](../product-pm.md) · [audit](../../playbooks/profession-audit-integrated.md) · [plan](../../playbooks/personal-90-day-plan.md).

---
**Sources:** profession automation review (GDPval, AEI, O*NET); book, Chapters 2, 3, and 5.
