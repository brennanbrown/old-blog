# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased]
- Add GA4 Measurement ID to `_config.yml`.
- Verify Disqus shortname and behavior on production.
- Improve tags page rendering and site-wide heading hierarchy.
- Consider updating/resetting CSS baseline and adding dark mode.

## [2025-09-13] Modernization pass
### Added
- `jekyll-seo-tag` and `jekyll-sitemap` to plugins and templates.
- `TODO.md` and `CHANGELOG.md` for tracking work.

### Changed
- Set `_config.yml:url` to `https://brennan-archive.netlify.app`, added `timezone`, and added `ga4_measurement_id` and `disqus_shortname`.
- Populated GA4 Measurement ID with `G-49BH4DQMC2` and added SEO metadata (author/social) for `jekyll-seo-tag`.
- Migrated Google Analytics to GA4 via `_includes/google_analytics.html` (config-driven).
- Updated `_includes/head.html` to include `{% seo %}` and corrected manifest path.
- Fixed `site.webmanifest` icon paths to `fav/` directory.
- Updated `Gemfile` to Jekyll `~> 4.3` and added SEO/Sitemap plugins.
- Improved `index.html` accessibility (post titles now `h2`) and replaced invalid categories `<select>` with a link to `/tagged`.
- Removed global Disqus count script from `_layouts/default.html`; comments load only on posts via `_includes/disqus.html`.
- Overhauled CSS in `css/main.css` with modern variables, grid/flex layout, responsive spacing, accessible colors, and optional dark mode while keeping class names stable.

### Deprecated
- Universal Analytics `UA-*` snippet.

### Security
- None.
