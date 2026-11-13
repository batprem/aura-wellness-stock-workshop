# Module 3 — Software essentials

A short reference for the third hour: layers, frontend and backend, requirements, and prompting for usable UX without overengineering. This module is mostly teaching, with an example prompt you can reuse. Teaching language is English.

Slide deck: [Module 3 — Software essentials](https://claude.ai/artifact/4VSsa5KJhmpscb2Dah1sLz)

Course materials: [github.com/batprem/aura-wellness-stock-workshop](https://github.com/batprem/aura-wellness-stock-workshop)

## The layers

Software sits on layers: **Hardware → CPU / Memory / I/O / GPU → Code → Software**.

In the products you build:

- **Frontend** shows — the graphical user interface.
- **Backend** decides — it receives requests from the frontend and talks to the database.
- **Database** remembers — long-term memory.

Keep frontend, backend and database **separate**. One layer per prompt. Build the smallest version that works.

## The overengineering loop — and how to get out of it

**The loop:** ask for everything at once → all layers change in one go → something breaks → add more code to fix it — and repeat.

**The way out:**

- One layer per prompt.
- Build the smallest version that works.
- Ship it, get feedback, then add.
- Write down what you are not building.

## Requirements, then work

Requirements documents (BRD, PRD, SRS) turn into sprint-sized work: **requirements → tasks → prompts → review**. Work in small sprints, not one giant build.

## Design system: `design.md`

A design system is a shared kit for the frontend: **tokens** (colors, fonts, spacing), **components** (buttons, cards, forms built once), and **rules** for using them. Write it once in a file such as [`examples/design.md`](examples/design.md), then point every UI prompt at that file so Claude reuses it instead of re-deciding the look each time.

That file is an **example — not real Aura data**, and not Aura’s real product design. Teams may replace the tokens with their own.

## Example prompt for usable UX — not a real Aura request

The brackets are for you to fill in.

> Build one screen for a \[role\] to \[task\]. Frontend only — use mock data, no backend yet. Follow `design.md`. Use its buttons and cards. Show empty, loading, and error states. Keep only what this task needs, and list anything you left out.

Habits behind that prompt: say who the user is and their one task; ask for the simplest screen that does it; point to `design.md` so the design system is reused; ask for empty, loading and error states; and ask “What can we remove?”

## Workshop — a simple data app

Solo, in Claude Code: build a small app that shows a prepared dataset as a chart and a table, with full CRUD (create, read, update, delete rows). React frontend, Python API, SQLite database, one layer per prompt. Brief: [workshop/README.md](workshop/README.md). Prompts: [workshop/PROMPTS.md](workshop/PROMPTS.md). Dataset: [workshop/data/example-activity-log.csv](workshop/data/example-activity-log.csv) (example data).

## Next

Module 4 — Context management: [module-4-context-management](../module-4-context-management/).
