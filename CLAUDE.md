# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Repository Is

A GitHub Pages personal profile site hosted at `hangaoyang.dev`. It uses the **jekyll-theme-cayman** theme and is deployed automatically by GitHub Pages on every push to `main` — there is no build or deploy command to run locally.

## Structure

- `index.md` — the sole page; rendered as the site homepage
- `README.md` — GitHub profile README (shown on github.com/coldhighsun, **separate** from `index.md`)
- `_config.yml` — Jekyll site config (theme, title, description, lang)
- `_includes/head-custom.html` — injects Google Analytics (gtag) and Google AdSense into every page's `<head>`
- `CNAME` — custom domain record (`hangaoyang.dev`)

## Key Points

- `index.md` and `README.md` are **independent files** with overlapping content but different audiences and different project orderings. Changes to one do not automatically apply to the other.
- There are no local build steps, tests, or linting tools. All rendering is handled by GitHub Pages.
- To preview locally, install Jekyll and run `bundle exec jekyll serve`, though this is rarely necessary given the site's simplicity.
- The only JavaScript in the repo lives in `_includes/head-custom.html` (analytics/ads snippets).
