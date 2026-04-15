# openclaw skill

# Arshis-Game-Design-Pro-v1.2.3

Professional game design tool for generating 90% complete commercial-grade game design documents. 26 core modules covering pricing, publishing, technical assessment, system design, dialogue, and event configuration.
---
# Arshis-Game-Design-Pro

<div align="center">

**Professional Game Design Tool**

[![Version](https://img.shields.io/badge/version-v1.2.3-blue.svg)](https://github.com/Arshis/Arshis-Game-Design-Pro/releases)
[![Python](https://img.shields.io/badge/python-3.8+-green.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/license-MIT-orange.svg)](LICENSE)
[![Modules](https://img.shields.io/badge/modules-26-red.svg)](docs/MODULES.md)

Generate 90% complete commercial-grade game design documents with 26 core modules and 70000+ lines of code.

[Features](#features) | [Quick Start](#quick-start) | [OpenClaw](#openclaw-integration) | [Examples](#examples) | [FAQ](#faq)

</div>

---

## Project Overview

Arshis-Game-Design-Pro is a professional game design assistant that generates 90% complete commercial-grade game design documents based on psychology, sociology, GDC talks, and industry case studies.

### Core Value

- **90% Completeness** - Generate production-ready design documents for your team
- **26 Core Modules** - Cover pricing, publishing, technical, system, dialogue, and events
- **Academic Data** - Based on Sensor Tower 2026, GDC 2023-2025, MIT Media Lab research
- **3-4x Efficiency** - Generate frameworks quickly, supplement 10% manually
- **Continuous Learning** - Support feedback and personalized learning

### Use Cases

| Scenario | Suitability | Description |
|---|---|---|
| **Indie Developers** | High | Generate complete design docs, reduce 70% documentation time |
| **Small Teams** | High | Standardize design, improve team collaboration |
| **Studio Designers** | Medium | Use as efficiency tool for drafts and frameworks |
| **New Designers** | High | Learn design knowledge and industry standards |
| **Producers/Investors** | Medium | Evaluate design document quality |

---

## Features

### Core Functions

#### 1. Pricing Strategy

```bash
python3 scripts/pricing_strategy.py rpg mass_market
```

- Complete price table (6 tiers: micro/small/medium/large/whale/premium)
- Regional pricing (10 major markets)
- Promotion strategies (daily/weekly/monthly/seasonal)
- Monetization model recommendations

#### 2. Publishing Operations

```bash
python3 scripts/publishing_operations.py rpg medium_budget
```

- Launch phases (pre-launch/soft/hard launch/growth/maturity)
- UA channel mix (Douyin/Tencent/Bilibili/Google/Facebook)
- KPI targets (retention/ARPU/LTV/ROI)
- Retention improvement strategies (D1/D7/D30)

#### 3. Technical Assessment

```bash
python3 scripts/technical_assessment.py rpg mid mobile medium
```

- Engine recommendations (Unity/UE/Cocos comparison)
- Server architecture (single/authoritative/MMO/hybrid)
- Performance optimization checklist
- Team configuration suggestions

#### 4. System Design

```bash
python3 scripts/system_design.py rpg combat
```

- 8 core systems (combat/progression/economy/social/exploration/narrative/customization/activity)
- UI design templates (8 interface types)
- Interaction flow design
- System loop design

#### 5. Dialogue Performance

```bash
python3 scripts/dialogue_performance.py village_elder gentle quest_give
```

- Character dialogue generation (8 types x 8 emotions)
- Storyboard design (camera sequence/emotion curve)
- Voice direction (tone/pace/volume)

#### 6. Event Configuration

```bash
python3 scripts/event_configuration.py rpg seasonal_event 2_weeks
```

- 8 event types (daily/weekly/limited/BP/seasonal/ranking/collaboration)
- Reward configuration (free/paid/whale tiers)
- Numerical balance (currency output/gacha pity)

### Modules

| Module Type | Count | Representative Modules |
|---|---|---|
| **Core Generation** | 10 | generator.py, worldview_builder.py, story_designer.py |
| **Monetization** | 5 | pricing_strategy.py, publishing_operations.py, event_configuration.py |
| **Technical** | 3 | technical_assessment.py, system_design.py, numeric_balance.py |
| **Dialogue** | 2 | dialogue_performance.py, dialogue_generator.py |
| **Knowledge** | 6 | psychology_knowledge.py, gdc_knowledge.py, market_analysis.py |
| **Learning** | 3 | auto_learner.py, feedback_learning.py, personal_learning.py |
| **Utilities** | 4 | data_analyzer.py, consistency_checker.py, version_manager.py |
| **Templates** | 5 | templates.py, templates_fps.py, templates_mobas.py |

Total: 26 core modules, 70000+ lines of code, 95000+ words of documentation

---

## Quick Start

### 1. Installation

```bash
# Clone repository
git clone https://github.com/Arshis/Arshis-Game-Design-Pro.git
cd Arshis-Game-Design-Pro

# Or download release
wget https://github.com/Arshis/Arshis-Game-Design-Pro/releases/download/v1.2.3/Arshis-Game-Design-Pro-v1.2.3.zip
unzip Arshis-Game-Design-Pro-v1.2.3.zip
```

### 2. Test Run

```bash
cd Arshis-Game-Design-Pro-release

# Test pricing strategy
python3 scripts/pricing_strategy.py rpg mass_market

# Test system design
python3 scripts/system_design.py rpg combat

# Test dialogue
python3 scripts/dialogue_performance.py village_elder gentle quest_give
```

### 3. Generate Complete Design

```bash
# Generate all modules
python3 scripts/pricing_strategy.py rpg mass_market > output/pricing.md
python3 scripts/publishing_operations.py rpg medium_budget > output/publishing.md
python3 scripts/technical_assessment.py rpg mid mobile medium > output/technical.md
python3 scripts/system_design.py rpg combat > output/combat.md
python3 scripts/worldview_builder.py generate "Project Name" > output/worldview.md

# Combine documents
cat output/*.md > complete_design.md
```

---

## OpenClaw Integration

This project is designed as an OpenClaw skill for seamless integration with the OpenClaw AI agent platform.

### What is OpenClaw?

OpenClaw is an AI agent platform that allows you to create and deploy custom skills for AI assistants. Learn more at [OpenClaw Documentation](https://docs.openclaw.ai).

### Installation as OpenClaw Skill

```bash
# Download the skill package
wget https://github.com/Arshis/Arshis-Game-Design-Pro/releases/download/v1.2.3/Arshis-Game-Design-Pro-v1.2.3.zip

# Extract to OpenClaw skills directory
unzip Arshis-Game-Design-Pro-v1.2.3.zip -d ~/.openclaw/workspace/skills/

# Verify installation
test -f ~/.openclaw/workspace/skills/Arshis-Game-Design-Pro-release/SKILL.md && echo "Installation successful"
```

### Usage in OpenClaw

Once installed, you can use the skill through OpenClaw chat:

```
# Simply ask in natural language:
"帮我生成一个 RPG 游戏的付费设计"
"生成一个战斗系统的策划案"
"帮我写一个二次元游戏的台词"
"生成一个完整的游戏策划案"
```

The skill will automatically generate professional game design documents based on your request.

### Skill Structure

```
Arshis-Game-Design-Pro-release/
├── SKILL.md # OpenClaw skill definition
├── index.js # OpenClaw plugin entry point
├── openclaw.plugin.json # Plugin configuration
├── scripts/ # 26 Python modules
└── docs/ # 11 documentation files
```

### OpenClaw Commands

```bash
# List installed skills
openclaw skills list

# Check skill status
openclaw skills status Arshis-Game-Design-Pro

# Reload skill (after updates)
openclaw skills reload Arshis-Game-Design-Pro
```

### Integration Features

- **Automatic Loading**: Skill loads automatically when OpenClaw starts
- **Natural Language**: Use natural language to request game design tasks
- **Context Aware**: Skill understands game type, audience, and requirements
- **Output Formats**: Generates Markdown documents ready for team use
- **Continuous Learning**: Learns from feedback to improve future outputs

---

## Examples

### Example 1: Pricing Report

```bash
python3 scripts/pricing_strategy.py rpg mass_market
```

Output includes:
- Complete price table with 6 tiers
- Regional pricing for 10 markets
- Promotion strategies
- Monetization model combinations

### Example 2: System Design

```bash
python3 scripts/system_design.py rpg combat
```

Output includes:
- System overview and subsystems
- UI design with 7 elements
- Interaction flow (5 steps)
- System loops (core/daily/weekly)
- Technical requirements
- Acceptance criteria

### Example 3: Dialogue

```bash
python3 scripts/dialogue_performance.py warrior angry conflict
```

Output includes:
- Character settings and traits
- Emotion expression keywords
- Specific dialogue lines (5 acts)
- Storyboard design (camera sequence)
- Voice direction (tone/pace/volume)

---

## Performance Comparison

| Task | Traditional | Arshis-Game-Design-Pro | Improvement |
|---|---|---|---|
| **Event Design** | 4-8 hours | 1-2 hours | 3-4x |
| **System Design** | 8-16 hours | 2-4 hours | 3-4x |
| **Numerical Framework** | 4-8 hours | 1-2 hours | 3-4x |
| **Writing** | 2-4 hours | 0.5-1 hour | 3-4x |
| **Competitor Analysis** | 4-8 hours | 1-2 hours | 3-4x |

---

## Supported Game Types

| Type | Support | Recommended Modules |
|---|---|---|
| **RPG** | Full | All modules |
| **MOBA** | Full | System/Dialogue/Events |
| **FPS** | Full | System/Technical/Publishing |
| **SLG** | Full | Monetization/System/Operations |
| **Anime** | Full | Dialogue/Monetization/Events |
| **Simulation** | Full | System/Numerical/Operations |
| **Roguelike** | Full | System/Gameplay/Numerical |
| **MMORPG** | Full | All modules |

---

## Project Structure

```
Arshis-Game-Design-Pro/
├── scripts/ # 26 core modules
│ ├── pricing_strategy.py # Pricing strategy
│ ├── publishing_operations.py # Publishing operations
│ ├── technical_assessment.py # Technical assessment
│ ├── system_design.py # System design
│ ├── dialogue_performance.py # Dialogue performance
│ └── ... (21 more modules)
├── docs/ # 11 core documents
│ ├── README.md # This file
│ ├── QUICK_START_v1.2.3.md # Quick start guide
│ ├── RELEASE_NOTES_v1.2.3.md # Release notes
│ └── ... (8 more documents)
├── case_studies/ # 9 case studies
└── templates/ # 8 game type templates
```

---

## Technical Details

### Requirements

- **Python**: 3.8+
- **Dependencies**: None (pure Python standard library)
- **Platform**: Windows / Linux / macOS

### Performance

- **Generation Time**: 1-3 seconds
- **Memory Usage**: <50MB
- **Output Size**: 5-10KB per report (average)

---

## FAQ

### Q1: Can I use the generated documents directly?

Yes, generates 90% complete documents. Remaining 10% requires team input for specific project parameters (budget/timeline/art assets, etc.).

### Q2: Which game types are supported?

8 major game types: RPG, MOBA, FPS, SLG, Anime, Simulation, Roguelike, MMORPG.

### Q3: Is the data reliable?

All data from authoritative sources: Sensor Tower 2026, GDC 2023-2025, MIT Media Lab, CD Projekt RED technical whitepaper.

### Q4: How to update?

Check the Releases page, download and replace with the latest version.

### Q5: Can I use it commercially?

Yes, MIT license, commercial-friendly.

### Q6: How to use with OpenClaw?

Install as OpenClaw skill and use natural language commands in chat. See [OpenClaw Integration](#openclaw-integration) for details.

---

## License

This project is licensed under the MIT License - commercial-friendly, free to use and modify.

---

## Acknowledgments

Thanks to the following research and resources:
- Sensor Tower 2026 Game Report
- GDC 2023-2025 Talk Highlights
- MIT Media Lab Research
- CD Projekt RED Technical Whitepaper
- Unity 2025 Technical Content Review
- OpenClaw Platform

---

## Contact

- **GitHub**: https://github.com/Tayllisun/Arshis-Game-Design-Pro
- **Issues**: https://github.com/Tayllisun/Arshis-Game-Design-Pro/issues
- **Email**: taylli@rpl.studio
- **OpenClaw Docs**: https://docs.openclaw.ai

---

<div align="center">

**Arshis-Game-Design-Pro v1.2.3**

Make game design more professional, efficient, and evidence-based!

If this project helps you, please give it a star!

</div>

...(truncated)...
