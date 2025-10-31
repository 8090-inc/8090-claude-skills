---
name: cp-writing-style
version: 3.0.0
lastUpdated: 2025-10-30
description: Expert guidance on writing in Chamath Palihapitiya's communication style across 5 formats (Annual Letters, Customer Briefs, Emails, Policy Ideas Briefs, Learn with Me Presentations). Use when helping with any writing task, document creation, editing, reviewing communications, or answering questions about how to write something. Includes 10 universal principles, format-specific playbooks, templates, decision frameworks, and quality control checklists. MODULAR ARCHITECTURE: Optimized for LLM consumption with selective context loading (core + format).
changelog: |
  v3.0.0 (2025-10-30): **MAJOR ARCHITECTURAL REDESIGN** - Transformed from monolithic 28.9K word guide to modular system optimized for LLM consumption. Created 7 specialized files (core-principles.md + 5 format modules + quick-reference.md) totaling ~9.3K words. ELIMINATED Section 4 (100% redundant). Customer Briefs section reduced 75% (1,700 lines → 400 lines) while preserving all actionable insights. Added MUST/SHOULD/MAY hierarchy to every principle. Added "When to Deviate" guidance. Created decision trees throughout. Token reduction: 85-90% per typical task (54K → 4.5-8K tokens). See MIGRATION-GUIDE.md for complete mapping from v2.1.0 to v3.0.0.
  v2.1.0 (2025-10-30): Added "The Prolific Cutting Rule" subsection to Principle 5 (Economy of Language) with three-stage cutting method targeting 50-80% reduction from first draft. Includes concrete before/after example showing progressive editing from corporate jargon (240 words) → first cut (85 words) → final cut (47 words). Added corporate jargon elimination list and balance principles for when NOT to cut.
  v2.0.0 (2025-10-30): Added Section 3.6 Progress Update Briefs with 4 core editing principles, timeline table patterns, thematic statement structure, and strategic language translation framework.
  v1.0.0 (2024-10-27): Initial comprehensive style guide with 10 universal principles and 5 format playbooks.
---

# CP Writing Style Guide v3.0.0

This skill provides comprehensive guidance on writing in Chamath Palihapitiya's distinctive communication style using a **modular, LLM-optimized architecture**.

## When to Use This Skill

Claude should invoke this skill when:
- User asks for help writing any type of document
- User requests document review or editing
- User asks "how should I write..." or "what format should I use..."
- User mentions any of the 5 formats: Annual Letters, Customer Briefs, Emails, Policy Ideas Briefs, or Learn with Me Presentations
- User asks about writing style, tone, structure, or formatting
- User needs templates or examples for business communications

## What's New in v3.0.0 (BREAKING CHANGES)

### Architectural Redesign
- **From**: Single 28.9K word file (54K tokens)
- **To**: 7 modular files totaling 9.3K words (4.5-8K tokens per task)
- **Reduction**: 68% total, 85-90% per typical use case
- **Performance**: Selective context loading based on task type

### New Modular File Structure
```
core-principles.md (~3K words) - ALWAYS LOAD
format-customer-briefs.md (~1.5K words) - Load for customer briefs
format-emails.md (~800 words) - Load for emails
format-annual-letters.md (~1K words) - Load for annual letters
format-policy-ideas.md (~1K words) - Load for policy briefs
format-learn-with-me.md (~1K words) - Load for presentations
quick-reference.md (~1K words) - Optional cheatsheet
```

### Major Improvements
1. **MUST/SHOULD/MAY hierarchy** explicit on all 10 principles
2. **"When to Deviate" guidance** for each principle
3. **Decision trees** throughout (format selection, pattern choice)
4. **At-a-glance specs tables** for every format
5. **Self-contained modules** - each format independently loadable
6. **Flatter hierarchy** - Max 3 header levels (vs 4 in v2.1.0)
7. **Eliminated redundancy** - Section 4 removed (100% duplicate)

## How to Use This Skill (v3.0.0)

### CRITICAL: Modular Loading Pattern

**ALWAYS follow this sequence:**

1. **Load core-principles.md first** (REQUIRED for every task)
   - Contains: 10 Universal Principles, format decision tree, banned/golden phrases, meta-rules

2. **Load appropriate format module** based on task:
   - Writing customer brief? → Load `format-customer-briefs.md`
   - Writing email? → Load `format-emails.md`
   - Writing annual letter? → Load `format-annual-letters.md`
   - Writing policy ideas? → Load `format-policy-ideas.md`
   - Creating presentation? → Load `format-learn-with-me.md`

3. **Optionally load quick-reference.md** for spot checks

### Response Format

**IMPORTANT**: When this skill is invoked, ALWAYS begin your response with:
```
Using CP Writing Style Guide v3.0.0 - Modular Architecture
Loaded: core-principles.md + [format-module-name]
```

### Example Usage

**Task: Help user write a customer brief**
```
Response starts with:
"Using CP Writing Style Guide v3.0.0 - Modular Architecture
Loaded: core-principles.md + format-customer-briefs.md"

[Then provide guidance using the loaded modules]
```

**Task: Help user write an email**
```
Response starts with:
"Using CP Writing Style Guide v3.0.0 - Modular Architecture
Loaded: core-principles.md + format-emails.md"

[Then provide guidance using the loaded modules]
```

## The 10 Universal Principles (Quick Reference)

