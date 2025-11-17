# Status Report Template

This template defines the format for all weekly status reports created after November 17, 2025, based on the actual format used at 8090.

---

## Complete Template

```markdown
[CATEGORY]_[Client]_[Project]_YYYYMMDD

[Client] - [Project] - Weekly Status Report

Client: [CLIENT NAME]
Project: [PROJECT NAME]
Client POC: [First-name Last-name]
Current Phase: [Descriptive Phase - e.g., "Active Development (API Integration)" or "Requirements Gathering and PRD Development" or "Maintenance (Post-Launch Support)"]

[Project-Specific Deadline Name]: [Month DD, YYYY], Cumulative Delay: [X days]
[Description of what this deadline represents and its significance]

Date of Next Exec Demo: [Month DD, YYYY] / N/A
[Brief description of demo scope and purpose, if applicable]

Date of Next Minor Demo: [Month DD, YYYY] / N/A
[Brief description of demo scope, or explanation why N/A]

Date of Next Release: [Month DD, YYYY] / N/A
[Brief description of release scope]

Date of Last Release: [Month DD, YYYY] / N/A
[Brief description of what was released]

Blockers or Potential Blockers:

● [Blocker Title]: [Detailed description including who, what, when, where. Include specific stakeholder names, dates, meeting times if applicable]. Risk Level: [High/Medium/Low]—[Impact description].

● [Next Blocker]: [Description]. Risk Level: [High/Medium/Low]—[Impact].

Notes:

● [Note Title or Category]: [Descriptive information about progress, decisions, feedback, or context]

● [Next Note]: [Continued context]

● [Additional Note]: [More information]

Work This Week:

● [Description of work completed this week - be specific about activities and outcomes]

● [Next completed item]

● [Additional work item]

Next Steps:

● [Upcoming work or action item - be specific about what will be done and when]

● [Next action]

● [Additional next step]

Software Factory Usage and Feedback

| Engineer | Refinery | Foundry | Planner | Validator |
|----------|----------|---------|---------|-----------|
| [Name] | [X hrs]<br>Rating: [X out of 5] | [X hrs]<br>Rating: [X out of 5] | [X hrs]<br>Rating: [X out of 5] | [X hrs]<br>Rating: [X out of 5] |
| [Name] | N/A | [X hrs]<br>Rating: [X out of 5] | N/A | [X hrs]<br>Rating: [X out of 5] |
```

---

## Field Definitions

### Header Fields

**CATEGORY**: Industry or project category prefix (e.g., HEALTH, FINANCE, ECOM)
- Used in filename for organization: `HEALTH_HealthCorp_PatientPortal_20251119`

**CLIENT**: Client/company name (e.g., HealthCorp, FinTech Solutions, ShopHub)

**PROJECT**: Specific project name (e.g., 360View Visit Assistant, Compliance Dashboard)

**Client POC**: Point of contact name in format "First-name Last-name" (e.g., "John Smith")

**Current Phase**: Descriptive phase with context, not rigid categories. Examples:
- "Active Development (API Integration and Prompt Refinement)"
- "Requirements Gathering and PRD Development"
- "Maintenance (Post-Launch Support and Enhancement)"

### Flexibility Note
The template is intentionally flexible. While the structural elements remain consistent, the specific deadline names, descriptions, and narrative content should be adapted to each project's reality.

---

### Timeline Fields

**Project-Specific Deadlines**:
Deadlines should be named according to project milestones, not forced into generic categories. Examples:
- "Demo-Ready Application Deadline" (for demo-driven projects)
- "PRD Acceptance Deadline" (for requirements phase)
- "Feature Complete Deadline" (for development phase)
- "Software Acceptance Deadline" (for maintenance transition)
- "Pilot Launch Deadline" (for pilot programs)

**Deadline Format**:
```
[Deadline Name]: [Month DD, YYYY], Cumulative Delay: [X days]
[Context paragraph explaining the deadline's purpose and current status]
```

**Cumulative Delay**: Always calculated from original baseline
- `0 days` if on schedule
- `X days` if delayed
- Include explanation of delays in context paragraph

