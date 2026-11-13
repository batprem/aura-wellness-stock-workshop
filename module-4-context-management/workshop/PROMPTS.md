# Module 4 workshop — prompts

Copy one at a time. Adapt the wording to your own work.

## 2. Hello-world skill

> say hello

Or type `/hello-world`. You should get the exact three-line reply from `.claude/skills/hello-world/SKILL.md`.

## 3. Let Claude create a skill

> Use the skill-creator skill to create a project skill called `changelog-entry`. It should write a short, dated entry at the top of `CHANGELOG.md` after each build: what changed for users, what was fixed, and what is not done yet. Ask me anything you need to know first. Save it under `.claude/skills/`.

Then:

> Show me the SKILL.md you wrote. Compare it with `.claude/skills/hello-world/SKILL.md` — what is the same, and what did you add?

## 4. Third-party skill

> List the skills that are installed now and say in one line what each one is for. Do not run any of them yet.

Then pick one and use it on a small task of your own.

## 5. MCP: Notion

> Using the Notion MCP server, find my page called [page name] and summarise it in three bullet points. Do not change anything in Notion.

## 6. Plan mode + interview

Switch to plan mode first (Shift+Tab, or `/plan`).

> I want to [small feature or change]. Before you plan anything, interview me: ask me questions, one at a time, until you have the context you need. Then propose a short plan. Do not edit any files.
