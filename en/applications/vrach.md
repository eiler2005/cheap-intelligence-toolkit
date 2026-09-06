<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/vrach
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

---
reading_level: b2-c1-technical
title: "Doctor: what to automate and which tools to use"
description: A practical map of medical documentation tasks AI can support, with strict clinical limits and verification steps.
---

# Doctor: what to automate and which tools to use

> Field: **Healthcare**. Role hub. **Checked: 2026-08-18.**
> **Warning:** AI is an assistant for writing and administration here, **not for diagnosis or treatment**.
> A doctor makes the decisions under the applicable procedures. Use any tool only inside a certified healthcare
> environment. Sources for this review are at the bottom of the page. The medical section is a guide.

## At a glance

AI reduces paperwork and writing, including visit documentation, letters, and explanations. Clinical
decisions, responsibility, and contact with the patient belong **only to a person**. This limit is not open
to negotiation. The risks are dangerous errors and invented data.

!!! info "What the data says (GDPval, Anthropic Economic Index, O*NET)"
    - **Capability (GDPval and market evidence):** visit documentation through ambient scribing, discharge
      summaries, and explanations. These are writing and administrative tasks.
    - **Use (AEI):** documentation is becoming more automated. Clinical work is not.
    - **A 2026 correction that matters here:** adjust task coverage for how often the attempt actually
      succeeds and **radiologists** turn out to be affected considerably more than raw coverage
      suggests. This is not a statement about doctors in general. It is about one part of the work:
      reading images, where a checkable ground truth exists. Diagnosis, prescription, and
      responsibility stay with a person, but wherever the work reduces to recognition against a
      reference, the squeeze arrives faster.
    - **Mode:** strong augmentation. AI supports paperwork and documentation. Only a doctor diagnoses,
      prescribes, and takes responsibility. See the [full data review](_super-analysis.md) and the
      [role AI strategy](strategy/vrach.md).

## What to automate first: writing and administration, not clinical care

1. **Visit documentation with ambient scribing.** AI listens to the visit and drafts the note. The doctor
   reviews and signs it.
2. **Discharge summaries and letters.** Draft them from the supplied data. Verification is mandatory.
3. **Plain-language explanations for patients.** Prepare supporting material for the visit.
4. **Literature search.** Build an initial list and verify every source.

## Task review: what AI can do and what you must check

| Task (O*NET) | Give to AI: method or tool | Keep or verify yourself | Prompt to start |
| --- | --- | --- | --- |
| Visit documentation | Ambient notes in a certified environment | **Review and sign** |  |
| Discharge summaries and letters | Draft from supplied data | Facts and dosages | `Draft a discharge summary from this data. I will verify it` |
| Patient explanation | Plain-language draft | Accuracy | `Explain this term to a patient in plain language` |
| Literature search | Initial list | Verify the sources | `Find literature on this topic and include links` |
| Diagnosis and prescription | Do not delegate | Only the doctor owns the decision |  |

> AI supports writing and administration, not clinical care. Put personal and medical data only in a
> verified environment.

## Tools by use case

=== "Leading assistants"

    - **ChatGPT or Claude** for administrative writing and patient explanations only, with no patient
      personal or medical data. Never for diagnosis or treatment.

=== "Specialist tools"

    - **Nuance DAX** and **Abridge** for ambient clinical documentation.

## One practical playbook

!!! example "Document a visit without spending all your energy on paperwork"
    1. In a certified environment, AI records the visit and drafts the note.
    2. **Human check:** the doctor reads, corrects, and signs it. The doctor owns the responsibility.
    3. Prepare a separate plain-language explanation for the patient.
    4. Output: less paperwork and more time for the patient. The doctor owns all clinical work.

## Where not to use AI

!!! danger "Red flags"
    - **AI diagnosis or treatment:** do not use it this way. It is a writing tool, not a doctor.
    - **Patient personal and medical data:** use only a verified and certified environment, never an open service.
    - **Facts and dosages:** verify them against professional sources.

## Prompt patterns: weak and better

| Weak | Better |
| --- | --- |
| `Make a diagnosis` | `Explain this term to a patient in plain language` |
| `Prescribe treatment` | `Create a list of questions the patient can bring to the visit` |

## Where to move your effort

Move time from paperwork into patient communication, clinical judgment, and responsibility. Human work
and accountable decisions remain central. See Chapter 10.

### The levels ladder in this role

The five levels from Chapter 5, in the language of this profession. Mark where you stand in your main
tasks this week.

| Level | What it looks like here |
|---|---|
| **1. AI user** | I use AI for visit documentation, discharge summaries, and patient explanations |
| **2. Validator** | I read every generated text before it reaches the chart. An invented detail in a record is dangerous |
| **3. Orchestrator** | I set up the visit so paperwork goes to the machine and the time it frees goes to the patient |
| **4. Outcome owner** | I own the clinical decision and its consequences. That is not delegated at any level |
| **5. System builder** | I set up documentation templates and checks for the department |

**Where people usually get stuck.** This ladder is about paperwork and how a visit is organized, not about clinical work. Diagnosis, treatment, and responsibility stay with the doctor at every level.

Next: [my level of usefulness](../playbooks/usefulness-levels-self-check.md) → [a plan for one level up](../playbooks/plus-one-level-plan.md).

## Ready-made skills and plugins for this role

You can turn repeatable procedures such as visit documentation, discharge summaries and letters, patient
explanations, and literature searches into a portable skill, or use an existing one. Browse
[skill banks](https://cheap-intelligence.vercel.app/en/watch/skill-banks), then see
[turn a workflow into a skill](../playbooks/make-it-a-skill.md) to build your own. Do not turn diagnosis or
treatment into an AI skill.

## Where to go next

[Map your week](../playbooks/week-inventory.md) → [run the integrated profession audit](../playbooks/profession-audit-integrated.md)
→ [make a 90-day plan](../playbooks/personal-90-day-plan.md). Or open the [workbook](../playbooks/tom1-workbook.md).

---
**Sources for this review:** OpenAI GDPval (2025): <https://openai.com/index/gdpval/> · Anthropic Economic Index: <https://www.anthropic.com/economic-index> · Stanford AI Index (2025): <https://hai.stanford.edu/ai-index> · McKinsey, "The State of AI": <https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai>. The medical section is a guide. Plus the book, Chapters 2, 3, and 10.
