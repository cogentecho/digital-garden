# Quick Start Guide

## Creating a New Episode

1. **Create episode directory:**
   ```bash
   mkdir episodes/2024/001-topic-name
   cd episodes/2024/001-topic-name
   ```

2. **Copy template:**
   ```bash
   cp ../../../templates/episode-readme.md README.md
   ```

3. **Create subdirectories:**
   ```bash
   mkdir sources sources/papers sources/articles sources/data sources/media
   mkdir outputs verification
   ```

4. **Start research:**
   - Add sources to `sources/` with naming convention: `type_YYYY-MM-DD_description.ext`
   - Update `sources/index.md` with new sources
   - Fill out episode README.md metadata

5. **Generate analysis:**
   ```bash
   cp ../../../templates/analysis-template.md analysis.md
   ```
   - Fill in analysis based on sources
   - Document AI prompts in `verification/ai-prompts.md`

## Backfilling Existing Podcasts

1. **Identify all published episodes** (YouTube/Spotify)
2. **Create directories chronologically** starting with earliest
3. **For each episode:**
   - Create README.md with platform links
   - Add transcript if available
   - Reconstruct source list
   - Create analysis.md summarizing key points
   - Mark verification_status as "legacy" if not fully verifiable

## File Naming Examples

```
episodes/2024/001-gpt-4-analysis/
├── README.md
├── transcript.md  
├── analysis.md
├── sources/
│   ├── paper_2024-03-14_gpt-4-technical-report.pdf
│   ├── article_2024-03-15_openai-announcement.md
│   └── data_2024-03-10_benchmark-results.csv
├── outputs/
│   ├── video.md
│   └── social.md
└── verification/
    ├── fact-check.md
    ├── ai-prompts.md
    └── changes.md
```

## Daily Workflow

1. **Source Collection:** Save interesting sources to appropriate `sources/` subdirectory
2. **Topic Tracking:** Update `sources/index.md` when adding sources
3. **Episode Development:** Use `research/in-progress/` for developing episodes
4. **Publication:** Move completed research to `episodes/YYYY/NNN-topic/`
5. **Cross-linking:** Update related episodes and topic indexes

## Maintenance Tasks

### Weekly
- Update `sources/index.md` with new additions
- Review `research/in-progress/` for stalled projects
- Check verification status of recent episodes

### Monthly  
- Archive completed research projects
- Update topic indexes for discoverability
- Review and update templates based on lessons learned