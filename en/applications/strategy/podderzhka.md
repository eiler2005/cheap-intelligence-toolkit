<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/strategy/podderzhka
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

# AI strategy: Customer support

> Prioritized AI adoption map. **Date: 2026-06.** Sources: GDPval, AEI, O*NET, and
> profession automation review (GDPval, AEI, O*NET). ← [Role hub](../podderzhka.md)

!!! abstract "Context"
    Bots are taking over standard first-line requests as automation rises. Complex cases,
    retention, and empathy are becoming more valuable.

## 1. Automated handling (high priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 1 | Bots for common questions **grounded in the knowledge base** | % resolved by the bot · CSAT | Bitrix24/Zendesk AI · natural language understanding based on a trusted source |
| 2 | Classify and route tickets | routing time · accuracy | automatic sorting by topic and priority |

## 2. Agent assistance (high priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 3 | Draft replies and ticket summaries | response time · quality | AI draft · fact check before sending |

## 3. Retention (medium priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 4 | Detect churn risk in customer success | % of high-risk customers retained | Pylon and triggers · human works with the risk |

## 4. The role (foundation)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 5 | Move people to complex and empathy-heavy work | share of high-stakes tasks · NPS | less standard work, more retention and conflict handling |

## Where to start: the first round

The tables are a map of what is possible, not your plan. Start with
[process scoring](../../playbooks/process-scoring.md). Ask whether the task repeats, has enough
volume, produces a checkable result, carries an affordable error cost, and has usable data. For
most support teams, the first round looks like this:

1. **No. 2, ticket classification and routing.** It repeats for every request and has the greatest
   volume. Compare the assigned topic with the real message. An error costs a reroute, not a reply
   sent to the customer.
2. **No. 3, draft replies and ticket summaries.** The support agent sees the draft before sending,
   so review is built into the process.
3. **No. 1, bots for common questions grounded in the knowledge base.** Start only while the bot
   answers strictly from a trusted source instead of making up an answer, and audit it closely.
   Without those conditions, this becomes the first incident rather than the first round.

**Not in the first round:** No. 4, "churn detection," needs request history that contains a visible
risk pattern. Without it, the model is guessing rather than predicting. No. 5, moving people to
complex and empathy-heavy work, is the result of the first three initiatives, not a separate
implementation task.

## Keep these parts of customer support human

- **Emotionally difficult and hostile cases.** Route them to a person immediately, without trying an automatic reply.
- **Unusual requests with no approved answer in the knowledge base.** A person decides the exception and its wording.
- **A conversation with a customer who may leave.** This needs a real conversation, not a template.
- **Customer personal data.** Control and de-identify it, and do not send it to third-party services.
- **Responsibility when the bot is wrong.** Escalate and investigate the case instead of silently correcting it.

For a similar path in practice, read the example of a support leader who worked through this exact
split between bot and person: [Sergey](../../cases/persona-rukovoditel-podderzhki.md).

## Review points and stop thresholds

| Initiative | What a person checks | Stop threshold (example, replace with your own) |
|---|---|---|
| No. 2 routing | sample whether the topic and priority are correct | a misrouting rate above your threshold means returning disputed cases to manual sorting |
| No. 3 drafts and summaries | support agent checks facts and tone before sending | a claim in the draft without source support means fixing the prompt and manually checking the next batch |
| No. 1 bot for common questions | audit N conversations per day against the knowledge base | one answer outside the knowledge base, or a hallucination, means quarantining the bot until review and retraining are complete |

Before you expand the flow, build a [reference set of 20 cases](../../playbooks/eval-set-builder.md):
20 real tickets with an approved answer and the correct route.

## Two paths from here

- **You are a support agent or specialist:** open the [role hub](../podderzhka.md), then use the
  [Volume 1 workbook](../../playbooks/tom1-workbook.md) to move from your week to an audit and a
  90-day plan.
- **You lead the support function:** use [process scoring](../../playbooks/process-scoring.md), write
  the [first agent contract](../../playbooks/agent-contract.md), run the
  [90-minute workshop](../../workshops/process-scoring-workshop.md) with the team, and complete the
  full path in the [Volume 2 workbook](../../playbooks/tom2-workbook.md).

!!! danger "Discipline"
    Unchecked answers damage trust. De-identify personal data. Keep difficult cases with people.

→ [Role hub](../podderzhka.md) · [audit](../../playbooks/profession-audit-integrated.md) · [plan](../../playbooks/personal-90-day-plan.md).

---
**Sources:** profession automation review (GDPval, AEI, O*NET); book, Chapters 2, 3, and 7.