**Example**:
```
Demo-Ready Application Deadline: November 20, 2025, Cumulative Delay: 0 days
Target date for demo-ready application to HealthCorp stakeholders.
```

---

### Milestone Fields

**Date of Next Exec Demo**:
- Format: `Month DD, YYYY` or `N/A`
- Executive-level demonstration of progress
- Typically during DEVELOPMENT phase
- May occur during MAINTENANCE for major updates

**Date of Next Minor Demo**:
- Format: `Month DD, YYYY` or `N/A`
- Team or working session demonstrations
- Primarily during DEVELOPMENT phase
- More frequent than exec demos

**Date of Next Release**:
- Format: `Month DD, YYYY` or `N/A`
- Planned deployment to production
- During DEVELOPMENT: Feature releases
- During MAINTENANCE: Bug fixes or enhancements

**Date of Last Release**:
- Format: `Month DD, YYYY` or `N/A`
- Most recent production deployment
- Relevant during DEVELOPMENT and MAINTENANCE

---

### Status Fields

**Blockers or Potential Blockers**:
- **MOST IMPORTANT SECTION** - This drives executive attention and action
- Use bullet points (●) not numbers
- Each blocker must include:
  - **Title**: Brief identifier of the blocker
  - **Detailed Description**: Who, what, when, where specifics
  - **Risk Level**: High / Medium / Low
  - **Impact**: Clear statement of what's at stake

**Format**:
```
● [Blocker Title]: [Detailed description with specific names, dates, meeting times, technical details]. Risk Level: [High/Medium/Low]—[Impact statement].
```

**Example**:
```
Blockers or Potential Blockers:

● SystemX EMR API Access: Scheduled validation call with Jane Doe (SystemX technical resource) on Monday, November 17th at 1:30 PM EST to discuss FHIR R4 Patient endpoint integration and obtain Client ID/Secret credentials. Risk Level: High—critical for accessing patient data for visit assistant recommendations.

● Payment Gateway Integration: Stripe webhook intermittent failures (3-5% of transactions) causing order confirmation delays. Stripe support ticket opened November 15th, awaiting response. Risk Level: Medium—impacts customer experience but has fallback notification system.
```

**Notes**:
- Contextual information for stakeholders
- Use bullet points (●) with descriptive labels
- More narrative than rigid "FYI #1" format (though FYI format acceptable)
- Include:
  - Progress updates and completed milestones
  - Design decisions and approach confirmations
  - Client feedback and requests
  - Team status and availability
  - Upcoming schedule changes
  - System performance metrics (for maintenance phase)
  - Scope clarifications

**Example**:
```
Notes:

● Key Update: Demo scheduled for November 20, 2025 to showcase real-time question generation during patient visits.

● Question Generation Approach: Finalized focus on 4 disease conditions (diabetes, heart disease, lung disease, cancer), limiting to top 3 recommendations per visit.

● Contract Continuation: Success of January 2026 pilot with experienced nurses is critical for project expansion.
```

**Work This Week**:
- Bullet point list (●) of completed work
- Be specific about activities and outcomes
- Include technical details, meetings, deliverables
- Shows weekly progress and effort

**Example**:
```
Work This Week:

● Priority: Athena API validation call on Monday 11/17 to obtain credentials and confirm FHIR R4 Patient endpoint approach

● Continued mock Athena API integration development locally

● Prepared FHIR R4 Patient endpoint integration plan (demographics, conditions, medications, labs, encounters, procedures, allergies, immunizations, care plans, appointments)
```

**Next Steps**:
- Bullet point list (●) of upcoming work
- Forward-looking action items
- Include timing when relevant
- Shows project momentum and planning

**Example**:
```
Next Steps:

● Implement OAuth authentication flow once Athena credentials received

● Build web-based transcription interface (click to start, runs in background, displays real-time questions)

● Continue development toward January 2026 pilot with experienced nurses
```

---

### Engineering Metrics

**Section Title**: "Software Factory Usage and Feedback" (not just "Engineering Metrics")

