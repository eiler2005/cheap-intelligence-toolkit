<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/skills/week-inventory/SKILL
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

---
name: week-inventory
description: >-
  Sorts a person's real working week into three baskets — 🟢 "AI on its own", 🟡 "human + AI",
  🔴 "human only" — measures the share of time in 🟢+🟡 (their exposure to cheap intelligence) and
  finds busywork tasks that pull no value lever. From chapter 3 of "The Human Edge".
  Use when the user lists their tasks for a week, asks which parts of their job AI can already do,
  or how exposed their role is. Triggers "sort my week", "what will AI take from my job",
  "my exposure", "week inventory".
license: MIT
---

# Week inventory (Practicum for "When Intelligence Became Cheap")

📋 A ready-made skill for an AI assistant. Drop this file into your agent's skills folder — or copy
the block below into any chat and list last week's tasks.

The worksheet this comes from, for filling in by hand:
[Week inventory](../../playbooks/week-inventory.md).

```text
Help me sort my working week into the three baskets from "The Human Edge" (chapter 3).

The baskets:
🟢 "AI on its own" — routine work with a clear input and a checkable output;
🟡 "human + AI" — the machine gives me a draft or volume, I hold the context and the check;
🔴 "human only" — judgment, accountability, trust, difficult conversations.

Collect from me if I have not given it:
1. Ten to fifteen real tasks from last week, taken from my calendar and messages — what actually
   happened, not what should have. Specific ones: "reviewed a contract", not "worked on a project".
2. Roughly how long each took.

What to do:
1. For each task, name the basket and the value lever it pulls: ① revenue and growth ·
   ② cost saving · ③ attention and trust · "—" if it is busywork pulling no lever.
2. Work out the share of my time in 🟢+🟡. That is my exposure to cheap intelligence.
3. Count how many tasks landed on lever "—".
4. Give me a summary I can copy and keep.
5. Ask me three honest questions. The first is fixed: where am I hiding in busywork instead of
   strengthening the 🔴 task where I am genuinely hard to replace?

Discipline:
- Do not decide for me. This is a map, not a verdict: a basket describes a task, not me.
- Do not flatter. If a task looks 🔴 only because I would prefer it that way, say so.
- The goal is not to get faster at 🟢 but to move weight into 🔴, where the price is rising.
- Baskets drift. Say that this is worth redoing in about six months.
- Do not invent tools, numbers or links. If unsure, say "check this".

Answer format:
1. Table: task | time | basket | lever.
2. Exposure: share of time in 🟢+🟡, one line.
3. Busywork tasks (lever "—") as a list.
4. Three honest questions.
5. One move for the week: which 🟡/🔴 task to strengthen and what I will check myself.
```
