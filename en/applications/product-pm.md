<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/product-pm
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

---
reading_level: b2-c1-technical
title: "Product manager: what to automate and which tools to use"
description: A practical map of product work AI can speed up, the choices a person must keep, and tools to consider.
---

# Product manager: what to automate and which tools to use

> Field: **IT and product**. Role hub. **Checked: 2026-08-18.** Tools change over time. Sources for this review are at the bottom of the page.

## At a glance

AI automates labor-heavy work: research synthesis, feedback clustering, first drafts of product requirement
documents, and support for prioritization. Deciding what to build and why, setting priorities, and earning
the team's trust become **more valuable**. The main risk is a convincing artifact with no real substance.

!!! info "What the data says (GDPval, Anthropic Economic Index, O*NET)"
    - **Capability (GDPval):** AI performs well on text and synthesis, including first drafts of product
      requirement documents and user stories, plus interview synthesis.
    - **Use (AEI):** automation is growing in research and documentation.
    - **What actually moved to agents in 2026:** continuous competitor monitoring, covering product
      updates, pricing, app-store reviews, ratings and engineering blogs, with a summary of what
      changed and why it matters; natural-language questions against product analytics without
      writing SQL; and, at the frontier, agentic systems that design, launch and report on product
      experiments with little human input.
    - **What that makes more valuable:** strategic and systems thinking, business judgment, customer
      empathy and stakeholder alignment. The role moves from processing information to making the
      call, which is the Chapter 5 argument in one profession.
    - **Mode:** augment. Let AI handle documentation and synthesis. Keep the choice of what to build and why,
      priorities, what not to do, and team trust. See the [full data review](_super-analysis.md) and the
      [role AI strategy](strategy/product-pm.md).

## What to automate first

1. **Interview and feedback synthesis.** Transcribe and cluster thousands of signals into possible insights.
2. **First drafts of product requirements, user stories, and release notes.** Remove the blank-page problem.
3. **Competitor and market research.** Require citations to the sources.
4. **Natural-language questions about metrics.** Find trends and anomalies faster than a manual review.
5. **Prioritization support.** Group ideas, remove duplicates, and suggest an order using your criteria.

## Task review: what AI can do and what you must check

| Task (O*NET) | Give to AI: method or tool | Keep or verify yourself | Prompt to start |
| --- | --- | --- | --- |
| Interview synthesis | Transcription and topic clusters | Real patterns versus noise | `Cluster the problems in these interviews` |
| Requirements and stories | First draft | Priorities and what not to do | `Ask the questions we must answer before writing the requirements` |
| Competitors and market | Research with sources | Check the figures | `Review competitors and link every claim to a source` |
| Metrics | Answers to natural-language questions | Definitions and causality | `What changed in this metric, and why?` |
| Prioritization | Suggestions using criteria | The bet and the decision | `Give me three prioritization options and the tradeoffs in each one` |

> Give documentation and synthesis to AI. You still decide what to build and why, set priorities, and hold
> the team's trust.

## Tools by use case

=== "Leading assistants"

    - **ChatGPT or Claude** for synthesis, product requirements, and a first strategy draft.

=== "Specialist tools"

    - **ChatPRD** for product requirements, **Dovetail** for research, **Crayon** for competitor work,
      **Aha!** for roadmaps, **Mixpanel** and **PostHog** for metrics, plus **NotebookLM** and **Granola**
      for meetings.

## One practical playbook

!!! example "Turn 50 interviews into insights and product requirements"
    1. Upload interview transcripts to a research tool and create topic and problem clusters.
    2. AI drafts product requirements and user stories from the clusters.
    3. **Human check:** you decide the priorities, what not to do, and the bet.
    4. Compare the insights with metrics. Do not trust only one source.
    5. Output: the research takes hours. You still own the decision and responsibility.

## Where not to use AI

!!! danger "Red flags"
    - **AI-selected priorities:** the model does not know your full context. You decide.
    - **Market or competitor figures from the model's memory:** check them against sources.
    - **User data:** remove identifying details.

## Prompt patterns: weak and better

| Weak | Better |
| --- | --- |
| `Create a roadmap` | `Give me three prioritization options and the tradeoffs in each one` |
| `Write the product requirements` | `Ask the questions we must answer before writing the requirements` |

## Where to move your effort

Move time from documentation into deciding what to build and why, setting priorities, and earning team
trust. This is the shift from output to outcome in Chapter 5.

### The levels ladder in this role

The five levels from Chapter 5, in the language of this profession. Mark where you stand in your main
tasks this week.

| Level | What it looks like here |
|---|---|
| **1. AI user** | I synthesize research and draft the PRD with AI |
| **2. Validator** | I check the artifact for emptiness. A convincing document with no real insight is this role's main risk |
| **3. Orchestrator** | I built the loop from feedback to synthesis to priorities to PRD |
| **4. Outcome owner** | I own whether what we built is what users needed, not the volume of documentation |
| **5. System builder** | I built a discovery and prioritization process the team runs on its own |

**Where people usually get stuck.** Level 1 is where people stop: more documents, no more decisions. Priorities and the ability to say what we are not building are what gain value.

Next: [my level of usefulness](../playbooks/usefulness-levels-self-check.md) → [a plan for one level up](../playbooks/plus-one-level-plan.md).

## Ready-made skills and plugins for this role

You can turn repeatable procedures such as interview synthesis, product requirements and user stories, and
release notes into a portable skill, or use an existing one. Browse [skill banks](https://cheap-intelligence.vercel.app/en/watch/skill-banks),
then see [turn a workflow into a skill](../playbooks/make-it-a-skill.md) to build your own.

## Where to go next

[Map your week](../playbooks/week-inventory.md) → [run the integrated profession audit](../playbooks/profession-audit-integrated.md)
→ [make a 90-day plan](../playbooks/personal-90-day-plan.md). Or open the [workbook](../playbooks/tom1-workbook.md).

---
**Sources for this review:** OpenAI GDPval (2025): <https://openai.com/index/gdpval/> · Anthropic Economic Index: <https://www.anthropic.com/economic-index> · Stanford AI Index (2025): <https://hai.stanford.edu/ai-index> · McKinsey, "The State of AI": <https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai>. Plus the book, Chapters 2, 3, and 5.
