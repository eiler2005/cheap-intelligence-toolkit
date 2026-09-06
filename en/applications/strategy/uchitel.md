<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/strategy/uchitel
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

# AI strategy: Teacher / instructor

> Prioritized AI adoption map. **Date: 2026-07.** Sources: GDPval, AEI, O*NET, and the education
> review. The [role hub](../uchitel.md) lists tools for schools, including
> Uchi.ru. ← [Role hub](../uchitel.md)

!!! abstract "Context"
    AI works well as an assistant that reduces preparation and grading work. Motivation and live
    contact with a student remain human responsibilities.

## 1. Preparation (high priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 1 | Lesson plans and assignments | preparation time · quality | an assistant for drafts · MagicSchool or Diffit for level-based materials |
| 2 | Materials for different ability levels | level coverage | versions of the same text for the class, which is instructional differentiation |

## 2. Assessment (high priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 3 | Draft feedback based on criteria | grading time | AI draft · **a person grades and remains accountable** |

## 3. Explanation (medium priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 4 | Explain one topic in different ways | student understanding | several explanations · practice tool such as Khanmigo |

## 4. Contact and facts (foundation)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 5 | More time for motivation and work with each student | engagement | less preparation, more live contact |
| 6 | Verify facts and protect children's data | incidents | check primary sources · handle personal data with care |

## Where to start: the first round

The tables are a map of what is possible, not your plan. Start with
[process scoring](../../playbooks/process-scoring.md). Ask whether the task repeats, has enough
volume, produces a checkable result, carries an affordable error cost, and has usable data. For
most teachers, the first round looks like this:

1. **No. 1, lesson plans and assignments.** The task repeats every week and has enough volume.
   Before class, compare the result with your own curriculum or national
   Standards, known as FGOS.
2. **No. 2, materials for different ability levels.** Start with one topic, create versions for
   different class levels, and have the teacher check each version before distribution.
3. **No. 4, different explanations of one topic.** The error cost is low because this is a draft
   explanation for the teacher's preparation, not unchecked direct contact with a student.

**Not in the first round:** No. 3, "draft feedback on student work," already affects a student's
assessment. Build the review habit on Nos. 1, 2, and 4 before adding feedback drafts. The teacher
always owns the grade and accountability. If a tutor such as Khanmigo from the
[role hub](../uchitel.md) works with a student directly, use the separate "hint, not answer"
discipline in [AI tutor training mode](../../playbooks/ai-tutor-training-mode.md). This is different
from a teacher preparing materials for personal use.

## Keep these parts of teaching human

- **A student's grade.** AI does not grade alone. The teacher makes and signs the final decision.
- **Student evaluations and references.** AI does not write them without human involvement.
- **Motivation and live contact.** Work with the actual student, not an "average" class member.
- **Data about minors.** It needs special handling and must not go into open services.
- **Facts in teaching materials.** Review them before the class receives the material.

## Review points and stop thresholds

Give every first-round initiative its own review point in the
[Human Review Matrix](../../playbooks/human-review-matrix.md) and set a threshold in advance in the
[agent contract](../../playbooks/agent-contract.md):

| Initiative | What a person checks | Stop threshold (example, replace with your own) |
|---|---|---|
| No. 1 lesson plans | verify facts and alignment with the curriculum or FGOS before class | one factual error means the plan cannot be used without a complete review |
| No. 2 level-based materials | check that the simpler version does not distort the topic | if the lower-level version loses the meaning of the topic, revise it manually before distribution |
| No. 4 topic explanations | compare at least one explanation with the textbook or curriculum | if the explanation conflicts with the curriculum, do not use it and revise the request |

Before you expand, build a [reference set of 20 cases](../../playbooks/eval-set-builder.md). For a
teacher, use 20 materials or lesson plans in the subject that were already reviewed by hand and
have a known correct level. Test a new tool on them before trusting the flow.

## Two paths from here

- **You are a teacher:** open the [role hub](../uchitel.md), map your week, and build a personal
  plan in the [Volume 1 workbook](../../playbooks/tom1-workbook.md).
- **You lead a curriculum or school function:** use [process scoring](../../playbooks/process-scoring.md),
  write the [first agent contract](../../playbooks/agent-contract.md), and complete the full path in
  the [Volume 2 workbook](../../playbooks/tom2-workbook.md).

!!! danger "Discipline"
    Verify facts in every teaching material. A person grades the student. Handle data about minors
    with care.

→ [Role hub](../uchitel.md) · [audit](../../playbooks/profession-audit-integrated.md) · [plan](../../playbooks/personal-90-day-plan.md).

---
**Sources:** profession automation review (GDPval, AEI, O*NET); book, Chapters 2, 3, and 7.
