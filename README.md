# Dr. Panneerselvam Ramaswamy — Portfolio

A corporate, navy-and-gold one-page portfolio for **Dr. Panneerselvam Ramaswamy** —
Principal Director & General Manager (Retd.), MSME Technology Centre · Indo-German
Tool Room. Built from the "Portfolio — B Corporate" design exported from
[Claude Design](https://claude.ai/design).

## What's here

| File | Purpose |
| --- | --- |
| `index.html` | The portfolio page — sticky nav, hero, stats, about, expertise, experience, education, and contact sections. All styling is inline. |
| `data.js` | All page content (`window.PORTFOLIO`): role, tagline, stats, experience, education, contact. Edit here to update copy. |
| `assets/portrait.webp` | Hero portrait. |
| `.github/workflows/deploy.yml` | GitHub Actions workflow that publishes the site to GitHub Pages. |

## Run locally

It's a static site — open `index.html` directly, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy

Pushing to `main` (or the development branch) runs the **Deploy portfolio to
GitHub Pages** workflow, which publishes the repository root as a static site.

To enable it once: in the repository's **Settings → Pages**, set the source to
**GitHub Actions**. After the next push the site is served at
`https://<owner>.github.io/<repo>/`.

## Design provenance

The design direction (from the handoff chat): *corporate & polished, one elegant
long-scroll page, deep navy & gold.* The prototype's interactive `<image-slot>`
component was replaced with a plain `<img>` for a self-contained, deployable build.
