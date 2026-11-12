# Product brief — mini ERP for stock checking

This is the whole brief, taken word for word from the Aura Wellness curriculum. Treat it as the boundary of today’s work.

> Create mini ERP for stock checking.
>
> Features: (1) User login (2) Read stock tables (3) Red label for almost empty items.

## What “mini ERP” means here

- **ERP:** a system a business uses to run its operations — stock is one part of it.
- **Mini:** one slice only: checking stock. Three features, nothing more.
- **Not today:** anything outside the three features — note it for a later build.

## Feature goals

1. **User login.** Only signed-in users reach the stock screens. A user signs in; the app checks who they are and lets them in — or says no.
2. **Read stock tables.** Signed-in users can see what is in stock. Read only: the table comes from the database and is easy to scan.
3. **Red label for almost-empty items.** Items that are almost empty stand out, so nobody misses them. The team decides what “almost empty” means: the \[threshold\]. If quantity is at or below that threshold, show a “Low stock” label in red, with the words, not color alone.

## Example data

Sample stock and users are in [`data/`](data/). They are **examples, not real Aura data.**
