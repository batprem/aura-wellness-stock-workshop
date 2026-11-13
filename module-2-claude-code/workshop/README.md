# Module 2 workshop — a personal finance report app

Solo, in Claude Code. Time: [__] minutes.

You build one page that turns a list of transactions into a personal finance report. It runs in the browser with **no server, no login and no database**, and you don't add or edit transactions (that comes in Module 3).

**Data:** [`../data/example-transactions.csv`](../data/example-transactions.csv) — example data, about three months. Columns: `date`, `description`, `category`, `amount`, `type` (`in` or `out`).

> Use the example file in class, not your own bank data.

## Core features

1. **Summary cards:** money in, money out, what's left, savings rate.
2. **Spending by category** chart.
3. **Month-by-month trend** of money in vs money out.
4. **Top 5 biggest expenses.**
5. A **month picker** that updates everything.
6. A **transactions table**, sortable, with search.

## Stretch — pick one as your own change

- Category budgets with an over-limit warning.
- Change vs last month.
- Recurring payments.
- Upload your own CSV with the same columns.
- Print or save as PDF.

## Steps

Copy-paste prompts are in [PROMPTS.md](PROMPTS.md). One step per prompt; check each before the next.

1. Make a new folder, put `example-transactions.csv` in it, and open it in Claude Code.
2. Ask Claude to describe the data.
3. Ask for a plan for the page. Read it before you say yes.
4. Build the totals: the four summary cards.
5. Add the category chart, the trend chart, the top 5 and the table.
6. Add the month picker, then make one change of your own from the stretch list.

## Done when

- The page opens in your browser straight from the folder.
- For one month you checked by hand, money in, money out and what's left match the file.
- The chart and the table show the same numbers as the data.
- Picking another month changes every part of the page.
- You can point at each part and say where its numbers come from.

## Reference app

[`reference-app/index.html`](reference-app/index.html) is one way the core features can look, built from the example data and following [`design.md`](../../module-3-software-essentials/examples/design.md). Open it in a browser to compare after you build yours, not before. Screenshot: [`reference-app/screenshot.png`](reference-app/screenshot.png).

## Links

- Module 2 reference: [../README.md](../README.md)
- Course materials: [github.com/batprem/aura-wellness-stock-workshop](https://github.com/batprem/aura-wellness-stock-workshop)
