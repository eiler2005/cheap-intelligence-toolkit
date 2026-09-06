# skills — навыки и браузерные инструменты

Две разные вещи в одной папке.

## `<slug>/SKILL.md` — навык для агента

Файл-инструкция в формате Agent Skills: агент подхватывает его сам, когда задача попадает в его
область. Положите папку навыка туда, где ваш агент их ищет — у Claude Code, Codex, Cursor и других
свой путь; смотрите документацию своего инструмента.

Работает и без всякого агента: внутри каждого файла лежит текст в код-блоке, который можно
скопировать целиком и вставить в обычный чат — с ChatGPT, Claude, Алисой, GigaChat. Это тот же
навык, просто вручную.

Как устроен такой файл и как написать свой под свою повторяющуюся процедуру —
[`playbooks/make-it-a-skill.md`](../playbooks/make-it-a-skill.md). Правило простое: если вы
объясняете ИИ одну и ту же логику в четвёртый-пятый раз, это уже навык.

## `<slug>/tool.html` — браузерный инструмент

Один самодостаточный файл. Скачайте и откройте в браузере — интернет не нужен. Считает у вас на
устройстве, никуда ничего не отправляет, аккаунта не требует.

У каждого инструмента на сайте есть чат-версия на случай, если браузера под рукой нет.

## Лицензии

`SKILL.md` и прочие тексты — CC BY-NC-SA 4.0. `tool.html` — MIT: берите код, меняйте, встраивайте.

---

**In English.** Two different things share this folder. `<slug>/SKILL.md` is an agent skill in the
Agent Skills format — put the folder where your agent looks for skills, or copy the text block inside
into any ordinary chat and it works as a prompt. `<slug>/tool.html` is a self-contained browser tool:
download it, open it, no internet and no account needed; it computes on your device and sends nothing.
To write your own skill, see [`playbooks/make-it-a-skill.md`](../playbooks/make-it-a-skill.md).
Texts are CC BY-NC-SA 4.0, code is MIT.
