# Module 4 — Context management

Materials for the fourth hour: example `CLAUDE.md` and `SKILL.md` layouts, a short MCP reference, and a solo workshop. These match the example layouts on the slides.

> **Example layouts only — not real Aura data** and not a required format.

Slide deck: [Module 4 — Context management](https://claude.ai/artifact/NfTyabyBwmrACeMSfPuL2m)

## What’s in this folder

| Path | What it’s for |
|---|---|
| [examples/CLAUDE.md](examples/CLAUDE.md) | Example project briefing for the stock-check app (same layout as Module 4, slide 10). The \[threshold\] is still for the team to fill. |
| [examples/SKILL.md](examples/SKILL.md) | Example skill: how to write a changelog entry (same layout as Module 4, slide 13). |
| [examples/hello-world/SKILL.md](examples/hello-world/SKILL.md) | Example hello-world skill for the workshop. Copy it to `.claude/skills/hello-world/SKILL.md`. |
| [workshop/README.md](workshop/README.md) | Solo workshop: skills, MCP (Notion) and plan mode. Prompts in [workshop/PROMPTS.md](workshop/PROMPTS.md). |

The Module 5 starter `CLAUDE.md` and changelog you will actually edit live at the [repository root](../CLAUDE.md) and in [CHANGELOG.md](../CHANGELOG.md). Example stock and user data: [`../data/`](../data/).

## How they differ

- **CLAUDE.md** answers *what* and *why* for the project, the whole time you work on it: purpose, scope, team rules.
- **SKILL.md** answers *how* for one kind of task, when that task comes up: when to use it, the steps, the result.

Example: CLAUDE.md says the MVP is login, stock tables and the red label. A skill describes how to write a changelog entry after each build. The *rule* “every build gets a changelog entry” belongs in CLAUDE.md; the *how-to* belongs in the skill.

## MCP — Model Context Protocol

MCP is an open standard for connecting agents such as Claude Code to outside tools and data — a database, GitHub, Notion. **If a resource is offered as an MCP server, any agent that speaks MCP can find it and use it — no custom wiring per agent.**

- **CLAUDE.md** — *what and why*: standing project instructions.
- **SKILL.md** — *how*: a procedure for one kind of task.
- **MCP** — *reach*: tools and data outside the project.

What an MCP tool returns lands in the agent's context window, so connect only what the task needs: right context, not most context.

In Claude Code a server can be added for you in one project (the default), for you in every project, or for the whole team through a `.mcp.json` file in the project. Official guide: [Connect Claude Code to tools via MCP](https://code.claude.com/docs/en/mcp).

## Workshop

Solo, in Claude Code: a hello-world skill by hand, a skill made with skill-creator, a third-party skill, Notion over MCP, and plan mode with an interview. Brief: [workshop/README.md](workshop/README.md).

## Preparing context for the workshop

- **Goal:** a mini ERP for stock checking.
- **MVP:** user login, read stock tables, red label for almost-empty items.
- **\[threshold\]:** still a team decision; write it into CLAUDE.md once agreed. Do not let Claude Code choose it.
- **Sample data:** the example CSVs in [`../data/`](../data/) — not real Aura records.

## Next

Module 5 — Stock management workshop: [the brief and starter files at the repo root](../BRIEF.md).
