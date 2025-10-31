# 8090 Claude Skills

Shared Claude Code skills for the 8090 team.

## What's in This Repo

This repository contains Claude Code skills that are shared across the 8090 team. When you work in this repo, these skills are automatically available to Claude.

### Available Skills

#### 🎯 CP Writing Style (`cp-writing-style`) - v3.0.0

Expert guidance on writing in Chamath Palihapitiya's communication style across 5 formats:
- Annual Letters (2,000-5,000 words)
- Customer Briefs (500-2,000 words)
- Emails (50-200 words)
- Policy Ideas Briefs (3,000-5,000 words)
- Learn with Me Presentations (40-80 slides)

**NEW in v3.0.0**: Modular architecture with 85-90% token reduction per task through selective context loading.

Includes 10 universal principles, format-specific playbooks, templates, decision frameworks, and quality control checklists.

## How to Use

### Option 1: Work in This Repo (Recommended for Writing Tasks)

When you need to write documents following CP's style:

```bash
# Clone this repo
git clone https://github.com/8090-inc/8090-claude-skills.git
cd 8090-claude-skills

# Open Claude Code in this directory
# The skills are automatically available!
```

Ask Claude things like:
- "Help me write an annual letter"
- "Review this customer brief"
- "What format should I use for this communication?"
- "Show me the template for a policy ideas brief"

### Option 2: Copy Skills to Your Project

If you want these skills available in a different project:

```bash
# From your project directory
cp -r /path/to/8090-claude-skills/.claude/skills/* ./.claude/skills/

# Commit to your project repo
git add .claude/skills/
git commit -m "Add 8090 shared skills"
```

### Option 3: Use Personal Skills (Individual Only)

Copy to your personal skills directory to have them available everywhere:

```bash
cp -r .claude/skills/* ~/.claude/skills/
```

Note: Personal skills won't be shared with the team.

## Updating Skills

To get the latest skills:

```bash
git pull origin main
```

To contribute updates to skills, create a PR against this repo.

## Skill Details

### CP Writing Style (v3.0.0)

**When it activates**: Claude automatically uses this skill when you ask for help with writing, document review, or questions about communication formats.

**What it provides**:
- 10 Universal Writing Principles (Radical Clarity, Data Over Adjectives, Honesty First, etc.)
- Complete playbooks for 5 different formats
- Templates and annotated examples
- Decision framework for choosing the right format
- Quality control checklists

**Architecture** (v3.0.0):
- **Modular design**: 7 specialized files for selective context loading
- **85-90% token reduction** per typical task vs v2.1.0
- **Core + Format pattern**: Load `core-principles.md` + specific format module as needed

**Documentation structure**:
```
.claude/skills/cp-writing-style/
├── SKILL.md (entry point with usage instructions)
├── core-principles.md (10 Universal Principles - ALWAYS load)
├── format-customer-briefs.md (Customer Brief playbook)
├── format-emails.md (Email playbook)
├── format-annual-letters.md (Annual Letter playbook)
├── format-policy-ideas.md (Policy Ideas playbook)
├── format-learn-with-me.md (Presentation playbook)
└── quick-reference.md (Cheatsheet for quick lookups)
```

**Migration from v2.1.0**: The monolithic guide has been replaced by modular files for better LLM performance. All content preserved, just reorganized for efficiency.

## Contributing

To add or update skills:

1. Create a branch: `git checkout -b add-new-skill`
2. Add your skill to `.claude/skills/your-skill-name/`
3. Must include `SKILL.md` with proper frontmatter
4. Create a PR for team review
5. After merge, team members pull to get the update

## Skill Structure

Each skill must follow this structure:

```
.claude/skills/skill-name/
├── SKILL.md (required - with YAML frontmatter)
└── [supporting files like guides, templates, etc.]
```

The `SKILL.md` must have:
```yaml
---
name: skill-name
description: Clear description of what it does and when to use it
---
```

## Questions?

See [Claude Code Skills Documentation](https://docs.claude.com/en/docs/claude-code/skills) for more details on how skills work.
