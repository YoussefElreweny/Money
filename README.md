# Salary

A simple, private monthly salary planner and expense tracker. One static page, no build
step, no backend — install it on your phone's home screen and it works offline.

## Deploy

Import this repo in Vercel (framework preset: **Other**, no build command, output = repo
root). Then open the URL in Safari → Share → **Add to Home Screen**.

## What it does

- **Plan**: categories (Essentials, Lifestyle, Personal Growth, Low-risk and Long-term
  investments by default) with line items. Fully editable from the sliders icon — rename,
  add or remove categories and lines, change colours, mark each as *Spending* or *Saving*.
- **Add expense**: amount, category, line, optional note and date. It comes off that line
  and its category; the home screen shows what's left this month.
- **Income**: tap the big number. *Every month* sources keep a history (a raise applies
  from that month on, earlier months keep their amounts); *Just this month* holds one-offs
  like a bonus. A note shows when income and plan don't match.
- **Week**: Sunday–Saturday spending by day and by category, against a steady pace (the
  monthly budget spread evenly over the days).
- **Hide amounts**: the eye icon at the top hides every figure on the main screen (the
  big number turns to dots, the rest blurs). It's remembered, so the app opens hidden
  until you tap the eye again.
- Each month starts fresh; arrows step back through earlier months and weeks.

## Data

Stored in the browser's `localStorage` under `salary.v1`, on that device only. Use
**Download a backup** / **Restore from a backup** in the plan sheet to move or keep it.

## Files

```
index.html            the whole app (HTML, CSS, JS)
manifest.webmanifest  home-screen install metadata
sw.js                 offline cache (network-first)
*.png                 icons
```
