# mariano-fernandez.github.io

Personal site built with [Hugo](https://gohugo.io/) and the [hugo-coder](https://github.com/luizdepra/hugo-coder) theme.

## Prerequisites

- [Hugo Extended](https://gohugo.io/installation/) (v0.147.4+)

## Run locally

```bash
# Clone with submodules
git clone --recurse-submodules git@github.com:mariano-fernandez/mariano-fernandez.github.io.git
cd mariano-fernandez.github.io

# Start dev server (includes draft posts)
hugo server -D
```

Site will be available at `http://localhost:1313/`.

## Deployment

Deployment is handled automatically via GitHub Actions on push to `master`. The workflow builds the site with Hugo and deploys to GitHub Pages.

**Setup required:** In the repo settings, go to **Settings > Pages > Source** and select **GitHub Actions**.

## Structure

- `content/_index.md` — Home page
- `content/posts/` — Blog posts
- `content/about/` — About page
- `assets/css/custom.css` — Custom dark theme styles
- `static/files/` — Downloadable files (CV PDF, etc.)
- `static/images/` — Images (avatar, etc.)
