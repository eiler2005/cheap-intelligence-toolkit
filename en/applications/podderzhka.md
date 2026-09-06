<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/podderzhka
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

---
reading_level: b2
title: "Customer support: what to automate and which tools to use"
description: A practical map of support tasks AI can handle, the cases a person must keep, and tools to consider.
---

# Customer support: what to automate and which tools to use

> Field: **Sales and customer work**. Role hub. **Checked: 2026-08-18.** Tools change over time.
> Sources for this review are at the bottom of the page.

## At a glance

Bots and AI take over standard answers. Complex cases, empathy, and retention become more valuable because
they still need a person. The main risk is a bot giving a confident but wrong answer to a customer.

!!! info "What the data says (GDPval, Anthropic Economic Index, O*NET)"
    - **Capability (GDPval):** a typical work product is a "customer support conversation." AI performs
      well on standard cases.
    - **Use (AEI):** retail and service work show high automation. Bots handle frequent questions.
    - **The honest scale:** support and IT are the most common functions for agents, yet McKinsey
      (The state of AI in 2025, published Nov 5, 2025) found only 23% of organizations scaling an
      agentic system anywhere, and no more than 10% inside any single function. The instructive
      counter-case: Klarna brought people back into support in 2025 to fix quality.
    - **Mode:** strong reduction in entry-level tasks. Bots take the standard support line. Complex cases,
      retention, and empathy remain. See the [full data review](_super-analysis.md) and the
      [role AI strategy](strategy/podderzhka.md).

## What to automate first

1. **Answers to common questions.** Answer from a trusted knowledge base, not from the model's memory.
2. **Ticket classification and routing.** Sort requests automatically by topic and priority.
3. **Response drafts.** An agent edits the draft before sending it.
4. **Ticket and history summaries.** Bring an agent into the context quickly.
5. **Churn detection in customer success.** Flag customers who may leave.

## Task review: what AI can do and what you must check

| Task (O*NET) | Give to AI: method or tool | Keep or verify yourself | Prompt to start |
| --- | --- | --- | --- |
| Common questions | Answer **from the knowledge base** | Accuracy before sending |  |
| Ticket classification | Sort by topic and priority | Disputed routing | `Identify the topic and priority of this request` |
| Response drafts | Suggested answer | Facts and tone | `Give me two tone options. I will check the facts myself` |
| Ticket summary | Short history | Customer context | `Summarize the request history and the core problem` |
| Complex or conflict case | Do not delegate | A person, empathy, and the decision |  |

> Use a bot for standard questions **from a trusted knowledge base**. Send complex and retention cases to
> a person. Never send unchecked answers.

## Tools by use case

=== "Leading assistants"

    - **ChatGPT or Claude** for complex or unusual responses.

=== "Specialist tools"

    - **Zendesk AI**, **Embrace.ai** for agents tuned to a brand, and **Pylon** for support and customer
      success.

## One practical playbook

!!! example "Use a bot for common questions and a person for complex cases"
    1. Connect AI answers **to the knowledge base**, so the system answers from a source instead of inventing one.
    2. Set the routing rule: a standard case gets an automatic draft, while a complex case goes to a person.
    3. **Human check:** review drafts before sending. Route emotionally difficult cases to a person at once.
    4. Use the saved time for retention and complex cases.
    5. Output: the queue is smaller, and customer trust remains intact.

## Where not to use AI

!!! danger "Red flags"
    - **Unchecked answers:** a bot may invent terms or instructions and lose the customer's trust.
    - **Customer personal data:** remove identifying details and do not send it to outside services.
    - **Emotionally difficult cases:** use a person, not a template.

## Prompt patterns: weak and better

| Weak | Better |
| --- | --- |
| `Reply to the customer` | `Give me two tone options. I will check the facts myself` |
| `Solve the problem` | `Give me three possible causes of this complaint and a way to check each one` |

## Where to move your effort

Move time from standard work into retention, conflict, complex decisions, and empathy. Human work becomes
more valuable. See Chapter 7.

### The levels ladder in this role

The five levels from Chapter 5, in the language of this profession. Mark where you stand in your main
tasks this week.

| Level | What it looks like here |
|---|---|
| **1. AI user** | I answer the customer faster with an AI suggestion |
| **2. Validator** | I check the bot's answer before the customer sees it. A confidently wrong answer costs more than a slow one |
| **3. Orchestrator** | I built the line where the bot takes the routine and I take the hard cases and escalations |
| **4. Outcome owner** | I own customer retention, not the number of tickets closed |
| **5. System builder** | I set up the knowledge base and escalation rules so the line runs without manual control |

**Where people usually get stuck.** The routine tier moves to bots entirely, so level 1 shrinks fastest here. Hard cases, conflict, and retention are what gain value.

Next: [my level of usefulness](../playbooks/usefulness-levels-self-check.md) → [a plan for one level up](../playbooks/plus-one-level-plan.md).

## Ready-made skills and plugins for this role

You can turn repeatable procedures such as answering from a knowledge base, routing tickets, and writing
an escalation summary into a portable skill, or use an existing one. Browse
[skill banks](https://cheap-intelligence.vercel.app/en/watch/skill-banks), then see
[turn a workflow into a skill](../playbooks/make-it-a-skill.md) to build your own.

## Where to go next

[Map your week](../playbooks/week-inventory.md) → [run the integrated profession audit](../playbooks/profession-audit-integrated.md)
→ [make a 90-day plan](../playbooks/personal-90-day-plan.md). Or open the [workbook](../playbooks/tom1-workbook.md).

---
**Sources for this review:** OpenAI GDPval (2025): <https://openai.com/index/gdpval/> · Anthropic Economic Index: <https://www.anthropic.com/economic-index> · Stanford AI Index (2025): <https://hai.stanford.edu/ai-index> · McKinsey, "The State of AI": <https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai>. Plus the book, Chapters 2, 3, and 7.
