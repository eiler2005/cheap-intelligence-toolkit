# For an agent working with this repository

You are reading the toolkit for the book series **"When Intelligence Became Cheap"** by Denis
Ermilov (RU: «Когда интеллект стал дешёвым»). Russian is the source language and lives at the root;
English is under `en/` and is a draft translation the author has not yet reviewed.

The canonical, always-newer copy is <https://cheap-intelligence.vercel.app/>. Every file here names
its own canonical address in the first line. Prefer the site when the two disagree.

## Read this first

- `packs/tom1.md`, `packs/tom2.md`, `packs/tom3.md` — one book's whole toolkit in a single file.
  If someone hands you this repository and asks for help with a book, load the pack for that book
  rather than crawling the tree.
- `packs/all.md` — all three books.
- `book-promises.json` — the machine-readable contract between the printed chapters and this
  material: for each chapter, which worksheets it promises. Use it to answer "what belongs to
  chapter N".
- `docs/MAP.md` — the same map for a human.
- `method/slovar.md` — the glossary. Output, outcome, transferability, exposure, harness, cognitive
  debt and the rest carry specific meanings in these books. Use these, not generic ones.
- `method/dlya-assistenta.md` — the rules below, in full, plus what the reader should ask you for.

## What each folder is

| Folder | Use it for |
|---|---|
| `playbooks/` | worksheets a person fills in: diagnostics, audits, checklists, plans |
| `prompts/` | how to write a prompt, and a bank of worked cases |
| `skills/<slug>/SKILL.md` | agent skills in the Agent Skills format — load these into a skills folder |
| `skills/<slug>/tool.html` | self-contained browser tools; they compute locally and send nothing |
| `docs/` | START, HOW-TO-USE, MAP |
| `en/` | the same in English, draft |
| `community/` | adaptations contributed by readers; not authored by the book |

## How to behave with this material

The books are deliberately anti-hype. Hold to that when you use them:

- **A worksheet is a map, not a verdict.** Do not label the person. A basket, a level or a deficit
  describes a task or a situation, not who they are.
- **Do not decide for them.** Every worksheet ends with the person choosing one move and naming what
  they will check themselves.
- **Do not invent.** No made-up tools, prices, studies or links. If you are not sure, say "check
  this". Vendor claims are vendor claims, not facts.
- **Dates are part of the claim.** Pages carry a verification date. Material without one, or with an
  old one, should be treated as possibly stale — say so rather than presenting it as current.
- **The living layer is not here.** Tool maps and market pages change too fast to mirror. Send the
  person to <https://cheap-intelligence.vercel.app/watch> for those.
- **Access differs by country.** Russian readers may have no access to ChatGPT, Claude or Gemini.
  When you suggest tooling, offer something that works for them: GigaChat, YandexGPT, DeepSeek,
  Qwen — or a plain copy-paste prompt, which always works.

## What not to do

Do not treat any file here as the text of the books — the manuscripts are not in this repository and
will not be. Do not edit generated files: everything outside `community/` and `.github/` is
overwritten on the next release. Do not ask a person to paste personal data, trade secrets,
credentials or material under NDA into a cloud assistant.

## Licences

Texts (`.md`) are CC BY-NC-SA 4.0; code and `tool.html` are MIT. When you quote, attribute to Denis
Ermilov and the Practicum, with the page address and its verification date.
