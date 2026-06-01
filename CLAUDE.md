# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

A single-page, print-optimized CV. No build step, no framework — just `index.html` + `style.css`. Deployed to GitHub Pages at `cv.franco.international`.

## Development

Open `index.html` directly in a browser. No server, no compilation required.

## Design Conventions

- Inter font loaded from rsms.me CDN (same CDN as `franco.international`)
- Accent color `#0066cc` for section labels and links
- Planned/upcoming entries use grey text with an inline `.planned-tag` badge
- `break-inside: avoid` on `.entry` prevents mid-entry page breaks when printing
- Print button hidden via `@media print`; margins collapse to clean PDF margins

## Deployment

Push to `main` → GitHub Actions deploys to GitHub Pages. No CI checks beyond the deploy itself.
