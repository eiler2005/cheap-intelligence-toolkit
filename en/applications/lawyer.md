<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/lawyer
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

---
reading_level: b2-c1-technical
title: "Lawyer: what to automate and which tools to use"
description: A practical map of legal tasks AI can speed up, the checks a lawyer must keep, and tools to consider.
---

# Lawyer: what to automate and which tools to use

> Field: **Legal and compliance**. Role hub. **Checked: 2026-08-18.** Tools change over time. Put confidential client information only in a verified environment.
> Sources for this review are at the bottom of the page.
>
> *This page shows the complete role template. The other role pages follow it.*

## At a glance

Lawyers are among the 44 occupations in the GDPval benchmark, under Professional Services. The best
models produce expert-level work on roughly half of the tested tasks. That means tasks, not whole jobs.
Production gets cheaper. Judgment, strategy, and the authority to sign become more valuable. The main
tool risk is a fabricated law, case, or citation.

!!! info "What the data says (GDPval, Anthropic Economic Index, O*NET)"
    - **Capability (GDPval):** a typical artifact is a "legal brief." Models reach expert level on about
      half of the tasks, but they may invent legal rules and citations.
    - **Use (AEI):** adoption is growing in specialist platforms such as Harvey and CoCounsel. High-stakes
      work still follows an augmentation model.
    - **New work that did not exist a year ago:** since **Aug 2, 2026** the EU AI Act's transparency
      duties are being enforced by the AI Office and national authorities, with penalties up to
      **€15M or 3% of worldwide annual turnover**. Marking obligations have a grace period to Dec 2026
      for systems already on the market. Advising on AI disclosure has moved from a future risk to a
      billable line. Current status by country: [trust and law](https://cheap-intelligence.vercel.app/en/watch/trust-regulation).
    - **Mode:** augment. Let AI handle first-pass research, drafting, and comparison, then verify every
      citation. Keep strategy, negotiation, court work, and signing with the lawyer. See the
      [full data review](_super-analysis.md) and the [role AI strategy](strategy/lawyer.md).

## What to automate first

1. **First-pass research.** Build an initial list of relevant laws and cases in minutes instead of hours.
   **Check every citation against the primary source.**
2. **Incoming contract review.** Ask: "Find the 10 biggest risks for my side, rank them by severity, and
   quote the clause." Then check every quote against the contract.
3. **Version comparison.** Turn two drafts into a differences table with a "who benefits" column.
4. **Document drafting.** Generate a contract, claim letter, or memo outline. You revise it and own the result.
5. **Due diligence workflow.** Use a repeatable process to review a document package in a specialist platform.

## Task review: what AI can do and what you must check

| Task (O*NET) | Give to AI: method or tool | Keep or verify yourself | Prompt to start |
| --- | --- | --- | --- |
| Legal research | First-pass list of laws and cases | **Check every citation against the primary source** | `Find the relevant law and cases, then flag everything I must verify` |
| Contract review | Risks with clause quotes | Materiality and legal position | `List 10 risks for my side by severity and quote each clause` |
| Version comparison | Differences table | Who benefits and what to concede | `Compare these drafts and add a "who benefits" column` |
| Document draft | Contract or claim outline | Language and responsibility | `Draft a contract outline and flag five clauses where risk often hides` |
| Dispute preparation | Timeline and arguments | Strategy and what not to say | `Build a timeline and find weak points in the position` |

> This is an **augmentation** workflow. AI makes the work faster, but the decision and signature stay
> with you. Always verify quotations from laws and cases.

## Tools by use case

=== "Leading assistants"

    - **ChatGPT or Claude** for complex review and drafting. Recheck laws and citations, and keep
      confidential material out of them.

=== "Specialist tools"

    - **Harvey** for workflows such as due diligence and contract review, **CoCounsel** from Thomson Reuters
      and Casetext for research, review, and deposition preparation, plus **Spellbook** and **Westlaw AI**.

## One practical playbook

!!! example "Review a contract in 15 minutes, then verify it"
    1. Upload the contract. Remove identifying details first if you use an external service.
    2. Prompt: "List the 10 biggest risks for [my side], rank them by severity, and quote each clause."
    3. **Human check:** compare every quote with the contract and judge how serious each risk is.
    4. Ask: "What might I have missed under [applicable law]?"
    5. Output: a risk list and a negotiation position. You own the strategy and responsibility.

## Where not to use AI

!!! danger "Red flags"
    - **Quotations from laws and cases:** models invent cases and sections. Verify every citation.
    - **Final position and signature:** never delegate them.
    - **Confidential client information:** legal privilege and personal data require a verified environment.
    - **Fluent does not mean correct:** the more convincing the text sounds, the more carefully you should check it.

## Prompt patterns: weak and better

| Weak | Better |
| --- | --- |
| `Draft a lease` | `Draft a lease outline and flag five clauses where risk often hides` |
| `Is this legal?` | `Which rules apply, and where might they not apply?` |
| `Find case law` | `Find relevant cases and separately flag everything I must verify by hand` |

## Where to move your effort

Move time from routine work into complex deals, negotiation, court work, client relationships, and
strategy. These are levers 1 and 3 in Chapter 2.

### Before, after, and still human

| Before AI, this was the barrier | Now available quickly | Still belongs to the person |
| --- | --- | --- |
| Standard contracts and term checks took hours | A first draft and term comparison take minutes | Complex deals and negotiation |
| Building a position with legal citations took a long time | A cited draft is fast, but every citation needs checking | Citation review, signature, and the decision |
| You produced standard documents | Production is cheaper | You manage the client relationship and strategy |

### The levels ladder in this role

The five levels from Chapter 5, in the language of this profession. Mark where you stand in your main
tasks this week.

| Level | What it looks like here |
|---|---|
| **1. AI user** | I ask the model for a contract draft or to pull case law. It beats starting from a blank page |
| **2. Validator** | I check every citation to a statute and a case. One invented rule costs more than the hour it saved |
| **3. Orchestrator** | I built the route: research, draft, citation check, revision, sign-off, with AI on the early steps |
| **4. Outcome owner** | I own the legal risk of the deal and I sign for it, not the number of documents produced |
| **5. System builder** | I packaged the standard contract flow into templates and checks the team uses without me |

**Where people usually get stuck.** Level 1 is where people stop: the draft arrives and checking citations stays optional. Level 4 is what gains value: accepted risk and a signature.

Next: [my level of usefulness](../playbooks/usefulness-levels-self-check.md) → [a plan for one level up](../playbooks/plus-one-level-plan.md).

## Ready-made skills and plugins for this role

You can turn repeatable procedures such as contract review, version comparison, and due diligence into a
portable skill, or use an existing one. Browse [skill banks](https://cheap-intelligence.vercel.app/en/watch/skill-banks), then see
[turn a workflow into a skill](../playbooks/make-it-a-skill.md) to build your own.

## Where to go next

[Map your week](../playbooks/week-inventory.md) → [run the integrated profession audit](../playbooks/profession-audit-integrated.md)
→ [make a 90-day plan](../playbooks/personal-90-day-plan.md). Or open the [workbook](../playbooks/tom1-workbook.md).

---
**Sources for this review:** OpenAI GDPval (2025): <https://openai.com/index/gdpval/> · Anthropic Economic Index: <https://www.anthropic.com/economic-index> · Stanford AI Index (2025): <https://hai.stanford.edu/ai-index> · McKinsey, "The State of AI": <https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai>. Plus the book, Chapters 2 and 3. EU AI Act enforcement checked against the European Commission on Aug 18, 2026.
