# TODO

This document tracks planned work for modernizing and maintaining the blog.

## Stage 1 — Core updates (Completed)
- [x] Set canonical `url` and keep `baseurl` in `_config.yml`.
- [x] Add `timezone` to `_config.yml`.
- [x] Add SEO and sitemap plugins (`jekyll-seo-tag`, `jekyll-sitemap`).
- [x] Migrate Google Analytics to GA4 (config-driven via `site.ga4_measurement_id`).
- [x] Parameterize Disqus shortname; remove global count script.
- [x] Fix manifest path in `<head>` and icon paths in `site.webmanifest`.
- [x] Improve accessibility on `index.html` (use `h2` for post titles).
- [x] Replace invalid Categories `<select>` with a simple link to `tagged.html`.
- [x] Bump Jekyll to `~> 4.3` and add new plugins to `Gemfile`.

## Stage 2 — Enhancements (In Progress)
- [x] Populate `ga4_measurement_id` in `_config.yml`.
- [ ] Verify Disqus shortname and comment behavior on production (`brennan-archive`).
- [ ] Add `jekyll-seo-tag` metadata: author, social links, and defaults.
- [ ] Validate sitemap output and canonical links after build.
- [ ] Consider switching to `jekyll-paginate-v2` in the future (keeping legacy for now).

## Stage 3 — UI/UX refresh (Planned)
- [ ] Update/reset CSS baseline (e.g., modern-normalize) or keep and upgrade normalize.
- [ ] Improve mobile spacing, headings hierarchy site-wide (one `<h1>` per page).
- [ ] Enhance pagination controls (bigger tap targets, clearer prev/next labels).
- [ ] Improve tags page rendering (grouped lists, smaller font on long lists).
- [ ] Optional: dark mode.

## Housekeeping
- [ ] Review README badges and update/remove outdated ones.
- [ ] Add simple CI to validate HTML and check broken links.
- [ ] Add `.editorconfig` and Prettier/Stylelint (optional) for consistency.
