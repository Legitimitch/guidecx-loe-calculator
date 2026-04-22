# GUIDEcx LOE Calculator

Branded, static, shareable LOE calculator for estimating GUIDEcx implementation and onboarding effort.

## Open locally

Open [index.html](/Users/mmitchell/Documents/Codex/2026-04-22-help-me-create-a-shareable-loe/index.html) in a browser, or serve the folder with a static host.

## Included files

- [index.html](/Users/mmitchell/Documents/Codex/2026-04-22-help-me-create-a-shareable-loe/index.html)
- [assets/guidecx-loe-brand.png](/Users/mmitchell/Documents/Codex/2026-04-22-help-me-create-a-shareable-loe/assets/guidecx-loe-brand.png)
- [netlify.toml](/Users/mmitchell/Documents/Codex/2026-04-22-help-me-create-a-shareable-loe/netlify.toml)
- [vercel.json](/Users/mmitchell/Documents/Codex/2026-04-22-help-me-create-a-shareable-loe/vercel.json)

## Core logic

- `building tasks = total tasks * hours per task`
- `template build weeks = (building tasks + process effort + team enablement + feature effort) / weekly template hours`
- `integration build weeks = building integrations / weekly integration hours`
- `overall readiness window = max(template build weeks, integration build weeks)`
- `recommended start date = target go-live date - overall readiness window`

## Share behavior

- `Copy Share Link` encodes the current estimate into the URL hash
- `Save Progress` stores the current inputs in browser local storage

## Hosting

This project is a plain static site and can be hosted on Netlify, Vercel, GitHub Pages, or any static web server.

### Netlify

- Create a new site from this folder or connect a repo
- Publish directory: `.`
- Build command: none

### Vercel

- Import the folder or repo as a project
- Framework preset: `Other`
- Build command: none
- Output directory: `.`

## Notes

The original form did not include every detailed effort assumption, so those assumptions remain visible and editable in the UI rather than being hidden in code.
