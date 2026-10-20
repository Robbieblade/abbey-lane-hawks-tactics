# Abbey Lane Hawks — Playbook

A multi-page site for the Hawks (U13, 9-a-side, 2-5-1). Players land on the home page, pick their position, and find every restart in one place.

## Pages

```
index.html         Home — the formation, your position card, team rules
goal-kicks.html    Building from our goal kicks + pressing theirs
corners.html       Attacking Routine 1 + defending corners
throw-ins.html     Four throw-in options
play-forward.html  Ten attacking principles with clips
goalkeeping.html   Josh’s page — one principle added per session
assets/            badges + the six pitch diagrams (SVG)
.nojekyll          serve files as-is on GitHub Pages
```

Shared header and tab navigation across all pages, so players can move between topics from anywhere. No build step, no dependencies — open any page in a browser, or publish the whole folder via GitHub Pages.

## Tactics sessions

`play-forward.html` holds the ten attacking principles from the 20 Oct 2026 session, each with its clip from `assets/clips/`. `goalkeeping.html` is Josh's page and grows by one principle per session.

To add a new session:

1. Put the clips in `assets/clips/` as `name.mp4`, with a poster frame `name.jpg` (360px wide).
2. New theme? Copy `play-forward.html` as the starting point for a new page and add a tab for it to the nav on every page. Same theme? Add `<article class="pcard">` blocks to the existing page.
3. Goalkeeper bit: copy the `<article>` block on `goalkeeping.html` to the top of the list (instructions are in the HTML comment there) and add a row to its session log.
4. Add a row to the session log at the bottom of each page you changed.

## Publishing

See `DEPLOY.md` for a Claude Code prompt that pushes this to GitHub and turns on Pages. The site goes live at `https://<your-username>.github.io/<repo-name>/`.

## Editing

Each page is standalone HTML with the shared CSS inline. The diagrams live in `assets/` as SVG — swap the file to change a diagram, no code change needed. Team colours are the CSS variables at the top of each page's `<style>` block (`--gold`, `--ink`, `--panel`).
