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
  Open it from **Edit plan** next to the Categories heading. A pill under the total turns
  green while some income is still unplanned and red when the plan is more than your income.
- **Add expense**: amount, category, line, optional note and date. It comes off that line
  and its category; the home screen shows what's left this month.
- **Income**: tap the “of … EGP income” line under the big number. *Every month* sources keep a history (a raise applies
  from that month on, earlier months keep their amounts); *Just this month* holds one-offs
  like a bonus. A note shows when income and plan don't match.
- **Week**: Sunday–Saturday spending by day and by category, against a steady pace (the
  monthly budget spread evenly over the days).
- **Hide income**: tap the big number to turn the big number and the income line into
  dots; spending and savings stay visible. It's remembered, so the app opens hidden until
  you tap it again.
- **Colours**: a spending category, or the Spent total, turns red as soon as it passes
  its plan (e.g. 5,800 / 5,500). Once a month is over, the ones that stayed inside turn
  green. Saving categories stay neutral.
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
