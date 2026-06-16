# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Purpose

Personal adventure travel notes — destination guides, home base logistics, hike details, and local context. No code, no build system.

## Structure

Files are organized by geographic area, then by destination:

```
<Region_Area>/
  <Location>.md     # one file per destination or home base
```

Example: `Brevard_Area/Lake_Toxaway.md`

## Content Conventions

Each destination file typically includes:
- **Home Base** — address, coordinates, host contact
- Activity sections (swimming, hikes, etc.) with distance-from-home-base context
- Tables for multi-item comparisons (waterfalls, coordinates)
- **Regional Context** — nearby forests/parks and what they're good for

## Markdown

Run `markdownlint --fix --config ~/.markdownlint.json` before committing. Table column alignment is handled automatically by that command.
