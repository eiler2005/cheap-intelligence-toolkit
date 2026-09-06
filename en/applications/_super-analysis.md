<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/_super-analysis
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

---
reading_level: b2-c1-technical
title: "How AI changes professions: a data review"
description: A careful task-level comparison of major professions using GDPval, the Anthropic Economic Index, and O*NET.
---

# How AI changes professions: a data review

> A detailed review of major professions through three sources, without hype or panic.
> **Date: 2026-08-18.** The figures show direction, not a verdict. Sources: OpenAI GDPval
> (<https://openai.com/index/gdpval/>), the Anthropic Economic Index
> (<https://www.anthropic.com/economic-index>), and O*NET (<https://www.onetonline.org/>).

## Method: three sources and three questions

| Source | Question | What it shows |
|---|---|---|
| **GDPval** (OpenAI, 2025; the GDPval-AA v2 scale was re-anchored Jun 15, 2026) | **Can** AI do the work? | On real tasks from 44 professions across 9 sectors, the best models produce work rated "as good as or better than an expert" in about **half of the tasks**. This is about tasks, not whole professions. The same work is also completed roughly **100 times faster and 100 times cheaper** than by a human expert. |
| **Anthropic Economic Index** (Jan and Jun 2026 reports) | **Do** people use it this way? | Where people already use AI at work and whether the mode is assistance, automation, or an API workflow. |
| **O*NET** | **What tasks** make up the profession? | A standard profession-to-task breakdown that shows which tasks move and which remain. |

!!! tip "The main reading rule"
    AI replaces **tasks, not whole professions**. Production, or output, moves first. Responsibility
    for the result, or outcome, remains with people: judgment, verification, trust, and decisions.
    The useful question is not "Will AI replace me?" It is "**Which level can I move to when
    production gets cheaper?**"

## What the 2026 data changed

Three things worth knowing before you read the table below.

**1. Task coverage rose, and quickly.** The Anthropic Economic Index puts the share of work tasks AI
touches in some way at **49%, up from 36% in January 2025**. That is not "half the work is gone." It
is "AI at least touches half the tasks."

**2. Task coverage and real impact on a profession are different things.** This is the most useful
finding of the year: adjust coverage for **how often the attempt actually succeeds**, and the ranking
of professions changes. **Data entry keyers and radiologists** are affected considerably more than
coverage alone suggests. **Teachers and software developers** are affected relatively less than you
might expect. The reader's takeaway is simple: "AI has been tried on your task many times" and "AI
does your task" are not the same statement, and they diverge sharply by profession.

**3. Augmentation overtook automation, but one reading is not a trend.** In the current data,
collaborative use runs at **52%** against **45%** for full delegation. The authors' own caveat
matters: this is a reversal from August 2025, and over the longer run the automation share had been
climbing, from 41% in January 2025. Do not build a conclusion on a single reading.

!!! warning "The risk to hold next to these numbers"
    The same data shows that tasks requiring **more education**, an average of about 14.4 years of
    schooling, are automated disproportionately often. The authors name the possible effect directly:
    **deskilling** in fields such as technical writing, travel agencies, and teaching. That is exactly
    the trap Chapter 8 describes. A tool that does the work for you also takes away the practice your
    judgment was built on.

## Summary: what moves first and what remains

| Profession | Mode | What AI takes first | What remains human |
|---|---|---|---|
| Developer | high task replacement | boilerplate, tests, review | architecture, security, production |
| Analyst | high task replacement | SQL, dashboards, data cleaning | choosing the question and judging whether the conclusion is reliable |
| Customer support | high task replacement | standard answers | difficult cases, retention, empathy |
| Marketer | augment→replace | content, SEO, reports | strategy, taste, brand, distribution |
| B2B sales | augment→replace | outreach, CRM updates, summaries | meetings, trust, closing |
| Accountant | high task replacement | source documents, reconciliation, spreadsheets | sign-off, disputed issues, work with auditors and regulators |
| Financial analyst | augment | data assembly, first-pass forecast | scenarios and turning figures into decisions |
| Lawyer | augment, high stakes | research, drafting, comparison | strategy, negotiation, sign-off |
| HR | augment | screening, sourcing, planning | hiring decisions, culture |
| Product / PM | augment | PRDs, research synthesis | what to build, why, and in what order |
| Designer | augment→replace | image generation and routine work | taste, art direction, the business problem |
| Teacher · Doctor | strong augmentation | preparation, documentation | live contact, judgment, responsibility |

---

## Developer → [hub](razrabotchik.md)

- **O*NET tasks:** write and test code, review, debug, design architecture, and maintain production.
- **GDPval capability:** generates code, tests, and documentation, and can make multi-file changes as an agent.
- **Adoption (AEI):** Computer and Mathematical is one of the task groups with the greatest exposure.
  Some tasks are moving from assistance into automated API workflows.
- **What replacement looks like:** **junior tasks** such as boilerplate, simple features, and tests move
  first. This disrupts the entry route into the profession. Architecture, security, responsibility for
  production, and the role of "agent boss" remain and gain value. The profession moves upward rather
  than disappearing.

## Data analyst → [hub](analitik.md)

- **O*NET:** collect and clean data, write queries, build visualizations, interpret results, and monitor KPIs.
- **GDPval:** natural-language-to-SQL, dashboards, and summaries are structured artifacts that suit AI.
- **Adoption:** high. SQL, reporting, and data cleaning are moving quickly to the "AI draft + human review" mode.
- **What replacement looks like:** report and SQL production moves almost entirely to AI, with review.
  The person decides **which question to ask of the data**, whether the conclusion is reliable, and how
  to turn it into a decision. "AI calculated it, so I believed it" is the trap.

## Customer support → [hub](podderzhka.md)

- **O*NET:** receive requests, answer questions, solve problems, escalate, and document the case.
- **GDPval:** a standard work product is a "customer support conversation," where AI performs well.
- **Adoption:** automation is high in retail and service. Bots handle frequent questions.
- **What replacement looks like:** the entry layer shrinks most because standard first-line work moves
  to bots. Difficult or confrontational cases, retention of valuable customers, and empathy remain.
  There are fewer operators, and the bar is higher.

## Accountant → [hub](buhgalter.md)

- **O*NET:** entries, reconciliation, source-document processing, reporting, tax, and audit.
- **GDPval:** real tasks include an Excel depreciation schedule, an audit of risk metrics on a
  "Population" worksheet, and a Form 1040 tax return converted to PDF. At task level, models already
  compete on structured artifacts.
- **Adoption:** growing in finance. Source documents, reconciliation, and spreadsheets automate before
  disputed accounting judgments.
- **What replacement looks like:** spreadsheet production, reconciliation, and source-document handling
  move away. Responsibility for the figure and the signature cannot be transferred. Disputed issues and
  communication with auditors and regulators remain. The profession gets smaller in headcount and heavier
  in responsibility.

## Marketer → [hub](marketolog.md)

- **O*NET:** market research, content, campaigns, SEO, analytics, and brand.
- **GDPval:** content and polished artifacts are areas where models perform well.
- **Adoption:** business outreach and content workflows automate quickly. Exact savings depend on the
  channel, the data, and the discipline of verification.
- **What replacement looks like:** content, SEO, and report production gets much cheaper, so **generic
  work loses value**. Strategy, taste, brand voice, audience relationships, and distribution remain.
  This is lever 3.

## B2B sales → [hub](sales-b2b.md)

- **O*NET:** find leads, write outreach, prepare proposals, negotiate, maintain the CRM, and close.
- **GDPval / adoption:** **business sales and outreach** show high and fast-growing automation in AEI.
- **What replacement looks like:** routine outreach, CRM entry, call summaries, and research move away.
  Meetings, trust, reading the situation, and closing the deal remain at the center. These connect to
  levers 1 and 3. This is augmentation, not full replacement.

## Financial analyst / FP&A → [hub](finanalitik.md)

- **O*NET:** models, forecasts, budgets, reports, scenarios, and variance analysis.
- **GDPval:** structured financial artifacts suit AI. Automated processing helps when there is a source
  of truth and a metric that can be checked.
- **What replacement looks like:** data assembly, rolling forecasts, and standard reports move to AI.
  The person decides **which scenarios matter**, negotiates the plan, and turns figures into business
  action. This is augmentation.

## Lawyer → [hub](lawyer.md)

- **O*NET:** legal research, document drafting, review, negotiation, representation, and risk assessment.
- **GDPval:** a standard artifact is a "legal brief." Models reach expert level in about half of tasks,
  **but hallucinations remain normal**.
- **Adoption:** use is growing in specialist platforms such as Harvey and CoCounsel. High stakes keep the
  dominant mode at **augmentation**.
- **What replacement looks like:** first-pass research, drafting, and redline comparison move to AI, with
  every source checked. Deal or dispute strategy, negotiation, court work, and **signing off on the
  position** remain. Tasks change, but the profession remains.

## HR specialist → [hub](hr.md)

- **O*NET:** sourcing, screening, interviews, onboarding, development, and conflict resolution.
- **GDPval / adoption:** screening and candidate communication automate well, but the final decision and
  an anti-bias audit remain human.
- **What replacement looks like:** screening, sourcing, planning, and communication move to AI. Hiring
  decisions, feedback, conflict, and culture remain. Because of bias risk, AI cannot own automatic
  rejection. This is augmentation.

## Product / PM → [hub](product-pm.md)

- **O*NET:** research, PRDs, prioritization, coordination, metric analysis, and releases.
- **GDPval:** AI performs well on first-pass PRDs, user stories, and interview synthesis.
- **What replacement looks like:** documentation and research synthesis move to AI. The PM still owns
  **what to build and why, priorities, what not to do, and team trust**. This is augmentation.

## Designer → [hub](dizayner.md)

- **O*NET:** concepts, layouts, visual assets, iteration, and client work.
- **GDPval / market:** image generation is getting cheaper very quickly.
- **What replacement looks like:** generation and routine tasks such as background removal, upscaling,
  and resizing move to AI. **Generic work loses value.** Taste, art direction, the system, and the
  business problem remain. The lower layer moves from augmentation toward replacement.

## Teacher and doctor → [teacher](uchitel.md) · [doctor](vrach.md)

- **O*NET for teachers:** lesson plans, materials, assessment, explanation, and motivation.
  **For doctors:** consultation, diagnosis, treatment, documentation, and patient communication.
- **What replacement looks like:** **strong augmentation, not replacement.** AI reduces preparation and
  documentation. For doctors, this includes ambient documentation during a visit. For teachers, it
  includes plans and assessment support. Live contact, clinical or educational judgment, and
  responsibility cannot be transferred. AI does not own a diagnosis or the assessment of a person.

---

## What to do with this

Do not race to "beat replacement." Move one level up in your role, from producing output to owning the
outcome. Start with a diagnosis and a plan:
[map your week](../playbooks/week-inventory.md) → [run the integrated audit](../playbooks/profession-audit-integrated.md)
→ [make a 90-day plan](../playbooks/personal-90-day-plan.md).

> ⚠️ The figures show direction, not a guarantee. The GDPval and AEI task descriptions are paraphrases.
> Check licenses and exact wording at the original source. Predictions of "expert parity by the end of
> 2026" and "frequently outperforming experts by 2027" come from the organization that built the
> benchmark. Treat them as an interested party's position, not a measurement.
