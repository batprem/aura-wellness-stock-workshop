# Module 3 workshop — a simple data app, one layer at a time

Solo, in Claude Code. Time: [__] minutes.

You build a small app that shows a prepared dataset as a chart and a table, with full CRUD: create, read, update and delete rows. The point is the Module 3 habit: **frontend, backend and database stay separate, and you build one layer per prompt.**

## Stack

| Layer | Tool |
|---|---|
| Frontend | React |
| Backend API | Python |
| Database | SQLite |

Let Claude Code propose how to set each one up. Ask it to explain its plan before it writes code.

## The dataset

[`data/example-activity-log.csv`](data/example-activity-log.csv) is example data: one row per activity, with `id`, `date`, `activity` and `minutes`.

## Steps — one layer per prompt, in this order

Copy-paste prompts for each step are in [PROMPTS.md](PROMPTS.md).

1. **Dataset.** Make a new folder, open it in Claude Code, and put `example-activity-log.csv` and a copy of `../examples/design.md` in it.
2. **Database.** Claude creates **one** SQLite table and loads the CSV into it. Check: the row count matches the CSV.
3. **Python API.** CRUD endpoints plus a summary:
   - list all rows;
   - create a row;
   - update a row;
   - delete a row;
   - return summary numbers for the chart (for example, total minutes per activity).

   **Test the endpoints before you build the screen.**
4. **React screen.** One page that follows [`../examples/design.md`](../examples/design.md):
   - a chart drawn from the summary endpoint;
   - the table, with add, edit and delete (delete asks for a confirm first);
   - the chart updates after each change;
   - empty, loading, saved and error states.
5. **One small change.** Add one field or one more chart. Then a few people show their app.

## Rules

- One layer per prompt. Do not ask for the screen, the API and the database in one go.
- No login. One table.
- Build the smallest version that works first, then change one thing.
- Keep a short "not now" list of what you chose not to build.

## Done when

- The table shows every row from the database, through the API.
- You can add, edit and delete a row (with a confirm before delete), and the chart changes to match after each one.
- You can point to which part is frontend, which is backend, and which is the database.
- You have a "not now" list.

## Links

- Module 3 reference: [../README.md](../README.md)
- Example design system: [../examples/design.md](../examples/design.md)
- Course materials: [github.com/batprem/aura-wellness-stock-workshop](https://github.com/batprem/aura-wellness-stock-workshop)
