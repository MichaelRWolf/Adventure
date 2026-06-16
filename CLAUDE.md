# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Purpose

Personal adventure travel notes — destination guides, home base logistics, hike details, and local context. No code, no build system.

## Structure

Files are organized by geographic area, then by destination:

```text
<Region_Area>/
  <Location>.md     # one file per destination or home base
```

Example: `Brevard_Area/Lake_Toxaway.md`

The home-base file (e.g., `Lake_Toxaway.md`) is the anchor for an area — it references other files in the same directory for parks and sub-areas.

## Content Conventions

Each destination file typically includes:

- **Home Base** — address, coordinates (decimal `lat, lon` format), host contact
- Activity sections (swimming, hikes, etc.) with distance-from-home-base context
- Tables for multi-item comparisons (waterfalls, parks)
- A **hub section** for a specific area (e.g., Panthertown Valley) when multiple attractions share a trailhead — table of attractions + bullet list of directions and detail

### Distances and mileage

- Driving distances: inline as `(drive 15 mi, 2 mi RT)` — no `~` on numbers
- Table column headings carry the approximation marker: `Drive (~mi)`, `Hike RT (~mi)`
- Values in those columns are plain numbers: `15`, `2.5`, not `~15`, `~2.5`

### Coordinates

Use decimal `lat, lon` with negative longitude for West — paste-ready for Google Maps and Apple Maps:

```text
35.1313, -82.8893
```

Not `35.1313°N, 82.8893°W`.

### Tables

- Keep all table rows within **120 columns** (Emacs / Typora readability)
- Move directions and long detail out of Notes cells into bullets below the table
- Standard Swim column values: `—`, `Prohibited`, `Permitted/Rugged`, `Permitted/Family`

### Cross-references

Link to sibling files with `[[Filename]]` (no path, no extension):

```text
See [[Pisgah_Ranger]] for details.
```

## Markdown

Run `markdownlint --fix --config ~/.markdownlint.json` before committing. Table column alignment is handled automatically by that command.
