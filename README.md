# Mewgi Website

Static site for Mewgi — mobile game development studio.

## What's in here

- `index.html` — the homepage
- `games.html` — the games list page (linked from "View All Games" and the nav)
- both are self-contained: HTML, CSS, and JS in one file each, images embedded

## Preview it locally

From inside this folder, run:

```
python3 -m http.server 8000
```

Then open `http://localhost:8000` in your browser. Refresh the page anytime you save a change.

(No Python? `npx serve` works too, once Node is installed.)

## Making changes with Claude Code

Open this folder in VS Code (`File > Open Folder`), then run `claude` in the built-in terminal. Ask it for changes in plain English — it edits `index.html` directly. Refresh your browser to see the result.

## Publishing changes to GitHub

First time only:
```
git init
git add .
git commit -m "first version"
git branch -M main
git remote add origin <your-github-repo-url>
git push -u origin main
```

Every time after that:
```
git add .
git commit -m "describe what changed"
git push
```

If this repo is connected to Cloudflare Pages, every push deploys automatically — no extra steps.

## Deploying

Connected via **Cloudflare Pages** (Git integration). Build command: none (leave blank — this is a plain static site). Output directory: `/` (project root).

Custom domain is configured under the Pages project's **Custom Domains** tab.
