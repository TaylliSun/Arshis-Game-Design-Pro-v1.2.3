---
name: Arshis-Game-Design-Pro
description: Professional game design workflow assistant for indie developers. Generate GDDs, review designs, plan Unity specs, and explore innovative concepts.
version: 2.4.4
author: Arshis
license: MIT
---

# Arshis-Game-Design-Pro

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![OpenClaw](https://img.shields.io/badge/OpenClaw-2026.4.0+-blue.svg)](https://docs.openclaw.ai)
[![Python](https://img.shields.io/badge/Python-3.9+-green.svg)](https://www.python.org)

Professional game design workflow assistant for indie developers and small teams. Generate structured game design documents, review designs for risks, plan Unity technical specifications, and explore innovative concepts through natural language.

## Core Features

### Game Design Documents
- Structured GDD generation with clear sections
- Professional 17-section format covering mechanics, systems, progression, UI, art direction, audio, technical implementation, and risk analysis
- 10 professional templates: Full GDD, System Design, Technical Design, Level Design, Character Design, Worldbuilding Bible, Art Requirements, UI/UX Flow, MVP Roadmap, Publisher Pitch

### Innovation Engine
- Differentiated concept generation through structured pipeline
- Genre convention analysis across 25 game types
- 5 concept types: Safe, Moderate, High, Experimental, Indie-Friendly
- Novelty Filter: 6-level judgment from Common to Emotional Experience Innovation
- Auto-rewrite for concepts flagged as reskin

### Technical Planning
- Convert GDD ideas into Unity-ready specifications
- C# script names, variable tables, data structures, event systems
- Art/audio asset lists with count and priority
- Development phases with timeline and cuttable features

### Design Review
- Check completeness, consistency, and innovation level
- Get specific improvement suggestions, not generic feedback
- Cross-check gameplay vs story, art vs scope, complexity vs team capacity

### Context Injection Control
- Summary-only mode by default
- Maximum 8 memories injected per query
- Relevance threshold filtering (default: 0.72)
- Max context token limit (default: 12,000)

## Usage

### Generate an Innovative Game Concept

```
generate_innovative_design({
  genre: "roguelike",
  theme: "time manipulation",
  target_emotion: "melancholy",
  output_mode: "markdown"
})
```

### Review an Existing Design

```
review_innovation_level({
  genre: "rpg",
  theme: "farming",
  design_content: "# My Game\n\nPlayers grow crops, sell them for gold..."
})
```

### Convert GDD to Technical Spec

```
gdd_to_tech({
  gdd_text: "NPC relationship system where players build bonds through gifts and quests...",
  output_mode: "technical_plan"
})
```

## Supported Genres (25)

RPG, Roguelike, Platformer, Puzzle, Simulation, Action, Strategy, Survival, Horror, Farming, Tower Defense, Deckbuilding, Metroidvania, Monster Taming, Survival Crafting, Management Sim, Visual Novel, Puzzle Adventure, Tactical RPG, City Builder, Rhythm Game, Cozy Exploration, Idle Game, Party Game, Social Deduction.

## Tool Functions

### Core Design
- `generate_design({ doc_type, topic, details, word_count })`
- `review_design({ content, doc_type })`
- `check_consistency({ content_type, content_data })`
- `store_worldview({ category, content, importance })`
- `query_worldview({ query, limit })`

### Workflow
- `create_project_profile({ game_title, genre, platform, ... })`
- `gdd_to_tech({ gdd_text, profile_file, obsidian })`
- `consistency_review({ design_json, profile_file, obsidian })`
- `review_score({ design_text, profile_file })`
- `obsidian_export({ profile_file })`

### Professional
- `professional_design({ topic, genre, details })`
- `production_spec({ topic, genre, details })`
- `combined_design({ topic, modes: "professional,innovation,production" })`
- `get_template_doc({ template_key })` -- 10 templates available

### Innovation Engine
- `generate_innovative_design({ genre, theme, target_emotion, output_mode })`
- `review_innovation_level({ genre, theme, design_content })`

## Output Modes

| Mode | Description |
|------|-------------|
| json | Raw structured data |
| markdown / gdd | Professional GDD format |
| obsidian | Obsidian with YAML frontmatter and internal links |
| technical_plan | Unity implementation plan |
| publisher_pitch | One-page pitch for publishers |

## Privacy

This plugin does not make outbound network requests, does not collect or upload user data, and does not require API keys. All outputs remain local to the OpenClaw environment.

## Requirements

- OpenClaw 2026.4.0+
- Python 3.9+

## License

MIT
