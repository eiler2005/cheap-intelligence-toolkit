<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/prompts/cases
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

# Case bank: before and after

> Practicum section. **Verified: 2026-06.** These techniques come from communities where people share
> how they use AI. They are **field self-reports, not verified business cases**. The numbers are the
> participants' own estimates, and we did not verify them. Take the pattern, including how the person
> framed and checked the task, rather than treating the number as a promise.

The community uses one practical test: **an ordinary person should be able to repeat the case from its
description.** You will not find elaborate setups below. Each case has four fields: input, process,
result, and the point where a person must check the work.

> Source: anonymized field reports from Telegram communities, February to June 2026. Every number
> below is a participant's estimate, not an independently confirmed result.

---

## Work and business

### 1. Contract and procurement: build a position with legal sources

- **Input:** contractor and customer terms and conditions, plus the country where the equipment was
  made and installed.
- **Process:** AI compared the terms, found the applicable law, and drafted a position with quotes. A
  person edited and sent every reply.
- **Result (self-reported):** a dispute that had lasted for months began to move. In a similar case,
  the annual contract price was revised downward. These claims come from the participants.
- **Review:** check legal references and wording against primary sources or with a lawyer. You make the
  decision.

### 2. ICP by rejection: who should NOT become a client

- **Input:** a prospective company's profile and your ideal customer criteria.
- **Process:** instead of asking why the company was a fit, the person asked AI to find **reasons to
  reject it**, such as the wrong size, market, or product. This counters confirmation bias.
- **Result (self-reported):** lead qualification became noticeably more accurate, according to the
  participant.
- **Review:** weigh reasons for and against the client yourself. The model only adds possible reasons
  against.

### 3. Meeting preparation: rehearse the questions

- **Input:** anonymized roles and materials for the participants, such as the CFO and operations
  director.
- **Process:** the person gave the model those roles and asked it to play the other side and ask hard
  questions. They rehearsed the meeting, including by voice while traveling.
- **Result (self-reported):** many of the real questions had come up in rehearsal. Time before the
  meeting became useful practice.
- **Review:** this is a dry run, not a script. The real conversation will take a different path.

### 4. Extract numbers from a real message thread

- **Input:** a message archive where amounts appeared in different formats and contexts.
- **Process:** the model classified the amounts and put them in a table using one format.
- **Result (self-reported):** one row out of about 30 was wrong in the sample that the participant
  checked.
- **Review:** check a manual sample. Models confuse number formats.

## Personal tasks

### 5. Claim for a defective product

- **Input:** details about the product and defect, partly from connected email and cloud storage.
- **Process:** AI collected the facts, outlined the steps, and prepared a claim draft. A person sent it.
- **Result (self-reported):** a clean, nearly finished draft without collecting every fact by hand.
- **Review:** verify the facts and recipient. You press the send button.

### 6. A purchase with tight limits

- **Input:** the available space, compatibility with existing equipment, and budget.
- **Process:** the person asked for an option that met every limit, not the "best" model. They also
  asked for one risk per option.
- **Result (self-reported):** the choice worked. The limits mattered more than an abstract request to
  "find the best one."
- **Review:** check price and stock with the store on the day you buy. Models invent both.

### 7. Personal memory: read-it-later that you can find again

- **Input:** a stream of links that the person would usually save and lose.
- **Process:** a bot saves each link, writes 10 to 20 lines on why it may help and what else it could be
  called, creates a daily digest, and supports semantic search.
- **Result (self-reported):** it addresses forgetting rather than reading. Later, the person can find
  something they would not have remembered well enough to search for.
- **Review:** the pattern has an obvious short-term use. The participant did not prove its long-term
  effect.

### 8. A knowledge base built from articles

- **Input:** dozens of specialist articles and PDFs.
- **Process:** the person put them in a local database, asked questions, and received reviews with
  formulas, ranges, and links to primary sources.
- **Result (self-reported):** a review that used to take one or two days took about 30 minutes.
- **Review:** the participant warns readers to check details and the underlying science. A model can
  summarize a source but is poor at extrapolation.

---

## Failure cases: where the method breaks

These limits are not an argument against AI. They show where a prompt becomes useful only when a
person remains responsible.

| Use caution with | What field reports show |
|---|---|
| **Medicine without a doctor** | Even a user with medical training warns that a meaningful share of AI medical answers may be wrong. Use AI to prepare questions for a doctor, not to make a diagnosis. |
| **Recording meetings without disclosure** | Transcripts and summaries can help, but a hidden recording may be unethical or illegal. Check consent, NDAs, biometric data rules, and local storage. |
| **Complex "autopilots"** | As the setup becomes more complex and the goal moves toward removing people completely, failures and evaluation work increase. |
| **Engineering specifications** | AI-generated specifications can contain requirements that are physically impossible. Without an expert, the error may survive many review rounds. |
| **Someone else's case is not your skill** | A case library cannot replace the ability to use a tool, just as a phrasebook cannot replace a language. That is why this section teaches a method instead of "magic" prompts. |

---

## Send us your case

This bank grows through submitted techniques. If AI saved you hours, or failed with confidence, tell
us about the task, prompt or technique, result, and **how you checked it**. A good case can be repeated
by an ordinary person. A slogan without detail does not qualify, as the note at the top explains.

Contact the [author on LinkedIn](https://www.linkedin.com/in/denis-ermilov) or use
[GitHub](https://github.com/eiler2005). We publish cases without names unless you ask us to include
yours, and we mark each one as a participant's self-report.

## Next

- Build your request with the [templates](templates.md) and [CLEAR method](index.md).
- Analyze your role with the [prompts for exploring your profession](explore-my-profession.md).

> Every number above is a participant's estimate, not an independently verified
> result. Check the facts, and do not treat someone else's metric as a promise about your outcome.
