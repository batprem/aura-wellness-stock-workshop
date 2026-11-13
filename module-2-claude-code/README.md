# Module 2 — Claude Code workshop

Workshop materials for Module 2: build a **personal finance report app** in Claude Code — one page in the browser, no server, no login, no database.

Slide deck: [Module 2 — Claude Code](https://claude.ai/artifact/1URWmLwRweaMHr89aijsne)

| Path | What it's for |
|---|---|
| [workshop/README.md](workshop/README.md) | The brief: core features, stretch options, steps, done checklist. |
| [workshop/PROMPTS.md](workshop/PROMPTS.md) | Six prompts, in order. |
| [data/example-transactions.csv](data/example-transactions.csv) | Example data: about three months of transactions. |
| [workshop/reference-app/](workshop/reference-app/) | A reference app built from the example data, and its screenshot. |
| [data/example-dashboard.csv](data/example-dashboard.csv) | Example data from the earlier dashboard warm-up, kept for reference. |

Use the example data in class, not your own bank data.

## Things to watch for

- **Overbuilding:** servers, logins or databases for a one-page report. Say "keep it small".
- **Approving blind:** read the plan and the commands before you say yes.
- **Too much at once:** one change per prompt is easier to check and undo.
- **Check the totals by hand:** pick one month and add it up yourself.

## Optional tools

`git` and `npx` are nice to have today, not needed to finish the warm-up. Official install pages (fill these in on the slides from the same sources if you want them on screen):

- git: [git-scm.com/downloads](https://git-scm.com/downloads)
- Node.js / npx: [nodejs.org](https://nodejs.org)
- Claude Code (required for the warm-up): the official [Claude Code docs](https://docs.anthropic.com/en/docs/claude-code)

This folder does not invent an install command or a sign-in step — use the official docs for the current ones.

## Next

Keep your finance app folder; Module 3 adds a backend and full CRUD on top of the same ideas. Next is Module 3 — Software essentials: [module-3-software-essentials](../module-3-software-essentials/).
