<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/buhgalter
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

---
reading_level: b2-c1-technical
title: "Accountant: what to automate and which tools to use"
description: A practical map of accounting tasks AI can handle, the checks a person must keep, and tools to consider.
---

# Accountant: what to automate and which tools to use

> Field: **Finance and accounting**. Role hub. **Checked: 2026-08-18.** Tools change over time. Put sensitive data only in a verified environment. The figures show
> direction, not a guaranteed result. Sources for this review are at the bottom of the page.

## At a glance

Accounting is one of the most automatable professions. Source documents, reconciliations, and standard
explanations move to automation before disputed decisions do. A person still owns every number and signature.

!!! info "What the data says (GDPval, Anthropic Economic Index, O*NET)"
    - **Capability (GDPval):** real tasks include depreciation in Excel, an audit of risk metrics, and
      turning Form 1040 data into a PDF. Models reach expert level on about half of the tasks.
    - **Use (AEI):** automation is growing in routine finance work. Disputed and accountable work stays
      with a person.
    - **The 2026 numbers:** enterprise use of generative AI in tax and accounting firms nearly tripled,
      from 8% in 2024 to 21% in 2025. The most common uses are tax research (77%), return preparation
      (63%), and advisory work (62%).
    - **Where the freed time goes:** accountants working with AI reallocated about **8.5% of working
      time**, roughly 3.5 hours in a 40-hour week, from data entry to client communication and quality
      assurance. That is the output-to-outcome move, counted in hours.
    - **An important reversal of cause:** the US profession has lost more than a third of its licensed
      workforce since 2019, and about 75% of partners are due to retire within a decade. AI here is
      more often adopted **as an answer to a staffing shortage** than to replace anyone. Most firms
      remain in the assistant phase, and professional judgment stays with a person.
    - **Mode:** high task substitution. Software takes over table production and reconciliation. People
      keep signing authority, disputed items, and work with auditors. See the
      [full data review](_super-analysis.md) and the [role AI strategy](strategy/buhgalter.md).

## What to automate first

1. **Source document capture with OCR.** A photo or scan of a receipt or invoice becomes accounting data
   automatically. Dext, Kontur, and SBIS are examples. This removes the largest amount of manual entry.
2. **Bank-feed reconciliation.** AI matches transactions by amount, date, and description, then flags
   differences and duplicates. Use an accounting system with automatic reconciliation.
3. **Transaction categorization.** The model learns from your entries and suggests categories. You confirm
   disputed items.
4. **Draft variance explanations.** AI drafts an explanation for a reporting variance. You correct it.
5. **Anomaly detection before close.** AI flags unusual amounts and duplicate entries before submission.

## Task review: what AI can do and what you must check

| Task (O*NET) | Give to AI: method or tool | Keep or verify yourself | Prompt to start |
| --- | --- | --- | --- |
| Source documents | OCR capture of receipts and invoices with Dext, Kontur, or SBIS | Sample-check extracted data |  |
| Bank reconciliation | Automatic matching by amount, date, and description | Review only the differences | `Match these transactions and flag differences in amount and date` |
| Categorization | Suggest categories from history | Confirm disputed items | `Suggest a category and explain why. Flag low-confidence items` |
| Reporting explanations | Draft a variance comment | Check facts and numbers | `Draft an explanation for the variance in these figures` |
| Tax calculation | Formula and list of required inputs | Recalculate and sign yourself | `Show the formula and required inputs. I will calculate it myself` |

> Delegate production and **strengthen verification**. Keep learning tasks, where you build your own skill,
> for yourself. See Chapter 8.

## Tools by use case

=== "Leading assistants"

    - **ChatGPT or Claude** for complex analysis and letters. Check every number and keep confidential
      material out of them.

=== "Specialist tools"

    - **Dext** captures data from receipts, invoices, and statements. **Docyt** provides end-to-end
      accounting with a copilot. **Xero and QuickBooks AI** support reconciliation and reporting.

## One practical playbook

!!! example "Reconcile a month in one evening instead of one day"
    1. Connect the bank feed to your accounting system or import the transactions.
    2. Run automatic matching. The system marks matches and differences.
    3. **Human check:** review only the differences, including timing, partial payments, and duplicates.
    4. For disputed entries, ask: "Which signs of an error should I check in this entry?"
    5. Output: the reconciliation is complete. Your time went into disputed items, not a full manual review.

## Where not to use AI

!!! danger "Red flags"
    - **Numbers and calculations:** a model may mix up rates and periods. Recalculate them.
    - **Signing and filing reports:** responsibility cannot be delegated.
    - **Personal and commercial data:** do not send it to outside or foreign services without a verified environment.

## Prompt patterns: weak and better

| Weak | Better |
| --- | --- |
| `Calculate the tax` | `Show the formula and required inputs. I will calculate and verify it myself` |
| `Was this entered correctly?` | `Which signs of an error should I check in this entry?` |
| `Write a response to this request` | `Give me a response outline and flag where you need facts from me` |

## Where to move your effort

Move time from routine work into disputed issues, tax positions, work with auditors, and client advice.
Competing with a machine on data-entry speed is a race to zero. See Chapter 2.

### Before, after, and still human

| Before AI, this was the barrier | Now available quickly | Still belongs to the person |
| --- | --- | --- |
| Entries, reconciliation, and input were manual | Initial processing and reconciliation are fast | Disputed issues and the tax position |
| Reviewing a document package took a long time | Initial review and a table take minutes | Work with auditors and ownership of every number |
| Your value was data-entry speed | Entry is cheaper | Your value is judgment and client advice |

### The levels ladder in this role

The five levels from Chapter 5, in the language of this profession. Mark where you stand in your main
tasks this week.

| Level | What it looks like here |
|---|---|
| **1. AI user** | I ask AI to post source documents or explain an entry. Faster than typing it in |
| **2. Validator** | I check the figure against the source. An error in a filing surfaces at the audit, not in the chat |
| **3. Orchestrator** | I built the stretch from source document to reconciliation to explanation, where the machine prepares and I accept |
| **4. Outcome owner** | I own the tax position and the signature on the filing, not the speed of data entry |
| **5. System builder** | I set up checks and rules so the work closes without me touching it daily |

**Where people usually get stuck.** Racing the machine on data entry speed is a race to zero. What gains value is the disputed case, the conversation with auditors, and the signature.

Next: [my level of usefulness](../playbooks/usefulness-levels-self-check.md) → [a plan for one level up](../playbooks/plus-one-level-plan.md).

## Ready-made skills and plugins for this role

You can turn repeatable procedures such as month-end close, bank and source-document reconciliation, and
difference review into a portable skill, or use an existing one. Browse [skill banks](https://cheap-intelligence.vercel.app/en/watch/skill-banks),
then see [turn a workflow into a skill](../playbooks/make-it-a-skill.md) to build your own.

## Where to go next

[Map your week](../playbooks/week-inventory.md) → [run the integrated profession audit](../playbooks/profession-audit-integrated.md)
→ [make a 90-day plan](../playbooks/personal-90-day-plan.md). Or open the [workbook](../playbooks/tom1-workbook.md).

---
**Sources for this review:** OpenAI GDPval (2025): <https://openai.com/index/gdpval/> · Anthropic Economic Index: <https://www.anthropic.com/economic-index> · Stanford AI Index (2025): <https://hai.stanford.edu/ai-index> · McKinsey, "The State of AI": <https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai>. Plus the book, Chapters 2 and 3.
