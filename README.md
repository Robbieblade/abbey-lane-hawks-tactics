# Abbey Lane Hawks — Playbook

A four-page site for the Hawks (U13, 9-a-side, 2-5-1). Players land on the home page, pick their position, and find every restart in one place.

## Pages

```
index.html         Home — the formation, your position card, team rules
goal-kicks.html    Building from our goal kicks + pressing theirs
corners.html       Attacking Routine 1 + defending corners
throw-ins.html     Four throw-in options
assets/            badges + the six pitch diagrams (SVG)
.nojekyll          serve files as-is on GitHub Pages
```

Shared header and tab navigation across all pages, so players can move between topics from anywhere. No build step, no dependencies — open any page in a browser, or publish the whole folder via GitHub Pages.

## Publishing

See `DEPLOY.md` for a Claude Code prompt that pushes this to GitHub and turns on Pages. The site goes live at `https://<your-username>.github.io/<repo-name>/`.

## Editing

Each page is standalone HTML with the shared CSS inline. The diagrams live in `assets/` as SVG — swap the file to change a diagram, no code change needed. Team colours are the CSS variables at the top of each page's `<style>` block (`--gold`, `--ink`, `--panel`).
