<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/playbooks/agent-contract
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

# Agent Contract

> Practicum for **Volume 2, Chapter 3**, "A Team with Agents." Time: 15-20 minutes per agent.
> Use one sheet for one agent. Copy the template and fill it in for your case.

An agent is not a "magic employee." It is a role with clear boundaries, review, and a **human owner**.
The contract turns "let's add AI" into an agreement the team can understand and enforce.

A minimum governance packet is the small set of documents that defines control and ownership. In that packet, the contract follows the [Human Review Matrix](human-review-matrix.md).
The matrix decides which tasks can be handed over. The contract defines **one** agent, its permissions, and its brakes.
Do not scale right away. Test the agent on an [evaluation set](eval-set-builder.md) and in shadow mode first, where it drafts or observes without taking live action.

## Template: 10 fields

| Field | What to enter |
|---|---|
| **Role** | the agent's name and function |
| **Mission** | one sentence explaining why it exists |
| **Inputs** | the data and formats it accepts |
| **Tools** | the systems, APIs, and files it may access |
| **Memory** | what it remembers between sessions, and what must **never** enter memory |
| **Boundaries** | what the agent **never** does without approval |
| **Escalation** | the conditions that send the task to a person |
| **Review** | how and when a person checks the result, rather than one AI checking another |
| **Metrics** | 1-2 numbers that show whether it works |
| **Owner** | the name of the person accountable for it |

> Default rule: without **Boundaries + Escalation + Owner**, this is a wish, not a contract. All three are required from day one.

### A measurable threshold gate: KPI -> escalation -> stop

A contract metric is not something to report at the end. It is a **guardrail**, a preset threshold that makes the agent stop and call a person.
Connect three fields in one rule:

| What you define | Example |
|---|---|
| **Signal metric** | share of answers accepted without edits; unusual numbers; escalation rate; daily cost |
| **Threshold**, set in advance | "below 85% accepted without edits"; "difference > 10%"; "> N requests in a row"; "above the ₽/day limit" |
| **Action at the threshold** | pause and human review; return to manual work; owner-triggered shutdown |

> Give the agent the smallest set of permissions it needs. This is called **least privilege**. A measurable threshold turns Metrics and Escalation into a working brake. Set the threshold **before** launch, not after an incident.

## Example 1: first-line support agent

- **Role:** sorts incoming requests and answers common questions. **Mission:** remove routine work from the support team.
  **Inputs:** request text and answer base. **Tools:** read-only access to the knowledge base.
- **Boundaries:** does not promise compensation or touch billing. **Escalation:** complaints, refunds, or conflict go to a person.
  **Review:** a person audits 10 conversations a day. **Metrics:** share resolved without a person and number of escalations.
  **Owner:** head of support.

## Example 2: reporting analyst agent

- **Role:** prepares the weekly sales summary. **Inputs:** CRM exports. **Tools:** read-only data access.
  **Boundaries:** does not send the report. **Escalation:** an anomaly > X% is flagged for a person.
  **Review:** the owner checks the totals against the source before sending. **Metrics:** time to finished report and share of figures accepted without edits.
  **Owner:** team analyst.

## Pre-flight check

- [ ] The three required fields are complete: Boundaries, Escalation, and Owner.
- [ ] Access follows **least privilege** and covers only what the mission requires.
- [ ] Memory contains no secrets or personal data that do not belong there.
- [ ] A human review method is built into the flow.
- [ ] The team has agreed on the signal that **shuts the agent down**.
- [ ] A **measurable threshold gate** is set: metric + number + action (pause / rollback / stop).

---

## Next

- Build shared context for the team and its agents with the [team-brain starter kit](team-brain-starter.md).
- Decide what the agent may do and what a person should keep with the [Human Review Matrix](human-review-matrix.md) (Chapter 2).
- Review third-party skills before they enter your system: [how to check them](https://cheap-intelligence.vercel.app/en/watch/skill-banks).
- Follow the full route in the [Volume 2 Workbook](tom2-workbook.md).
