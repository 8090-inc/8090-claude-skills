# CP Writing Style Skill - Installation Guide

## Package Information

- **Skill Name**: cp-writing-style
- **Version**: 3.0.0
- **Size**: 35KB (compressed), ~100KB (uncompressed)
- **Files**: 8 markdown files (SKILL.md + 7 content modules)

## Installation Instructions

### For Claude Native Client (Desktop App)

1. **Download the zip file**: `cp-writing-style.zip`

2. **Install the skill**:
   - Open Claude desktop app
   - Go to Settings → Skills (or Skills Manager)
   - Click "Import Skill" or "Add Custom Skill"
   - Select `cp-writing-style.zip`
   - The skill will be automatically extracted and installed

3. **Verify installation**:
   - The skill should appear in your skills list as "cp-writing-style"
   - You can invoke it by typing `/cp-writing-style` or selecting it from the skills menu

### Manual Installation (Alternative)

If you prefer manual installation:

1. Extract `cp-writing-style.zip`
2. Copy the `cp-writing-style/` folder to your Claude skills directory:
   - **macOS**: `~/.claude/skills/`
   - **Windows**: `%USERPROFILE%\.claude\skills\`
   - **Linux**: `~/.claude/skills/`
3. Restart Claude if it's running

## Usage

Once installed, invoke the skill when you need help with writing:

```
/cp-writing-style
```

Or simply activate it from the skills menu. The skill provides:

- **10 Universal Principles** for clear communication
- **5 Format-Specific Playbooks**:
  - Annual Letters
  - Customer Briefs
  - Emails
  - Policy Ideas Briefs
  - Learn with Me Presentations
- **Templates and decision frameworks**
- **Quality control checklists**

## What's Included

1. **SKILL.md** - Skill manifest and entry point
2. **core-principles.md** - 10 universal principles (always loaded)
3. **format-customer-briefs.md** - Customer brief playbook
4. **format-emails.md** - Email playbook
5. **format-annual-letters.md** - Annual letter playbook
6. **format-policy-ideas.md** - Policy ideas playbook
7. **format-learn-with-me.md** - Presentation playbook
8. **quick-reference.md** - Quick lookup cheatsheet

## Features

- **Modular Architecture**: Loads only relevant content for your task (85-90% token savings)
- **3-Pass Writing Method**: Write to think → Apply principles → Cut 30%
- **Data Integrity**: Never fabricates data - uses bracketed placeholders when missing
- **Decision Frameworks**: Helps choose the right format and approach
- **Quality Control**: Built-in checklists ensure complete application

## Support

For issues or questions about this skill, refer to the project repository or Claude Code documentation.

---

**Last Updated**: 2025-10-30
**Skill Version**: 3.0.0
