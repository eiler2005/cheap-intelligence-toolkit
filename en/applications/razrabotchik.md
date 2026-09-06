<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/razrabotchik
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

---
reading_level: b2-c1-technical
title: "Developer: what to automate and which tools to use"
description: A practical map of software tasks AI can speed up, the engineering checks a person must keep, and tools to consider.
---

# Developer: what to automate and which tools to use

> Field: **IT and product**. Role hub. **Checked: 2026-08-18.** Tools change over time. Keep private code
> and secrets local or inside your own environment. Sources for this review are at the bottom of the page.

## At a glance

AI performs well on code generation, tests, review, and changes across multiple files. More of this work now
follows an "agent drafts it" workflow. Writing code is not the same as owning a working product. Value moves
to architecture, verification, security, and responsibility for production.

!!! info "What the data says (GDPval, Anthropic Economic Index, O*NET)"
    - **Capability (GDPval):** AI generates code, tests, and documentation. Agents can change several files
      in one task.
    - **Use (AEI):** Computer and Mathematical occupations are among the most exposed task groups, at
      about a third of all Claude.ai conversations and nearly half of API traffic.
    - **An important 2026 correction:** adjust task coverage for how often the attempt actually
      succeeds, and developers turn out to be affected **relatively less** than raw coverage suggests.
      Data entry keyers and radiologists sit far higher. High task exposure is not the same as high
      replacement of the profession.
    - **How much of this is already in real code:** by Feb 2026, Claude Code alone was authoring about
      **4% of all public GitHub commits**, roughly 135,000 a day.
    - **What demand is doing:** postings requiring experience with AI coding tools grew about **340%**
      between Jan 2025 and Jan 2026, while postings for pure implementation roles fell about **17%**.
    - **Mode:** high task substitution. Junior-level tasks leave first. Architecture, security, and ownership
      of production remain. See the [full data review](_super-analysis.md) and the
      [role AI strategy](strategy/razrabotchik.md).

## What to automate first

1. **Boilerplate, tests, and documentation.** Delegate routine work with clear patterns, then review it.
2. **Code explanation and navigation.** Ask the model to explain a module and flag risky areas.
3. **Pull request summaries and first-pass review.** Let AI draft review comments. A person performs the final review.
4. **Agent tasks.** Let an agent move from plan to code, tests, and fixes across multiple files with tools
   such as Cursor Composer or a Copilot agent.
5. **Migrations and security scans.** Translate between language versions and scan for vulnerabilities inline.

## Task review: what AI can do and what you must check

| Task (O*NET) | Give to AI: method or tool | Keep or verify yourself | Prompt to start |
| --- | --- | --- | --- |
| Boilerplate and tests | Generate from an example | Edge cases and test execution | `Draft function X and add tests for edge cases` |
| Code explanation | Explain a module | Risky areas | `Explain this module and flag risky areas` |
| Pull request review | Draft comments | Final review and security |  |
| New feature | Agent plans, codes, and tests | Review the diff and production readiness | `Implement this against the acceptance criteria and show me the diff` |
| Debugging | Hypotheses from symptoms | Reproduce and fix | `Give me two likely causes of this bug and a way to test each one` |

> Code reaches production only after your review. Never paste secrets. Use local models for private code.

## Tools by use case

=== "Leading assistants"

    - **Claude or ChatGPT** for complex tasks, with secrets kept out of the prompt.
    - **Local models through Ollama** with DeepSeek or Qwen, when the code must not leave your own
      environment.

=== "Specialist tools"

    - **GitHub Copilot** with its agent, **Cursor** with Composer and multi-file editing, **Claude Code**,
      **OpenAI Codex**, **Amazon Q** for security and migrations, and **Gemini Code Assist**.
    - **The pattern companies settled into during 2026** is not "pick one." It is Copilot deployed to
      everyone as an autocomplete baseline, plus an agent such as Claude Code adopted bottom-up by
      senior engineers for harder agentic work. Two layers, two different jobs.

## One practical playbook

!!! example "Build a new feature with an agent and keep control"
    1. Give the agent the task and acceptance criteria in Cursor or a Copilot agent.
    2. The agent makes a plan, writes code and tests, runs them, and fixes errors.
    3. **Human check:** review the diff, edge cases, and security. Run your own tests.
    4. For a difficult bug, diagnose it yourself first, then ask for possible causes.
    5. Output: the feature arrives faster, but it reaches production only after your review.

## Where not to use AI

!!! danger "Red flags"
    - **Production code without review:** AI generates plausible bugs and vulnerabilities.
    - **Secrets, keys, and private code:** do not send them to outside services. Use local models for private work.
    - **Architecture decisions:** AI offers options. A person owns the choice.
    - **Licenses for generated code:** check origin and compatibility.

## Prompt patterns: weak and better

| Weak | Better |
| --- | --- |
| `Write function X` | `Draft function X and show where it could break under load` |
| `Fix the bug` | `Give me two likely causes of this bug and a way to test each one` |
| `Optimize this` | `Where is the bottleneck, and what tradeoffs come with each option?` |

## Where to move your effort

Move time from routine work into architecture, security, agent orchestration, and responsibility for
production. See Chapter 5.

### Before, after, and still human

| Before AI, this was the barrier | Now available quickly | Still belongs to the person |
| --- | --- | --- |
| You wrote every feature, test, and migration by hand | First drafts of code, tests, and migrations take minutes | Architecture and system boundaries |
| Finding a bug in logs took hours | A hypothesis from logs and a possible fix arrive quickly | Production review, security, and incident responsibility |
| Semi-technical tasks had a high entry barrier | Plugins, exports, and integrations are within reach | Deciding what is worth building and why, the outcome |

### The levels ladder in this role

The five levels from Chapter 5, in the language of this profession. Mark where you stand in your main
tasks this week.

| Level | What it looks like here |
|---|---|
| **1. AI user** | I generate code and tests with an assistant |
| **2. Validator** | I review what the agent produced: security, edge cases, and the dependencies it pulled in |
| **3. Orchestrator** | I run several agents on multi-file changes and work as their manager |
| **4. Outcome owner** | I own working production, not lines of code |
| **5. System builder** | I built the system of tests, logs, and rollbacks that holds quality without my supervision |

**Where people usually get stuck.** Junior tasks go first, so level 1 stops being a job. Architecture, security, and responsibility for production are what gain value.

Next: [my level of usefulness](../playbooks/usefulness-levels-self-check.md) → [a plan for one level up](../playbooks/plus-one-level-plan.md).

## Ready-made skills and plugins for this role

You can turn repeatable procedures such as a first-pass pull request review, edge-case tests, migrations,
and security checks into a portable skill, or use an existing one. Browse
[skill banks](https://cheap-intelligence.vercel.app/en/watch/skill-banks), then see
[turn a workflow into a skill](../playbooks/make-it-a-skill.md) to build your own.

## Where to go next

[Map your week](../playbooks/week-inventory.md) → [run the integrated profession audit](../playbooks/profession-audit-integrated.md)
→ [make a 90-day plan](../playbooks/personal-90-day-plan.md). Or open the [workbook](../playbooks/tom1-workbook.md).

---
**Sources for this review:** OpenAI GDPval (2025): <https://openai.com/index/gdpval/> · Anthropic Economic Index: <https://www.anthropic.com/economic-index> · Stanford AI Index (2025): <https://hai.stanford.edu/ai-index> · McKinsey, "The State of AI": <https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai>. Plus the book, Chapters 2 and 3. The commit-share and job-posting figures were checked on Aug 18, 2026; see the [tool map](https://cheap-intelligence.vercel.app/en/watch/tools-map).
