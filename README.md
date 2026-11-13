# Aura Wellness — course materials

Public materials for the Aura Wellness training (about six hours: four hours of teaching and a two-hour workshop). Teaching language is English.

This repository is the home for every module’s handouts and workshop files. The finished Module 5 app is not in here — you build that in Claude Code.

> **Example data and example layouts only — not real Aura data.**

**Clone or download**

```bash
git clone https://github.com/batprem/aura-wellness-stock-workshop.git
cd aura-wellness-stock-workshop
```

Or [Download ZIP](https://github.com/batprem/aura-wellness-stock-workshop/archive/refs/heads/main.zip).

## Modules

| Module | Time | What’s in this repo | Slides |
|---|---|---|---|
| 1 — Basic AI Agent | 1h | [module-1-basic-ai-agent](module-1-basic-ai-agent/) — one-page reference: LLM + harness, the agent loop, habits | [Module 1](https://claude.ai/artifact/9aGQyVuaeMfwNXa8aCkx5U) |
| 2 — Claude Code | 1h | [module-2-claude-code](module-2-claude-code/) — warm-up: create a dashboard from data, with [`example-dashboard.csv`](module-2-claude-code/data/example-dashboard.csv) | [Module 2](https://claude.ai/artifact/1URWmLwRweaMHr89aijsne) |
| 3 — Software essentials | 1h | [module-3-software-essentials](module-3-software-essentials/) — layers, the way out of overengineering, an example [`design.md`](module-3-software-essentials/examples/design.md) and UX prompt, and a [workshop](module-3-software-essentials/workshop/README.md): a simple data app (React, Python API, SQLite) | [Module 3](https://claude.ai/artifact/4VSsa5KJhmpscb2Dah1sLz) |
| 4 — Context management | 1h | [module-4-context-management](module-4-context-management/) — example `CLAUDE.md` and `SKILL.md` layouts, MCP reference, and a [workshop](module-4-context-management/workshop/README.md): skills, MCP (Notion), plan mode | [Module 4](https://claude.ai/artifact/NfTyabyBwmrACeMSfPuL2m) |
| 5 — Stock management workshop | 2h | Brief, starter `CLAUDE.md`, changelog, prompts, and example stock and login data — paths below | [Module 5](https://claude.ai/artifact/HEQi7fGEx67Qoki6hmFZpr) |

## Module 5 — stock workshop (this repository’s root)

You build a mini ERP for stock checking in Claude Code, and own it as its product owner. Three features only: (1) user login (2) read stock tables (3) red label for almost-empty items.

| Path | What it’s for |
|---|---|
| [BRIEF.md](BRIEF.md) | The product brief — today’s scope. |
| [CLAUDE.md](CLAUDE.md) | Starter project context. Fill in the \[threshold\] once the team agrees it. |
| [CHANGELOG.md](CHANGELOG.md) | Empty changelog. One entry per build, newest at the top. |
| [PROMPTS.md](PROMPTS.md) | Prompting habits, plus an example prompt (labelled as an example). |
| [data/example-stock.csv](data/example-stock.csv) | Example stock table — not real Aura data. |
| [data/example-users.csv](data/example-users.csv) | Example login accounts — classroom only, not real users. |
| [data/README.md](data/README.md) | How to use the example data. |

Open this folder in Claude Code for Module 5. Suggested build order: one feature at a time — build it, check it, record a build, add one changelog line, then move on. Frontend, backend and database stay separate. The team agrees the \[threshold\]; do not let Claude Code choose it. Full how-to is in the original Module 5 sections that follow the same files.

### Feature checkpoints

| Feature | Done when |
|---|---|
| 1. User login | A right login reaches the stock page. A wrong login is refused. You can point to which part is frontend and which is backend. |
| 2. Read stock tables | Data comes from the database. Only shown after login. Easy to scan at a glance. |
| 3. Red label | The team agreed the \[threshold\]. The label uses **red plus the words “Low stock”**, not color alone. The rule is written in `CLAUDE.md`. |

### What this repository does not include

- A finished Module 5 app — you build that in the workshop.
- A chosen tech stack, or a chosen \[threshold\].
- Security and hosting guidance — that slot belongs to King’s team in the session.
- Invented clock times or breaks.

## License

[MIT](LICENSE) — workshop and course materials for the Aura Wellness training.
