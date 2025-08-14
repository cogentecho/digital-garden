# Cogent Echo Digital Garden Schema

## Directory Structure

```
/
├── episodes/               # Published podcast episodes
│   ├── 2024/
│   │   ├── 001-topic-name/
│   │   │   ├── README.md          # Episode metadata & summary
│   │   │   ├── transcript.md      # Full transcript
│   │   │   ├── analysis.md        # AI-generated critical analysis
│   │   │   ├── sources/           # All source materials
│   │   │   │   ├── papers/        # Academic papers, PDFs
│   │   │   │   ├── articles/      # Web articles, saved as markdown
│   │   │   │   ├── data/          # Raw datasets, JSON, CSV
│   │   │   │   └── media/         # Images, videos, audio clips
│   │   │   ├── outputs/           # Generated content
│   │   │   │   ├── video.md       # YouTube video script/notes
│   │   │   │   ├── social.md      # Social media posts
│   │   │   │   └── newsletter.md  # Newsletter version
│   │   │   └── verification/      # Audit trail
│   │   │       ├── fact-check.md  # Verification log
│   │   │       ├── ai-prompts.md  # AI prompts used
│   │   │       └── changes.md     # Revision history
│   │   └── 002-another-topic/
│   └── 2025/
├── research/               # Ongoing/unpublished research
│   ├── in-progress/       # Active research projects
│   └── archived/          # Completed but unpublished research
├── sources/               # Shared source library
│   ├── papers/            # Academic papers by topic
│   ├── datasets/          # Reusable datasets
│   └── contacts/          # Expert interviews, quotes
├── templates/             # Standard templates
│   ├── episode-readme.md
│   ├── analysis-template.md
│   └── verification-checklist.md
└── tools/                 # Scripts and automation
    ├── source-ingestion/  # Scripts to process sources
    └── content-generation/ # AI workflow scripts
```

## File Naming Conventions

### Episodes
- `YYYY/NNN-topic-kebab-case/` (e.g., `2024/001-gpt-4-analysis/`)
- Sequential numbering within year
- Topic should be memorable and URL-friendly

### Sources
- `source-type_YYYY-MM-DD_descriptive-name.ext`
- Examples: `paper_2024-03-15_attention-is-all-you-need.pdf`
- Examples: `article_2024-03-20_openai-announcement.md`

## Metadata Standards

### Episode README.md
```yaml
---
episode: 001
title: "GPT-4 Analysis: Capabilities and Limitations"
date_published: 2024-03-15
date_recorded: 2024-03-10
duration: "45:30"
platforms:
  youtube: "https://youtube.com/watch?v=..."
  spotify: "https://open.spotify.com/episode/..."
topics: [ai-models, gpt-4, analysis]
status: published
sources_count: 12
verification_status: verified
---
```

## Linking Strategy

- Use relative paths for internal links
- Maintain `sources/index.md` with all source metadata
- Create topic-based indexes in `/topics/` for cross-episode discovery
- Use consistent tagging for discoverability

## Principles

1. **Chronological Primary**: Episodes organized by publication date for timeline clarity
2. **Source Deduplication**: Shared sources library prevents duplication across episodes
3. **Verification Trail**: Every claim traceable to source with AI prompt history
4. **Content Reuse**: Multiple output formats from single research project
5. **Scalability**: Structure works for 10 episodes or 1000