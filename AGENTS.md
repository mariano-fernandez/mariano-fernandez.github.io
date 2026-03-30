# Project Guidelines

## Overview

Personal GitHub Pages site at `mariano-fernandez.github.io`, built with [Hugo](https://gohugo.io/) and the [hugo-coder](https://github.com/luizdepra/hugo-coder) theme. Deployed via GitHub Actions on push to `master`.

## Workflow Rules

- **Never commit or push without explicit approval.** Make changes locally, then ask before committing.
- **Always work on a feature branch.** Never commit directly to `master`. Create a branch, push, and open a PR.
- **No AI attribution in commits.** Do not add `Co-Authored-By` or similar trailers.
- **Conventional Commits.** Use the [Conventional Commits](https://www.conventionalcommits.org/) format for commit messages.

## Technical Decisions

- **Theme:** hugo-coder with dark color scheme (`colorScheme = "dark"`)
- **Blog toggle:** `params.enableBlog` in `hugo.toml` controls blog visibility. When `false`, the Blog menu item is hidden and blog pages redirect to home. Implemented via layout overrides in `layouts/_partials/header.html` and `layouts/posts/`.
- **Layout overrides:** Custom partials override the theme in `layouts/` (header for blog toggle, footer removed, posts list/single for blog toggle redirect).
- **Custom CSS:** `assets/css/custom.css` — dark backgrounds (#0d1117), monospace headings, green accent on hover, navigation title lowercase override.
- **Favicon:** Circular mate icon with dark background, generated as PNG (16x16, 32x32, 180x180).

## Workplan

See [.claude/TODO.md](.claude/TODO.md) for current progress and next steps.