**Table Structure**:
| Column | Description |
|--------|-------------|
| Engineer | Engineer name (use actual names, not "Eng #1") |
| Refinery | Time spent on requirements/analysis<br>Rating separate (1-5) |
| Foundry | Time spent on development/implementation<br>Rating separate (1-5) |
| Planner | Time spent on planning/coordination<br>Rating separate (1-5) |
| Validator | Time spent on testing/QA<br>Rating separate (1-5) |

**Time Spent**:
- Format: "X hrs" is standard
- Reflects actual allocation for the week
- Use "N/A" if engineer didn't work in that category

**Quality Rating**:
- Scale: 1-5 (5 being highest quality)
- Assesses output quality in that category
- Format: "Rating: X out of 5"
- **IMPORTANT**: Time and rating are on **separate lines** in the table cell
- Use `<br>` HTML tag or markdown line break in table

**Role Definitions**:
- **Refinery**: Requirements gathering, user research, documentation, PRD creation
- **Foundry**: Coding, implementation, technical development
- **Planner**: Sprint planning, task breakdown, timeline management, coordination
- **Validator**: Testing, QA, bug verification, acceptance criteria validation

**Example Table**:
```
Software Factory Usage and Feedback

| Engineer | Refinery | Foundry | Planner | Validator |
|----------|----------|---------|---------|-----------|
| Alex Johnson | 4 hrs<br>Rating: 2 out of 5 | N/A | N/A | N/A |
| Sam Patel | N/A | 4 hrs<br>Rating: 3 out of 5 | 4 hrs<br>Rating: 3 out of 5 | N/A |
```

Interpretation:
- Alex spent 4 hours on requirements work (quality rating 2/5)
- Sam spent 4 hours on development (quality 3/5) and 4 hours on planning (quality 3/5)

---

## Formatting Guidelines

1. **Consistent Date Format**: Use same format throughout report (prefer `Month DD, YYYY`)
2. **Explicit Zero Delays**: Write "0 Days" not blank for on-schedule items
3. **N/A for Non-Applicable**: Use "N/A" not blank for fields that don't apply
4. **Table Alignment**: Use markdown table formatting with proper column alignment
5. **Clear Section Headers**: Maintain exact header text for parsing/automation
6. **Line Breaks**: Single blank line between major sections

---

## Phase-Specific Guidance

### REQUIREMENTS Phase
Typical characteristics:
- PRD Acceptance deadline is primary focus
- Feature Complete and Software Acceptance may be estimated
- Exec/Minor demos may be N/A
- Next Release likely N/A
- High Refinery allocation
- Lower Foundry allocation
- Validator allocation minimal

### DEVELOPMENT Phase
Typical characteristics:
- All three deadlines actively tracked
- Demo dates should be populated
- Next Release date set
- Last Release shows progress
- High Foundry allocation
- Moderate Refinery, Planner, Validator allocation
- Quality scores critical for on-time delivery

### MAINTENANCE Phase
Typical characteristics:
- PRD Acceptance completed (historical)
- Feature Complete completed (historical)
- Software Acceptance completed (historical)
- Exec demos likely N/A (unless major update)
- Next Release for bug fixes/enhancements
- Last Release shows recent deployment
- Lower overall time allocation
- Higher Validator allocation (proportion)

---

## Automation Notes

This template is designed for:
- Automated weekly generation (every Tuesday)
- Consistent parsing and data extraction
- Executive dashboard integration
- Historical trend analysis

**Filename Convention**: `CATEGORY_ClientName_ProjectName_YYYYMMDD.ext`
- CATEGORY: Industry/project category (HEALTH, FINANCE, ECOM, etc.)
- ClientName: No spaces (use underscore if needed)
- ProjectName: No spaces (use underscore if needed)
- YYYYMMDD: Current date in ISO format (year, month, day)
- Extension: .md for markdown, .pdf for final reports

Examples:
- `HEALTH_HealthCorp_PatientPortal_20251119.pdf`
- `FINANCE_FinTech_Compliance_20251119.md`
- `ECOM_ShopHub_Platform_20251119.md`

---

## Version Control

**Format Version**: 1.0.0
**Effective Date**: November 17, 2025
**Previous Format**: Pre-November 17, 2025 reports used different structure

When comparing to historical reports, extract available information and note format differences in the Notes section if relevant to understanding timeline changes.
