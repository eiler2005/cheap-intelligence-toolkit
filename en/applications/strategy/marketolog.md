<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/strategy/marketolog
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

# AI strategy: Marketing specialist

> A prioritized AI adoption map for marketing. It shows an individual what to learn and gives a
> function leader initiatives and department KPIs. **Date: 2026-06.** Sources: GDPval, Anthropic
> Economic Index and O*NET. All figures show direction, not a
> guarantee. ← [Role hub](../marketolog.md)

!!! abstract "Context from the data"
    Content, reporting, and business outreach are being automated quickly. The actual savings
    depend on your data, channels, and review process. Anthropic Economic Index estimates are a
    guide, not a guarantee. The role is moving away from manual production and toward strategy,
    taste, and audience trust.

## 1. Process automation (high priority)

| No. | Goals or directions | KPIs | Initiatives |
|---|---|---|---|
| 1 | Automate routine digital campaign work: setup, launch, and basic monitoring | % of tasks automated · launch time · number of errors | AI marketing automation platform · templates and rules · ad account integrations |
| 2 | Automated campaign reporting and anomaly alerts | reporting time · attribution accuracy · % of data-informed decisions | automated reports with Improvado · alerts for drops in CTR or conversion · attribution models |
| 3 | Automatic behavior-based audience segmentation | segmentation accuracy · segment conversion · reach | AI-enabled CDP · dynamic rules · training on historical data |

## 2. Content generation and optimization (high priority)

| No. | Goals or directions | KPIs | Initiatives |
|---|---|---|---|
| 4 | Generate text content such as posts, emails, and descriptions | volume · time per item · CTR or conversion | Claude or ChatGPT · templates and brand voice guide · **human quality control** |
| 5 | SEO optimization and keyword research | rankings · organic traffic · relevance | AI SEO tools such as Surfer and Semrush · trend analysis · automatic meta tag generation |
| 6 | Visual content such as banners, creative assets, and adaptations | time · volume · CTR · cost | Midjourney or Firefly · libraries · A/B test |

## 3. Hyper-personalization (medium-high priority)

| No. | Goals or directions | KPIs | Initiatives |
|---|---|---|---|
| 7 | Personalized content and offers | CTR · conversion · LTV · NPS or CSAT | recommendation engines · real-time data · personalization A/B tests |
| 8 | Next best action for a customer | recommendation conversion · average order value · funnel speed | next-best-action model · action catalog · channel integrations |
| 9 | Dynamic pricing and discounts | margin · conversion · response | AI pricing model · CRM and catalog integrations · competitor monitoring |

## 4. Analytics and forecasting (medium priority)

| No. | Goals or directions | KPIs | Initiatives |
|---|---|---|---|
| 10 | Demand forecasting | accuracy (MAPE) · inventory level · unmet demand | AI forecast · add external factors · calibration |
| 11 | Customer churn forecasting | accuracy · % of high-risk customers retained · churn reduction | churn model · retention triggers · CRM integration |
| 12 | Sentiment and topic analysis across social media and reviews | response speed · number of topics found · sentiment index | AI social listening and Voice of Customer · notifications · support integration |

## 5. Interaction and lead generation (medium priority)

| No. | Goals or directions | KPIs | Initiatives |
|---|---|---|---|
| 13 | AI chatbots for standard questions | % resolved by the bot · response time · CSAT | a bot platform · natural language understanding grounded in the knowledge base · CRM integration |
| 14 | Lead generation and scoring | number of qualified leads · cost per lead · processing time | AI scoring · automatic verification · CRM integration |

## 6. Media planning and buying (where applicable)

| No. | Goals or directions | KPIs | Initiatives |
|---|---|---|---|
| 15 | AI planning for channels and budgets | ROAS · target audience reach · CPA | AI media planning · channel forecasts · optimization |
| 16 | Dynamic creative optimization (DCO) | CTR · viewability · cost per conversion | DCO · creative variations · performance analysis |

## 7. Data, skills, and ethics (foundation)

