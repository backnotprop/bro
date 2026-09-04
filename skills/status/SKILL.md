---
name: status
description: Render the state of the work in flight as an ASCII status board in the terminal, instead of a status paragraph.
disable-model-invocation: true
---

# Status board

Show me where everything stands as a board in the terminal. The board replaces the status paragraph. Do not write both.

- Group rows under a short uppercase header with a rule line, one section per phase or stream of work.
- One row per item: a short name, a dotted leader to a fixed column, one status mark, then a terse note. Keep names short and put the detail in the note.
- Use one glyph per state, the same across the whole board: ✅ done, 🔨 in progress, 🟡 blocked or waiting, ⬜ not started, ✖ dropped or closed. Marks go in the mark column only.
- Write a dependency in the note as `← waits on X`. If everything waits on the same thing, say it once.
- Close with a section for what waits on the human: decisions, approvals, anything only they can do. Add one line for what is running right now if agents or jobs are in flight.
- Include only rows you can vouch for. Unknown state is ⬜ with "not verified". Never guess a mark.
- Fit about 80 columns, align the columns, and use no box-drawing tables and no prose paragraphs.

```
INTAKE ──────────────────────────────────────────────────────────────
scope note ......................... ✅  3 items, agreed
source data ........................ ✅  1.2k rows, spot checked
field mapping ...................... ✅  12 of 12 mapped
access keys ........................ 🟡  ← waits on your approval

BUILD ───────────────────────────────────────────────────────────────
importer ........................... ✅  handles the 3 known formats
dedupe pass ........................ 🔨  running, ~200 dupes so far
report layout ...................... ⬜  not started
csv export ......................... ✖  dropped, nobody asked for it

RELEASE ─────────────────────────────────────────────────────────────
staging run ........................ ⬜  ← waits on dedupe pass
team review ........................ ⬜  not scheduled
rollback note ...................... ⬜  not verified

WAITING ON YOU ──────────────────────────────────────────────────────
approve the access keys, which closes intake
pick the report layout: one page, or one per region

RUNNING NOW: dedupe pass, about 5 minutes left
```
