# Quick Start Guide

## Creating a New Episode

1. **Create the date directory:**
   ```bash
   mkdir -p episodes/2025/08/25
   ```

2. **Write the analysis** directly in the date directory using a descriptive filename:
   ```bash
   # Single-file episode — just the analysis
   cp templates/analysis-template.md "episodes/2025/08/25/Analysis of Topic Title.md"
   ```

3. **For multi-file episodes** (transcript, source URLs, etc.), create a subdirectory:
   ```bash
   mkdir "episodes/2025/08/25/Topic Title"
   cp templates/analysis-template.md "episodes/2025/08/25/Topic Title/An Analytical Review of Topic Title.md"
   ```
   Add transcripts, `.url` files, and other supporting materials alongside the analysis.

4. **Follow the Cogent Echo Protocol** when writing the analysis:
   - Fill in findings with evidence and confidence levels
   - Add source citations
   - Complete the verification checklist
   - See [METHODOLOGY.md](METHODOLOGY.md) for the full 7-phase research pipeline

## Research Workflow

Active research lives in `research/in-progress/`. When a research project becomes an episode, move it to `episodes/YYYY/MM/DD/`.

For the complete AI-assisted research pipeline — from curated prompts through knowledge graph construction to personalized ranking — see [METHODOLOGY.md](METHODOLOGY.md).

## File Naming Examples

**Single-file episode:**
```
episodes/2025/08/13/An Analytical Review of Topic Title.md
```

**Multi-file episode:**
```
episodes/2025/08/14/Forget Network Layers — Cortical Columns Think Like Graphs/
├── An Analytical Audit of 'Forget Network Layers...'.md
├── Transcript - Cortical Columns as Graphs.md
└── Forget Network Layers — YouTube.url
```

## Daily Workflow

1. **Source Collection:** Save interesting sources and update `sources/index.md`
2. **Research:** Develop ideas in `research/in-progress/`
3. **Publish:** Move completed work to `episodes/YYYY/MM/DD/`

## Maintenance

### Weekly
- Review `research/in-progress/` for stalled projects
- Update `sources/index.md` with new additions

### Monthly
- Review and update templates based on lessons learned
