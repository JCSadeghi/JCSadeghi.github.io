# JCSadeghi.github.io

Personal academic website for Jonathan Sadeghi, built with [al-folio](https://github.com/alshedivat/al-folio) and deployed to GitHub Pages by GitHub Actions.

## Local development

The deployment workflow uses Ruby 3.3.5, Node.js 20, Python 3.13, and ImageMagick. After installing those dependencies:

```bash
bundle install
npm ci
bundle exec jekyll serve
```

The site is available at <http://localhost:4000>.

## Deployment

Pushing site changes to `master` or `main` runs `.github/workflows/deploy.yml`. The workflow builds the site and publishes `_site` to the `gh-pages` branch. In the repository's GitHub Pages settings, the publishing source should be the `gh-pages` branch.

## Upstream

This site was ported to the al-folio v1 plugin architecture from upstream commit `9b55c63` (2026-08-31). Theme behavior is supplied by pinned `al_*` gems in `Gemfile`; site-specific content stays in this repository.
