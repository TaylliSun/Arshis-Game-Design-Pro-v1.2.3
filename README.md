# Arshis-Game-Design-Pro

> Professional game design workflow assistant for indie developers and small teams.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![OpenClaw](https://img.shields.io/badge/OpenClaw-2026.4.0+-blue.svg)](https://docs.openclaw.ai)
[![Python](https://img.shields.io/badge/Python-3.9+-green.svg)](https://www.python.org)

Generate structured game design documents, review designs for risks, plan Unity technical specifications, and explore innovative concepts -- all through natural language.

---

## Overview

Arshis-Game-Design-Pro helps you go from a game idea to production-ready design:

- **Generate GDDs** -- Structured game design documents with clear sections, not walls of text
- **Review Designs** -- Check completeness, identify risks, get improvement suggestions
- **Plan Technical Specs** -- Unity scripts, variables, data structures, development phases
- **Explore Innovations** -- Differentiated concepts through a structured innovation pipeline
- **Check Consistency** -- Catch contradictions between story, mechanics, and worldbuilding
- **Export Anywhere** -- Markdown, Obsidian, GDD, technical plan, or publisher pitch

## What It Is NOT

- Not a memory plugin
- Not a replacement for professional game designers
- Not a game engine or code generator
- Does not make external network requests
- Does not require API keys

## Quick Start

### Installation

1. Copy the `Arshis-Game-Design-Pro-release/` folder to your OpenClaw skills directory:
   ```
   ~/.openclaw/workspace/skills/Arshis-Game-Design-Pro/
   ```
2. Install Python dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Restart OpenClaw.

### Examples

#### 1. Generate an Innovative Game Concept

```
generate_innovative_design({
  genre: "roguelike",
  theme: "time manipulation",
  target_emotion: "melancholy",
  output_mode: "markdown"
})
```

**Output**: Full innovation design document with genre convention analysis, 5 unique concepts (Safe/Moderate/High/Experimental/Indie), each with novelty filter check, 6-metric scoring, Unity prototype plan, and MVP scope.

#### 2. Review an Existing Design's Innovation Level

```
review_innovation_level({
  genre: "rpg",
  theme: "farming",
  design_content: "# My Game\n\nPlayers grow crops, sell them for gold..."
})
```

**Output**: Innovation score across 4 metrics, common vs different elements, reskin detection, improvement suggestions, indie feasibility tips.

#### 3. Convert GDD Idea into Unity Technical Planning

```
gdd_to_tech({
  gdd_text: "NPC relationship system where players build bonds through gifts and quests...",
  profile_file: "profile_my_game.json",
  output_mode: "technical_plan"
})
```

**Output**: Required Unity systems, C# script names (PascalCase), variable tables (with types), event systems, UI requirements, art/audio asset lists, development phases with timeline.

## Full Tool Reference

### Core Design

| Function | Description |
|----------|-------------|
| `generate_design` | Generate game design documents |
| `review_design` | Review design documents for completeness and risks |
| `check_consistency` | Check design consistency (worldview/characters/systems) |
| `store_worldview` | Manage worldview settings |
| `query_worldview` | Query stored worldview settings |

### Workflow (v2.2.0+)

| Function | Description |
|----------|-------------|
| `create_project_profile` | Create game project profiles |
| `gdd_to_tech` | Convert GDD to technical design |
| `consistency_review` | Run consistency checks |
| `review_score` | Score designs on key metrics |
| `obsidian_export` | Export as Obsidian Markdown |

### Professional (v2.3.0+)

| Function | Description |
|----------|-------------|
| `professional_design` | Professional GDD generation (17 sections) |
| `production_spec` | Production-ready specifications |
| `combined_design` | Multi-mode combined output |
| `get_template_doc` | Get professional templates |

### Innovation Engine (v2.4.0+)

| Function | Description |
|----------|-------------|
| `generate_innovative_design` | Full innovation pipeline with 5 concept types |
| `review_innovation_level` | Review existing design innovation level |

## Output Modes

| Mode | Use Case |
|------|----------|
| `json` | Raw structured data |
| `markdown` / `gdd` | Professional GDD format |
| `obsidian` | Obsidian with YAML frontmatter and internal links |
| `technical_plan` | Unity implementation plan |
| `publisher_pitch` | One-page pitch for publishers |

## Supported Genres (25)

RPG, Roguelike, Platformer, Puzzle, Simulation, Action, Strategy, Survival, Horror, Farming, Tower Defense, Deckbuilding, Metroidvania, Monster Taming, Survival Crafting, Management Sim, Visual Novel, Puzzle Adventure, Tactical RPG, City Builder, Rhythm Game, Cozy Exploration, Idle Game, Party Game, Social Deduction.

Each genre includes: common mechanics, progression patterns, goals, rewards, common risks, innovation breakpoints, and indie-friendly prototype advice.

## Innovation Engine

The Innovation Engine generates differentiated game design concepts through a structured pipeline:

1. **Genre Convention Analysis** -- What does this genre typically do?
2. **Innovation Breakpoints** -- Where can we diverge? (10 dimensions)
3. **Innovation Methods** -- Inversion, Constraint as Mechanic, Genre Fusion, Emotion-First Design, System Replacement, Player Role Shift, Resource Reinterpretation, Failure Innovation, World-Mechanic Binding, Small-Team Innovation
4. **Innovation Matrix** -- Combinatorial generation from 6 element pools (core verbs, constraints, emotions, system sources, world rules, player roles)
5. **Divergent Ideas** -- 5 concepts: Safe, Moderate, High, Experimental, Indie-Friendly
6. **Novelty Filter** -- 6-level judgment: Common / Generic, Reskin Only, Minor Innovation, Rule Innovation, Player Behavior Innovation, Emotional Experience Innovation
7. **Innovation Score** -- 6-metric scoring per concept
8. **Production-Ready Plan** -- Unity prototype steps, MVP scope, full expansion

## Privacy

- **No outbound network requests** -- This skill does not connect to any external services
- **No data collection** -- No analytics, telemetry, or user profiling
- **No API keys required** -- Uses OpenClaw's configured model by default
- **All outputs remain local** -- No data is sent to external servers

## Requirements

- OpenClaw 2026.4.0+
- Python 3.9+

## Project Structure

```
Arshis-Game-Design-Pro/
  index.js                  # OpenClaw plugin entry point (28 tool functions)
  openclaw.plugin.json      # Plugin metadata
  package.json              # Package info
  SKILL.md                  # Skill documentation
  README.md                 # This file
  PRIVACY.md                # Privacy policy
  SECURITY.md               # Security documentation
  CHANGELOG.md              # Version history
  requirements.txt           # Python dependencies
  scripts/                   # Core Python scripts (41 files)
    generator.py            # GDD generation
    reviewer.py             # Design review
    templates.py            # Template system
    system_design.py        # System design
    numeric_balance.py      # Numeric balance
    story_designer.py       # Story/narrative design
    dialogue_generator.py   # Dialogue generation
    worldview_builder.py    # Worldbuilding
    consistency_checker.py  # Consistency checking
    innovation_engine.py    # Innovation engine
    workflow_assistant.py   # Workflow tools
    professional_generator.py  # Professional modes
    ... and 29 more
```

## Version History

| Version | Key Change |
|---------|-----------|
| v2.4.4 | Emoji cleanup, stable release |
| v2.4.3 | Score calibration -- type-aware scoring with content-quality variance |
| v2.4.2 | 25 genre conventions, robustness fixes, 5 test cases verified |
| v2.4.1 | Quality improvements: real game-like names, novelty filter with auto-rewrite, 6 output modes |
| v2.4.0 | Innovation Engine: genre analysis, breakpoints, matrix, novelty filter, scoring |
| v2.3.0 | Professional modes: Professional, Innovation, Production-Ready, Templates |
| v2.2.0 | Workflow: project profiles, GDD-to-tech, consistency review, review score |

## Contributing

Contributions are welcome. Please read the existing code structure before submitting changes.

## License

[MIT License](LICENSE)

---

*Arshis-Game-Design-Pro v2.4.4*
*A game design workflow assistant for indie developers and small teams.*
