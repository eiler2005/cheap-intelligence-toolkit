<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/playbooks/team-brain-starter
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

# Team-brain starter kit: a shared team brain in 14 days

> Practicum for **Volume 2, Chapter 3**, "A Team with Agents." For a manager or founder.
> This follows the [Agent Contract](agent-contract.md). Once agents have boundaries, give them shared context. Without it, each agent fails in its own way.

Agents and new team members can only work with the context they receive. A "team-brain" is a small shared knowledge repository.
It is not a year-long corporate wiki project. It is a handful of files that an agent reads first.

## Minimum structure

```
team-brain/
  product/        - what we make, who it is for, and the main metrics
  customers/      - who the customer is and what we know about them
  decisions/      - decision log (decisions.md)
  glossary/       - team terms (the agent reads these first)
  skills/         - reusable instructions and prompts
```

You do not need more folders. Five active files beat thirty empty ones.

## Decision log (`decisions/decisions.md`)

Use one line per decision so agents and new colleagues do not have to ask why it was made:

```
Date | Decision | Context (why) | Alternatives rejected | Owner | Review date
```

## Memory: three states

New knowledge moves through three states so the shared brain does not fill with junk:

- **staged:** a candidate has been recorded but is not yet shared, like a memory draft;
- **review:** a person has checked that it is true and reusable;
- **prompted:** it is now part of the context that the agent actually reads.

Nothing moves from *staged* to *prompted* without a person.

## Agent evaluation template

Before you trust an agent with a task, run it **with and without the context** and compare the results.

| Task | Inputs | What counts as a good answer | Score without team-brain | Score with team-brain | Decision |
|---|---|---|---|---|---|
| `____` | `____` | `____` | `_/5` | `_/5` | `____` |

If there is no difference, the context is not working, or the task does not depend on context.

## 14-day plan

- **Days 1-3.** Find one bottleneck where the team loses time by explaining the same thing again.
- **Days 4-7.** Collect the minimum knowledge for it in `product/`, `customers/`, and the first entries in `decisions/`.
- **Days 8-14.** Launch **one** agent with an [Agent Contract](agent-contract.md). Run the evaluation with and without context. Keep it only if the difference is measurable.

---

## Next

- Give each agent its own [Agent Contract](agent-contract.md) with a role, boundaries, and owner.
- Decide what the agent may do and what a person should keep with the [Human Review Matrix](human-review-matrix.md).
- Follow the full route in the [Volume 2 Workbook](tom2-workbook.md).

> The goal is a few files that become useful quickly, not a corporate wiki project.
