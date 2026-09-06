<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/playbooks/klarna-compass-example
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

# Example: Klarna through the Change Compass, a win and a skipped gate

> A second public review for **Volume 2, Chapter 11**. The first is [IKEA](ikea-compass-example.md).
> Klarna is a Swedish fintech service for consumer payments. The case shows **both sides**:
> where an agent produced a real return and which gate the company skipped, with a public cost.
> This review uses public reporting and was **checked in 2026-07**. The Klarna figures are company claims
> without independent verification. Business media reported the 2025 reversal.

## The timeline in three lines

- **February 2024.** Klarna announced that its OpenAI-powered assistant handled 2.3 million support conversations in one month,
  work it compared with about 700 full-time agents. It reported resolution in about 2 minutes instead of 11 and forecast
  a $40 million increase in annual profit. These are company claims.
- **2024.** The company freezes hiring and publicly builds a story around "AI instead of people."
- **May 2025.** CEO Sebastian Siemiatkowski says that the focus on lower cost went too far and hurt quality.
  Klarna starts hiring customer service staff again in a hybrid model where the customer can **always** reach a person.
  CX Dive and business media reported this in May 2025.

## 1. WHERE arrow: the process choice was sound

Run "common fintech support questions" through [Process Scoring](process-scoring.md) and it earns 5 out of 5.
The work repeats, the volume is huge, you can check the result, data exists, and the cost of an error is manageable *for common cases*.
An agent can pay off here. Klarna's 2025 reversal did **not** cancel that result. AI still handles the common flow.

## 2. PEOPLE arrow: this is where Klarna skipped a gate

The problem was the order of moves, not the technology. Klarna removed people **before** it had tested what happens in hard cases,
including disputes, fraud, and difficult personal situations.
Under the [Human Review Matrix](human-review-matrix.md), these are classic red-zone tasks. The cost of an error is high,
the result cannot be checked instantly, and emotional context matters. The CEO later described the lesson clearly:
the model was not the problem. The company put **too much emphasis on cost**.

## 3. EFFECT arrow: what Klarna counted and missed

Klarna counted staffing savings and response speed. It did not count the cost of confident but wrong answers about money,
fees, and terms. In fintech, such an answer is more than a customer satisfaction problem. It creates **compliance risk**,
meaning a risk of breaking legal or regulatory requirements. An effect metric without a quality metric is half a dashboard.

## 4. CONTROL arrow: what was missing

Against the [Agent Contract](agent-contract.md) and [evaluation set](eval-set-builder.md):

- Klarna did not name a **stop threshold** in advance, such as "if quality complaints rise above X, bring people back."
  The threshold fired after the fact through the press and the CEO.
- Edge cases such as disputes and fraud did not have a clear "the correct answer is escalation to a person" rule.
- Reversal was expensive. The reputation of a "company that replaced people" stayed in every article.

## 5. The seven gates in the Klarna case

| Gate | Passed? |
|---|---|
| 1. A testable, high-volume process is selected | Yes. Common questions |
| 2. Data and a knowledge base exist | Yes |
| 3. Reference quality check includes difficult cases | Common cases: yes. Edge cases: judging by the reversal, no |
| 4. Pilot keeps a person in the loop | Yes at first, but the loop was removed quickly |
| 5. Stop threshold is named in advance | No. This skipped gate is the case's main lesson |
| 6. People move into new roles instead of leaving | No. Klarna skipped it and hired again in 2025 under a new hybrid model |
| 7. Scaling starts after the metric holds | No. Scaling followed a savings forecast rather than a quality metric |

## 6. Apply it to your business

1. **The reversal does not mean "AI does not work."** Klarna kept the agent and returned people to the points where they must remain.
   AI for the common flow and a person for the difficult flow is the working model from Chapter 2.
2. **Name the stop threshold before launch, not after a press story.** One number and one action create a line in the
   [Agent Contract](agent-contract.md) that costs nothing and can protect your reputation.
3. **Passing the PEOPLE gate costs less than skipping it.** Moving a team into audit and knowledge-base roles,
   as in [Sergei's case](../cases/persona-rukovoditel-podderzhki.md), costs less than a public reversal and a second hiring round.

---

**Sources, checked 2026-07:**

- Klarna, 27.02.2024. AI assistant powered by OpenAI: 2.3 million conversations, work compared with about 700 full-time equivalents (FTE),
  and a forecast of about $40 million in 2024 profit. Company claim:
  <https://www.klarna.com/international/press/klarna-ai-assistant-handles-two-thirds-of-customer-service-chats-in-its-first-month/>
- OpenAI customer story, "Klarna's AI assistant does the work of 700 full-time agents":
  <https://openai.com/index/klarna/>
- Customer Experience Dive, 09.05.2025. Klarna again recruits people for customer service:
  <https://www.customerexperiencedive.com/news/klarna-reinvests-human-talent-customer-service-AI-chatbot/747586/>
- FinTech Weekly, 12.05.2025. Klarna resumes human customer-service hiring after its AI pivot:
  <https://www.fintechweekly.com/magazine/articles/klarna-hires-customer-service-after-ai-pivot>

Details change. Check them on the date you read this.

Your route: [Process Scoring](process-scoring.md) -> [Gate Sheet](change-gates.md).
Back: [Volume 2 Workbook](tom2-workbook.md).
