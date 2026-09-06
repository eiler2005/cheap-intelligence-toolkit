# skills — agent skills and browser tools

Two different things share this folder.

## `<slug>/SKILL.md` — a skill for an agent

An instruction file in the Agent Skills format: the agent picks it up on its own when a task falls
into its area. Put the skill folder wherever your agent looks for skills — Claude Code, Codex, Cursor
and others each have their own path; check your tool's documentation.

It also works without any agent. Inside each file the instruction sits in a code block: copy the
whole block into an ordinary chat and it works as a prompt. Same skill, done by hand.

How such a file is built, and how to write one for your own repeating procedure:
[`playbooks/make-it-a-skill.md`](../playbooks/make-it-a-skill.md). The rule is simple — if you are
explaining the same logic to an AI for the fourth or fifth time, that is already a skill.

## `<slug>/tool.html` — a browser tool

One self-contained file. Download it and open it in a browser; no internet needed. It computes on
your device, sends nothing anywhere and asks for no account.

Each tool also has a chat version on the site, for when no browser is at hand.

## Licences

`SKILL.md` and the other texts are CC BY-NC-SA 4.0. `tool.html` is MIT: take the code, change it,
embed it.

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

---

## Every instruction in full

Below are the instructions themselves, not descriptions of them. Each is self-contained: copy the
block you need into any AI chat. Copy the whole page and your assistant has all six. The same
content as one file: [`../../packs/en/skills.md`](../../packs/en/skills.md).

### The agent contract (Practicum for "When Intelligence Became Cheap")

Builds a contract for an AI agent across ten fields — role, mission, inputs, tools, memory, boundaries, escalation, review, metrics, owner — and turns the metric into a measurable threshold at which the agent stops itself. From chapter 3 of "Business in the Age of AI Agents".

```text
Help me write a contract for an AI agent, using the model from "Business in the Age of AI Agents"
(chapter 3). An agent on a team is not a magic employee: it is a role with explicit boundaries, a
review step and a human owner.

Collect from me if I have not given it:
1. What the agent is and which process it will work in.
2. What data and systems it will have access to.
3. Who on the team is accountable for it, by name.

What to do — fill in ten fields, asking me where the information is missing:
Role · Mission (one sentence) · Inputs · Tools · Memory (and what must NOT go into it) ·
Boundaries (what the agent never does without confirmation) · Escalation (the condition under which
it hands over to a human) · Review (how and when the result is checked) · Metrics (one or two
numbers) · Owner (a name).

Then tie metric, escalation and stop into a single guardrail:
— signal metric (share of answers needing no edits · anomaly in the numbers · escalation rate ·
  cost per day);
— threshold: a specific number, named BEFORE launch;
— action at the threshold: pause and human review · roll back to manual · switch off.

Discipline (hold to this):
- Without Boundaries, Escalation and Owner this is not a contract but a wish. If I do not supply
  them, do not fill them in with plausible text — say plainly that the contract is not ready.
- The owner is a named person. "The team" and "the department" are not accepted.
- Review is not delegated to AI: name where a human looks at the result.
- Access is least privilege: only what the mission needs.
- The threshold is named before launch, not after an incident.
- Do not scale straight after the contract: next come the eval set and shadow mode.
- Do not invent system names, integrations or numbers on my behalf.

Answer format:
1. Contract table: field | value.
2. The guardrail: metric | threshold | action.
3. Pre-flight: the six-point checklist, marking what is closed and what is not.
4. The weakest point here, in one honest sentence.
```

### The five deficits audit (Practicum for "When Intelligence Became Cheap")

Runs a person's real tasks through the five deficits that grow more valuable as AI makes routine work cheap: judgment, taste, trust, attention, distribution. Picks the one deficit where a move pays off most this quarter. From chapter 7 of "The Human Edge".

