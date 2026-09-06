<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/skills/agent-contract/SKILL
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

---
name: agent-contract
description: >-
  Builds a contract for an AI agent across ten fields — role, mission, inputs, tools, memory,
  boundaries, escalation, review, metrics, owner — and turns the metric into a measurable threshold
  at which the agent stops itself. From chapter 3 of "Business in the Age of AI Agents".
  Use when the user is about to put an agent into a team process and needs its limits, escalation
  path, owner and stop threshold written down. Triggers "agent contract", "agent boundaries",
  "who owns this agent", "where should the agent stop", "we are putting AI into this process".
license: MIT
---

# The agent contract (Practicum for "When Intelligence Became Cheap")

📋 A ready-made skill for an AI assistant. Drop this file into your agent's skills folder — or copy
the block below into any chat and describe the one agent you are about to launch.

One agent, one contract. The worksheet, the template, two worked examples and the pre-flight list:
[The agent contract](../../playbooks/agent-contract.md). Before the contract, work through the
[Human Review Matrix](../../playbooks/human-review-matrix.md): the matrix decides which tasks can be
handed over at all, the contract pins down a single agent.

```text
Help me write a contract for an AI agent, using the model from "Business in the Age of AI Agents"
(chapter 3). An agent on a team is not a magic employee: it is a role with explicit boundaries, a
review step and a human owner.

Collect from me if I have not given it:
1. What the agent is and which process it will work in.
2. What data and systems it will have access to.
3. Who on the team is accountable for it, by name.

What to do — fill in ten fields, asking me where the information is missing:
Role · Mission (one sentence) · Inputs · Tools · Memory (and what must NOT go into it) ·
Boundaries (what the agent never does without confirmation) · Escalation (the condition under which
it hands over to a human) · Review (how and when the result is checked) · Metrics (one or two
numbers) · Owner (a name).

Then tie metric, escalation and stop into a single guardrail:
— signal metric (share of answers needing no edits · anomaly in the numbers · escalation rate ·
  cost per day);
— threshold: a specific number, named BEFORE launch;
— action at the threshold: pause and human review · roll back to manual · switch off.

Discipline (hold to this):
- Without Boundaries, Escalation and Owner this is not a contract but a wish. If I do not supply
  them, do not fill them in with plausible text — say plainly that the contract is not ready.
- The owner is a named person. "The team" and "the department" are not accepted.
- Review is not delegated to AI: name where a human looks at the result.
- Access is least privilege: only what the mission needs.
- The threshold is named before launch, not after an incident.
- Do not scale straight after the contract: next come the eval set and shadow mode.
- Do not invent system names, integrations or numbers on my behalf.

Answer format:
1. Contract table: field | value.
2. The guardrail: metric | threshold | action.
3. Pre-flight: the six-point checklist, marking what is closed and what is not.
4. The weakest point here, in one honest sentence.
```
