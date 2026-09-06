<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/prompts
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

# Prompts: method and review

> Practicum section. **Verified: 2026-06.** This is not a list of "100 prompts that will make you
> money." Exact wording ages as models change. The method lasts longer: **how to think about a prompt
> and how to check the output.** A prompt can speed up one step. A process with review creates a result.

The book's main idea applies here too. AI makes *output* cheaper: a draft, a piece of text, or a
calculation. Value moves to the work around it. You define the task, provide context, and **check the
result**. A good prompt is only half of the job. The other half is a checkpoint outside the model.
Without one, even an excellent prompt produces a demo rather than a dependable result.

> A community that collects real AI cases noticed a pattern: **some of the weakest cases came from
> people who called themselves "AI consultants." They offered many slogans and little that another
> person could reproduce.** A useful technique is simple enough for an ordinary person to repeat. That
> is the standard here.

---

## The CLEAR framework

Use one framework instead of collecting ten acronyms. **CLEAR** comes from Leo Lo's 2023 paper in
*The Journal of Academic Librarianship*. It is a cited method, not a framework invented for this
Practicum. A good request has five properties:

- **C, Concise.** Remove what the model does not need. A long, vague prompt produces a vague answer.
- **L, Logical.** Put the ideas in order: role and context first, then the task, then the format.
- **E, Explicit.** State the output format and limits. For example: "use a table," "no more than five
  points," or "if you are unsure, say so and do not invent an answer."
- **A, Adaptive.** Treat the first answer as a draft. Rephrase the request, narrow it, or ask for a
  better option. Use a conversation instead of a single attempt.
- **R, Reflective.** Review both the output and the prompt. Decide what you should improve next time.

CLEAR works well here because Adaptive and Reflective build review and iteration into the method. It
connects directly to the [Personal AI System](../playbooks/personal-harness-builder.md) in Chapter 6
and evaluation in Volume 2, Chapter 2. This is a habit of thinking, not a bag of tricks.

Add only what your task needs. Give the model a role and context, such as "you are a lawyer working for
the buyer." Show an example of the format you want (few-shot prompting). Apply the Chapter 8 method:
ask for options and criticism instead of a finished answer. AI widens the choice, and you decide. This
also reduces [cognitive debt](https://cheap-intelligence.vercel.app/en/watch/cognitive-practices).

---

## The pattern: weak prompt, better prompt, review

Each technique uses a pair. A better prompt usually includes a role, context, format, boundary, and a
clear review step.

**1. Review a document**

- Weak: "Summarize this contract."
- Better: "Work from my side of the deal. I am the buyer. List the risks for me in order of severity.
  For each risk, quote the relevant clause and suggest an edit. Use a table. Mark any clause that could
  have more than one meaning instead of smoothing it over."
- Review: compare every quote with the contract. You own the decision and the responsibility.

**2. Compare and choose**

- Weak: "Which washing machine should I buy?"
- Better: "Suggest three options for these limits: a 60 x 85 cm space, a dryer stacked above it, a
  budget of N, and a brand that works with the old stacking kit. For each option, explain why it fits
  and name one risk. Do not give me ten choices."
- Review: check current prices and availability. A model can invent both with confidence.

**3. Create a draft (email, post, or reply)**

- Weak: "Write a post about our product."
- Better: "The audience is [who], and their problem is [what]. Give me five post ideas: one expert
  explanation, one that starts a discussion, and one that sells through useful detail. Keep the tone
  calm and avoid hype. Do not invent product facts. Leave a blank when information is missing."
- Review: you own the product facts and numbers. Edit the tone until it sounds like you.

**4. Find weak spots instead of seeking support**

- Weak: "Why is this company a good client for us?"
- Better: "Find reasons to reject this company as a client, such as the wrong size, market, product, or
  budget. Be strict." This uses *via negativa* to push against confirmation bias.
- Review: make the decision after considering both sides. The model only expands the negative side.

**5. Extract structure from text**

- Weak: "Analyze this message thread."
- Better: "Extract every amount and date from this message archive into a table with these columns:
  date, amount, subject, person. Numbers appear in several formats, so normalize them and mark anything
  uncertain."
- Review: inspect a sample of 10 to 15 rows. Expect at least one mistake.

---

## Next

- Start with a [prompt template for your task](templates.md): role, goal, context, format, and review.
- Read the [bank of real cases](cases.md) with before and after examples. It shows where AI saved time
  and where skipping review would have caused trouble.
- If you are tired of explaining the same method again, package it as a
  [skill](../playbooks/make-it-a-skill.md). That page covers packaging. This page covers wording and
  review.

> Update after a material change in model behavior. AI can be confidently wrong, so
> check facts, numbers, quotes, and judgments yourself.
