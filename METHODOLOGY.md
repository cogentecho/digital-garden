---
title: Methodology
description: 7-phase AI-assisted research workflow for producing verified intelligence.
layout: page
---

# AI-Assisted Research Workflow

A repeatable, agent-driven research pipeline that produces verified, prioritized intelligence from raw topics. The system uses multi-model orchestration, automated verification, knowledge graphs for traceability, and persistent memory systems that compound research investment across sessions.

The output is a comprehensive report optimized for rapid decision-making — structured so you know within the first few paragraphs whether the topic warrants deeper attention.

---

## Table of Contents

- [Overview](#overview)
- [Phase 1: Curated Prompt Pipeline](#phase-1-curated-prompt-pipeline)
- [Phase 2: Multi-Model Deep Dive and Evidence Gathering](#phase-2-multi-model-deep-dive-and-evidence-gathering)
- [Phase 3: Knowledge Graph Construction](#phase-3-knowledge-graph-construction)
- [Phase 4: Threshold-Based Organization](#phase-4-threshold-based-organization)
- [Phase 5: Personalized Value Ranking](#phase-5-personalized-value-ranking)
- [Phase 6: Report Assembly and Challenge](#phase-6-report-assembly-and-challenge)
- [Phase 7: Persistent Memory and Tooling](#phase-7-persistent-memory-and-tooling)
- [Getting Started](#getting-started)

---

## Overview

This workflow combines four things most people skip when working with generative AI:

1. **Modular prompts** that keep each step auditable and focused.
2. **Multi-model cross-validation** across model families that catches blind spots inherent in any single system.
3. **A knowledge graph** that maintains full traceability from raw source to final assertion.
4. **A persistent memory layer** that compounds your research investment over time rather than starting from zero each session.

The personalized ranking layer on top means you are not just getting information — you are getting *your* information, ordered by what matters to *you*.

### Agentic Execution

Each phase can be executed manually (human-in-the-loop) or delegated to autonomous agents. Modern AI tooling — multi-agent orchestration, tool use, web search, and code execution — means phases that previously required manual prompt chaining can now run as supervised agent workflows. The human role shifts from operating each step to setting objectives, reviewing outputs, and making judgment calls at phase boundaries.

---

## Phase 1: Curated Prompt Pipeline

The workflow is built on a set of single-purpose prompts, each responsible for exactly one step in the process. This modular design keeps each interaction focused and auditable.

Rather than asking an AI to "research topic X" in one shot, you break the work into discrete stages — evidence gathering, source verification, content synthesis, challenge and review — each driven by a dedicated prompt or agent task. This gives you a clear decision point between every step, so you maintain control over what gets accepted into the dataset and what gets discarded or flagged for further investigation.

**Key principle:** You stay in the loop. Automation handles the repetitive mechanics, but judgment calls remain yours. The system is designed to clearly delineate what is provable versus what is speculative, so you always know where the boundary is when deciding how to handle a finding.

---

## Phase 2: Multi-Model Deep Dive and Evidence Gathering

Use multiple model families to conduct parallel deep dives on your target topic. Each model has different training data, reasoning tendencies, and knowledge cutoffs, so running several increases coverage and exposes blind spots.

**Recommended model mix (as of February 2026):**

| Role | Examples |
|---|---|
| **Primary reasoning** | Claude Opus/Sonnet 4.6, GPT-4.5 |
| **Broad knowledge / search** | Gemini 2.0, Perplexity |
| **Open-source cross-check** | Llama 4, DeepSeek-V3, Mistral Large, Qwen |
| **Specialized tasks** | Domain-specific fine-tuned models as available |

The specific models matter less than the principle: **no single model should be your only source of truth.** Model rankings shift frequently. What matters is that you are cross-validating across architecturally distinct systems.

**The iterative cycle:**

1. **Create** — Generate initial content and findings on the topic.
2. **Edit** — Refine and restructure the output for accuracy and clarity.
3. **Update** — Incorporate new information as it surfaces from subsequent passes.
4. **Verify** — Cross-check sources, validate claims, and flag anything unsubstantiated.

This cycle repeats. Each pass feeds back into the dataset, progressively enriching it. The process continues until it hits one of several predefined thresholds (see [Phase 4](#phase-4-threshold-based-organization)).

**Agentic acceleration:** This phase benefits most from agent-driven execution. A research orchestrator can dispatch parallel model queries, aggregate results, identify contradictions, and surface them for human review — compressing what was previously hours of manual prompt work into minutes of supervised automation.

---

## Phase 3: Knowledge Graph Construction

As findings accumulate, they are organized into a knowledge graph rather than flat documents. Each node in the graph carries:

- **Semantic references** — Connections to related concepts, enabling traversal across topics.
- **Data lineage metadata** — A record of where each piece of information originated, which model produced it, what verification steps it passed through, and when it was last updated.
- **Provenance tracking** — Full traceability from raw source to final assertion, so any claim in the final report can be traced back to its evidence chain.

This structure is what makes the system trustworthy at scale. Without lineage and provenance, you are just accumulating unverified AI output.

**Tooling:** Knowledge graphs can be maintained through structured memory services (MCP-based memory servers, graph databases, or purpose-built research tools) rather than manual construction. The key requirement is that whatever system you use preserves the lineage and provenance metadata — the graph structure is a means to that end, not an end in itself.

---

## Phase 4: Threshold-Based Organization

The iterative cycle from Phase 2 does not run indefinitely. You define thresholds that trigger the transition from gathering to organizing. Examples include:

| Threshold | Description |
|---|---|
| **Saturation** | New passes are returning diminishing novel information. |
| **Coverage** | All identified subtopics have been addressed to a minimum depth. |
| **Confidence** | A sufficient percentage of claims have been independently verified. |
| **Contradiction Resolution** | Outstanding conflicts between sources have been investigated and resolved or explicitly flagged. |

When a threshold is met, the system transitions to assembly.

---

## Phase 5: Personalized Value Ranking

Before the report is assembled, all findings are ranked by value. "Value" is not generic — it is defined by a personalized rubric generated through a structured process:

1. **Contextual interviews** — The AI conducts a series of structured interviews with you to understand your priorities, decision-making style, domain expertise, and what constitutes actionable intelligence for your specific situation.
2. **Tenet and rule generation** — From those interviews, a set of tenets and ranking rules are produced. These encode your preferences into a repeatable scoring system.
3. **Priority ordering** — All content is then organized highest-value-first, so the report front-loads the information most likely to matter to you.

**The result:** You can determine within the first section of any report whether it warrants continued reading. The system is optimized for your time and judgment, not for completeness for its own sake.

These preferences persist across sessions. As your priorities evolve, the ranking system adapts — but the history of how your priorities changed is itself a valuable record.

---

## Phase 6: Report Assembly and Challenge

Once organized, the system assembles a comprehensive report. Before finalization:

- Every component is **analyzed and challenged** — claims are stress-tested, alternative interpretations are considered, and weak evidence is flagged rather than buried.
- **Complete traceability** is maintained — every assertion links back through the knowledge graph to its source material and verification history.
- The report is **structured for rapid triage** — the most important findings appear first, with supporting detail available for drill-down as needed.

---

## Phase 7: Persistent Memory and Tooling

All datasets produced by this workflow are saved, indexed, analyzed, and ingested into a persistent memory system. This means the AI retains and builds on prior research across sessions, rather than starting from zero each time.

### Memory Architecture

Modern AI development environments provide native memory capabilities:

| Layer | Purpose | Examples |
|---|---|---|
| **Project memory** | Conventions, preferences, and context specific to a project or research domain. | `CLAUDE.md` files, project-level instructions, `.cursorrules` |
| **Session memory** | Working context for the current research session — intermediate findings, open questions, active hypotheses. | Conversation context, scratchpad files |
| **Persistent memory** | Accumulated knowledge that persists across sessions and topics. The compounding layer. | MCP memory servers, structured knowledge bases, git-backed archives |
| **Version history** | How understanding evolved over time — what changed, why, and when. | Git commits, document revision history |

### Key Principles

1. **Memory should be automatic.** If you have to remember to save something, the system is too fragile. Prefer tools that capture context as a side effect of doing the work.

2. **Git remains valuable as an audit trail.** Commits provide a searchable, timestamped record of how research evolved. Commit messages are semantic entry points into the history. This is complementary to — not replaced by — purpose-built memory tools.

3. **Separate working memory from long-term memory.** Not everything from a research session belongs in persistent storage. The system should make it easy to promote findings from session context to long-term memory, and to prune what turns out to be noise.

4. **Memory compounds.** The value of persistent memory increases non-linearly over time. Early sessions build the foundation that later sessions accelerate from. This is the single highest-ROI investment in the entire workflow.

---

## Getting Started

If you are new to this workflow, the recommended path is:

1. **Start with memory** — Set up your persistent memory system first. This is the foundation everything else builds on, and it provides immediate value even before you implement the full pipeline.
2. **Experiment with Phases 1–2** — Build a small set of single-purpose prompts and run a few iterative research cycles on a topic you care about. Try at least two different model families.
3. **Add structure incrementally** — Layer in the knowledge graph, thresholds, and personalized ranking as you get comfortable with the core loop.

You do not need to implement all seven phases at once. Each phase adds value independently.
