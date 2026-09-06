<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/playbooks/human-review-matrix
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

# What AI should do and what people should keep (Human Review Matrix)

> Practicum for **Volume 2, Chapter 2**, "More Output Does Not Mean More Value."
> Time: 15-20 minutes. One process on one screen, not a 10-page AI policy.

An outcome does not come from producing more output. It comes from a process with the right review and the right metric.
This worksheet turns the chapter's main advice into an exercise: take one process and decide what the machine may do,
what needs review, and what a person should keep.

**How to fill it in.** List 5-7 tasks from **one** process as rows. Work through the columns for each task.
Record the decision in the "Mode" column.

A minimum governance packet is the small set of documents that defines control and ownership. This matrix is the second worksheet. First choose a process with
[process scoring](process-scoring.md). Use this matrix to assign a mode to each task. Then define the agent with an
[Agent Contract](agent-contract.md) and test it on an [evaluation set](eval-set-builder.md).

| Task | Cost of error | Reversible? | Can it be described as a process? | Can you check it? | Mode | Control layer | Flow metric |
|---|---|---|---|---|---|---|---|
| `________` | low / medium / high | yes / no | yes / no | yes / no | AI alone / review required / person only |  |  |
| `________` | | | | | | | |
| `________` | | | | | | | |
| `________` | | | | | | | |
| `________` | | | | | | | |

**What the columns mean:**

- **Cost of error:** what happens if AI gets it wrong and nobody notices.
- **Reversible:** whether you can undo the action if the wrong result goes out.
- **Can it be described as a process?** This is the chapter's filter. If the answer is no, the task is not ready for a machine.
- **Can you check it?** Whether you have a quick way to tell if the result is right, such as a reference answer, rule, or eval.
- **Mode:** the final decision for the task.
- **Control layer** for "review required": visibility, guardrails, access limits, or a person at the critical point.
- **Flow metric:** one end-to-end measure instead of output volume, such as time to result or the share completed without rework.

## Default logic

- High cost of error plus poor reversibility means **person only**, or a person at the critical point.
- If you cannot describe the task as a process, **do not hand it over yet**. Understand it first.
- If you cannot check the result, **build the check first**. Otherwise, you have a demo rather than a result.

## Output

A completed matrix for one process and **one** end-to-end metric that you track instead of volume.
Return in three months and see what has moved from "person only" to "review required."

---

## Next

- For tasks marked "AI alone" or "review required," define the agent with an
  [Agent Contract](agent-contract.md) (Chapter 3).
- Do not send the first version straight to production. Build an [evaluation set](eval-set-builder.md) and run it in shadow mode, where it drafts or observes without taking live action.
- Reviewing output is a scarce skill. Train it with [Skills Watch](https://cheap-intelligence.vercel.app/en/watch/skills-that-pay) (Volume 1, Chapter 7).
- Follow the full route in the [Volume 2 Workbook](tom2-workbook.md).

> The chapter covers flow metrics. This worksheet decides who does what. ⚠️ Check the output outside the model.
