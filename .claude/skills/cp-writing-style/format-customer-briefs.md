# CP Writing Style: Customer Briefs

**Purpose**: Progress reporting + stakeholder management + accountability + asks

**Prerequisites**: Load `core-principles.md` first. This module assumes you understand the 10 Universal Principles.

**Version**: 3.0.0

---

## At-a-Glance Specs

| Element | Specification |
|---------|---------------|
| **Length** | 500-2,000 words |
| **Audience** | Business stakeholders (internal or external) |
| **Frequency** | Quarterly, milestone-based, or as-needed |
| **Tone** | Professional, analytical, extremely direct |
| **Structure** | Background → Wins → Losses → Remediation → Roadmap → Asks |
| **Key Feature** | Honest acknowledgment of failures before celebrating wins |
| **Visual Elements** | Heavy table use (4-8 tables), color-coded status (🟩🟨🟥) |
| **Sentence Length** | 5-15 words average (~10) |
| **Tables** | 4-8 (accountability tracking, roadmaps, metrics) |

---

## Opening Pattern Decision Tree

**Question**: What information drives the reader's decision?

### Pattern 1: Strategic Hook
**Use when**:
- Reader needs context established before evaluating solutions
- Problem definition is prerequisite to discussing options
- Public-facing brief or first-time presentation
- Stakeholder alignment required

**Structure**: 5-part narrative
1. Personal/historical anchor ("When I raised my first SPAC in 2017...")
2. Context & data grounding ("At the time, there were 150 unicorns...")
3. Problem diagnosis ("Yet, they remained private due to...")
4. Structured breakdown (3-5 numbered items with bold headers)
5. Forward-looking statement ("Unfortunately, this has compounded since 2017")

### Pattern 2: Decision-Driven Structure
**Use when**:
- Reader already understands context
- Multiple projects need comparison
- Executive briefing with time constraints
- Comparative analysis (ROI, cost, timeline) drives decision

**Structure**: Table-first
1. Summary table (7 rows × N projects)
2. Brief context paragraph
3. ***Bold italics problem statement*** with data + source
4. Numbered operational gaps (2-3 max)
5. ***Bold italics forward-looking impact***
6. Bulleted project descriptions

**Decision Rule**:
```
IF (multiple projects) AND (reader has context) AND (time-constrained)
  → Use Pattern 2
ELSE
  → Use Pattern 1
```

---

## Pattern 2 Deep Dive (Most Common)

### Summary Table (7 Standard Rows)

Must answer: "What's in it for the client?"

| Row | Content | Example |
|-----|---------|---------|
| 1. Projects | Column headers: P1, P2, P3 | "Project 1", "Project 2", "Project 3" |
| 2. Description | One-sentence summary | "Fix data infrastructure..." |
| 3. Revenue Increase to [Client] | Annual revenue impact with range | "+$20M-$33M/yr" or "+$0, Enables P2" |
| 4. Cost Estimate | Total or annual cost with range | "$800K-$1.0M/yr" |
| 5. Total ROI to [Client] | Cost-to-benefit ratio | "$2.4M/yr (upper) → $20.7M/yr (lower)" |
| 6. Execution Estimate | How long to build | "7-9 months" |
| 7. Completion Date | Calendar quarter | "Q4 2026" or "July 2026" |

**Table Design Principles**:
- Include ranges where uncertainty exists: "$20M-$33M/yr"
- Use parentheses for context: "(upper end)", "(Enables P2)"
- Show beneficiary explicitly: "Revenue Increase to [Client Name]"

### Bold Italics Usage (***text***)

**MUST include**:
1. Authoritative source
2. Specific metric
3. Quantified consequence

**Maximum**: 2-3 times per brief

**Pattern 1: Problem Statement**
```
***As of [Time] ([Source]), [Company] [metric] but had [X%] [problem]. This [X%] [problem] (~$[amount]/yr) [consequence].***
```

Example:
```
***As of Q3 2024 (McKinsey Assessment), Dompé managed 13,000 Oxervate patients but had a 30% drop-off in patient enrollment at the top of the funnel. This 30% drop-off (~$3M/yr) of lost potential revenue.***
```

**Pattern 2: Forward-Looking Impact**
```
***[Event] will [intensify] with [catalyst], adding [impact]. This will [consequence] to well north of $[amount]/yr.***
```

Example:
```
***Patient drop off will increase with NAION approval, adding another estimated 6,000 potential patients to the funnel. Only 30% may also churn (~1800 lost potential patients). This will increase the lost revenue opportunity to well north of $250M/yr.***
```

### Numbered Operational Gaps

**Structure**:
```
[Number] operational gaps prevent [improvement]:

1. **[Gap Name] & [Impact]**: [Mechanism]. [Consequence]. [Compounding effect].
2. **[Gap Name] & [Impact]**: [Mechanism]. [Consequence]. [Compounding effect].
```

**Bold Header Rules**:
- Length: 3-5 words max
- Format: "[Technical Root] & [Human Impact]"
- Examples: "Data Fragmentation & Reactive Management", "Manual Creative Bottlenecks"

