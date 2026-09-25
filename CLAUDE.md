# skyphusion

Conrad Rockenhaus's GitHub profile README, rendered as a static site. This is a content /
marketing repo, not application code.

## What it is

- `README.md` is the whole page. GitHub Pages runs it through the `github-pages` gem
  (`jekyll-theme-minimal`), which renders the README as `index.html` by default; there is no
  separate template.
- Custom domain via `CNAME` (`github.skyphusion.net`, DNS CNAME to `skyphusion.github.io`).
  `_config.yml` sets the Jekyll site metadata (title, description, social links, SEO tag,
  sitemap) that feeds the rendered `<head>` and `og:` tags.
- Deploy: `.github/workflows/pages.yml`, GitHub-hosted `ubuntu-latest`, three jobs (build with
  `actions/jekyll-build-pages`, deploy via `actions/deploy-pages`, then a `purge-cache` job that
  hits the Cloudflare API to purge the edge cache for `github.skyphusion.net` using the
  `CLOUDFLARE_PURGE_TOKEN` repo secret). Push to `main` triggers it; no PR preview build.

## Maintenance note

The README is a live project index (Vivijure constellation, Postern, Prism estate, and more),
each entry linking to its `skyphusion-labs` repo. When a linked project's name, URL, or
version train changes, update the corresponding line here; a stale link or a renamed repo
404s from a page people actually land on.
