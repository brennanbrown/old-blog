# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased]
### Fixed
- Unified branding across `license.md` and `about.markdown` (previously stale "Notebook de Casa" / `brenblog.netlify.app` references) to "Brennan's Old Blog" / `brennan-archive.netlify.app`.
- Replaced dead `wandernotebook.com` links in `README.md` and `about.markdown` with Wayback Machine archive links; replaced the hotlinked (and now-broken) author photo in `author.markdown` with the local `/img/avatar.png`.
- Fixed mismatched Twitter handle in `_includes/sidebar.html` and removed unused `twitter_username`/`twitter` SEO fields from `_config.yml`; replaced Twitter links site-wide with Mastodon (`social.lol/@brennan`).
- Rewrote the sidebar bio to remove stale age/location details, framing the site as a personal archive, and added a link to the current site, [brennan.day](https://brennan.day).
- Fixed invalid `<em>`/`<q>` tag nesting in `_includes/header.html`.
- Populated empty `name`/`short_name` fields in `site.webmanifest`.
- Removed unused `badgerbadgerbadger` gem from `Gemfile`.

### Changed
- Replaced `css/main.css` with a minimal, brutalist stylesheet: no decorative borders/dividers, no monospace type, no centered/justified text, no list or paragraph indentation, system fonts only (dropped the Google Fonts and normalize.css dependencies).
- Enforced accessible link styling everywhere: always underlined, a clearly different hover color, and a distinct visited-link color.
- Header, footer, and nav remain centered (`.full-width`).
- Sidebar avatar is now square (not circular), greyscale, and floated left with body text wrapping around it.
- Replaced the Substack newsletter embed with a Buttondown form (matching brennan.day).
- Fixed a Liquid quirk on the homepage where whitespace-only `{% unless %}` blocks were silently dropped, causing post tags to render with no space between them.
- Added spacing between the sidebar and pagination when stacked on mobile.

### Removed
- Disqus commenting system entirely (`_includes/disqus.html`, `disqus_shortname`, and its use in `post.html`).
- Google Analytics (GA4) entirely (`_includes/google_analytics.html`, `ga4_measurement_id`, and its use in `default.html`) — the site now ships with no analytics/tracking scripts.

### Added
- Re-imported all posts from a newer, better-formatted export tool (`_posts/new-better-import/`), replacing the 76 posts it had improved matches for and adding 69 new posts (2015-2024) that weren't previously on this site, expanding the archive's range from 2015-2021 to 2015-2024.
- Merged in Jekyll-required metadata (`permalink`, `categories`, `tags`) from the old versions of replaced posts so historical URLs are preserved; new tags were additionally derived from `_data/lists/*.json` (Medium reading lists) matched by `medium_id`.
- Wired the new import's `subtitle`, `image`/`image_caption`, and `canonical_url` fields into `_layouts/post.html`: a subtitle line under the title, a hero image with caption, and an "Originally published on Medium" attribution link.

### Changed
- Updated the "2015-2021 archive" framing in `README.md`, `about.markdown`, and `_includes/sidebar.html` to "2015-2024" to reflect the expanded post range.
- Added `height: auto` to the global `img` rule so images with explicit HTML `width`/`height` attributes still scale proportionally under `max-width: 100%`, regardless of where they're embedded.
- Applied the sidebar's avatar treatment (square, greyscale, floated left) to the photo on `author.markdown`; made the `.avatar` CSS rule global instead of sidebar-only.
- Converted 9 in-post `![image](url)` + plain-text-caption pairs (across 6 posts) into proper `<figure>`/`<figcaption markdown="span">` blocks, using a conservative pattern match to avoid mislabeling body prose or headings as captions; added matching CSS for `.post-figure`/`figcaption` and `.post-subtitle-full`/`.post-origin`.
- Switched from `jekyll-paginate` to `jekyll-paginate-v2` so the homepage feed can be sorted independently of `site.posts`; the homepage now lists posts chronologically (oldest first, starting from the 2015 post) via `sort_reverse: false`, while the RSS feed and tags page remain newest-first/unaffected.

### Planned
- Improve tags page rendering and site-wide heading hierarchy.
- Audit in-post links/images (imgur, YouTube, Tumblr, old WordPress `wp-content` embeds) for dead links.

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
