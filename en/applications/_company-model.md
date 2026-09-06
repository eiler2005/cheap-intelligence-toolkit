<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/applications/_company-model
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

> The tools and services named here go out of date. The current version is on the site — see the link above.

---
reading_level: b2-c1-technical
title: "Company model: where professions fit"
description: A value-chain map of 13 roles and the evidence used to judge how AI changes their tasks.
---

# Company model: where professions fit

> The classic way to map a business by activity is **Michael Porter's value chain** (1985). A company
> has *primary* activities that create value directly and *support* activities that make them possible.
> Each profession has a natural place in this model, and sources such as GDPval can sit on top of it.
> **Date: 2026-06.** Find your activity, then your role, and open the role hub.

The link to Chapter 2 is simple. Value comes through three levers: new revenue, savings, and attention
and trust. Porter's primary activities often connect to new revenue and attention. Support activities
often connect to savings.

!!! abstract "A role's color shows how much of its work AI can already replace"
    🔴 **high task replacement** · 🟠 **augment→replace** (the lower layer gets cheaper) ·
    🟢 **strong augmentation** (AI helps but does not replace the role). The color describes *tasks*,
    not the disappearance of a profession. See the [data review](_super-analysis.md) for the reasoning
    behind each color (GDPval · Anthropic Economic Index · O*NET).

---

## 🟢 Primary activities that create value directly

=== "Marketing and sales"

    Attract, persuade, and sell. These activities use the "new revenue" and "attention and trust" levers.

    - 🟠 [Marketer](marketolog.md) · 🟠 [Designer](dizayner.md) · 🟠 [B2B sales](sales-b2b.md)

=== "Operations: creating the product or service"

    Make the product or deliver the service. In knowledge work, this includes IT, product, and data,
    which appear below under Technology. Specific industries have their own operating roles.

    - Industry roles: 🟢 [Teacher](uchitel.md) (education) · 🟢 [Doctor](vrach.md) (healthcare)

=== "Service"

    Keep the customer after the sale.

    - 🔴 [Customer support](podderzhka.md)

=== "Inbound and outbound logistics"

    Supply and delivery. Warehouse, procurement, and logistics roles are planned for later waves and
    Volume 2.

## 🧱 Support activities that make the primary work possible

=== "Technology development"

    Software, data, procedures, and technical knowledge.

    - 🔴 [Developer](razrabotchik.md) · 🟢 [Product / PM](product-pm.md) · 🔴 [Analyst](analitik.md)

=== "Firm infrastructure"

    Accounting, law, finance, planning, and quality assurance in Porter's model.

    - 🔴 [Accountant](buhgalter.md) · 🟢 [Financial analyst](finanalitik.md) · 🟢 [Lawyer](lawyer.md)

=== "Human resources"

    Hiring, developing, and retaining people.

    - 🟢 [HR specialist](hr.md)

=== "Procurement"

    Supplier relationships and price negotiations. These roles are planned for later waves and Volume 2.

---

## The source layer behind each role

The profession pages use three data engines instead of relying on our opinion:

| Source | What it provides | How we use it |
|---|---|---|
| **GDPval** (OpenAI, 2025) | 44 professions and 1320 tasks across **9 sectors**: healthcare, finance, law, manufacturing, retail, media, government, real estate, and wholesale | capability: whether AI can complete the task, based on real work products |
| **Anthropic Economic Index** (2026) | analysis of about 2 million real conversations organized by profession | adoption: which tasks people actually delegate |
| **O*NET** | a standard breakdown from profession to tasks | the common backbone for task lists |

### Professions covered by GDPval: 44 roles

!!! note "Roles named directly in the benchmark"
    GDPval directly includes roles such as **lawyer, accountant, software developer, and nurse**.
    The full list of 44 professions is available at [gdpval.dev](https://www.gdpval.dev/).

| Our role | In GDPval? | Sector |
|---|---|---|
| Lawyer | ✅ yes | law |
| Accountant | ✅ yes | finance |
| Financial analyst | ✅ yes, finance | finance |
| Developer | ✅ yes | media/IT |
| Product / PM | ~ adjacent project-management tasks, not a direct match | n/a |
| Doctor | ✅ sector coverage through nurse/healthcare | healthcare |
| Marketer · Designer | ~ adjacent media tasks, not direct roles | media |
| B2B sales · Customer support | ~ adjacent retail tasks, not direct roles | retail |
| Analyst · HR · Teacher | outside the direct list, so we use O*NET + web research | n/a |

> For roles outside GDPval's direct list, we use O*NET task breakdowns
> (<https://www.onetonline.org/>) and dated web research. The figures show direction, not a guarantee.

---

## Coverage: what is here and what is still missing

!!! tip "The main office professions are covered"
    Marketing and sales, service, technology, product, data, infrastructure, finance, law, accounting,
    and HR are covered. **13 roles are ready.** Industry operations include teacher and doctor.

!!! warning "Not yet in the catalog: later waves and Volume 2"
    Direct operations and production, logistics and procurement, and skilled trades are not yet included.
    Business roles such as an SMB owner or an agent-based team belong to **Volume 2**.

---

> If your exact role is missing, search by task in [_by-task.md](_by-task.md). For the flat catalog,
> open [_index.md](_index.md).
