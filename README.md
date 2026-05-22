# amarine9331.github.io

Personal academic site for **David A. Marinelarena**, built with [Quarto](https://quarto.org) and deployed to GitHub Pages.

Live: https://amarine9331.github.io

## Stack

- Quarto (1.9+) website project, theme layered over Cosmo (Bootstrap)
- Custom SCSS for a shadcn-style brutalist-minimal look with light + dark modes (dark default)
- GitHub Pages serving from `master` `/docs`

## Local development

```sh
# preview with live reload
quarto preview

# one-shot render into docs/
quarto render
```

## Project layout

```
.
├── _quarto.yml                 site config (navbar, footer, theme)
├── _includes/default-dark.html font loader + dark-mode default
├── theme/                      SCSS — fonts.scss, light.scss, dark.scss, components.scss
├── index.qmd                   Home (hero, bio, focus tags, timeline, recent projects)
├── projects/                   project portfolio (grid listing)
│   ├── index.qmd
│   ├── skidle/index.qmd
│   ├── tcga/index.qmd
│   └── rnaseq/index.qmd
├── publications/index.qmd      empty listing scaffold
├── talks/index.qmd             empty listing scaffold
├── teaching/index.qmd          empty listing scaffold
├── blog/index.qmd              empty listing scaffold
├── assets/img/                 hero image + favicon
├── files/                      CV PDF
└── docs/                       build output, committed for GitHub Pages
```

## Adding content

- **A new project**: create `projects/<slug>/index.qmd` with `title`, `subtitle`, `date`, `categories`, `image:` front-matter, drop the cover image into the same folder, and `quarto render`.
- **A publication / talk / teaching entry**: create `<section>/<slug>/index.qmd` with `title`, `date`, `categories`, optional `description`. The listing on the section's `index.qmd` picks it up automatically.
- **A blog post**: create `blog/<slug>/index.qmd` with `title`, `date`, `categories`, optional `image`.

## Deployment

1. `quarto render` — writes the static site to `docs/`.
2. Commit and push (`master` branch).
3. GitHub Pages → Source: `Deploy from a branch` → `master` `/docs` (one-time setup at https://github.com/Amarine9331/Amarine9331.github.io/settings/pages).

## License

MIT — see [LICENSE](LICENSE).
