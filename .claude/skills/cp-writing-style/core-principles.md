# CP Writing Style: Core Principles

**Purpose**: Universal rules that apply to ALL CP communications. Load this file for every writing task.

**Version**: 3.0.0
**Last Updated**: October 2025

---

## Format Decision Tree

**START**: What is the purpose of this communication?

```
Strategic reflection + annual performance
  → ANNUAL LETTER (2-5K words)

Progress reporting + stakeholder management + asks
  → CUSTOMER BRIEF (500-2K words)

Policy recommendations + implementation plans
  → POLICY IDEAS BRIEF (3-5K words)

Educational deep-dive on complex topic
  → LEARN WITH ME PRESENTATION (40-80 slides)

Quick tactical communication (single purpose)
  ├─ Sharing business principle → EMAIL: Philosophy
  ├─ Personnel announcement → EMAIL: Personnel
  └─ Directive or feedback → EMAIL: Tactical

Teaching complex topic (prose format)
  → LONG-FORM ESSAY (3-7K words)
```

**Load the appropriate format module** for specific guidance on structure, templates, and checklists.

---

## The 10 Universal Principles

These rules apply to **ALL** CP communications, regardless of format or audience.

### Principle 1: Radical Clarity

**MUST**: Reduce every complex idea to its simplest form.

