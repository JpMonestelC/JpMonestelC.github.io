# JpMonestelC.github.io

Personal portfolio site for **Jose Pablo Monestel Cruz** — Software Developer / Data Analyst, Guanacaste, Costa Rica.

Live at: **https://jpmonestelc.github.io**

## What this is

A single static page (`index.html`, no build step, no framework, no dependencies besides Google Fonts) that links out to the real, audited projects in my other repositories:

- [`retail-inventory-system`](https://github.com/JpMonestelC/retail-inventory-system) — C# / .NET 9 / ASP.NET Core / Blazor WASM / SQL Server
- [`task-manager-flask`](https://github.com/JpMonestelC/task-manager-flask) — Python / Flask / SQLAlchemy / Playwright
- [`dragon-inscriptor`](https://github.com/JpMonestelC/dragon-inscriptor) — Python / PLY (lexer + LALR parser) / Tkinter
- [`world-of-invenio`](https://github.com/JpMonestelC/world-of-invenio) — Java 17 / Swing / Maven
- `AdoPaws (BD)` — SQL Server, in preparation

Every project entry lists real bugs found and how they were verified (recompiles, HTTP test suites, headless GUI automation, Playwright/Chromium runs) instead of just a feature list — see each repo's own README for the full write-up.

## Why a plain static site

This repo exists so the portfolio has a stable, professional URL to put on a CV/resume (`https://jpmonestelc.github.io`) instead of a link to a third-party tool. It's served directly by **GitHub Pages** from this repo's `main` branch — no build pipeline, so any push to `main` goes live within a minute or two.

## How to update it (add a new project, fix a typo, etc.)

1. Edit `index.html` directly — it's plain HTML/CSS, one file, no build step.
2. To add a new project card, copy one `<article class="project">…</article>` block under `.projects-list` and fill in the name, tags, description, stats, and GitHub link. To move a project from "in preparation" to published, swap `<span class="status prep">In preparation</span>` for `<span class="status ok">Verified</span>` and add the GitHub link.
3. Commit and push to `main`:
   ```
   git add .
   git commit -m "update: <what changed>"
   git push
   ```
4. GitHub Pages rebuilds automatically — check **Settings → Pages** in this repo if it ever needs re-enabling (Source: Deploy from a branch, Branch: `main`, folder: `/root`).

## License

Code in this repo (`index.html`) is MIT-licensed — see [LICENSE](LICENSE). This doesn't cover the content of the linked project repositories, which each carry their own license.
