<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/analitik
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

---
reading_level: b2-c1-technical
title: "Data analyst: what to automate and which tools to use"
description: A practical map of analytics tasks AI can speed up, the checks a person must keep, and tools to consider.
---

# Data analyst: what to automate and which tools to use

> Field: **Analytics and data**. Role hub. **Checked: 2026-08-18.** Task baskets and tools change over time.
> Sources for this review are at the bottom of the page.

## At a glance

AI is quickly taking over first drafts of SQL, reports, data cleaning, and summaries. The value moves to
two questions: **What should you ask the data?** and **Can you trust the answer?** The main risk is a
confidently wrong number or correlation.

!!! info "What the data says (GDPval, Anthropic Economic Index, O*NET)"
    - **Capability (GDPval):** natural language to SQL, dashboards, and summaries are structured artifacts,
      an area where AI performs well.
    - **Use (AEI):** task exposure is high. Reports, queries, and summaries often follow an "AI draft,
      human verification" workflow.
    - **A 2026 correction:** in current AEI data, collaborative use (52%) has overtaken full
      delegation (45%). For an analyst that is direct confirmation of the job: what gets paid for is
      not "the model calculated it" but "the model calculated it and a person checked it." The
      authors' caveat: this reverses August 2025, and the longer trend had automation rising.
    - **Mode:** high task substitution. AI takes over SQL and report production. The person keeps the choice
      of question and responsibility for trusting the result. See the [full data review](_super-analysis.md)
      and the [role AI strategy](strategy/analitik.md).

## What to automate first

1. **Regular dashboards and KPIs.** Automate high-frequency work that needs little context, with checks.
2. **SQL drafts.** Turn a natural-language question into SQL or Python with **editable code** you can inspect.
3. **Cleaning and normalization.** Extract data from APIs and bring it into one schema.
4. **Report summaries.** Draft written findings from a table or dashboard.
5. **Anomaly detection.** Monitor metrics for unusual changes.

## Task review: what AI can do and what you must check

| Task (O*NET) | Give to AI: method or tool | Keep or verify yourself | Prompt to start |
| --- | --- | --- | --- |
| SQL queries | Natural language to SQL with **editable code** | Read the SQL for logic and edge cases | `Draft the SQL and flag where it could return the wrong result` |
| Data cleaning | Normalization and deduplication | Compare with the source of truth | `Put this into one schema and show what may have been lost` |
| Dashboards and KPIs | Regular automatic reports | Match metric definitions to the data dictionary |  |
| Interpretation | Hypotheses from the data | Which conclusion you can defend | `Give two hypotheses and show where the data does not support them` |
| Forecasting | Baseline model | Assumptions and risks | `Which assumptions do you need, and how weak are they?` |

> The trap is simple: "AI calculated it, so I believed it." Always compare the aggregate with the source of truth.

## Tools by use case

=== "Leading assistants"

    - **ChatGPT or Claude** for complex SQL, Python, and logic review.

=== "Specialist tools"

    - **Querio** turns natural language into SQL or Python with editable code, so you can check every answer.
      **ThoughtSpot** works directly with a data warehouse. **Domo** is another reference option.

## One practical playbook

!!! example "From an ad hoc question to a verifiable answer"
    1. Ask the data question in plain language in a tool that converts natural language to SQL.
    2. Get the **code and the result**, not a hidden answer.
    3. **Human check:** compare the aggregate with the source of truth, read the SQL for logical errors, and
       confirm that metric definitions match your data dictionary.
    4. Use the answer in a decision only after those checks.
    5. Output: an answer in minutes, under your review. You are not trusting a number only because AI produced it.

## Where not to use AI

!!! danger "Red flags"
    - **Numbers, correlations, and statistical conclusions:** sounding statistical does not make them correct.
      Compare them with the source of truth.
    - **User and customer data:** do not send it to outside services without a verified environment.
    - **Decisions based on analysis:** a person owns the bet and the responsibility.

## Prompt patterns: weak and better

| Weak | Better |
| --- | --- |
| `Draw a conclusion from this table` | `Give two hypotheses and show where the data does not support them` |
| `Write SQL` | `Draft the SQL and flag where it could return the wrong result` |
| `Build a forecast` | `Which assumptions do you need, and how weak are they?` |

## Where to move your effort

Move time from routine production into choosing the question, owning the metric, and becoming the person
whose judgment others trust. This is the shift from output to outcome in Chapters 2 and 5.

### Before, after, and still human

| Before AI, this was the barrier | Now available quickly | Still belongs to the person |
| --- | --- | --- |
| Collecting and joining data took hours or days | A first report and summary take minutes | Deciding what question to ask |
| Reviewing dozens of sources took one or two days | A cited review takes about 30 minutes when sources are already collected | Verifying conclusions, setting the quality bar, and earning business trust |
| You supplied tables | Table production is cheaper | You own the metric, and others rely on your judgment |

### The levels ladder in this role

The five levels from Chapter 5, in the language of this profession. Mark where you stand in your main
tasks this week.

| Level | What it looks like here |
|---|---|
| **1. AI user** | I write SQL and assemble the report with AI faster |
| **2. Validator** | I check the numbers and the logic. A confidently wrong number is more dangerous than no number |
| **3. Orchestrator** | I built the loop from question to data to calculation to check to conclusion |
| **4. Outcome owner** | I own the metric and the decision made on my conclusion |
| **5. System builder** | I built the data and checking layer the team uses without me |

**Where people usually get stuck.** Levels 1 and 2 are where people stop: queries write themselves, and somebody else still decides what to ask the data. Framing the question is what gains value.

Next: [my level of usefulness](../playbooks/usefulness-levels-self-check.md) → [a plan for one level up](../playbooks/plus-one-level-plan.md).

## Ready-made skills and plugins for this role

You can turn repeatable procedures such as checked SQL drafts, data quality checks, and KPI dashboard
summaries into a portable skill, or use an existing one. Browse [skill banks](https://cheap-intelligence.vercel.app/en/watch/skill-banks),
then see [turn a workflow into a skill](../playbooks/make-it-a-skill.md) to build your own.

## Where to go next

[Map your week](../playbooks/week-inventory.md) → [run the integrated profession audit](../playbooks/profession-audit-integrated.md)
→ [make a 90-day plan](../playbooks/personal-90-day-plan.md). Or open the [workbook](../playbooks/tom1-workbook.md).

---
**Sources for this review:** OpenAI GDPval (2025): <https://openai.com/index/gdpval/> · Anthropic Economic Index: <https://www.anthropic.com/economic-index> · Stanford AI Index (2025): <https://hai.stanford.edu/ai-index> · McKinsey, "The State of AI": <https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai>. Plus the book, Chapters 2, 3, and 5.
