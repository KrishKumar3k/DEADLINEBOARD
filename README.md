# DEADLINEBOARD

A lightweight, self-contained deadline tracker that runs entirely in your browser. Add every program you register for — competitions, scholarships, grants, internships, conference CFPs — and the board keeps track of what's due, when, and how urgent it is.

## Features

- **List view** — every deadline sorted by how much time is left, with color-coded urgency bands:
  - 🔴 urgent (≤ 3 days)
  - 🟠 soon (≤ 7 days)
  - 🔵 upcoming (≤ 30 days)
  - 🟢 safe (30+ days)
  - ⚪ overdue / done
- **Calendar view** — a month grid with every deadline dropped on its date, color-coded the same way. Navigate between months or jump back to today, and click any event to edit it.
- **Hero strip** — the next deadline, with a live countdown.
- **Quick capture** — a "Paste list" bulk mode: dump `Name, YYYY-MM-DD` lines and import them all at once.
- **Stats** — due this week, due this month, and how many you've completed.
- **Filters** — Active / Overdue / Done, plus a per-category filter.
- **Persistent** — everything is saved to `localStorage`, so it survives refreshes and browser restarts.
- **Keyboard & touch friendly** — proper focus states, aria labels, and reduced-motion support.

## Usage

1. Open `index.html` in any modern browser (or host it on GitHub Pages — see below).
2. Click **+ Add program** and enter a name, deadline, category, and optional link/notes.
3. Or click **Paste list** to import several programs at once. Format: `Name, YYYY-MM-DD` — category is optional and comes third.

Your data stays in your browser; nothing ever leaves your machine.

## Hosting with GitHub Pages

This repo is a single static file, so it's ready for GitHub Pages:

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Source**, select `Deploy from a branch`, choose `main`, folder `/ (root)`, and save.
4. Your board is live at `https://<username>.github.io/DEADLINEBOARD/`.

## Local development

No build step, no dependencies, no package manager required.

```bash
git clone https://github.com/KrishKumar3k/DEADLINEBOARD.git
cd DEADLINEBOARD
start index.html   # or just double-click it
```

## Project structure

```
DEADLINEBOARD/
├── index.html     # the entire app — styles, markup, and logic
└── README.md
```

## License

MIT