# Example design system — `design.md`

> EXAMPLE — NOT REAL AURA DATA. This is a practice `design.md` for the Module 3 UX/UI lesson. It is not Aura Wellness’s real product design. Teams may replace these tokens with their own.

A design system written as a file Claude can read. When you prompt for a screen, point at this file so every screen reuses the same tokens, components, and rules — nobody re-decides the basics in each prompt.

## Tokens

These hex values are examples for practice, not official Aura brand colors.

| Token | Example hex | Use |
|---|---|---|
| paper | `#F6F4EE` | page background |
| ink | `#1E3833` | body text |
| ink-muted | `#55655F` | secondary text |
| accent | `#2C6E61` | links, focus, primary actions |
| card | `#FCFBF8` | card fill; border `#D9DFDA` |
| alert | `#B3261E` (fill `#F8E1DE`) | almost-empty red label only |

- Headings: a clear sans-serif, larger and bolder than body text.
- Body: a readable sans-serif.
- Do not invent new colors in a prompt. If something is missing, ask first.

## Components

- **Buttons:** one primary action per screen (accent fill, light text). Secondary actions are quieter — outline or text only.
- **Cards:** rounded container, light fill, clear title, short body. Use for a group of related content.
- **Forms:** labels in the user’s words, above the field. Show a validation message next to the field that needs it.
- **Tables:** one header row; numeric quantities aligned for scanning. Almost-empty rows use the alert component, not a new color.
- **Red label (almost empty):** alert color, on items at or below [threshold]. The number is a team decision — do not invent it.

## Rules

- One main action per screen.
- Clear labels in the user’s words.
- Show what happened: empty, loading, saved, and error states.
- Reuse these tokens and components. Do not add a new pattern when an existing one works.
- Keep only what this task needs.

## How to point Claude at this file

In a UI prompt, name the file and ask Claude to follow it, for example:

> Follow `design.md`. Use its buttons and cards. Show empty, loading, and error states.
