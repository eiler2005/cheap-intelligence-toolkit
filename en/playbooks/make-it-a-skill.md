<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/playbooks/make-it-a-skill
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

# Turn a repeated task into a skill

> Practicum for Chapter 6, "The Human as a System." Time: 20 to 30 minutes.
> Continue here after the [Personal Harness Builder](personal-harness-builder.md). Once you can see your harness, package one repeatable part as a portable skill.

## Why this helps

Use a simple rule: **If you explain the same logic to AI for the fourth or fifth time, it is already a skill.** The problem is not that the model is slow to learn. You have not yet built a system for that procedure. Repeating one explanation can cost 8 to 12 minutes a day. Across a month and several tasks, that becomes hours.

A skill is an instruction file called `SKILL.md`. An agent loads it when a task falls within its scope. Write the logic once, then stop explaining it from scratch. You can find skills made by other people in [skill banks](https://cheap-intelligence.vercel.app/en/watch/skill-banks). This worksheet helps you make your own.

## Step 1. Find a candidate

Choose a repeated procedure that you keep explaining from the beginning.

| Sign | Your example |
| --- | --- |
| I have explained this to AI at least four times | |
| I explain it a little differently each time, so the result varies | |
| I know what "done correctly" means | |

If all three rows fit, you have a skill candidate. Start with the one you repeat most often.

## Step 2. Describe the procedure in plain language

Answer four questions. Your answers will form the body of the skill.

1. **When to use it.** Which tasks should trigger this skill?
2. **What goes in.** Which materials or data do you provide?
3. **How to do it.** Write the steps you usually explain each time.
4. **What comes out and how to check it.** Define the output format and your verification point.

## Step 3. Build the `SKILL.md` file

Copy and complete this minimal template:

```markdown
name: contract-review
desc: Reviews an incoming contract and lists risks for my side, with a quote from each relevant clause.

## When to use

Use this skill when I provide a contract and ask you to assess its risks.

## Input

The contract text, link, or file.

## Steps

1. Identify risks for MY side. I am the customer.
2. Sort the risks by severity.
3. Quote the relevant clause for each risk.
4. Suggest revised wording.

## Output

Table: risk | severity | clause quote | suggested revision.

I check every quote against the contract and take responsibility for the decision.
```

## Step 4. Put it where the agent can find it

- Add the file to the skills folder used by your AI tool or agent. Claude Code, Codex, Cursor, and other tools use different paths.
- Give the file a clear name. One job belongs in one skill.

## Step 5. Test and update it

- Run the skill on one or two real tasks. If the result varies, make the steps more precise.
- Review it once a month. Remove what is outdated and add what is missing.
- **Access and security:** A skill that can reach email, files, or money should require confirmation and run in a [sandbox](personal-harness-builder.md). Treat someone else's skill as you would treat someone else's code. See [trusting a skill](https://cheap-intelligence.vercel.app/en/watch/skill-banks).

## What you get

Your list of skills becomes a portable part of your harness. When you start an agent, it can load the right skill for the task. The irritation of explaining the same thing again is useful evidence. It points to the next skill you should write.

> Related: [Personal Harness Builder](personal-harness-builder.md) | [Skill banks](https://cheap-intelligence.vercel.app/en/watch/skill-banks) | [Prompts: method and verification](../prompts/index.md) | [Profession library](../applications/_index.md).