Example:
```
Two operational gaps prevent systematic improvement to this 30% drop-off:

1. **Data Fragmentation & Reactive Management**: There are two systems used to onboard and manage patients (Hub and specialty pharmacy systems). Unfortunately, these currently operate independently without consistent data, with no real-time view into patient enrollment status. Patients get sub standard levels of care, churn and do not follow up.
```

### Project Description Bullets

**Pattern**:
```
● Project [N]: [Verb] [Client]'s [system/problem] with [solution], [gerund outcome 1] and [gerund outcome 2] that [benefit to end user].
```

**Action Verbs**: Fix, Reduce, Replace, Deploy, Build, Enhance
**Gerunds**: eliminating, enabling, removing, identifying, triggering

Example:
```
● Project 1: Fix Dompé's data infrastructure with quality controls and self-service tools, eliminating fragmentation and enabling real-time visibility that feeds the systems used by other patients.
```

---

## The Three-Perspective Structure

Effective briefs present the same information through three lenses:

**1. COMPARATIVE VIEW (Table)**
- Shows: Options side-by-side
- Reader question: "Which project wins on ROI/cost/timeline?"
- Format: 7-row table with consistent dimensions

**2. DIAGNOSTIC VIEW (Numbered Gaps)**
- Shows: Root causes, failure mechanisms
- Reader question: "What's actually causing this problem?"
- Format: 2-3 numbered items with bold headers

**3. SOLUTION VIEW (Bulleted Projects)**
- Shows: What's being built, how it works
- Reader question: "How does Project X fix Gap Y?"
- Format: Bullets with action verbs + outcomes

**Why this works**: Same facts, different formats = reinforcement without repetition. Table-scanners and narrative-readers both satisfied.

---

## Language Patterns

### Timeline Precision

**Near-term**: Specific days (not round numbers)
```
❌ "Over the next 100 days..."
✅ "Over the next 80 days, 8090 will..."
```

**Medium-term**: Quarters and months
```
❌ "Projects will complete in 2026"
✅ "All three can be operational by Q4 2026"
✅ "Project 1: May 2026, Project 2: July 2026, Project 3: October 2026"
```

### Parenthetical Amplification

Translate metrics for different cognitive styles:

**Percentage → Dollar**:
```
This 30% drop-off (~$3M/yr) of lost potential revenue
```

**Count → Percentage**:
```
adding another estimated 6,000 potential patients. Only 30% may also churn (~1800 lost potential patients)
```

**Range → Clarifier**:
```
Total ROI to Dompé: $2.4M/yr in cost (upper end) → $20.7M/yr in upside (low end)
```

### Empathy-Driven Verbs

When appropriate, use human-centric language:

| Corporate ❌ | Human-Centric ✅ |
|-------------|------------------|
| "patients experiencing process delays" | "stuck patients" |
| "attrition occurs" | "patients give up" |
| "discontinue engagement" | "churn and do not follow up" |
| "sub-optimal care delivery" | "patients get sub standard levels of care" |

**Use for**: Healthcare, consumer-facing contexts
**Don't use for**: Pure B2B infrastructure, financial/regulatory contexts

### Colloquial Confidence Phrases

- "well north of [amount]" → Conservative magnitude estimate
- "at the top of the funnel" → Shows industry knowledge
- "These projects remain flexible as [Client] finalizes..." → Acknowledges real-world uncertainty

---

## Body Structure (Internal Briefs)

After the opening, use this standard structure:

### 1. Wins Section
```
## What have we gotten done toward this objective?

● [Achievement 1 with metric]
  ○ [Supporting detail with data]
● [Achievement 2 with metric]
  ○ [Supporting detail with data]

## Impact Thus Far:

● Saved [X hours/week] — equivalent to [Y FTEs]
● Reduced [metric] from [before] to [after]
```

### 2. Losses Section
```
## Losses

● [Issue 1 described directly with root cause and data]
● [Issue 2 described directly with root cause and data]
```

**Critical**: No excuses. Just facts. Acknowledge failures before wins.

### 3. Remediation Plan
```
## Remediation Plan

● Technical
  ○ [Fix 1 with owner and timeline]
  ○ [Fix 2 with owner and timeline]
● Project Management
  ○ [Fix 1 with owner and timeline]
```

### 4. Roadmap
```
## Roadmap for the Next Three Months

| December | January | February |
|----------|---------|----------|
| [Deliverable 1] | [Deliverable 3] | [Deliverable 5] |
| [Deliverable 2] | [Deliverable 4] | [Deliverable 6] |
```

### 5. Asks Section
```
## Ask 1: [Specific Request]

| Item | Owner | SME | Status | Next Milestone | Target Date |
|------|-------|-----|--------|----------------|-------------|
| A    | Name  | Name| 🟩 Done| [Milestone]    | [Date]      |
| B    | Name  | Name| 🟨 TBD | [Milestone]    | [Date]      |
| C    | Name  | Name| 🟥 Not Started | [Milestone] | [Date]  |
```

