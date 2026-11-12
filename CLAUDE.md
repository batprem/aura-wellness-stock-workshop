# CLAUDE.md — Aura Wellness stock workshop

Starter context for this project. Keep this file current as you build. Rules here apply to every prompt, so you do not have to repeat them.

This file is a starting draft for the classroom. Adapt it. It is not a finished product document, and it is not real Aura policy.

## What we are building

A mini ERP for stock checking, in this folder, with exactly three features:

1. User login — only signed-in users reach the stock screens.
2. Read stock tables — a clear, read-only table from the database.
3. Red label for almost-empty items — “Low stock” in red plus those words, not color alone.

Do not add features that are not in this brief. If something extra is suggested, park it for a later build.

## The almost-empty rule

If an item’s quantity is at or below **\[threshold\]**, show a “Low stock” label in red, with the words.

The team agrees \[threshold\]. Write the agreed number in place of \[threshold\] in this file before Feature 3. Do not invent a number.

## Structure

Keep frontend, backend and database separate:

- Frontend: login screen, stock table view, red label.
- Backend: checks the login, serves stock data through an API, applies the \[threshold\] rule.
- Database: users, stock items.

## Data

Use the example files in `data/`, or other example rows. **Not real Aura data.** Classroom login details in `data/example-users.csv` are for this exercise only.

## Builds and changelog

After each feature passes its checkpoint: record a build, and add one line at the top of `CHANGELOG.md` in plain words.