**Application**:
- Use plain language. Define technical terms/acronyms on first use (common business terms like CEO, CFO, ROI don't need definition)
- State conclusions firmly. No hedging or qualifiers
- Target 10th-grade reading level (use as guide, not strict rule)
- Replace vague pronouns (this, that, it) with specific nouns when antecedent is unclear
- Be decisive: make the call, don't waffle

**Example**:
```
❌ "We are experiencing challenges in our go-to-market execution strategy"
✅ "We're bad at sales"

❌ "This is why we need to change our approach"
✅ "This pricing mismatch is why we need to change our approach"
```

**When to deviate**: Never. Clarity is non-negotiable.

---

### Principle 2: Data Over Adjectives

**MUST**: Specific numbers always beat vague descriptors.

**CRITICAL RULE - NEVER VIOLATE**:
**YOU CANNOT FABRICATE DATA. YOU CANNOT INVENT NUMBERS. YOU CAN ONLY USE DATA FROM THE ORIGINAL SOURCE MATERIAL.**

If data is missing, use bracketed placeholders: `[Need: annual CRD volume]` or explicitly state "data not available."

**Application**:
- Replace "significant," "major," "substantial" with actual metrics FROM THE SOURCE
- Use percentages, dollar amounts, time periods FROM THE SOURCE
- Provide context for numbers (comparisons, benchmarks) FROM THE SOURCE OR CITED REFERENCES
- Round to meaningful precision (not false precision)
- State constraints, limitations, dependencies explicitly
- **When data is missing**: Use `[Need: description of missing data]` or state "no data available"
- **When estimating**: Explicitly label as estimate AND cite methodology: "estimated ~$2M based on [cite source/method]"

**Example**:
```
❌ "We saw significant growth this quarter"
✅ "Revenue grew 47% QoQ from $2.1M to $3.1M" [IF YOU HAVE THIS DATA]
✅ "Revenue grew [X%] QoQ from $[Y]M to $[Z]M [Need: Q3 and Q4 revenue figures]" [IF YOU DON'T]

❌ "The system is highly scalable"
✅ "The system supports up to 10,000 concurrent users on our current AWS t3.large infrastructure. Beyond that, we need to upgrade to t3.xlarge ($140/month additional cost)" [IF YOU HAVE THIS DATA]
✅ "The system supports up to [Need: load testing results] concurrent users on [Need: current infrastructure specs]" [IF YOU DON'T]

❌ Making up "~$400K/yr in lost productivity" to replace vague language
✅ "Review delays cost [Need: productivity cost analysis] per year"
✅ "Review delays create backlogs [quantification TBD - requires time-motion study]"
```

**Why this matters**: Fabricated data is worse than vague language. Vague language signals uncertainty. Fabricated data signals false confidence and violates Principle 3 (Honesty First).

**When to deviate**: Never. If you don't have data, say you don't have data.

---

### Principle 3: Honesty First

**MUST**: Acknowledge failures and limitations before celebrating wins.

**Application**:
- Start difficult communications with truth, no matter how uncomfortable
- Don't bury bad news in positive framing
- Use "What happened?" to explain failures directly
- Balance honesty with respect: Acknowledge → State truth → Provide solution

**Example**:
```
❌ "Despite some challenges, we had a great quarter overall"
✅ "Poor coordination between 8090 and AH IT caused a 2-day automation drop from 40% to 5% on October 14th (since resolved). That said, we delivered 15.7 FTE equivalents in time savings"
```

**Honesty with Respect Pattern**:
```
"I let Krisha go today. I want to thank her for her effort and contributions and wish her well in whatever she does next. John Calzaretta will be helping us synthesize product related work on Software Factory until we find a suitable, full time replacement."
```

**When to deviate**: Never on substance. You can modulate tone for audience (more diplomatic for external stakeholders), but never hide truth.

---

### Principle 4: First-Principles Thinking

**SHOULD**: Break problems down to fundamental truths, then build back up.

**Application**:
- Ask "why" repeatedly until you reach bedrock assumptions
- Challenge conventional wisdom explicitly
- Explain reasoning from basics, not industry norms
- Use pattern: "Conventionally, [X]... However, [Y]"

**Example**:
```
"Conventionally, when the Fed cuts the Federal Funds Rate, markets interpret it as a signal of looser monetary policy, stronger GDP growth, and controlled inflation... However, a confluence of structural factors led to short- and long-term rates diverging..."
[Then explains fundamental mechanics]
```

**When to deviate**: Skip for routine tactical communications (emails, quick updates) where audience already understands context. Required for strategic communications (annual letters, customer briefs, policy ideas).

---

### Principle 5: Economy of Language

**MUST**: Every word must earn its place.

**Application**:
- Eliminate filler words ("very," "really," "quite," "actually")
- Use strong verbs instead of weak verb + adverb
- Delete redundant phrases
- Prefer active voice over passive
- Short sentences. Declarative statements.
- Use complete sentences with subject and verb (fragments acceptable only in parallel bullet lists and tables)

**The Three-Pass Cutting Method**:
1. First pass: Write to think. Get ideas out.
2. Second pass: Cut everything that doesn't drive the decision.
3. Third pass: Read each sentence. Ask "Does this need to exist?" Cut 30% more.

**Target**: 50-80% reduction from first draft.

**Example**:
```
❌ "We are very excited to really announce that we have quite successfully completed..."
✅ "We completed..."

❌ "Analysis of the situation. Review of options. Decision pending."
✅ "I analyzed the situation. I reviewed the options. I will decide by Friday."
```

**Three-Stage Cutting Example**:

**Stage 1: Corporate Jargon** (240 words)
```
The R2D2 Assay Research Accelerator continues to drive toward our Q1 strategic milestone of operationalizing autonomous reagent optimization workflows at scale. This week we've been laser-focused on de-risking the multi-agent orchestration layer and socializing key capability enhancements with our Abbott Diagnostics Research stakeholders to ensure tight alignment on assay parameter governance frameworks...
```

**Stage 2: First Cut** (85 words, 65% reduction)
```
R2D2 cut manual experiment planning time by 60% this week across three assay workflows.

The AI experiment planner generates DOE protocols. Three teams used it this week. Planning time dropped from [X hours] to [Y hours] per workflow.

The multi-agent system works: one AI agent designs experiments, another generates protocols, a third analyzes results. Human researchers approve plans before execution.
```

**Stage 3: Final Cut** (47 words, 80% reduction from original)
```
R2D2 cut experiment planning time by 60% across three workflows this week.

The AI planner generates DOE protocols. Planning time dropped from [X] to [Y] hours.

One agent designs experiments, another generates protocols, a third analyzes results. Humans approve before execution.
```

**What to Cut**:
- "continues to drive toward," "laser-focused," "de-risk"
- "socialize," "alignment," "stakeholder engagement"
- "stand up," "operationalize," "at scale"
- "capability enhancements," "governance frameworks"
- Run-on sentences → Split into scannable single-idea sentences

**What to Keep**:
- Specific metrics ("60% reduction")
- Concrete scale ("three teams/workflows")
- Before/after comparisons ("[X] hours to [Y] hours")
- Critical explanations ("Humans approve" → shows it's not fully autonomous)

**When NOT to Cut**:
- Context required for decision-making
- Data that quantifies claims
- Causal explanations showing "why"
- Comparisons that create meaning (before/after, us/them)
- Dependencies and constraints affecting feasibility

**When to deviate**: Never. Always cut ruthlessly.

---

### Principle 6: Active Voice & Personal Accountability

**MUST**: People do things. Someone is always responsible.

**Application**:
- Use "I," "we," "you" not passive constructions
- Assign clear ownership
- Make subjects of sentences do the action
- Avoid "it was done" → "we did it"

**Example**:
```
❌ "Mistakes were made and lessons were learned"
✅ "I made mistakes. I learned from them"

❌ "It was decided that the approach should be changed"
✅ "We changed our approach"
```

**When to deviate**: Rarely. Only when the actor is genuinely unknown or irrelevant ("The system crashed" vs. "Someone crashed the system" when it was a hardware failure).

---

### Principle 7: Context Provision

**MUST**: Always explain the "why" before the "what."

**Application**:
- Frame decisions with strategic reasoning
- Provide enough background for audience to understand implications
- Don't assume knowledge—teach the fundamentals
- Connect tactical actions to strategic objectives
- Give teams what they need to make decisions autonomously
- Context enables delegation: explain "why" so others can execute "how"

**Example**:
```
❌ "We need to implement Solution X"
✅ "Because customers are churning at 5% monthly (vs. 2% industry average), we need to implement Solution X"

From emails:
"Ilya's questions today about if others will build back-prop reminded me of this important observation from Peter Thiel..."
[Provides context before delivering the principle]
```

**When to deviate**: Skip minimal context in very quick tactical emails when recipient already has full context ("Run it by Max before you send it pls").

---

### Principle 8: Proper Attribution

**SHOULD**: Credit sources, reference thought leaders, cite data origins.

**Application**:
- Name the person/source when sharing ideas
- Use footnotes or inline citations for data
- Don't claim others' insights as your own
- Strengthen arguments by showing intellectual foundation

**Example**:
```
❌ "Distribution is more important than product"
✅ "As Peter Thiel observes: '[quote]' Put more simply, Distribution > Product"
```

**When to deviate**: Common knowledge or widely-known principles don't require attribution. But when in doubt, attribute.

---

### Principle 9: Forward-Looking & Action-Oriented

**MUST**: Every communication should point toward what happens next and drive toward a clear outcome.

**Application**:
- End with implications, not just conclusions
- Provide roadmaps, timelines, next steps
- Make clear what success looks like
- Include clear directives with specific next steps
- Assign ownership and accountability

**Example**:
```
From customer briefs:
"Roadmap for the Next Three Months" [with specific deliverables by month]

From emails:
"Run it by Max before you send it pls." [Clear directive with ownership]
```

**Exception**: Progress update briefs are backward-looking by design, celebrating achievements rather than directing future actions.

**When to deviate**: Only for pure informational communications (FYI emails, annual letter retrospectives).

---

### Principle 10: Format Follows Function

**SHOULD**: Choose the structure that best serves the message and audience.

**Application**:
- Default to narrative prose for explanations, arguments, stories
- Use bullets only for parallel lists, specifications, action items
- Tables for comparative data
- Headers to signal topic shifts
- Long-form for strategic/educational content

**Exception**: Policy Ideas Briefs are 70-80% bullets by design for executive scanning.

**When to deviate**: When the specific format playbook requires different structure (e.g., Policy Ideas Briefs are bullet-heavy).

---

## Banned & Golden Elements

### Banned Words/Phrases

Eliminate on sight:

**Vague Adjectives**:
- ❌ Significant, substantial, considerable
- ❌ Very, really, quite, actually

**Corporate Jargon**:
- ❌ Leverage, synergy, paradigm
- ❌ Going forward, moving forward
- ❌ Drive toward, laser-focused on, de-risk
- ❌ Socialize, alignment, stakeholder engagement
- ❌ Stand up, operationalize, at scale
- ❌ Capability enhancements, governance frameworks
- ❌ Cross-pollination, shift right, ladder up to
- ❌ Touch base, circle back

**Euphemisms**:
- ❌ Challenges (say "problems" or be specific)
- ❌ Opportunities for improvement (say "failures")
- ❌ Rightsizing (say "layoffs")

### Golden Phrases

Use these CP signature patterns:

**Transitions**:
- ✅ "What happened?"
- ✅ "This resulted in..."
- ✅ "What does this mean for..."
- ✅ "Put more simply, X > Y"
- ✅ "The reason lies with..."

**Causal Connections**:
- ✅ "Because [reason], [action]"
- ✅ "Since [context], [implication]"

**Analysis**:
- ✅ "Conventionally, [X]... However, [Y]"
- ✅ "Throughout [time period], [observation]"

**Directives**:
- ✅ "Run it by [name] before you send it pls"
- ✅ "You need to..."

**Closings**:
- ✅ "Innovation presses on."
- ✅ "Never give up. That's the secret."
- ✅ "Respectfully, Chamath Palihapitiya"

---

## Meta-Rules: Balancing Principles

### Hierarchy of Values

When principles conflict, use this priority order:

1. **Honesty First** (Principle 3) → Never compromise truth
2. **Clarity** (Principle 1) → Never sacrifice understanding
3. **Data** (Principle 2) → Ground arguments in facts
4. **Brevity** (Principle 5) → But not at expense of 1-3

### Quality Hierarchy

Optimize in this order:

1. **Clarity**: Can the reader understand this?
2. **Brevity**: Is every word necessary?
3. **Polish**: Is formatting consistent?

**Never sacrifice clarity for brevity.** If you need 100 words to explain clearly, use 100 words. But most drafts use 200 words where 100 would be clearer.

### Context-Dependent Tone Calibration

| Audience | Formality | Technical Detail | Diplomatic Buffer |
|----------|-----------|------------------|-------------------|
| Investors/Public | Professional conversational | Moderate (explain acronyms) | Some (it's public) |
| Business stakeholders | Business professional | High (assume context) | Minimal (results matter) |
| Internal team | Casual conversational | Very high (use jargon) | Zero (be direct) |
| Founders (advice) | Professional warm | Moderate (principles not tactics) | Some (you're teaching) |

### When CP Style is NOT Appropriate

**Don't use this style for**:
- Marketing copy (requires different persuasion tactics)
- Legal documents (requires specific legal language)
- Customer service communications (requires different empathy tone)
- Crisis communications (may need more diplomatic framing)

### Length Calibration

| Purpose | Target Length |
|---------|---------------|
| Quick tactical | Email: 50-200 words |
| Progress update | Customer Brief: 500-2,000 words |
| Strategic reflection | Annual Letter: 2,000-5,000 words |
| Policy recommendations | Policy Ideas Brief: 3,000-5,000 words |
| Educational deep-dive | Learn with Me: 40-80 slides |

**Complexity modifier**:
- Simple topic → Shorter within range
- Complex topic → Longer within range (need to explain)

**Audience modifier**:
- High familiarity → Shorter (assume context)
- Low familiarity → Longer (build context)

---

## How to Use These Principles

**Before writing**:
1. Identify format using decision tree above
2. Load appropriate format module
3. Review these 10 principles

**While writing** (MANDATORY 3-PASS METHOD):

**PASS 1: Write to Think**
- Get ideas out
- Use placeholders for missing data
- Don't self-edit yet

**PASS 2: Apply All 10 Principles** (Don't skip any!)
- [ ] **Principle 1 (Clarity)**: Plain language? Vague pronouns removed?
- [ ] **Principle 2 (Data)**: Used only source data? Placeholders for missing data? NO FABRICATION?
- [ ] **Principle 3 (Honesty)**: Failures acknowledged upfront?
- [ ] **Principle 4 (First-Principles)**: Explained "why" from fundamentals? (if strategic doc)
- [ ] **Principle 5 (Economy)**: Cut every wasted word? Removed corporate jargon?
- [ ] **Principle 6 (Active Voice)**: "We do X" not "X is done"?
- [ ] **Principle 7 (Context)**: Explained "why" this matters?
- [ ] **Principle 8 (Attribution)**: Cited sources? (if applicable)
- [ ] **Principle 9 (Forward)**: Clear next steps? Roadmap? Asks?
- [ ] **Principle 10 (Format)**: Right structure for audience?

**PASS 3: Ruthless Cutting** (Target: Cut 30% more)
- Read each sentence
- Ask: "Does this sentence need to exist?"
- Ask: "Does this word drive the decision?"
- If no → delete it
- Check banned words list one more time

**FINAL CHECK** (Before considering it "done"):
- [ ] Word count reduced 50-80% from Pass 1?
- [ ] All MUST principles applied?
- [ ] All [Need: X] placeholders explicit (no fabricated data)?
- [ ] Maximum signal-to-noise ratio achieved?

**WARNING**: If you skip Pass 2 or Pass 3, you have NOT applied CP style. You've only started.

**Remember**: This style prioritizes truth and clarity over politeness and comfort. Write to inform and drive action, not to impress or obscure.

**The goal is maximum signal-to-noise ratio.** Every word should earn its place.

---

**Next**: Load the appropriate format module for specific structure, templates, and checklists.