```text
Run my work through the five deficits that grow more valuable as AI makes routine work cheap
("The Human Edge", chapter 7): judgment, taste, trust, attention, distribution.

Collect from me if I have not given it:
1. Two or three real tasks from last week — what I actually did, not my job description.
2. How each one ended: who accepted the result and what happened next.

What to do:
1. For each of the five deficits, give one of four marks:
   — strong: there is an example with consequences, not a self-assessment;
   — neutral;
   — weak;
   — "not counted": I do have it, but the market, my manager or the client does not see or price it.
2. Trust is confirmed by other people's behaviour — they sign without reading, call me without a
   tender, rely on me without checking — not by how I feel about myself. Hold to that rule.
3. Do not give me three moves. Pick ONE deficit where a move pays off most over the coming quarter.
4. Propose a concrete step, and say how I will know in three months that I actually closed it.

Discipline:
- Mark by evidence, not by how I describe myself. No example means "not counted" — say so.
- Call it out separately when a strength exists but nobody sees it: that calls for a different move
  than building the skill further.
- No "develop your taste" without specifics. The step has to be something I can start this week.
- Do not invent studies, numbers or courses. If unsure, say "check this".

Answer format:
1. Table: deficit | mark | what the mark rests on.
2. The one deficit chosen, and why that one.
3. The concrete step for the quarter.
4. The three-month check: what has to change for this to count as closed.
```

### Optimize work by profession

Helps professionals break their work into tasks and decide what to give AI, what to keep, and which tools may help, using the method from *When Intelligence Became Cheap*: output gets cheaper, while value moves to outcome.

```text
You are a practical assistant who avoids hype. Do not promise "easy money" or "100 prompts." Help the
person see their work clearly and make one real move. Keep your voice calm and direct.

Ask for anything the user did not provide:
1. Profession or role.
2. 5-10 real tasks from the past week. Ask for specifics, such as "reviewed a contract," not "worked
   on a project."
3. Optional: their country or region, tools they already use, and any access, budget, or employer
   limits that affect which services they can use.

What to do:
1. Sort the tasks into three groups. Use the logic of GDPval for capability and the Anthropic
   Economic Index for what people actually delegate:
   - GREEN, "AI alone": routine work with a clear input and a result that a person can check quickly.
   - YELLOW, "person + AI": the machine provides volume or a draft; the person holds context and review.
   - RED, "person only": judgment, accountability, trust, and difficult communication.
2. Explain what becomes cheaper and what becomes more valuable in this role (output to outcome).
3. Suggest a minimum stack of no more than 3 tools. Name the category, give 1-2 examples that may be
   available in the user's region, and mark important access or price limits. Options may include
   ChatGPT, Claude, Gemini, Perplexity, DeepSeek, or Qwen. Do not assume that any service is available.
   Say "check current availability."
4. Name red flags: where AI is dangerous in this profession, including hallucinations, personal data,
   and accountability. State what must not be delegated.
5. Give one move for this week. Choose one YELLOW or RED task, take it to an outcome, and say what the
   person must check.
6. Show one weak and better prompt pair for the user's task. Ask for options and weak spots instead of
   a finished answer, which helps limit cognitive debt.

Required discipline:
- "Do not trust it. Check it." Mark what the person must verify.
- Do not invent tools, prices, or links. If unsure, say "check current information" or [verify].
- Do not present one answer as permanent. Task groups move and tools age, so include the date.
- Do not label the person. A mode or level describes a task, not a personality.
- End with one specific move, not a five-page program.

Response format:
1. A table: task / group / what becomes cheaper or more valuable.
2. Minimum stack (no more than 3, with access labels).
3. Red flags (2-4 points).
4. One move for the week and what to check.
5. One weak to better prompt pair.
6. Where to go next: suggest combining the diagnosis in the integrated audit and building a 90-day plan.
```

### The trust compass (Practicum for "When Intelligence Became Cheap")

Helps choose the depth of checking in advance from the cost of being wrong rather than from how convincing a message looks: no questions · one question · all three plus independent confirmation on a second channel. Produces a trust protocol for home and work. From chapter 13 of "The Economics of Trust".

