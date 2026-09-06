<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/hr
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

---
reading_level: b2-c1-technical
title: "HR specialist: what to automate and which tools to use"
description: A practical map of HR tasks AI can speed up, the hiring decisions a person must keep, and tools to consider.
---

# HR specialist: what to automate and which tools to use

> Field: **HR and people**. Role hub. **Checked: 2026-08-18.** Tools change over time. Sources for this review are at the bottom of the page.

## At a glance

AI is moving quickly into screening, sourcing, interview scheduling, and candidate communication. Human
assessment, culture, and difficult conversations become **more valuable**. The main risk is bias in an
AI assessment of candidates.

!!! info "What the data says (GDPval, Anthropic Economic Index, O*NET)"
    - **Capability (GDPval):** AI can draft structured artifacts such as job posts and emails, and it can
      screen against stated criteria.
    - **Use (AEI):** HR tasks have meaningful exposure, especially screening, first-pass communication,
      and scheduling.
    - **The scale:** two thirds of large enterprises already use AI to screen candidates. In 2024 alone
      such systems processed more than 30 million applications, and drew hundreds of discrimination
      complaints.
    - **Work that did not exist a year ago, compliance:** in 2026 California and Illinois adopted
      enforceable regimes covering AI-assisted hiring, focused on discriminatory outcomes,
      documentation, and transparency, and a US Department of Labor task force began enforcement
      against automated hiring systems that show adverse impact without documentation. In practice
      that means bias testing, records kept for at least four years, notice to candidates, and an
      alternative assessment route.
    - **The rule to carry away:** the **employer** is liable for the vendor's algorithm. If your
      supplier's model is biased, the regulator comes to you, not to the supplier.
    - **Mode:** augment. Let AI support screening, sourcing, and scheduling. Keep hiring decisions, culture,
      and conflict with people. AI must not reject candidates automatically because the process may be biased.
      See the [full data review](_super-analysis.md) and the [role AI strategy](strategy/hr.md).

## What to automate first

1. **Resume screening and ranking.** Semantic matching reads context, not only keywords. A person still
   makes the final selection and owns the decision.
2. **Candidate sourcing.** Find and score possible candidates.
3. **Interview scheduling.** Chatbots and calendars coordinate available times.
4. **Candidate communication.** Automatic updates reduce candidate drop-off.
5. **Draft job posts, emails, and policies.**

## Task review: what AI can do and what you must check

| Task (O*NET) | Give to AI: method or tool | Keep or verify yourself | Prompt to start |
| --- | --- | --- | --- |
| Resume screening | Rank against stated criteria | **Review borderline candidates by hand. Do not auto-reject** |  |
| Sourcing | Search for and score candidates | Relevance and bias | `Write search criteria for this role` |
| Job posts and emails | Drafts | Cliches and tone | `Give me three versions. I will choose one and remove the cliches` |
| Interview preparation | Questions for a skill | Assess the candidate yourself | `Give me five questions that test these skills` |
| Hiring decision | Do not delegate | A person owns the decision |  |

> Do not let AI reject candidates automatically. Bias is a real risk. A person owns the decision and the culture.

## Tools by use case

=== "Leading assistants"

    - **ChatGPT or Claude** for sensitive writing such as policies and communication.

=== "Specialist tools"

    - **Phenom**, **HireVue**, and AI-enabled applicant tracking systems.

## One practical playbook

!!! example "Screen candidates without blind automatic rejection"
    1. AI parses and ranks resumes against stated criteria, with confidence bands.
    2. **Human check:** review borderline candidates by hand. Do not reject them on autopilot.
    3. AI drafts five questions for the target skill. You test the skill yourself in the interview.
    4. Automatic messages keep candidates informed.
    5. Output: the pipeline moves faster. A person still owns the decision and fairness.

## Where not to use AI

!!! danger "Red flags"
    - **Automatic candidate rejection:** bias and unfairness are real risks. A person decides, and the
      process needs an audit.
    - **Candidate and employee personal data:** use only a verified environment.
    - **Personality assessment from text:** AI gives plausible but unsupported judgments.

## Prompt patterns: weak and better

| Weak | Better |
| --- | --- |
| `Assess this candidate` | `Give me five questions so I can test these skills myself` |
| `Write a job post` | `Give me three versions. I will choose one and remove the cliches` |

## Where to move your effort

Move time from routine work into hiring decisions, feedback, conflict, culture, and trust. Human work
becomes more valuable.

### The levels ladder in this role

The five levels from Chapter 5, in the language of this profession. Mark where you stand in your main
tasks this week.

| Level | What it looks like here |
|---|---|
| **1. AI user** | I write job posts and candidate emails with AI |
| **2. Validator** | I check screening for bias. A model will quietly filter out a strong candidate |
| **3. Orchestrator** | I built a hiring funnel where AI holds sourcing and scheduling while I do interviews |
| **4. Outcome owner** | I own whether the person we hired settled in and stayed, not how fast the role closed |
| **5. System builder** | I built a hiring and onboarding process that runs without me in every step |

**Where people usually get stuck.** Levels 1 and 2 are where people stop: roles close faster and nobody measures hire quality. The hiring decision and the hard conversations are what gain value.

Next: [my level of usefulness](../playbooks/usefulness-levels-self-check.md) → [a plan for one level up](../playbooks/plus-one-level-plan.md).

## Ready-made skills and plugins for this role

You can turn repeatable procedures such as criteria-based screening, interview-question sets, and candidate
communication into a portable skill, or use an existing one. Browse [skill banks](https://cheap-intelligence.vercel.app/en/watch/skill-banks),
then see [turn a workflow into a skill](../playbooks/make-it-a-skill.md) to build your own.

## Where to go next

[Map your week](../playbooks/week-inventory.md) → [run the integrated profession audit](../playbooks/profession-audit-integrated.md)
→ [make a 90-day plan](../playbooks/personal-90-day-plan.md). Or open the [workbook](../playbooks/tom1-workbook.md).

---
**Sources for this review:** OpenAI GDPval (2025): <https://openai.com/index/gdpval/> · Anthropic Economic Index: <https://www.anthropic.com/economic-index> · Stanford AI Index (2025): <https://hai.stanford.edu/ai-index> · McKinsey, "The State of AI": <https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai>. Plus the book, Chapters 2, 3, and 7.
