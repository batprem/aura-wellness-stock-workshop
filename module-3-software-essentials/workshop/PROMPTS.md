# Module 3 workshop — prompts, one per layer

Copy one prompt at a time. Check the result before you send the next one. Adapt the wording to your own app.

## 1. Dataset

> This folder has `example-activity-log.csv`. Read it and tell me its columns, how many rows it has, and what kind of chart would suit it. Do not write any code yet.

## 2. Database

> Database only. Create one SQLite table for `example-activity-log.csv` and load every row into it. Use the CSV's columns. Do not build an API or a screen yet. When you are done, show me the row count so I can check it matches the CSV.

## 3. Python API

> Backend only. Build a small Python API on top of the SQLite table. I need three endpoints: one that returns all rows, one that updates a single row by `id`, and one that returns summary numbers for a chart (total minutes per activity). No login, no delete. Explain your plan first, then build it, then show me how to test each endpoint.

## 4. React screen

> Frontend only. Build one React page that follows `design.md`. Use its buttons and cards. Show a chart from the summary endpoint and a table of all rows from the read endpoint, with an edit action on each row that calls the update endpoint. After a save, refresh the chart. Show empty, loading, saved and error states. Keep only what this task needs, and list anything you left out.

## 5. One small change

> Make one small change only: [add one field / add one more chart]. Tell me which layers it touches before you change anything.
