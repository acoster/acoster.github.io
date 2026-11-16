# acoster.github.io

Source for [alex.coster.ch](https://alex.coster.ch), built with [Hugo](https://gohugo.io) and deployed to GitHub Pages by GitHub Actions.

## Layout

| Path | What lives there |
| --- | --- |
| `content/_index.md` | Home page text |
| `content/` | Any further pages or posts (Markdown) |
| `layouts/` | Templates (no external theme) |
| `assets/css/main.css` | Stylesheet, minified and fingerprinted at build time |
| `static/` | Files copied as-is, e.g. `tilt.html` is served at `/tilt.html` |
| `hugo.toml` | Site config, tagline and the "Elsewhere" links |

## Local development

```sh
brew install hugo
hugo server        # http://localhost:1313, live reload
hugo new content posts/my-post.md
```

## Deployment

Every push to `main` runs `.github/workflows/hugo.yml`, which builds the site and publishes it to Pages.
