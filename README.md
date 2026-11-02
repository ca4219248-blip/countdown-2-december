# Countdown to 2 December

A single-file, dependency-free countdown website that ticks down to **2 December 2026, 12:00 AM IST** (UTC+05:30).

Live site: https://ca4219248-blip.github.io/countdown-2-december/

## What it does

- Live days / hours / minutes / seconds remaining, updated every second
- A progress bar showing how much of the wait is already over (measured from 2 November 2026)
- Total seconds remaining, formatted in the Indian numbering system
- Switches to an "It's here" state once the target moment passes
- Fully responsive, dark themed, respects `prefers-reduced-motion`

## Change the target date

Open `index.html` and edit these two lines near the bottom:

```js
const TARGET = new Date("2026-12-02T00:00:00+05:30").getTime();
const START  = new Date("2026-11-02T00:00:00+05:30").getTime();
```

`TARGET` is the moment the countdown reaches zero. `START` is only used for the progress bar.

## Hosting

Served with GitHub Pages from the `main` branch, root folder. Push a change to `index.html` and the site rebuilds automatically in a minute or so.