| No. | Goals or directions | KPIs | Initiatives |
|---|---|---|---|
| 17 | One marketing data store | data quality · access speed | data lake or CDP · data policy · source integrations |
| 18 | Teach the team AI basics | % trained · number of AI initiatives | training program · workshops · internal knowledge base |
| 19 | Ethical AI guidelines for brand safety and personal data | number of incidents · compliance | AI use rules · fact check before publication · audit |

## Where to start: the first round

The tables are a map of what is possible, not your plan. Start with
[process scoring](../../playbooks/process-scoring.md). Ask whether the task repeats, has enough
volume, produces a checkable result, carries an affordable error cost, and has usable data. For
most marketing teams, the first round looks like this:

1. **No. 4, text content generation with human acceptance.** It gets five yes answers: the work
   repeats daily, has enough volume, can be checked with a checklist, and an error costs a rework
   while a person still controls the Publish button.
2. **No. 2, automated reporting and alerts.** Compare the output with the source ad account. This
   work has a rare advantage: an error is visible in the figure.
3. **No. 13, a chatbot for standard questions.** Start only if the request flow is genuinely
   repetitive. Check the history instead of trusting an impression.

**Not in the first round, and that is a useful result:** No. 9, "dynamic pricing," carries a high
cost of error in both money and reputation. For Nos. 7 and 8, personalization and next best action,
answer the fifth question honestly: do the data and rules exist, or are they only in someone's
head? Nos. 15 and 16, media planning and DCO, should wait until reporting in No. 2 is reliable.
Otherwise, you optimize against bad figures.

## Keep these parts of marketing human

- **Brand voice and positioning.** AI can write "in the voice," but it cannot choose what that voice should be.
- **The final Publish decision for any external text.** Treat it as a signature that cannot be delegated.
- **Relationships with core customers, partners, influencers, and media.** Keep them personal.
- **Crisis communication.** AI speed can cause more harm than help here.
- **Budget decisions.** The model can suggest a reallocation, but the budget owner decides.

## Review points and stop thresholds

Give every first-round initiative its own review point in the
[Human Review Matrix](../../playbooks/human-review-matrix.md) and set a threshold in advance in the
[agent contract](../../playbooks/agent-contract.md):

| Initiative | What a person checks | Stop threshold (example, replace with your own) |
|---|---|---|
| No. 4 content | acceptance checklist: product facts, tone, and prohibited claims | more than 1 factual correction per 5 items means returning to a full read of every item |
| No. 2 reports | sample figures against the source ad account | a discrepancy in a core metric means returning to manual reporting until the cause is understood |
| No. 13 bot | audit 10 conversations per day | pause if the share resolved without a person falls below your threshold or a customer complains about tone |

Before you expand, build a [reference set of 20 cases](../../playbooks/eval-set-builder.md). For
content, use 20 accepted pieces. For the bot, use 20 real requests with known answers.

## Two paths from here

- **You are a marketing specialist:** open the [role hub](../marketolog.md), map your week, and
  build a personal plan in the [Volume 1 workbook](../../playbooks/tom1-workbook.md).
- **You lead the function:** use [process scoring](../../playbooks/process-scoring.md), write the
  [first agent contract](../../playbooks/agent-contract.md), run the
  [90-minute workshop](../../workshops/process-scoring-workshop.md) with the team, and complete the
  full path in the [Volume 2 workbook](../../playbooks/tom2-workbook.md).

!!! danger "Discipline"
    Verify facts and figures in public content because AI can invent them. A person owns brand
    voice and strategy. Do not send audience data to third-party services without an approved environment.

---
**Sources for this review:** OpenAI GDPval (2025): <https://openai.com/index/gdpval/> · Anthropic Economic Index: <https://www.anthropic.com/economic-index> · Stanford AI Index (2025): <https://hai.stanford.edu/ai-index> · McKinsey, "The State of AI": <https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai>. Plus the book, Chapters 2, 3, and 7.
