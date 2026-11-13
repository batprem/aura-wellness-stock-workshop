# Module 4 workshop — skills, MCP and plan mode

Solo, in Claude Code. Time: [__] minutes.

Work in a new, empty folder and open it in Claude Code. Six short steps; copy-paste prompts are in [PROMPTS.md](PROMPTS.md). Commands below are quoted from the official docs linked in each step.

## 1. Recap: CLAUDE.md and SKILL.md

- **CLAUDE.md** — standing instructions for the whole project: what we build, the scope, the rules.
- **SKILL.md** — how to do one kind of task, used when that task comes up.

## 2. A hello-world skill, by hand

Copy [`../examples/hello-world/SKILL.md`](../examples/hello-world/SKILL.md) (example) into your folder at:

```
.claude/skills/hello-world/SKILL.md
```

That is a **project** skill. (A personal skill for all your projects lives in `~/.claude/skills/<name>/SKILL.md`.) Then check Claude picks it up: say "say hello", or type `/hello-world`. You should get the three-line reply from the file.

Docs: [Skills in Claude Code](https://code.claude.com/docs/en/skills)

## 3. Let Claude create a skill

Anthropic's [skill-creator](https://github.com/anthropics/skills/tree/main/skills/skill-creator) skill helps Claude write new skills. It is part of the `example-skills` plugin in [github.com/anthropics/skills](https://github.com/anthropics/skills). In Claude Code:

```
/plugin marketplace add anthropics/skills
/plugin install example-skills@anthropic-agent-skills
```

Then ask Claude to use skill-creator to make a **changelog-entry** skill. Compare the result with your hand-written hello-world skill and with [`../examples/SKILL.md`](../examples/SKILL.md): what did it add, and what would you cut?

## 4. Use a third-party skill

Skills are shareable. Example: Matt Pocock's public [skills repo](https://github.com/mattpocock/skills) (for example `grill-me` and `tdd`). Its README gives this install for Claude Code:

```
claude plugin install mattpocock-skills@claude-plugins-official
```

Read a skill's `SKILL.md` before you use it, so you know what it will do. Then pick one and try it on a small task.

## 5. MCP: connect Notion

MCP (Model Context Protocol) is an open standard for connecting agents to outside tools and data. If a resource is offered as an MCP server, any agent that speaks MCP can use it.

Each person needs **their own Notion account**. From the [Notion MCP guide](https://developers.notion.com/guides/mcp/get-started-with-mcp):

```
claude mcp add --transport http notion https://mcp.notion.com/mcp
```

Then run `/mcp` in Claude Code and sign in to Notion. Ask Claude to find one of your pages and summarise it.

Scope: by default the server is added for you, in this project only. A project-scoped server is shared through a `.mcp.json` file in the project. Docs: [Connect Claude Code to tools via MCP](https://code.claude.com/docs/en/mcp)

## 6. Plan mode and the interview pattern

Press **Shift+Tab** to cycle permission modes until you reach plan mode (or type `/plan`). In plan mode Claude researches and proposes changes without editing your files. Ask Claude to **interview you first** — questions to gather context — and only then propose a plan. Docs: [Permission modes](https://code.claude.com/docs/en/permission-modes)

## Done when

- **Skill by hand:** your hello-world skill answers in its exact format, by name or by `/hello-world`.
- **Skill by Claude:** skill-creator made a changelog-entry skill, and you can say how it differs from yours.
- **Shared skill:** you installed a third-party skill and used one of its skills once.
- **MCP:** Claude Code read a page from your own Notion through the Notion server.
- **Plan mode:** Claude asked you questions first, then gave a plan, and no file changed.
- **In your words:** you can say when you would reach for CLAUDE.md, a skill, or an MCP server.

## Links

- Module 4 reference: [../README.md](../README.md)
- Course materials: [github.com/batprem/aura-wellness-stock-workshop](https://github.com/batprem/aura-wellness-stock-workshop)
