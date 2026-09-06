<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/uchitel
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

---
reading_level: b2
title: "Teacher and instructor: what to automate and which tools to use"
description: A practical map of teaching tasks AI can speed up, the decisions a teacher must keep, and tools to consider.
---

# Teacher and instructor: what to automate and which tools to use

> Field: **Education**. Role hub. **Checked: 2026-08-18.** Tools change over time. Sources for this review are at the bottom of the page. The education section is a guide, not a complete review.

## At a glance

AI helps with material preparation and first-pass grading. Attention to the student, motivation, and live
contact become **more valuable**. See Chapter 7. The main risk is a factual error in learning material.

!!! info "What the data says (GDPval, Anthropic Economic Index, O*NET)"
    - **Capability (GDPval and market evidence):** lesson plans, exercises, material for different ability
      levels, and first-pass grading comments.
    - **Use (AEI):** automation is growing in material preparation.
    - **A 2026 correction that matters here:** the same data shows **teachers** are affected
      relatively less than raw task coverage would suggest. It comes with a direct caveat from the
      authors, though: teaching is named among the fields at risk of **deskilling**. Hand preparation
      and grading to a model and you lose the practice your own judgment rests on. A smaller hit to
      employment is not a smaller risk to craft.
    - **Mode:** strong augmentation. AI supports preparation and grading drafts, with factual checks. A person
      keeps motivation, live contact, and responsibility for assessment. See the
      [full data review](_super-analysis.md) and the [role AI strategy](strategy/uchitel.md).

## What to automate first

1. **Lesson plans and exercises.** Draft options for a topic and class level.
2. **Materials for different ability levels.** Turn one text into versions for several levels in the class.
3. **First-pass grading comments and feedback.** Work from stated criteria. A person owns the grade and responsibility.
4. **Topic explanations.** Produce several explanations for different levels.

## Task review: what AI can do and what you must check

| Task (O*NET) | Give to AI: method or tool | Keep or verify yourself | Prompt to start |
| --- | --- | --- | --- |
| Lesson plans | Draft and options | Facts and fit with the class | `Create a lesson plan and exercises on this topic for [class level]` |
| Multi-level materials | Versions for different levels | Fit with the curriculum | `Write three versions of this text for different levels in the class` |
| Student work review | Criteria and first feedback draft | **Grade and take responsibility yourself** | `Create criteria and a feedback draft for this work` |
| Topic explanation | Several explanations | Accuracy | `Explain this topic in three ways for different levels` |
| Motivation and contact | Do not delegate | Live contact with the student |  |

> Use AI for preparation and check the facts. The teacher keeps the student assessment and live contact.

## Tools by use case

=== "Leading assistants"

    - **ChatGPT or Claude** for sensitive writing and material for different levels.

=== "Specialist tools"

    - **MagicSchool**, **Diffit** for level-based materials, and **Khanmigo** as a guided practice tutor.

## One practical playbook

!!! example "Build multi-level material in 15 minutes"
    1. Give AI the topic and class level. Ask for a lesson plan and exercises.
    2. Request three versions of the text for different levels in the class.
    3. **Human check:** verify facts against a primary source and adapt the material to your class.
    4. Let AI draft feedback on student work. You assign the grade and own the result.
    5. Output: preparation is faster, so you have more time for live work with students.

## Where not to use AI

!!! danger "Red flags"
    - **Facts in learning material:** recheck them. AI makes confident errors.
    - **Assessing a student from their text:** a person makes the decision and owns it.
    - **Data about minors:** take extra care and do not send it to open services.

## Prompt patterns: weak and better

| Weak | Better |
| --- | --- |
| `Grade these essays` | `Create criteria and a feedback draft. I will grade and correct it myself` |
| `Explain the topic` | `Give me three explanations for different levels. I will choose one for the class` |

## Where to move your effort

Move time from preparation into motivation, work with the individual student, and education in the broader
sense. Human work becomes more valuable.

### The levels ladder in this role

The five levels from Chapter 5, in the language of this profession. Mark where you stand in your main
tasks this week.

| Level | What it looks like here |
|---|---|
| **1. AI user** | I prepare materials and assignments with AI |
| **2. Validator** | I check the facts in the material before class. An error goes straight into a student's head |
| **3. Orchestrator** | I built the flow from lesson plan to tiered assignments to first-pass grading, with AI taking the prep |
| **4. Outcome owner** | I own whether the student learned it, not the volume of material handed out |
| **5. System builder** | I built a bank of materials and checks that colleagues use |

**Where people usually get stuck.** Level 1 is where people stop: prep is faster and there is no more time for the individual student. Motivation and live contact are what gain value.

Next: [my level of usefulness](../playbooks/usefulness-levels-self-check.md) → [a plan for one level up](../playbooks/plus-one-level-plan.md).

## Ready-made skills and plugins for this role

You can turn repeatable procedures such as lesson planning, multi-level materials, and criteria-based
feedback drafts into a portable skill, or use an existing one. Browse [skill banks](https://cheap-intelligence.vercel.app/en/watch/skill-banks),
then see [turn a workflow into a skill](../playbooks/make-it-a-skill.md) to build your own.

## Where to go next

[Map your week](../playbooks/week-inventory.md) → [run the integrated profession audit](../playbooks/profession-audit-integrated.md)
→ [make a 90-day plan](../playbooks/personal-90-day-plan.md). Or open the [workbook](../playbooks/tom1-workbook.md).

---
**Sources for this review:** OpenAI GDPval (2025): <https://openai.com/index/gdpval/> · Anthropic Economic Index: <https://www.anthropic.com/economic-index> · Stanford AI Index (2025): <https://hai.stanford.edu/ai-index> · McKinsey, "The State of AI": <https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai>. The education section is a guide. Plus the book, Chapters 2, 3, and 7.
