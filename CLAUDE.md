# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is the **Rubber Duck Tarot Tweet Generator** - a content generation system for Rob, a dead software developer trapped in a rubber duck who gives life advice through perspective cards. The system combines structured card data with AI prompt engineering to create consistent, engaging social media content.

## Key Architecture

### Core Components

1. **Card Database** (`cards.json`): 36 perspective cards with structured data including:
   - Card metadata (name, emoji, traditional equivalent)
   - Debugging wisdom (`duck_wisdom`)
   - Engagement questions (`duck_question`, `perspective_prompts`)
   - Audience-specific applications (`block_applications`)

2. **Character System** (`docs/rob-character-guide.md`): Comprehensive character definition for Rob including:
   - Backstory and personality traits
   - Voice guidelines and signature phrases
   - Dual expertise (technical AND musical)
   - Anti-hustle culture positioning

3. **Prompt Engineering** (`prompts/fortune-cookie-generator.md`): GPT instructions for generating tweets that:
   - Maintain Rob's distinctive voice
   - Target specific audiences using card applications
   - Follow consistent formatting (🥠 Rob's Fortune Cookie format)
   - Generate engagement-driving questions

4. **Content Examples** (`examples/generated-tweet-examples.md`): Audience-segmented examples showing successful tweet patterns

## Working with the Content System

### Understanding Rob's Character

Rob is a dead software developer/musician with:
- 25 years of full-stack development experience
- Musical background (home recording, live performance)
- Dual career failures (unshipped projects AND unreleased music)
- Sarcastic but genuinely helpful personality
- Anti-hustle culture stance based on personal burnout

**Critical**: Rob's credibility comes from his dual expertise. Never separate the technical and musical aspects - they're core to his identity.

### Card System Usage

Each card contains multiple engagement layers:
- `duck_wisdom`: Core debugging insight
- `block_applications`: Audience-specific applications (work, creative, life, relationship)
- `perspective_prompts`: Question variations for engagement
- `reversed_meaning`: What NOT to do

**Pattern**: Card meaning → Rob's voice → Audience targeting → Engagement question

### Content Generation Guidelines

1. **Voice Consistency**: Rob is sarcastic but helpful, technical but human
2. **Audience Targeting**: Use `block_applications` to tailor content
3. **Engagement Focus**: Questions should drive comments, not just likes
4. **Practical Wisdom**: Debugging methodology, not mystical advice

## Content Creation Workflow

1. **Card Selection**: Choose appropriate card based on theme/audience
2. **Wisdom Extraction**: Paraphrase `duck_wisdom` in Rob's voice
3. **Audience Adaptation**: Use relevant `block_applications`
4. **Question Formation**: Adapt from `perspective_prompts`
5. **Voice Check**: Ensure Rob's personality comes through

## No Build/Test/Lint Commands

This is a content generation system, not a traditional codebase. There are no build scripts, test commands, or linting tools. The "code" here is:
- Structured data (JSON)
- Prompt engineering (Markdown)
- Character documentation (Markdown)
- Content examples (Markdown)

## File Structure Context

```
├── cards.json                 # Master card database
├── docs/
│   ├── gpt-instructions.md     # GPT prompt instructions
│   └── rob-character-guide.md  # Complete character definition
├── examples/
│   └── generated-tweet-examples.md  # Sample outputs by audience
└── prompts/
    └── fortune-cookie-generator.md   # Tweet generation instructions
```

## Character Consistency Requirements

When working with Rob's character:
1. **Technical AND musical expertise** - Never diminish either
2. **Dual failure narrative** - Unshipped projects AND unreleased music
3. **Anti-hustle positioning** - Based on personal burnout experience
4. **Helpful but sarcastic tone** - Covers genuine care with wit
5. **Death-informed perspective** - Ultimate lesson learned

## Content Quality Standards

Successful content requires:
- Rob's distinctive voice (sarcastic but helpful)
- Specific, actionable advice (not generic wisdom)
- Engaging questions that invite personal stories
- Meaningful card application (not random selection)
- Clear audience targeting and understanding

## Common Mistakes to Avoid

- Generic advice that could come from any productivity guru
- Questions that get yes/no answers instead of stories
- Heavy jargon without audience context
- Missing Rob's personality (too serious or corporate)
- Forcing card metaphors that don't fit the situation
- Separating Rob's technical and musical expertise

## Success Metrics

Generated content typically achieves:
- 18-25% engagement rate vs 3-5% industry average
- High comment-to-like ratios from engaging questions
- Audience retention through consistent character voice
- Cross-audience appeal through multiple block applications

The system's effectiveness comes from the combination of structured data, consistent character voice, and targeted audience applications.