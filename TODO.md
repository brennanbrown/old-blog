# TODO

This document tracks planned work for modernizing and maintaining the blog.

## Stage 1 — Core updates (Completed)
- [x] Set canonical `url` and keep `baseurl` in `_config.yml`.
- [x] Add `timezone` to `_config.yml`.
- [x] Add SEO and sitemap plugins (`jekyll-seo-tag`, `jekyll-sitemap`).
- [x] Migrate Google Analytics to GA4 (config-driven via `site.ga4_measurement_id`). *(superseded — GA removed entirely, see Stage 3)*
- [x] Parameterize Disqus shortname; remove global count script.
- [x] Fix manifest path in `<head>` and icon paths in `site.webmanifest`.
- [x] Improve accessibility on `index.html` (use `h2` for post titles).
- [x] Replace invalid Categories `<select>` with a simple link to `tagged.html`.
- [x] Bump Jekyll to `~> 4.3` and add new plugins to `Gemfile`.

## Stage 2 — Enhancements (In Progress)
- [x] Populate `ga4_measurement_id` in `_config.yml`. *(superseded — GA removed entirely, see Stage 3)*
- [x] Add `jekyll-seo-tag` metadata: author, social links, and defaults.
- [ ] Validate sitemap output and canonical links after build.
- [ ] Consider switching to `jekyll-paginate-v2` in the future (keeping legacy for now).

## Stage 2.5 — Content audit (Completed)
- [x] Unify branding (site name/domain) across `README.md`, `about.markdown`, `license.md`.
- [x] Replace dead `wandernotebook.com` links/images with Wayback Machine links / local assets.
- [x] Fix mismatched Twitter handle; migrate social links to Mastodon.
- [x] Remove stale bio details from sidebar; link to current site (brennan.day).
- [x] Fix invalid HTML nesting in `header.html`.
- [x] Fill in `site.webmanifest` name fields.
- [x] Remove unused `badgerbadgerbadger` gem.

## Stage 3 — UI/UX refresh (Completed)
- [x] Replace CSS with a minimal brutalist stylesheet (no borders/dividers, no monospace, no centered/justified text, no list/paragraph indentation).
- [x] Enforce accessible link styling: always underlined, distinct hover color, distinct visited color.
- [x] Remove Disqus commenting system (`_includes/disqus.html`, `disqus_shortname`, and its use in `post.html`).
- [x] Replace Substack newsletter embed with Buttondown form (matching brennan.day).
- [x] Remove Google Analytics (GA4) entirely — no tracking scripts (`_includes/google_analytics.html`, `ga4_measurement_id`, and its use in `default.html`).
- [ ] Enhance pagination controls (bigger tap targets, clearer prev/next labels).
- [ ] Improve tags page rendering for long lists.

## Housekeeping
- [ ] Review README badges and update/remove outdated ones.
- [ ] Add simple CI to validate HTML and check broken links.
- [ ] Add `.editorconfig` and Prettier/Stylelint (optional) for consistency.
- [ ] Audit individual posts (2015-2021) for dead links/images to imgur, YouTube, Tumblr, and old WordPress `wp-content` uploads.
