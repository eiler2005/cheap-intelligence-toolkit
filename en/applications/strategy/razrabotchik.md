<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/strategy/razrabotchik
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

# AI strategy: Software developer

> Prioritized AI adoption map. **Date: 2026-06.** Sources: GDPval, AEI, O*NET, and
> profession automation review (GDPval, AEI, O*NET). ← [Role hub](../razrabotchik.md)

!!! abstract "Context"
    Computer and mathematical work is among the task classes with the greatest AI exposure in the
    Anthropic Economic Index, which is only a guide. Coding assistants are already common. Junior
    tasks are moving first. Architecture, security, and production responsibility are becoming
    more valuable.

## 1. Code production (high priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 1 | Boilerplate, tests, and docs | time · test coverage | Copilot or Cursor · human review |
| 2 | Agentic tasks across multiple files | feature time · share of accepted diffs | Cursor Composer/Copilot agent · acceptance criteria |

## 2. Quality and review (high priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 3 | PR summaries and automated review | review time · defects found | AI comments · **final human review** |
| 4 | Security scans and migrations | vulnerabilities · migration time | Amazon Q or scanners · automated transformations |

## 3. Understanding systems (medium priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 5 | Explain and navigate the codebase | onboarding time · debugging speed | prompt: "Explain this module and its risky areas" |

## 4. Data security (foundation)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 6 | Keep private code from leaking | incidents | local models such as Ollama · never paste secrets |

## 5. The role (foundation)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 7 | Become an "agent boss" and own architecture | % of time on architecture and review | orchestrate agents · own production responsibility |

## Where to start: the first round

The tables are a map of what is possible, not your plan. Start with
[process scoring](../../playbooks/process-scoring.md). Ask whether the task repeats, has enough
volume, produces a checkable result, carries an affordable error cost, and has usable data. For
most developers, the first round looks like this:

1. **No. 1, boilerplate, tests, and documentation.** It repeats on every task and has enough
   volume. Run the tests instead of taking the output on faith.
2. **No. 3, PR summaries and draft review comments.** An error is cheap because a person still
   performs the final review. AI only speeds up the first pass.
3. **No. 5, code explanation and navigation.** The error cost is low because this is guidance for
   a person during onboarding or debugging, not code going to production.

**Not in the first round:** No. 2, "agentic tasks across multiple files," has a higher error cost
because changes spread across several files. Build review discipline on Nos. 1 and 3 first. No. 4,
"security scans and migrations," can miss an expensive vulnerability. Trust it only after the
review practice in No. 3 is reliable. Never send secrets or private code from No. 6 to third-party
services. This is a boundary, not a scheduling choice. See the red flags in the
[role hub](../razrabotchik.md).

## Keep these parts of software development human

- **Architecture and system boundaries.** AI can offer options; a person decides.
- **Final review before production.** It cannot be delegated at any maturity level.
- **Secrets, keys, and private code.** Do not put them into third-party services. Use local models for private material.
- **Responsibility for a production incident.** A person owns it even when an agent wrote the code.
- **Licenses for generated code.** A person checks provenance and compatibility.

## Review points and stop thresholds

Give every first-round initiative its own review point in the
[Human Review Matrix](../../playbooks/human-review-matrix.md) and set a threshold in advance in the
[agent contract](../../playbooks/agent-contract.md):

| Initiative | What a person checks | Stop threshold (example, replace with your own) |
|---|---|---|
| No. 1 boilerplate and tests | run tests and inspect edge cases | if a test fails or an edge case is missing, finish it by hand and do not merge |
| No. 3 PR review | a person completes final review of the diff | a missed bug or vulnerability means revising the review-bot prompt and rechecking recent PRs |
| No. 5 code explanation | compare the explanation with real behavior in at least one example | if the explanation differs from the code, do not use it for onboarding without verification |

Before you trust the flow, build a [reference set of 20 cases](../../playbooks/eval-set-builder.md):
20 reviewed PRs or tasks with known correct diffs. Test a new agent or prompt on them before using
it in the live task flow.

## Two paths from here

- **You are a developer:** open the [role hub](../razrabotchik.md), map your week, and build a
  personal plan in the [Volume 1 workbook](../../playbooks/tom1-workbook.md).
- **You lead engineering:** use [process scoring](../../playbooks/process-scoring.md), write the
  [first agent contract](../../playbooks/agent-contract.md), and complete the full path in the
  [Volume 2 workbook](../../playbooks/tom2-workbook.md).

!!! danger "Discipline"
    Send code to production only after review. Never paste secrets. A person owns the architecture.

→ [Role hub](../razrabotchik.md) · [audit](../../playbooks/profession-audit-integrated.md) · [plan](../../playbooks/personal-90-day-plan.md).

---
**Sources:** profession automation review (GDPval, AEI, O*NET); book, Chapters 2 and 3.
