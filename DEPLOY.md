# Publishing with Claude Code

Download the `hawks-site` folder, open Claude Code **in that folder**, and paste one of the prompts below. You'll need the GitHub CLI (`gh`) authenticated — the same setup you use for the Nova sites. Check with `gh auth status`.

---

## Option A — brand-new repo (recommended)

> I'm in a folder called `hawks-site` containing four HTML pages (`index.html`, `goal-kicks.html`, `corners.html`, `throw-ins.html`), an `assets/` folder with badge images and SVG diagrams, a `README.md` and `.nojekyll`. It's a static multi-page site, no build step.
>
> Please:
> 1. Initialise a git repo and commit everything on `main` with the message "Hawks playbook site".
> 2. Create a new **public** GitHub repo called `hawks-playbook` and push to it.
> 3. Enable GitHub Pages on the `main` branch, root folder.
> 4. Give me the live URL and confirm all four pages load, the tab navigation works between them, and the badges and diagrams appear.

---

## Option B — into an existing repo as a subfolder

> I have an existing GitHub Pages repo at `<path-to-repo>`. Add this Hawks site as a subfolder called `hawks` (or a name I'll give you).
>
> Please:
> 1. Copy all four HTML pages and the `assets/` folder into that subfolder inside the repo.
> 2. Commit with "Add Hawks playbook site" and push to `main`.
> 3. Give me the live URL (existing Pages URL + `/hawks/`).

---

## After it's live

Push any change to update the site. To edit later, open the repo in Claude Code and describe the change — for example "swap the CMs and CBs on the defending-corners diagram", "add a second corner routine to corners.html", or "add a fifth page for free kicks".

The home page links to the other three, and every page's top tabs link to all four, so players only need the one URL.
