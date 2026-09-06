<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/playbooks/resilient-automation
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

# Resilient automation checklist

Worksheet for Volume 2, Chapter 4, "The One-Person Company."

Use this checklist to test one agent-run function before it touches customers, money, documents, or reputation.
This is not a guide to automating everything. It tells you what must be visible, testable, and easy to stop.

## 1. Function

Choose one function, not the whole company.

| Question | Your answer |
|---|---|
| What repeatable result should this function produce? |  |
| What goes in: emails, applications, documents, deals, or data? |  |
| What comes out: an answer, record, invoice, report, or recommendation? |  |
| Where does the cost of an error become high? |  |
| What must the agent never do without a person? |  |

If you cannot describe the output in one sentence, it is too early to automate the function.

## 2. Tests

Collect at least ten test cases.

| Type of case | What to include |
|---|---|
| Normal case | Work the function handles every day |
| Difficult customer | Large order, unusual promise, or sensitive tone |
| Legal risk | Contract, invoice, personal data, or disputed wording |
| Bad input | Missing data, contradiction, or an attachment in the wrong format |
| Red zone | A case where the agent must stop |

A test works only when you decide in advance which answers are acceptable.

## 3. Logs

The agent must leave a record of its actions.

- What the agent received.
- Which sources or tools it used.
- What it decided on its own.
- Where it was uncertain.
- Which rules fired.
- Why it stopped or continued.

If you cannot reconstruct the path after an error, you do not have a function. You have a black box.

## 4. Warning signals

Write down what should raise a flag.

| Signal | Action |
|---|---|
| A new promise is made to a customer | Stop and show it to a person |
| A price, discount, or deadline changes | Stop and show it to a person |
| A document is about to leave the company | Require human review |
| The agent is uncertain or finds a contradiction | Escalate instead of guessing |
| The same error happens again | Stop the flow and repair the system |

A warning signal without an owner is useless. Name the person who will see each signal.

## 5. Permissions

Give the agent the least access it needs.

| Access question | Decision |
|---|---|
| Is access read-only, or may the agent write? |  |
| May the agent send a message to a customer without approval? |  |
| May it change the price, deadline, or deal status? |  |
| Is there a money or risk limit? |  |
| When does access turn off automatically? |  |

The chapter's rule is simple: give the agent exactly the access the task requires, and nothing more.

## 6. Repair

Decide what happens after a failure before one occurs.

1. Who sees the incident?
2. Who stops the flow?
3. Who repairs the rule, prompt, integration, or data?
4. Who tells the customer if the error reached them?
5. How does the new case enter the test set?

Without repair, automation builds up debt. With repair, it becomes a system.

## Final decision

| Check | Yes / no |
|---|---|
| The function is described separately from the company |  |
| Test cases exist |  |
| Actions are logged |  |
| Warning signals exist |  |
| Permissions are minimal |  |
| The person who repairs a failure is known |  |
| A person remains at the critical points |  |

If three or more answers are "no," the function is not ready for live work. Start with one pain point, one agent, and one stop rule.
