# Aura Wellness — Stock management workshop

Workshop materials for **Aura Wellness Module 5** (2 hours). You will build a mini ERP for stock checking in [Claude Code](https://docs.anthropic.com/en/docs/claude-code), and own it as its product owner.

The finished app is not in this repository. You build it here, one feature at a time.

> **Example data only — not real Aura data.** Names, categories, quantities and login details in `data/` are invented for the classroom. Do not treat them as live stock or real user accounts.

Slide deck for this module: [Module 5 — Stock management workshop](https://claude.ai/artifact/HEQi7fGEx67Qoki6hmFZpr)

## How to get these files

**ZIP (often easiest in the room)**

1. Open this repository on GitHub.
2. Click the green **Code** button → **Download ZIP**.
3. Unzip it into a folder you will work in, for example `Documents/aura-wellness-stock-workshop/`.

Direct ZIP: <https://github.com/batprem/aura-wellness-stock-workshop/archive/refs/heads/main.zip>

**Or with git**

```bash
git clone https://github.com/batprem/aura-wellness-stock-workshop.git
cd aura-wellness-stock-workshop
```

Then open that folder in Claude Code.

## The brief

Taken word for word from the curriculum:

- Create a mini ERP for stock checking.
- Features: (1) User login (2) Read stock tables (3) Red label for almost-empty items.

This is the boundary of today’s build. If something is not in these three features, it is not in today’s build — note it for a later one. See [BRIEF.md](BRIEF.md).

**Mini**, here, means one slice only: checking stock. An ERP is a system a business uses to run its operations; stock is one part of it. You are not building a full ERP.

## The three features

| Feature | Goal | Checkpoint |
|---|---|---|
| 1. User login | Only signed-in users reach the stock screens. A user signs in; the app checks who they are and lets them in — or says no. | A right login reaches the stock page. A wrong login is refused. You can point to which part is frontend and which is backend. |
| 2. Read stock tables | Signed-in users can see what is in stock. Read only: the table comes from the database and is easy to scan. | Data comes from the database. Only shown after login. Easy to scan at a glance. |
| 3. Red label for almost-empty items | Items that are almost empty stand out, so nobody misses them. The team decides what “almost empty” means: the **\[threshold\]**. | The team agreed the \[threshold\]. The label uses **red plus the words “Low stock”**, not color alone. The rule is written in `CLAUDE.md`. |

## Suggested build order

**One feature at a time.** For each step:

1. Build it.
2. Check it works (use that feature’s checkpoint).
3. Record a build.
4. Add one changelog line.
5. Then move on.

Do not ask Claude Code for all three features in one prompt.

**Frontend, backend and database stay separate**, and the app stays small:

- **Frontend:** login screen, stock table view, and the red label.
- **Backend:** checks the login, serves stock data through an API, applies the \[threshold\] rule.
- **Database:** users, and stock items.

## What’s in this folder

| Path | What it’s for |
|---|---|
| [BRIEF.md](BRIEF.md) | The product brief — today’s scope. |
| [CLAUDE.md](CLAUDE.md) | Starter project context for Claude Code. Fill in the \[threshold\] once the team agrees it. |
| [CHANGELOG.md](CHANGELOG.md) | Empty changelog. One entry per build, newest at the top. |
| [PROMPTS.md](PROMPTS.md) | Prompting habits, plus an example prompt (labelled as an example). |
| [data/example-stock.csv](data/example-stock.csv) | Example stock table — not real Aura data. |
| [data/example-users.csv](data/example-users.csv) | Example login accounts — classroom only, not real users. |
| [data/README.md](data/README.md) | How to use the example data. |

## Before you prompt

1. Open this folder in Claude Code.
2. As a team, agree the **\[threshold\]** (what “almost empty” means). Write that number into `CLAUDE.md`. Do not let Claude Code choose it for you.
3. Use the example data in `data/`, or replace it with other example rows — still not real Aura records.
4. Prompt one feature at a time. Name which part you are changing (frontend, backend, or database). Say what “done” looks like, ask for the plan first, and say what not to add.

## Product owner habits

You own the product, even when Claude Code writes the code.

- **Builds:** a working version you can name, show, and go back to. Make one each time a feature passes its checkpoint — about three by the end. If you used git in Module 2, a commit or tag per build works well.
- **Changelog:** [CHANGELOG.md](CHANGELOG.md) is a plain file in the project. One entry per build, newest at the top, in plain words: what was added, changed or fixed. You can ask Claude Code to add the line; you check it, because you own it.
- **Demo:** show the app, its latest build, and its changelog.

## What this repository does not include

- A finished app — you build that in the workshop.
- A chosen tech stack — you and Claude Code pick one that keeps frontend, backend and database separate.
- A chosen \[threshold\] — the team decides that.
- Security and hosting guidance — that slot belongs to King’s team in the session.

## License

[MIT](LICENSE) — workshop materials for the Aura Wellness training.
