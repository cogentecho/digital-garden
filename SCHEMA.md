# Cogent Echo Digital Garden Schema

## Directory Structure

```
/
├── episodes/                # Published episode analyses
│   └── YYYY/MM/DD/          # Organized by publication date
│       ├── Analysis Title.md              # Single-file analysis
│       └── Episode Title/                 # Multi-file episode
│           ├── Analysis Title.md          # Critical analysis
│           ├── Transcript - Topic.md      # Episode transcript
│           └── Source Title.url           # Source links
├── research/                # Ongoing research
│   └── in-progress/         # Active research projects
├── sources/                 # Shared source library
│   └── index.md             # Master source index with quality tiers
├── templates/               # Standard templates
│   ├── analysis-template.md # Critical analysis format (Cogent Echo Protocol)
│   └── episode-readme.md    # Episode metadata with YAML frontmatter
├── METHODOLOGY.md           # 7-phase AI-assisted research workflow
├── QUICKSTART.md            # Getting started guide
└── README.md                # Project overview and platform links
```

## Episode Organization

Episodes are organized by **publication date** using the path `episodes/YYYY/MM/DD/`.

**Single-file episodes** place the analysis markdown directly in the date directory:
```
episodes/2025/08/13/An Analytical Review of Topic Title.md
```

**Multi-file episodes** (with transcripts, source URLs, supplementary material) get their own subdirectory under the date folder:
```
episodes/2025/08/14/Forget Network Layers — Cortical Columns Think Like Graphs/
├── An Analytical Audit of 'Forget Network Layers...'.md
├── Transcript - Cortical Columns as Graphs.md
└── Forget Network Layers — Cortical Columns Think Like Graphs - YouTube.url
```

### Naming Conventions

- **Analysis files**: Use descriptive titles as filenames (e.g., `An Analytical Review of Topic.md`)
- **Transcripts**: Prefix with `Transcript - ` (e.g., `Transcript - Topic Name.md`)
- **Source URLs**: Use the source page title with `.url` extension
- Filenames may contain spaces, em dashes, and other readable characters — always quote paths in shell commands

## Metadata Standards

### Episode README (optional)

When included, episode README files use YAML frontmatter:

```yaml
---
episode: 5
title: "Episode Title"
date_published: 2025-08-14
date_recorded: 2025-08-12
duration: "45:30"
platforms:
  youtube: "https://youtube.com/watch?v=..."
  spotify: "https://open.spotify.com/episode/..."
topics: [ai-models, graph-theory, analysis]
status: published
sources_count: 12
verification_status: verified
---
```

## Analysis Format

All analyses follow the **Cogent Echo Protocol** (see `templates/analysis-template.md`):

- Numbered sections with bold headers
- Inline source citations (superscript numbers)
- Evidence-backed findings with confidence levels
- Methodological notes and bias considerations
- Verification checklists

For the full research methodology, see [METHODOLOGY.md](METHODOLOGY.md).

## Source Quality Tiers

Defined in `sources/index.md`:

| Tier | Confidence | Examples |
|------|-----------|----------|
| **Tier 1** | High | Peer-reviewed research, official announcements, direct interviews, government reports |
| **Tier 2** | Medium | Reputable journalism, analyst reports, conference presentations |
| **Tier 3** | Caution | Unverified claims, single-source reports, anonymous sources, opinion |

## Principles

1. **Chronological Organization**: Episodes organized by publication date for timeline clarity
2. **Source Deduplication**: Shared sources library prevents duplication across episodes
3. **Verification Trail**: Every claim traceable to source material
4. **Simplicity**: Flat structure within date directories — no deep nesting unless needed
