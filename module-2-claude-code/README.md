# Module 2 — Claude Code warm-up

Workshop materials for the Module 2 warm-up: **create a dashboard from data**, in Claude Code.

> **Example data only — not real Aura data.** The file in `data/` is invented for the classroom.

Slide deck: [Module 2 — Claude Code](https://claude.ai/artifact/1URWmLwRweaMHr89aijsne)

Sample data file: [`data/example-dashboard.csv`](data/example-dashboard.csv)

## Scope — small on purpose

One dataset, one page, a few charts. Nothing more today. No server, no login, no database. This is practice for working with the agent, not a production system. Frontend and backend thinking comes in Module 3.

## Goal and what “done” looks like

**Goal:** get the agent to turn the data into a dashboard, while you steer.

**Done when:**

- The page opens on your machine.
- It shows the data in a few clear views.
- You can explain what each view says.

Pretty is a bonus. If you finish early, improve one view — do not add a new system.

## Suggested steps

1. Make a new folder and put `example-dashboard.csv` in it (copy it from this folder, or clone this repository).
2. Open a terminal there and start Claude Code.
3. Ask the agent to look at the data and describe it.
4. Ask for a simple dashboard; let it plan, then read the plan.
5. Let it build and run; open the result.
6. Give one piece of feedback at a time until it is done.

If git is installed, you may optionally commit after each working step. It is not required today.

## Example prompt — not a required script

This is a sample only. Write your own. It names the data, sets a small scope, and asks for a plan first.

> Look at `example-dashboard.csv` and tell me what it contains. Then propose a simple one-page dashboard with three views. Keep it to a single page with no server or login. Show me the plan before you build.

## Things to watch for

- **Overbuilding:** servers, logins or databases for a one-page dashboard. Say “keep it small”.
- **Approving blind:** read the plan and the commands before you say yes.
- **Too much at once:** one change per prompt is easier to check and undo.

## Optional tools

`git` and `npx` are nice to have today, not needed to finish the warm-up. Official install pages (fill these in on the slides from the same sources if you want them on screen):

- git: [git-scm.com/downloads](https://git-scm.com/downloads)
- Node.js / npx: [nodejs.org](https://nodejs.org)
- Claude Code (required for the warm-up): the official [Claude Code docs](https://docs.anthropic.com/en/docs/claude-code)

This folder does not invent an install command or a sign-in step — use the official docs for the current ones.

## Next

Keep the dashboard folder; it can be a reference later in the day. Next is Module 3 — Software essentials: [module-3-software-essentials](../module-3-software-essentials/).
