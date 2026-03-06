# Changelog

All notable changes to the AAA Authority Acceleration System will be documented in this file.

Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

---

## [1.1.0] - 2026-03-06

### Added — Voice DNA Skill Enhancement

Four new analysis sections across three voice DNA layers, giving the skill significantly deeper extraction capability.

#### Layer 1: Structural DNA
- **Section 5 — Transition Vocabulary**: Captures how a creator bridges between ideas, shifts topics, recovers from tangents, and maintains connective tissue across long-form content. Measures explicit bridge phrase frequency vs. implicit flow.
- **Section 6 — Closing Strategies Per Platform**: Documents how a creator ends content differently across video, LinkedIn, X, email, YouTube Shorts, and podcast formats. Distinguishes formal closes from casual trail-offs.

#### Layer 4: Narrative DNA
- **Section 5 — Evidence and Proof Patterns**: Maps how a creator supports claims — data integration style, source attribution habits, specificity level, proof hierarchy (personal testing > named data > logical reasoning), anti-proof patterns, and claim qualification frequency.

#### Layer 5: Ideological DNA
- **Section 5 — Proprietary Language and Framework Voice**: Analyzes how owned concepts, branded frameworks, and community identity markers appear organically in content. Covers frequency, natural vs. forced integration, positioning language, branded vocabulary, and trust signal connection.

### Why This Matters

Previous voice DNA extractions captured *what* someone says and *how* they say it. These additions capture three critical gaps:

1. **How ideas connect** — Transition patterns are invisible but define a creator's rhythm. Two creators can use identical vocabulary but feel completely different based on how they move between ideas.
2. **How claims land** — The difference between "AI is powerful" and "I tested 4 tools over 2 weeks and Claude outperformed on 3 of 4 tasks" is the difference between generic and authentic. Evidence patterns are a major authenticity signal.
3. **How brands breathe** — Proprietary language that feels natural builds trust. Proprietary language that feels forced breaks it. This section ensures frameworks are captured as organic vocabulary, not marketing.

### Upgrade Instructions

If you previously installed the AAA skills:

```bash
# Pull latest changes
cd aaa-authority-acceleration
git pull origin main

# Re-copy the updated skill templates
cp .claude/skills/voice-dna/resources/layer-1-structural.md ~/.claude/skills/voice-dna/resources/
cp .claude/skills/voice-dna/resources/layer-4-narrative.md ~/.claude/skills/voice-dna/resources/
cp .claude/skills/voice-dna/resources/layer-5-ideological.md ~/.claude/skills/voice-dna/resources/
```

No other files changed. Existing voice profiles remain valid — these additions enhance future extractions only.

### Impact on Existing Voice Profiles

- **No breaking changes.** Existing voice DNA profiles generated before this update continue to work.
- **Re-running `/voice-dna`** on existing content samples will now produce richer output with the four new sections.
- **Recommended**: Re-run `/voice-dna` on your highest-value client profiles to capture the additional patterns.

---

## [1.0.1] - 2026-03-05

### Security
- Removed hardcoded credentials from extraction scripts

---

## [1.0.0] - 2026-02-15

### Added
- Initial release of the AAA Authority Acceleration System
- 23 modular skills for the complete content lifecycle
- Voice Meta v2.0 with 5-layer voice DNA extraction
- Disgust Mapper for negative boundary mapping
- Authority Engine with competitor analysis suite
- Trust Signal generator with 6 E-E-A-T content types
- Airtable integration for content queue management
- n8n workflow for automated publishing
- Python extraction tools for YouTube, Kit, podcasts, and Gemini synthesis