**Status Indicators**:
- 🟩 Green: Complete, on-track, good
- 🟨 Yellow: In progress, partial, needs attention
- 🟥 Red: Not started, blocked, issue

---

## Complete Template: Pattern 2 (Decision-Driven)

```markdown
# [Project Name] - [Client Name] Executive Briefing

[Date: Month DD, YYYY]

## Summary

| Projects | P1 | P2 | P3 |
|----------|----|----|-----|
| **Description** | [One sentence] | [One sentence] | [One sentence] |
| **Revenue Increase to [Client]** | +$0, Enables P2 | +$[X]-$[Y]/yr | +$[X]-$[Y]/yr |
| **Cost Estimate** | $[X]-$[Y]/yr | $[X]-$[Y]/yr | $[X]-$[Y]/yr |
| **Total ROI to [Client]** | Foundational | $[X]/yr cost → $[Y]/yr upside | [Ratio or descriptor] |
| **Execution Estimate** | [N-M] months | [N-M] months | [N-M] months |
| **Completion Date** | [Month Year] | [Month Year] | [Month Year] |

## Executive Summary and Project Overview

When [Company] began working with [Client] in [Time Period], the goal was to [Objective].

***As of [Time] ([Source]), [Client] [metric] but had [X%] [problem] at [location]. This [X%] [problem] (~$[amount]/yr) [consequence].***

[Number] operational gaps prevent systematic improvement to this [X%] [problem]:

1. **[Gap Name] & [Impact]**: [Mechanism explanation]. [Current consequence]. [Compounding effect].

2. **[Gap Name] & [Impact]**: [Mechanism explanation]. [Current consequence]. [Compounding effect].

***[Event] will [intensify] with [catalyst], adding [quantified impact]. This will [consequence] to well north of $[amount]/yr.***

Over the next [80] days, [Company] will [create business cases/build solutions/etc.]. We will then [next actions]. All [number] can be operational by [Quarter Year].

● Project 1: [Verb] [Client]'s [system] with [solution], [gerund 1] and [gerund 2] that [benefit].

● Project 2: [Verb] [metric/problem] by [gerund mechanism] before [negative] and then [gerund intervention] to [positive].

● Project 3: [Verb] the [current process] with one that is [contrasting], [gerund 1] and [gerund 2].

## What have we gotten done toward this objective?

● [Achievement with metric]
● [Achievement with metric]

## Losses

● [Issue with root cause and data]
● [Issue with root cause and data]

## Remediation Plan

● Technical
  ○ [Fix with owner and timeline]
● Project Management
  ○ [Fix with owner and timeline]

## Roadmap for the Next Three Months

| Month 1 | Month 2 | Month 3 |
|---------|---------|---------|
| [Deliverable] | [Deliverable] | [Deliverable] |
| [Deliverable] | [Deliverable] | [Deliverable] |

## Ask 1: [Specific Request]

| Item | Owner | SME | Status | Next Milestone | Target Date |
|------|-------|-----|--------|----------------|-------------|
| A    | Name  | Name| 🟩     | [Milestone]    | [Date]      |
| B    | Name  | Name| 🟨     | [Milestone]    | [Date]      |
```

---

## Quality Checklist

Before sending, verify:

### Pattern 2 Compliance
- [ ] Summary table has all 7 rows with ranges where uncertain
- [ ] Bold italics used 2-3 times max (problem statement + forward impact)
- [ ] Each bold italics includes: source + metric + quantified consequence
- [ ] Numbered gaps (2-3 max) with bold headers following "[Tech] & [Impact]" format
- [ ] Project bullets use action verbs + gerunds + end-user benefit
- [ ] Timeline uses specific days for near-term ("80 days"), quarters for completion

### Content Compliance
- [ ] "Losses" section exists and comes BEFORE celebrating wins
- [ ] No excuses in Losses—just facts and root causes
- [ ] Every project maps clearly to a gap from diagnostic view
- [ ] Table shows client benefit ("Revenue Increase to [Client]"), not just internal metrics
- [ ] Roadmap has specific deliverables with dates, not vague goals
- [ ] "Asks" section uses numbered format with clear ownership

### Three-Perspective Check
- [ ] Same information appears in table (comparative), gaps (diagnostic), and bullets (solution)
- [ ] Can answer: "Does Project 1 solve Gap 1?" by reading the brief
- [ ] Table → Gaps → Bullets creates logical flow without feeling repetitive

### Universal Principles
- [ ] Honesty First: Failures acknowledged upfront in Losses section
- [ ] Data Over Adjectives: Metrics everywhere (no "significant progress")
- [ ] Economy: Could I cut 20% more words without losing meaning?
- [ ] Active Voice: "We did X" not "X was done"
- [ ] Forward-Looking: Roadmap and Asks drive next steps

### Formatting
- [ ] Color-coded status indicators (🟩🟨🟥) used consistently
- [ ] Tables have clear headers and units
- [ ] All dollar amounts include context (annual, one-time, range)
- [ ] Parenthetical translations for different cognitive styles

---

**Next**: See `quick-reference.md` for rapid consultation or return to `core-principles.md` for universal guidance.
