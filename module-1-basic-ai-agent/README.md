# Module 1 — Basic AI Agent

A one-page reference for the first hour. This module is theory, not a build. Teaching language is English.

Slide deck: [Module 1 — Basic AI Agent](https://claude.ai/artifact/9aGQyVuaeMfwNXa8aCkx5U)

Course materials: [github.com/batprem/aura-wellness-stock-workshop](https://github.com/batprem/aura-wellness-stock-workshop)

## The two parts of an agent

An AI agent is an **LLM** plus a **harness**.

- **LLM (Large Language Model):** the brain. It reads text, plans, and generates text, including commands. On its own it cannot touch a file or run anything. It is a language model, trained with data, and **probabilistic** — likely is not certain.
- **Harness:** the software around it — the hands. It executes those commands and feeds the results back to the LLM.

We talk to the model through **chat messages**. That list is its context.

## The full loop

1. You ask for a task (the goal).
2. The **LLM** plans and generates a command.
3. The **harness** executes it.
4. The harness **feeds the result back** to the LLM.
5. Repeat until the task is done. Then the LLM gives a final answer.

That loop is what makes something an agent rather than a chatbot. In Module 2 you will watch it happen in Claude Code.

## Habits when you work with an agent

- **State the goal clearly.** The plan is only as good as the request.
- **Give it context.** It knows its training data, not your team.
- **Check the results.** It is probabilistic: likely is not certain.
- **Ask for less.** Small, simple steps beat an overengineered build.

## Next

Module 2 — Claude Code: [module-2-claude-code](../module-2-claude-code/).
