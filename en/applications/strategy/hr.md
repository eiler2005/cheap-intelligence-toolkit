<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/strategy/hr
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

# AI strategy: HR specialist

> Prioritized AI adoption map. **Date: 2026-06.** Sources: GDPval, AEI, O*NET, and
> profession automation review (GDPval, AEI, O*NET). ← [Role hub](../hr.md)

!!! abstract "Context"
    AI is common in HR, and screening can save substantial time. AEI and O*NET adoption estimates
    are only a guide. Hiring decisions and culture stay with people. Bias is a serious risk.

## 1. Recruiting (high priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 1 | Screen and rank resumes | time to hire · shortlist quality | ATS with AI · confidence bands, which show how certain the system is · **review borderline cases manually** |
| 2 | Source candidates | coverage · relevance | semantic search with Potok, Huntflow, or hh.ru |

## 2. Coordination (high priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 3 | Schedule interviews and communicate | drop-off · speed | scheduling bots · automatic candidate updates |

## 3. Content (medium priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 4 | Job posts, letters, and policies | time · quality | drafts with an assistant · human removes cliches |
| 5 | Onboarding and a policy-based knowledge base | onboarding time | NotebookLM based on policies · AI answers for new hires |

## 4. Ethics and decisions (foundation)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 6 | Control bias and protect personal data | incidents · audits | ban automatic rejection · audit algorithms · approved data environment |

## Where to start: the first round

The tables are a map of what is possible, not your plan. Start with
[process scoring](../../playbooks/process-scoring.md). Ask whether the task repeats, has enough
volume, produces a checkable result, carries an affordable error cost, and has usable data. For
most HR teams, the first round looks like this:

1. **No. 3, interview scheduling and communication.** It repeats for every candidate and has
   enough volume. Compare the output with the calendar. An error costs a rescheduled slot, not a
   hiring decision.
2. **No. 2, candidate sourcing.** A recruiter can see whether the results are relevant, and a
   person makes the final decision to put someone into the pipeline.
3. **No. 4, job posts, letters, and policies.** A person always edits the draft, checks the terms,
   and removes cliches before publication.

**Not in the first round:** No. 1, "resume screening and ranking," has the highest error cost even
though the table labels it high priority. Biased automatic rejection is a red flag in the
[role hub](../hr.md). Do not start without confidence bands and regular algorithm audits. No. 5,
"onboarding and the knowledge base," works only when the policies are already in order. Otherwise,
AI will answer from bad material. No. 6, bias control, is a continuing check across all initiatives,
not a separate task for later.

## Keep these parts of HR human

- **The hiring decision.** It is final and cannot be delegated at any maturity level.
- **Rejection feedback.** A person chooses the words and tone, with the legal risks of an unjustified rejection in mind.
- **Culture, conflict, and difficult conversations.** These shape trust inside the company.
- **Assessing personality and soft skills in an interview.** This requires judgment from a live conversation, not just text.
- **Candidate and employee personal data.** Keep it inside an approved environment and own the consequences of a leak.

## Review points and stop thresholds

| Initiative | What a person checks | Stop threshold (example, replace with your own) |
|---|---|---|
| No. 3 interview scheduling | compare slots and reminders with the real calendar and candidate replies | if a candidate is lost because communication failed, return to manual message control |
| No. 2 sourcing | check relevance and look for skew against any candidate group | a systematic drop for one group means auditing the search criteria |
| No. 4 job posts and letters | remove cliches and verify terms before publication | an inaccurate term or cliche in a published role means pausing publication and manually reviewing the next batch |

Before you trust the flow, build a [reference set of 20 cases](../../playbooks/eval-set-builder.md):
20 resumes with a known human hiring decision. Test every new screening tool against them first.

## Two paths from here

- **You are an HR specialist:** open the [role hub](../hr.md), then use the
  [Volume 1 workbook](../../playbooks/tom1-workbook.md) to move from your week to an audit and a
  90-day plan.
- **You lead the HR function:** use the [Human Review Matrix](../../playbooks/human-review-matrix.md),
  write the [first agent contract](../../playbooks/agent-contract.md) with boundaries for automatic
  rejection, personal data, and escalation, then continue with the
  [Volume 2 workbook](../../playbooks/tom2-workbook.md).

!!! danger "Discipline"
    Do not let AI reject candidates automatically because bias can hide in the system. A person
    owns hiring decisions, feedback, and culture.

→ [Role hub](../hr.md) · [audit](../../playbooks/profession-audit-integrated.md) · [plan](../../playbooks/personal-90-day-plan.md).

---
**Sources:** profession automation review (GDPval, AEI, O*NET); book, Chapters 2, 3, and 7.