**🚨 CRITICAL: NEVER FABRICATE DATA 🚨**
When applying Principle 2 (Data Over Adjectives), you can ONLY use data from the original source material. If data is missing, use bracketed placeholders `[Need: description]` or state "data not available." Fabricated numbers are worse than vague language.

1. **Radical Clarity**: Say it simpler [MUST]
2. **Data Over Adjectives**: Show numbers from source, not descriptions [MUST] - NEVER INVENT DATA
3. **Honesty First**: Acknowledge failures upfront [MUST]
4. **First-Principles Thinking**: Explain from fundamentals [SHOULD]
5. **Economy of Language**: Cut every wasted word [MUST]
6. **Active Voice**: People do things [MUST]
7. **Context Provision**: Always explain "why" [MUST]
8. **Attribution**: Credit sources [SHOULD]
9. **Forward-Looking**: Point to next, drive outcomes [MUST]
10. **Format Follows Function**: Structure serves message [SHOULD]

*See `core-principles.md` for detailed explanations, examples, and "When to Deviate" guidance.*

## 5 Complete Format Playbooks

### 1. Annual Letters (2,000-5,000 words)
- **Purpose**: Strategic reflection + performance reporting
- **Audience**: Investors/public
- **Key Feature**: Frontload performance data (no hiding)
- **Load**: `format-annual-letters.md`

### 2. Customer Briefs (500-2,000 words)
- **Purpose**: Progress reporting + stakeholder management
- **Audience**: Business stakeholders (internal or external)
- **Key Feature**: Losses before wins, heavy tables, color-coded status
- **Load**: `format-customer-briefs.md`
- **Patterns**: Pattern 1 (Strategic Hook) vs Pattern 2 (Decision-Driven)

### 3. Emails (50-200 words)
- **Purpose**: Quick tactical communication
- **Audience**: Colleagues, team members
- **Key Feature**: Single purpose only, minimal formatting
- **Load**: `format-emails.md`
- **Types**: Philosophy sharing, Personnel changes, Directives

### 4. Policy Ideas Briefs (3,000-5,000 words)
- **Purpose**: Policy recommendations + implementation plans
- **Audience**: Policymakers, decision-makers
- **Key Feature**: 70-80% bullets, imperative verbs
- **Load**: `format-policy-ideas.md`

### 5. Learn with Me Presentations (40-80 slides)
- **Purpose**: Educational deep-dives on complex topics
- **Audience**: Learners, curious audience
- **Key Feature**: Visual-first, one idea per slide
- **Load**: `format-learn-with-me.md`

## Key Decision Framework

```
Purpose: Quick tactical → Email (50-200 words)
Purpose: Progress update → Customer Brief (500-2,000 words)
Purpose: Strategic reflection → Annual Letter (2,000-5,000 words)
Purpose: Policy recommendations → Policy Ideas Brief (3,000-5,000 words)
Purpose: Educational deep-dive → Learn with Me (40-80 slides)
```

*See `core-principles.md` for complete decision tree with detailed criteria.*

## File Reference

| File | Purpose | When to Load |
|------|---------|--------------|
| `core-principles.md` | 10 Universal Principles + decision tree | ALWAYS (required) |
| `format-customer-briefs.md` | Customer brief playbook | Writing customer briefs |
| `format-emails.md` | Email playbook (3 types) | Writing emails |
| `format-annual-letters.md` | Annual letter playbook | Writing annual letters |
| `format-policy-ideas.md` | Policy ideas playbook | Writing policy briefs |
| `format-learn-with-me.md` | Presentation playbook | Creating presentations |
| `quick-reference.md` | Cheatsheet (tables, checklists) | Quick lookups |
| `MIGRATION-GUIDE.md` | v2.1.0 → v3.0.0 mapping | Understanding changes |
| `cp-writing-style-guide.md` | v2.1.0 (legacy, preserved) | Backward compatibility |

## What Got Eliminated in v3.0.0

**Section 4: The 5-Part Framework Deep Dive**
- **Why**: 100% redundant with Format Playbooks (Section 3)
- **Status**: Content integrated into individual format modules
- **Benefit**: Eliminated ~5K words of duplicate content

## Token Efficiency Comparison

| Task Type | v2.1.0 Tokens | v3.0.0 Tokens | Reduction |
|-----------|---------------|---------------|-----------|
| Email | ~54K | ~6.5K | 88% |
| Customer Brief | ~54K | ~8K | 85% |
| Annual Letter | ~54K | ~7K | 87% |
| Policy Ideas | ~54K | ~8K | 85% |
| Learn with Me | ~54K | ~8K | 85% |

*v2.1.0: Always loaded entire 28.9K word guide (~54K tokens)*
*v3.0.0: Selective loading (core + one format = 4.5-8K tokens)*

## Backward Compatibility

**v2.1.0 file status**: Preserved as `cp-writing-style-guide.md`
- Legacy users can continue using v2.1.0
- v3.0.0 files created alongside (not replacing)
- See `MIGRATION-GUIDE.md` for detailed section mapping

## Migration Path

If you're familiar with v2.1.0:
1. Read `MIGRATION-GUIDE.md` for section mapping
2. Learn new modular loading pattern (core + format)
3. Review at-a-glance specs tables in each format module
4. Familiarize with MUST/SHOULD/MAY hierarchy
5. Use `quick-reference.md` for rapid lookups

---

**For detailed guidance**: Load the appropriate module files based on your task.
**For migration help**: See `MIGRATION-GUIDE.md`
**For quick lookups**: See `quick-reference.md`
