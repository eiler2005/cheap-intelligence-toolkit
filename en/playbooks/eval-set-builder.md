<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/playbooks/eval-set-builder
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

# Evaluation set: test an agent before it lets you down

> Practicum for **Volume 2, Chapter 2** (from output to outcome). This continues the
> [Human Review Matrix](human-review-matrix.md). Time: one evening for your
> first set of 20 cases.

The [Human Review Matrix](human-review-matrix.md) answers "what can I give to an agent?" This worksheet
answers the next question: **how can you tell whether the agent can handle the work before it causes
damage?** The reliable answer is not exciting. Build an evaluation set: a list of real cases where you
already know the correct result. Run the agent against that set after every change.

In a minimum governance packet, this is the final check before launch. [Process scoring](process-scoring.md)
selects the process, the [matrix](human-review-matrix.md) assigns a review mode, the
[contract](agent-contract.md) sets permissions and a stop threshold, and the evaluation set shows that
the agent can maintain quality before it touches live work.

Without an evaluation set, you judge the agent by feel: "its answers seem fine." With a set, you have
a number: "34 of 40 were correct, and all six errors involved refunds." People can argue about an
impression in a meeting. The number gives them something concrete to examine.

---

## Step 1. Collect 20 real cases

Do not invent examples. Take the latest 20 real requests, documents, or applications from the process
you plan to give the agent.

Selection rules:

- **15 common cases plus 5 edge cases.** Common cases test usefulness. Edge cases test safety: an
  unusual tone, two questions in one request, missing data, or a case that the agent should send to a
  person.
- **Use completed cases with a known outcome.** You know the right answer because a person already
  gave it, and the client did not return with a complaint.
- **Remove personal data.** Replace names, phone numbers, and contract numbers with placeholders.

## Step 2. Define "correct" for every case

| # | Input (case) | Correct result | How you check it |
|---|---|---|---|
| 1 | `request text / document` | `the answer a person gave` | meaning match / checklist / number |
| ... | | | |
| 16-20 | edge cases | **correct result = escalation to a person** | the agent did NOT answer on its own |

Use one of three checks, from lightest to strictest:

1. **Meaning match.** The agent's answer says the same thing as the reference answer. A person reviews
   it quickly.
2. **Checklist.** Check three to five required points, such as naming a deadline, making no promise of
   compensation, and including a link.
3. **Number.** When the result can be counted, compare the amount, date, or quantity.

## Step 3. Run the set and count honestly

Run all 20 cases through the agent. Record three numbers:

- **Accuracy on common cases:** how many of the 15 were correct.
- **Safety on edge cases:** how many of the five the agent sent to a person. **The requirement here is
  5 out of 5.** An agent that answers with confidence when it should ask for help is more dangerous
  than one that makes a mistake on a common case.
- **Worst error in the run:** describe it in one sentence. It often tells you more about risk than the
  average score.

## Step 4. Use shadow mode before the agent speaks

There is a handoff between "passed the set" and "works with clients": **shadow mode.** The agent works
on live cases, but only a person sees its answers. That person compares them with their own answers and
records the differences. Two weeks in shadow mode exposes the agent to real variety without putting a
client at risk.

Whenever the agent makes a mistake in shadow mode, add that case to the evaluation set. The set should
grow from real work.

## Step 5. Decide whether the agent is ready, and stays ready

The agent is ready to work on its assigned area only when every item is true:

- [ ] common cases: the score stays at or above your threshold (an honest 90% or more is a reasonable
  starting point, not "almost always");
- [ ] edge cases: 5 out of 5 escalations in two runs in a row;
- [ ] shadow mode: two weeks without an error that you would not be willing to explain to a client;
- [ ] the agent has a [contract](agent-contract.md) with an owner and a stop threshold;
- [ ] you have agreed **when to run the set again**: after any change to the model, prompt, or knowledge
  base, and once per quarter even when "nothing changed" (the outside world still changes).

> Rule from Chapter 2: **AI does not judge AI.** A person owns the reference answer and the final
> decision. The agent may prepare a first comparison, but the owner signs off on "ready."

---

Next: if you have not completed the contract, open [Agent Contract](agent-contract.md). If you selected
the process by instinct, return to [process scoring](process-scoring.md). After the set passes, use
shadow mode instead of moving straight to production. See a live 40-request set in
[Sergey, support team lead](../cases/persona-rukovoditel-podderzhki.md).
Back: [Volume 2 Workbook](tom2-workbook.md).
