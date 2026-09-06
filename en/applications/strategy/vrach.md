<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/strategy/vrach
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

# AI strategy: Physician

> Prioritized AI adoption map. **Date: 2026-06.**
> WARNING: Use AI for text and administration, **not diagnosis or treatment**. A physician makes
> decisions under the applicable clinical rules. ← [Role hub](../vrach.md)

!!! abstract "Context"
    AI works well as an assistant for documentation and text. Only a physician makes a clinical
    decision and carries responsibility for it.

## 1. Documentation (high priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 1 | Ambient visit documentation, which captures and structures the conversation | paperwork time · note quality | Nuance DAX or Abridge for ambient documentation · **physician review and signature** |
| 2 | Discharge summaries and letters | time · errors | draft from the data · verify facts and dosages |

## 2. Communication (medium priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 3 | Explain information to the patient | understanding · satisfaction | plain-language text prepared for the visit |

## 3. Knowledge (medium priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 4 | Literature search | speed · quality | initial collection · verify sources |

## 4. Safety and the role (foundation)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 5 | Personal and medical data | incidents · compliance | certified environment only |
| 6 | Time with the patient | contact · visit quality | less paperwork, more time with the patient; clinical judgment stays with the physician |

## Where to start: the first round

The tables are a map of what is possible, not your plan. In medicine, the first round covers only
administration and documentation, **never diagnosis or prescribing**. This is a red line, not a
task postponed until later. See "Keep these parts human" below. Apply
[process scoring](../../playbooks/process-scoring.md): repetition, volume, verifiability, error
cost, and data. The first round usually looks like this:

1. **No. 1, ambient visit documentation.** It repeats at every visit and has enough volume. The
   physician reviews and signs the note before it enters the medical record, so an error can be found.
2. **No. 2, discharge summaries and letters.** Start with a draft based on data already entered.
   Checking facts and dosages before signature is mandatory, with no exceptions.
3. **No. 4, literature search.** The error cost is low at the initial collection stage. Verify
   every source before using it.

**Not in the first round:** No. 3, "patient explanation," is already direct contact with a patient.
Build the documentation review habit on Nos. 1 and 2 before adding it. Diagnosis and prescribing
are intentionally absent from the initiative tables. This is not a matter of sequence. AI does not
diagnose or prescribe at any maturity level. See the red flags in the [role hub](../vrach.md).
Keep patient personal and medical data from No. 5 inside a certified and approved environment.
That is also an admissibility rule, not an implementation sequence.

## Keep these parts of medical practice human

- **Diagnosis and prescribing treatment.** Only a physician does this, without exceptions and without calling it "just a draft."
- **Responsibility for the clinical decision.** It is not shared with a tool.
- **Delivering bad news and having difficult patient conversations.** Only a physician handles them.
- **Signing any documentation.** The signature records that the physician checked the document and accepts responsibility.
- **Patient personal and medical data.** Use only a certified and approved environment, never open services.

## Review points and stop thresholds

Give every first-round initiative its own review point in the
[Human Review Matrix](../../playbooks/human-review-matrix.md) and set a threshold in advance in the
[agent contract](../../playbooks/agent-contract.md):

| Initiative | What a person checks | Stop threshold (example, replace with your own) |
|---|---|---|
| No. 1 ambient documentation | physician reviews and signs the note before it enters the medical record | a substantive error means not signing, returning to manual notes, and investigating the cause |
| No. 2 discharge summaries and letters | compare facts and dosages with the primary data | a dosage or factual error means quarantining the tool and manually checking recent summaries |
| No. 4 literature search | verify every source before using it in a decision | if a source cannot be found or does not exist, do not use the collection and repeat the search manually |

Before you expand, build a [reference set of 20 cases](../../playbooks/eval-set-builder.md). For
medical documentation, use 20 notes or discharge summaries that were already reviewed and signed
and have known correct text. Diagnosis and prescribing do not belong in this set and must never be added.

## Two paths from here

- **You are a physician:** open the [role hub](../vrach.md), map your week, and build a personal
  plan in the [Volume 1 workbook](../../playbooks/tom1-workbook.md).
- **You lead a clinical function or healthcare facility:** use the
  [Human Review Matrix](../../playbooks/human-review-matrix.md), write the
  [agent contract](../../playbooks/agent-contract.md) with hard boundaries for diagnosis,
  prescribing, and patient confidentiality, then complete the full path in the
  [Volume 2 workbook](../../playbooks/tom2-workbook.md).

!!! danger "Discipline"
    Only a physician diagnoses and prescribes. Keep personal and medical data inside an approved
    environment. Verify facts and dosages.

→ [Role hub](../vrach.md) · [audit](../../playbooks/profession-audit-integrated.md) · [plan](../../playbooks/personal-90-day-plan.md).

---
**Sources:** profession automation review (GDPval, AEI, O*NET); book, Chapters 2, 3, and 10.
