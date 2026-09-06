<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/prompts/templates
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

# Prompt templates by task type

> Practicum section. **Verified: 2026-06.** Copy a template, replace the text in `[square brackets]`,
> and check the output. This is not magic. It is the [method plus review](index.md). Every template ends
> with **"What to check."** Without that line, a prompt produces a demo rather than a result.

Every template uses the same frame: **role / goal / context / format / boundary / review**. Remove names,
real numbers, and sensitive data while keeping the substance. Do not send information to an outside
service if it should not leave your system.

---

## 1. Review a document

```text
You are a [role: lawyer on my side / analyst / editor]. I am the [context: buyer / author].
Here is the document: [paste the text].
Task: identify the [risks / unclear points / main terms] for me.
Format: a table with clause / meaning / why it matters to me / quote / suggested change.
Boundary: do not smooth over uncertainty. If the text does not contain something, say so. Do not guess.
```

**What to check:** compare every quote with the original. You own the decision and responsibility.

## 2. Compare options and choose

```text
Suggest [N] options for [what] that meet these limits: [budget, dimensions, compatibility, deadline,
how you access it].
For each option, explain which task it fits and name one honest risk or disadvantage.
Do not give me a long list. Give me only [N] options and explain why you chose them.
```

**What to check:** verify current prices, availability, and specifications with primary sources. Models
can invent them.

## 3. Create a draft (email, post, or reply)

```text
Audience: [who]. Their problem or interest: [what]. My goal: [what should happen].
Give me [N] versions of a [email / post] in a [calm, businesslike, low-hype] tone.
Do not invent facts or numbers about me or the product. Leave a blank [...] where information is missing.
```

**What to check:** you own the facts and numbers. Edit the tone and remove stiff business language until
the draft sounds like you.

## 4. Find weak spots (criticism, not support)

```text
Find reasons why [decision / plan / candidate / company] is a bad idea.
Be strict. Look for [risks, gaps, reasons to reject it] rather than arguments in favor.
Mark what I can verify in advance and explain how.
```

**What to check:** weigh the arguments for and against it yourself. The model only expands the list
against.

## 5. Explain or teach at several levels

```text
Explain [topic] at three levels: to a child, to a beginner in the field, and to a colleague.
Guide me with questions instead of giving everything at once. Ask one review question after each part.
Point out any common misconception.
```

**What to check:** for high-stakes subjects such as medicine, law, and finance, compare the answer with
a primary source or ask a qualified professional.

## 6. Extract structure from text

```text
Extract [items: amounts, dates, names, tasks] from this text into a table with these columns: [columns].
The formats vary, so normalize them. Mark uncertain rows separately.
Do not add anything. Leave a field blank when the text does not contain the answer.
```

**What to check:** inspect a sample of 10 to 15 rows. Expect at least one error.

## 7. Break a task into steps or a plan

```text
Goal: [what I want] by [deadline]. Limits: [time, resources, prohibited actions].
Break the work into steps. Mark what I should do first, what AI can handle, and what I should keep.
Add a checkpoint to every step. Give me one next move for this week, not the full list at once.
```

**What to check:** you must judge whether the deadlines and dependencies are realistic. The plan is a
hypothesis, not a fact.

## 8. Prepare for a conversation or meeting (dry run)

```text
Meeting context: [who, subject, my goal]. Participant roles: [CFO / client / manager].
Play the other side. Ask me hard questions and raise objections one at a time.
At the end, name my 3 weakest arguments and tell me what to prepare.
```

**What to check:** this is rehearsal, not a script. The live conversation will take a different path.

---

## What to do with the result

- If you repeat one technique every day, [turn it into a skill](../playbooks/make-it-a-skill.md).
- To analyze your profession step by step, use the
  [prompts for exploring your profession](explore-my-profession.md).
- To see the method on real tasks, open the [case bank](cases.md).

> Update after a material change in model behavior. Check facts, numbers, and quotes.
> AI can be confidently wrong.
