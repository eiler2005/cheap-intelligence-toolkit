# Когда интеллект стал дешёвым — инструменты

**Рабочие материалы к книжной серии Дениса Ермилова: листы, промпты и навыки для ИИ-ассистента.**
*Worksheets, prompts and agent skills for the book series "When Intelligence Became Cheap".
English below.*

ИИ удешевил производство — и быстро устаревает не идея, а конкретика. Поэтому «вечное» живёт в
книге, а живое и обновляемое — в **Практикуме**: [cheap-intelligence.vercel.app](https://cheap-intelligence.vercel.app/).
Этот репозиторий — его слепок в файлах: чтобы материалы можно было забрать к себе, положить в своего
ИИ-ассистента, поправить под свою отрасль и поделиться.

> **Сайт всегда свежее.** Здесь копия, которая обновляется релизами; у каждой страницы в шапке —
> адрес живой версии. Живой слой (карта инструментов, что осваивать сейчас, разборы рынка) сюда
> намеренно не попадает: он устаревает быстрее, чем файл в репозитории.

---

## Быстрый старт

**Хотите просто начать.** Возьмите пакет тома и положите его в своего ИИ-ассистента — в проект
ChatGPT, в проект Claude, в Алису Про, GigaChat или NotebookLM. Дальше спрашивайте:
«разбери мою неделю по корзинам», «собери план на 90 дней».

| Пакет | Что внутри |
|---|---|
| [`packs/tom1.md`](packs/tom1.md) | Том 1 «Человек»: рычаги ценности, неделя по корзинам, уровни полезности, личная система, план на 90 дней |
| [`packs/tom2.md`](packs/tom2.md) | Том 2 «Бизнес в эпоху ИИ-агентов»: зрелость процесса, контракт с агентом, гейты, штаб МСП |
| [`packs/tom3.md`](packs/tom3.md) | Том 3 «Доверие»: компас доверия, периметр, цепочка происхождения, пакет свидетельств |
| [`packs/all.md`](packs/all.md) | всё вместе |

Шесть рецептов подключения по шагам — [`docs/HOW-TO-USE.md`](docs/HOW-TO-USE.md).
Никогда толком не пользовались нейросетью — [`docs/START.md`](docs/START.md).

**Хотите разобраться, что где лежит.** Карта «глава → материал» —
[`docs/MAP.md`](docs/MAP.md) и машиночитаемый [`book-promises.json`](book-promises.json).

---

## Что здесь лежит

| Папка | Что это |
|---|---|
| [`packs/`](packs/) | материалы одного тома одним файлом — для загрузки в ассистента |
| [`playbooks/`](playbooks/) | рабочие листы: диагностика, аудиты, чек-листы, планы |
| [`prompts/`](prompts/) | метод составления промптов и банк кейсов — не «100 промптов для заработка» |
| [`skills/`](skills/) | `SKILL.md` для агентов (Claude Code, Codex и др.) и браузерные инструменты `tool.html`, работающие из файла без интернета |
| [`docs/`](docs/) | старт, подключение, карта материалов |
| [`en/`](en/) | то же по-английски, черновой перевод |
| [`community/`](community/) | ваши адаптации листов под отрасль — единственная папка, куда принимаются PR |

---

## Три книги

**Том 1 «Человек»** — что дешевеет и что дорожает в вашей профессии.
**Том 2 «Бизнес в эпоху ИИ-агентов»** — команды, процессы, клиенты.
**Том 3 «Доверие»** — кому и чему верить, когда контент, работник и клиент стали синтетическими.

Здесь нет текста книг: репозиторий продолжает главы, а не пересказывает их.

---

## Как это поддерживается

Файлы **генерируются** из Практикума и перезаписываются при каждом релизе. Правка, сделанная прямо
здесь в сгенерированном файле, потеряется — присылайте её в `community/` или пишите в Issues.
Исключение: `community/` и `.github/` генератор не трогает никогда.

Нашли устаревшее, сломанное или просто неработающее на практике — заведите Issue. Шаблоны разведены
по смыслу: лист не сработал, сломался инструмент, нет вашей профессии. Правила вклада —
[`CONTRIBUTING.md`](CONTRIBUTING.md).

---

## Лицензии

**Тексты** (`.md`) — [CC BY-NC-SA 4.0](LICENSE-CONTENT): пользуйтесь, меняйте под себя, делитесь на
тех же условиях, с указанием автора, без коммерческого использования.
**Код** — `tool.html` и скрипты — [MIT](LICENSE).

Ссылаясь на материал, называйте автора (Денис Ермилов), Практикум, адрес страницы и её **дату
проверки**. Живые страницы меняются: дата — часть утверждения.

Автор: [github.com/eiler2005](https://github.com/eiler2005) ·
Telegram-канал «AI Meets Reality»: [t.me/aimeetsreality](https://t.me/aimeetsreality)

---

## In English

The toolkit for **"When Intelligence Became Cheap"** — a three-book series by Denis Ermilov:
*The Human Edge*, *Business in the Age of AI Agents*, *The Economics of Trust*.

Take [`packs/en/tom1.md`](packs/en/tom1.md) and load it into a ChatGPT or Claude project,
NotebookLM, or any assistant that accepts an attachment. Then work through it question by question.
Setup recipes: [`en/docs/HOW-TO-USE.md`](en/docs/HOW-TO-USE.md).

> **The English material is a draft translation, not yet reviewed by the author.** The Russian
> edition is the source of truth. Every English file says so until that changes.

Everything here is generated from the Practicum at
[cheap-intelligence.vercel.app](https://cheap-intelligence.vercel.app/), which is always the newer
copy. Texts CC BY-NC-SA 4.0, code MIT. Issues and `community/` pull requests welcome.
