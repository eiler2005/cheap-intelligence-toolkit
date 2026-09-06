<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/harness-examples/examples-by-level
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

# Examples by level: from a project to an agent harness

> Practicum for Chapter 6, "The Human as a System."
> The examples below do not recommend specific services. They show how a simple setup can grow into an agent harness.

## The main rule

An agent harness begins when AI has a real working environment, not when you add a fashionable tool. It needs:

1. a goal;
2. context;
3. rules;
4. tools;
5. memory;
6. verification;
7. access limits;
8. reusable skills.

A skill is a saved procedure that the system can reuse for a specific kind of task. Without these elements, you still have a chat with a model.

---

## Level 0. An empty chat

**What it is:** you open a model and start from zero.

**When it works:** you need a one-time idea, a quick draft, or a low-risk conversation.

**Where it breaks:** the model does not know your goals, past decisions, limits, style, or the point where someone must verify its work.

**The sign:** every session starts with a long explanation of who you are, what you do, and which rules matter.

---

## Level 1. A project workspace

**Examples in this class:** ChatGPT Projects and Claude Projects.

**What you add:** a separate space for a long-running topic. It holds files, chats, instructions, and project context. For most people, this is the simplest way into a harness.

**A good example:** a "Job Search" project with your resume, a story bank, job listings, criteria for choosing companies, tone instructions, and an application log.

**What already works like a harness:**

- context carries over between chats;
- instructions live inside the project;
- you can return to a long task without explaining everything again;
- you can keep the project separate from unrelated topics.

**The limit:** a project does not replace verification. It keeps context, but it cannot take responsibility for a correct decision.

---

## Level 2. A personal knowledge base plus a model

**Examples in this class:** Obsidian, Notion, NotebookLM, a local Markdown folder, or a personal document collection connected to a chat.

**What you add:** your knowledge no longer lives inside one product. You control the collection of notes, decisions, templates, cases, and sources.

**A good example:** an analyst keeps a glossary of metrics, decisions from past meetings, common data errors, and verification templates. When a new task arrives, the analyst gives the model the right part of that context instead of sending everything.

**What already works like a harness:**

- you can reuse knowledge across different tools;
- you can assemble relevant context and give it to a model quickly;
- you depend less on one chat or platform.

**The limit:** a knowledge base without a Task-to-Outcome Map becomes an archive. This map links each task to a result. Ask one question: which result does each item help you produce?

---

## Level 3. A custom assistant or a project with rules

**Examples in this class:** a custom GPT, a Claude Project with instructions, an assistant for a specific role, or a saved set of instructions and files.

**What you add:** the model gets a role, rules, and a repeatable way to work.

**A good example:** a sales proposal assistant that knows the brand voice, limits on promises, common objections, the email format, and the facts it must never invent.

**What already works like a harness:**

- the system has rules;
- it has context;
- it has a defined output format;
- you have the first version of skills, which are reusable instructions for common tasks.

**The limit:** without verification, the assistant can turn into a factory for confident but false text.

---

## Level 4. A skill as a reusable capability

**Examples in this class:** Agent Skills in Claude or Codex, a local `SKILL.md`, a procedure template, or a command in a work repository.

**What you add:** a good way of working no longer depends on one person's memory. The system can use it as a skill.

**A good skill explains:**

1. when to use it;
2. which inputs it needs;
3. which steps to follow;
4. what to verify;
5. when to stop and ask a person;
6. what a finished result looks like.

**Skill examples:**

- "review a contract with our risk matrix";
- "prepare an executive summary, a short decision-focused recap, of a meeting";
- "run a weekly review of personal goals";
- "draft a README from the project structure";
- "prepare questions for a doctor from the collected information without offering a diagnosis."

**The limit:** a skill is stronger than a prompt, but poor rules make it more dangerous. The skill will repeat the mistake too.

---

## Level 5. An agent in a messenger or dashboard

**Examples in this class:** Hermes, an OpenClaw agent, a local Telegram assistant, or an internal dashboard.

**What you add:** the agent works inside a familiar environment instead of living only in a model's chat. It can receive events, send reminders, gather data, prepare actions, and return the result to a person.

**A good example:** a personal assistant in Telegram that:

- collects your priorities in the morning;
- asks for a short review in the evening;
- shows recurring tasks once a week;
- suggests one skill worth improving;
- does not contact people or move money without approval.

**What already works like a harness:**

- it has an environment;
- it follows a regular cycle;
- it has memory;
- it produces logs;
- it can use tools;
- you can add approvals, which require a person to confirm an action.

**The limit:** this level needs a sandbox, meaning a restricted space where the agent cannot reach everything. An agent with access to email, files, remote servers through SSH, a customer relationship management (CRM) system, or payments is a risk unless important actions need approval and produce logs.

---

## Level 6. A catalog of agents and templates

**Examples in this class:** OpenClaw `SOUL.md` templates, catalogs of agent roles, and internal libraries of assistants.

**What you add:** roles and skills become reusable templates rather than personal notes. You can start with an agent for marketing, software development, finance, HR, support, or learning, then adjust it to your own limits.

**What helps:** the template lets you see which parts a role needs, such as a goal, data, tools, a security policy, memory, and an output format.

**What can go wrong:** you copy someone else's agent without understanding its context. The template does not know your customers, risks, or rules.

---

## A short path to the next level

| What you have now | The next honest step |
|---|---|
| An empty chat | Create one project for a long-running task |
| A project without structure | Add instructions, files, and a definition of done |
| Many notes | Build one context folder for three recurring tasks |
| A recurring task | Turn one procedure into a skill |
| An agent with access | Add a sandbox, approvals, and logs |
| Many agent templates | Keep only the ones tied to an outcome |

---

## Sources and verification notes

- OpenAI Help Center: [Projects in ChatGPT](https://help.openai.com/en/articles/10169521-projects-in-chatgpt).
- Claude Help Center: [What are projects?](https://support.claude.com/en/articles/9517075-what-are-projects).
- OpenAI Developers: [Agent Skills in Codex](https://developers.openai.com/codex/skills).
- Anthropic Docs: [Agent Skills](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview).
- OpenClaw examples: [awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents).
- Hermes: internal research materials in this project. Before public release, add a direct URL or have the author approve it as a community case.
