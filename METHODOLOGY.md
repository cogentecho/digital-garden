# AI-Assisted Research Workflow

A repeatable, AI-assisted research pipeline that produces verified, prioritized intelligence from raw topics. The system uses multiple LLMs (Claude and Gemini), iterative verification loops, a knowledge graph for traceability, and a persistent memory layer backed by Git.

The output is a comprehensive report optimized for rapid decision-making — structured so you know within the first few paragraphs whether the topic warrants deeper attention.

---

## Table of Contents

- [Overview](#overview)
- [Phase 1: Curated Prompt Pipeline](#phase-1-curated-prompt-pipeline)
- [Phase 2: Deep Dive and Evidence Gathering](#phase-2-deep-dive-and-evidence-gathering)
- [Phase 3: Knowledge Graph Construction](#phase-3-knowledge-graph-construction)
- [Phase 4: Threshold-Based Organization](#phase-4-threshold-based-organization)
- [Phase 5: Personalized Value Ranking](#phase-5-personalized-value-ranking)
- [Phase 6: Report Assembly and Challenge](#phase-6-report-assembly-and-challenge)
- [Phase 7: Persistent Memory System (Setup Guide)](#phase-7-persistent-memory-system-setup-guide)
- [Getting Started](#getting-started)
- [License](#license)

---

## Overview

This workflow combines four things most people skip when working with generative AI:

1. **Modular prompts** that keep each step auditable and focused.
2. **Parallel model usage** (Claude + Gemini) that catches blind spots inherent in any single model.
3. **A knowledge graph** that maintains full traceability from raw source to final assertion.
4. **A persistent memory layer** that compounds your research investment over time rather than starting from zero each session.

The personalized ranking layer on top means you are not just getting information — you are getting *your* information, ordered by what matters to *you*.

---

## Phase 1: Curated Prompt Pipeline

The workflow is built on a set of single-purpose prompts, each responsible for exactly one step in the process. This modular design keeps each interaction focused and auditable.

Rather than asking an AI to "research topic X" in one shot, you break the work into discrete stages — evidence gathering, source verification, content synthesis, challenge and review — each driven by a dedicated prompt. This gives you a clear decision point between every step, so you maintain control over what gets accepted into the dataset and what gets discarded or flagged for further investigation.

**Key principle:** You stay in the loop. Automation handles the repetitive mechanics, but judgment calls remain yours. The system is designed to clearly delineate what is provable versus what is speculative, so you always know where the boundary is when deciding how to handle a finding.

---

## Phase 2: Deep Dive and Evidence Gathering

Use both Claude and Gemini to conduct parallel deep dives on your target topic. Each model has different training data and reasoning tendencies, so running both increases coverage and exposes blind spots.

**The iterative cycle:**

1. **Create** — Generate initial content and findings on the topic.
2. **Edit** — Refine and restructure the output for accuracy and clarity.
3. **Update** — Incorporate new information as it surfaces from subsequent passes.
4. **Verify** — Cross-check sources, validate claims, and flag anything unsubstantiated.

This cycle repeats. Each pass feeds back into the dataset, progressively enriching it. The process continues until it hits one of several predefined thresholds (see [Phase 4](#phase-4-threshold-based-organization)).

---

## Phase 3: Knowledge Graph Construction

As findings accumulate, they are organized into a knowledge graph rather than flat documents. Each node in the graph carries:

- **Semantic references** — Connections to related concepts, enabling traversal across topics.
- **Data lineage metadata** — A record of where each piece of information originated, which model produced it, what verification steps it passed through, and when it was last updated.
- **Provenance tracking** — Full traceability from raw source to final assertion, so any claim in the final report can be traced back to its evidence chain.

This structure is what makes the system trustworthy at scale. Without lineage and provenance, you are just accumulating unverified AI output.

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

1. **Contextual interviews** — Claude conducts a series of structured interviews with you to understand your priorities, decision-making style, domain expertise, and what constitutes actionable intelligence for your specific situation.
2. **Tenet and rule generation** — From those interviews, a set of tenets and ranking rules are produced. These encode your preferences into a repeatable scoring system.
3. **Priority ordering** — All content is then organized highest-value-first, so the report front-loads the information most likely to matter to you.

**The result:** You can determine within the first section of any report whether it warrants continued reading. The system is optimized for your time and judgment, not for completeness for its own sake.

---

## Phase 6: Report Assembly and Challenge

Once organized, the system assembles a comprehensive report. Before finalization:

- Every component is **analyzed and challenged** — claims are stress-tested, alternative interpretations are considered, and weak evidence is flagged rather than buried.
- **Complete traceability** is maintained — every assertion links back through the knowledge graph to its source material and verification history.
- The report is **structured for rapid triage** — the most important findings appear first, with supporting detail available for drill-down as needed.

---

## Phase 7: Persistent Memory System (Setup Guide)

All datasets produced by this workflow are saved, indexed, analyzed, and ingested into a persistent memory system. This means the AI retains and builds on prior research across sessions, rather than starting from zero each time.

### Step 1: Create a GitHub Account

If you do not already have one, create a free account at [github.com](https://github.com).

### Step 2: Create a Private Repository

Create a new **private** repository specifically for your GenAI memories. Name it something descriptive (e.g., `genai-memory` or `ai-research-memory`). Keep it private — this will contain your curated knowledge and research context.

### Step 3: Connect VS Code to the Repository

Have Claude help you configure VS Code to connect to this repository as a tool. The repository serves dual purposes:

| Memory Type | Purpose |
|---|---|
| **Short-term** | Active working context for current research sessions. |
| **Long-term** | Accumulated knowledge that persists across sessions and topics. |

### Step 4: Leverage Git Commits as Semantic History

This is the key architectural insight: **Git commits provide the AI with a built-in mechanism for leaving metadata and semantic reference history.** Each commit message becomes a searchable entry point into what changed, why, and when.

This gives you:

- A **searchable memory layer** across all prior research.
- **Version history** showing how understanding evolved over time.
- The ability for the AI to primarily work with **the best of what you know**, while still having access to the full history when needed.

---

## Getting Started

If you are new to this workflow, the recommended path is:

1. **Start with Phase 7** — Set up your persistent memory repo first. This is the foundation everything else builds on, and it provides immediate value even before you implement the full pipeline.
2. **Experiment with Phase 1–2** — Build a small set of single-purpose prompts and run a few iterative research cycles on a topic you care about.
3. **Add structure incrementally** — Layer in the knowledge graph, thresholds, and personalized ranking as you get comfortable with the core loop.

You do not need to implement all seven phases at once. Each phase adds value independently.

---

## License

This work is shared for personal and educational use. Feel free to adapt it to your own workflow.