```text
Help me build a trust protocol using the trust compass from "The Economics of Trust" (chapter 13).

The core rule: the depth of checking is set by the cost of being wrong, not by how convincing the
message is. The other side controls how convincing it looks. I control the cost of being wrong.

Three depths:
— No questions: the mistake is small and reversible (a clip, an image, someone's opinion). Do not
  check; save the attention for what is expensive.
— One question: I am about to cite it, forward it or form a view on it. Ask "where did this come
  from?" and find the source.
— All three questions plus independent confirmation: money, access, documents, health, work,
  reputation. Check the origin, the speaker and the accountability — and step onto a second channel
  the sender does not control.

Collect from me if I have not given it:
1. My three expensive scenarios: one at home, one at work, one of any kind.
2. Who usually gets in touch in them, and through which channels.

What to do:
1. Assign a depth to each scenario and justify it by the cost of being wrong, not by how convincing
   the approach looks.
2. For the deepest scenarios, name a specific second channel the sender does not control. Not
   "call the number in the message" but "call the number I already had".
3. Help me separate three states honestly: confirmed · probable · unknown. "Probable" is not "yes";
   spell out what I did not check.
4. Propose one household agreement and one work agreement — short enough to say out loud and
   remember in a hurry.
5. Finish with ONE move for the coming week.

Discipline:
- Do not rule that something "is fake" or "is genuine": you have no grounds for that.
- Do not tell me to check everything. Attention is finite, which is the whole point of the compass.
- Do not offer AI-detection services as proof.
- Say separately what I will present when it is me being checked.

Answer format:
1. Table: scenario | cost of being wrong | depth | what I actually do.
2. The second channel for the expensive scenarios.
3. The honesty line: confirmed / probable / unknown.
4. Two agreements: home and work.
5. One move for the week.
```

### The three value levers (Practicum for "When Intelligence Became Cheap")

Runs a single task through the three value levers — growth and new revenue, cost saving, attention and trust — and says what in it is output (getting cheaper, automate) and what is outcome (getting more valuable, keep). From chapter 2 of "The Human Edge".

```text
Help me take ONE task through the three value levers from "The Human Edge" (chapter 2).

Collect from me if I have not given it:
1. One specific task. Not "marketing" but "I write the weekly customer newsletter".
2. How long it takes and how often it repeats.

What to do:
1. Name the lever — exactly one, the main one:
   ① growth and new revenue — the thing others cannot do;
   ② cost saving — the same thing cheaper or faster;
   ③ attention and trust — the reason people pick me specifically.
   If none of them fits, say so plainly: this is busywork.
2. Answer two questions honestly:
   (1) can cheap AI already do this — almost entirely / partly / no;
   (2) does it set me apart — uniquely / somewhat / no more than anyone else.
3. Reach a verdict: this is output (getting cheaper — automate it and free the time) or outcome
   (strengthen it — ownership, judgment, trust, attention).
4. Give ONE move: what exactly to hand to AI, and which outcome to keep.

Discipline:
- No hype and no promises of money. Not "you will earn more" but "the price rises here, falls there".
- If the task looks unique but everyone in the field does it, say so directly.
- "Automate" does not mean "stop being accountable": name what I still check.
- Do not invent tools, prices or links. If unsure, say "check this".

Answer format:
1. The lever and why that one.
2. Two answers: can AI do it · does it set me apart.
3. Verdict: output or outcome, in one line.
4. One move: what to hand over, what to keep, what I will check.
```

### Week inventory (Practicum for "When Intelligence Became Cheap")

Sorts a person's real working week into three baskets — 🟢 "AI on its own", 🟡 "human + AI", 🔴 "human only" — measures the share of time in 🟢+🟡 (their exposure to cheap intelligence) and finds busywork tasks that pull no value lever. From chapter 3 of "The Human Edge".

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
