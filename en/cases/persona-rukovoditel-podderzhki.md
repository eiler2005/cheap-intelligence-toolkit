<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/cases/persona-rukovoditel-podderzhki
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

---
reading_level: b2-c1-technical
title: "Example: Sergey, a support manager, follows the Volume 2 route"
description: A completed support automation route with evaluation, escalation, ownership, and rollout gates.
---

# Example: Sergey, a support manager, follows the Volume 2 route

> Sergey is a composite character, and the figures are illustrative. This example shows an honest
> route for a function leader through the [Volume 2 workbook](../playbooks/tom2-workbook.md).

**Sergey is 41 and leads customer support at a service company with about 200 employees. His support
team has 9 people.** Executives tell him to "adopt AI because competitors already have." His team fears
layoffs. A year ago, the company "connected a bot," and the result was worse. Customers got angry, and
the team had to redo its work.

---

## Step 1. Reconstruction, not a cosmetic fix, Chapter 1

He put the "answer a customer request" process through the
[maturity check](../playbooks/ai-native-maturity-check.md):

- **Maturity level: 1 out of 5.** The bot sat on top of the old process. The same queue and templates
  remained, while AI wrote the first reply. This was a standard cosmetic fix.
- **Where AI was bolted on:** it was inserted into the "write the reply" step. The expensive step is
  "understand what kind of case this is and where it should go."

*Why this step matters:* admitting that the previous deployment was cosmetic is already a result. Most
teams defend the old decision at this point.

## Step 2. Move from output to outcome, Chapter 2

He used the [Human Review Matrix](../playbooks/human-review-matrix.md) to sort customer requests:

- **Task suitable for evaluation:** routine requests such as "Where is my order?", "How do I return
  it?", or "Why does X not work?" They make up about 60% of the flow. The result can be checked because
  the team has a source of correct answers and customer ratings.
- **Who owns the decision:** refunds, complaints, and the tone used in a conflict always belong to a person.
- He built an **evaluation set of 40 real requests** with known correct answers. Every bot change now
  runs against it first. See the [agent evaluation set](../playbooks/eval-set-builder.md).

## Step 3. Contract for the first agent, Chapter 3

He completed the [agent contract](../playbooks/agent-contract.md) for the first line:

- **Role:** classify incoming requests and answer standard questions from the knowledge base.
  **Access:** read-only access to the knowledge base.
- **Boundaries:** it cannot promise compensation, change billing, or apologize "on behalf of the CEO."
- **Escalation:** complaints, money, conflict, or uncertainty → a person. **Owner:** Sergey personally.
- **Threshold gate:** if the daily share of answers "resolved without a person and without a repeat
  request" falls below 80%, pause and review. More than three consecutive escalations from one customer
  switches that customer to manual handling.
- **Verification:** the whole team takes turns auditing a sample of 10 conversations each day. This is
  also training because the team sees where the agent fails.

## Steps 5 and 6. Money and the market

- **The function with the fastest financial return:** the night shift. Requests used to pile up until
  morning. Standard questions are now resolved at once, so the morning backlog is gone. This shows up
  in money through fewer cancellations and in working conditions through calmer mornings.
- **Where a customer agent cannot find the company:** the
  [visibility checklist](../skills/visible-to-agent/index.md) showed that the knowledge base blocks
  indexing and the FAQ is stored as images inside a PDF. If a customer asks an AI assistant, "How do I
  return an order to ...?", it cannot find the answer. The fix went into the site backlog.

## Final step. Compass and gates, Chapter 11

- **First-round process:** routine first-line requests, with 5 out of 5 "yes" answers in the
  [scoring worksheet](../playbooks/process-scoring.md).
- **Gates passed:** process map → evaluation set → contract with an owner → pilot on 20% of the flow.
  **Next gate:** expand to the whole flow after the metric holds for two months.
- **PEOPLE direction:** no one was laid off. Two team members now maintain the knowledge base and audit
  the agent. These are the new roles described in Chapter 3. Fear eased after people saw their new work,
  not after a reassuring speech.

---

## What to notice in this example

1. **The first move is admitting that the fix was cosmetic.** The maturity check exists to stop the
   team from improving the wrong process, not to create a report.
2. **The evaluation set came before expansion, not after an incident.** 40 requests with known
   answers are cheap insurance and make changes reversible.
3. **Gates replace a deadline.** "We expand after the metric holds for two months" is manageable.
   "We launch by the end of the quarter" is a gamble.

Complete your own route in the [Volume 2 workbook](../playbooks/tom2-workbook.md). See
[the catalog](index.md) for more examples.
