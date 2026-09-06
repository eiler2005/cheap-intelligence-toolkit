<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/strategy/lawyer
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

# AI strategy: Lawyer

> Prioritized AI adoption map. **Date: 2026-06.** Sources: GDPval, AEI, O*NET, and
> profession automation review (GDPval, AEI, O*NET). ← [Role hub](../lawyer.md)

!!! abstract "Context"
    In GDPval, AI produced an expert-level legal brief in about half of the tasks, **but it can
    invent statutes and case law**. Use it to augment the lawyer's work. AI can speed up the task,
    while strategy and the signature remain with a person.

## 1. Research and drafting (high priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 1 | First-pass research | research time · completeness | Harvey or CoCounsel · **check every citation** |
| 2 | Draft documents and memoranda | drafting time · revisions | contract and claim structures · human completion |

## 2. Review and comparison (high priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 3 | Review a contract for risk | time · risks found | prompt for "risks with a clause citation" · verify citations |
| 4 | Compare versions | time · accuracy | differences table with a "who benefits" column |

## 3. Due diligence (medium priority)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 5 | Repeatable review workflows | review volume · errors | workflow builder in Harvey · checklists |

## 4. Knowledge and compliance (foundation)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 6 | AI search across a knowledge and precedent base | access speed · answer quality | internal base + AI search grounded in a trusted source |
| 7 | Client confidentiality | incidents · compliance | approved environment · de-identification · policy |

## 5. The role (foundation)

| No. | Goals | KPIs | Initiatives |
|---|---|---|---|
| 8 | Shift weight to strategy and negotiation | % of time on high-stakes tasks | less document production, more deals, disputes, and client work |

## Where to start: the first round

Use [process scoring](../../playbooks/process-scoring.md): repetition, volume, verifiability, error
cost, and data.

1. **No. 3, review an incoming contract.** This is the best starting point because the result is
   mechanically checkable. Search the contract for every quotation, and an error becomes visible
   within a minute.
2. **No. 4, compare versions.** It has the same advantage. Check the differences line by line.
3. **No. 1, first-pass research.** Start only with a firm rule: verify every citation against the
   primary source. Without that rule, research becomes the first incident, not the first round.

**Not in the first round:** No. 5, the "due diligence workflow," should wait until the team has
built a reliable review habit on Nos. 3 and 4. AI may draft final documents for signature under No.
2, but a person must review the complete document every time. Never send attorney-client privileged
material or a client's personal data to outside services. This is a boundary, not a scheduling
choice. See the red flags in the [role hub](../lawyer.md).

## Keep these parts of legal work human

- **The legal position and signature.** They cannot be delegated at any maturity level.
- **Materiality of risk.** AI finds clauses; a person decides which ones matter to the deal.
- **Negotiation, court work, and the client relationship.** Trust makes this work more valuable.
- **Assessing the prospects of a dispute.** This requires judgment across the full case, not a database search.

## Review points and stop thresholds

| Initiative | What a person checks | Stop threshold (example, replace with your own) |
|---|---|---|
| No. 1 research | verify every statute and case citation against the primary source | one invented rule means quarantining the tool and rechecking recent conclusions |
| No. 3 contract review | find every quotation in the document text | if a quotation cannot be found, complete a full manual review and fix the prompt |
| No. 4 version comparison | sample rows in the differences table | one missed material difference means returning to manual comparison until the cause is understood |

Before you trust the flow, build a [reference set](../../playbooks/eval-set-builder.md): 20 contracts
already reviewed by hand, with known risks. Test every new tool or prompt against them first.

## Two paths from here

- **You are a lawyer:** open the [role hub](../lawyer.md), then use the
  [Volume 1 workbook](../../playbooks/tom1-workbook.md) to move from your week to an audit and a
  90-day plan.
- **You lead a legal function or firm:** use the [Human Review Matrix](../../playbooks/human-review-matrix.md),
  write the [agent contract](../../playbooks/agent-contract.md) with boundaries for privilege,
  signature, and escalation, then continue with the [Volume 2 workbook](../../playbooks/tom2-workbook.md).

!!! danger "Discipline"
    Verify citations to statutes and case law against the primary source. Only a person owns the
    legal position and signature.

---
**Sources:** profession automation review (GDPval, AEI, O*NET); book, Chapters 2 and 3.
