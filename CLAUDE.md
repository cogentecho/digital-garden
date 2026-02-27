# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Cogent Echo Digital Garden — the research archive backing the [Cogent Echo](https://www.youtube.com/@cogentecho) YouTube channel and Spotify podcast. Contains AI research analyses, episode transcripts, source materials, and in-progress research. This is a **content repository**, not a software project; there are no build steps, tests, or dependencies.

## Repository Structure

```
episodes/YYYY/MM/DD/   # Published episode analyses, organized by date
research/in-progress/  # Active research projects (move to episodes/ when published)
sources/               # Shared source library
  index.md             # Master source index with quality tiers
templates/             # Episode and analysis templates
  analysis-template.md # Critical analysis format (Cogent Echo Protocol)
  episode-readme.md    # Episode metadata with YAML frontmatter
METHODOLOGY.md         # 7-phase AI-assisted research workflow
```

## Content Conventions

### Episode Organization
Episodes are organized by **date** (`episodes/YYYY/MM/DD/`), using descriptive filenames directly in date directories.

Multi-file episodes (with transcripts, source URLs, etc.) get their own subdirectory under the date folder. Single-file analyses sit directly in the date directory.

### Analysis Format
All analyses follow the **Cogent Echo Protocol** — a structured format with:
- Numbered sections with bold headers
- Inline source citations (superscript numbers)
- Evidence-backed findings with confidence levels
- Methodological notes and bias considerations
- Verification checklists

Use `templates/analysis-template.md` as the starting point. See `METHODOLOGY.md` for the full 7-phase research pipeline.

### Episode Metadata
Episode README files use YAML frontmatter (see `templates/episode-readme.md`) with fields: `episode`, `title`, `date_published`, `date_recorded`, `duration`, `platforms`, `topics`, `status`, `sources_count`, `verification_status`.

### Source Quality Tiers
Defined in `sources/index.md`:
- **Tier 1** (High): Peer-reviewed research, official announcements, direct interviews, government reports
- **Tier 2** (Medium): Reputable journalism, analyst reports, conference presentations
- **Tier 3** (Caution): Unverified claims, single-source reports, anonymous sources, opinion

## Git Workflow

**Never use `git add -A` or `git add .`** — always add files explicitly. Many filenames contain spaces and special characters (em dashes, colons, parentheses); always quote paths.
