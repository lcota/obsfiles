# AGENTS.md

# Atlas Organizational Intelligence System
Version: 1.0
Status: Canonical
Audience: Human operators, AI Agents, VS Code Copilot, Obsidian automations, future Atlas maintainers

---

# PURPOSE

Atlas is an Organizational Intelligence System.

Atlas exists to answer:

- Who owns this?
- Who influences this?
- Who understands the history?
- Which teams support this?
- Which platforms matter?
- Which projects are active?
- How are people connected?
- Who can help navigate the organization?
- What organizational realities should influence decision making?

Atlas is designed to create organizational awareness and institutional memory.

Atlas is not a personal knowledge management system.

---

# WHAT ATLAS IS

Atlas stores:

- People
- Teams
- Desks
- Platforms
- Projects
- Relationships
- Institutional History
- Organizational Assessments
- Organizational Initiatives
- Stakeholder Communications
- Meeting Evidence

---

# WHAT ATLAS IS NOT

Atlas does NOT store:

- Personal research
- Book notes
- Learning notes
- Framework development
- Writing projects
- Intellectual capital
- Long-form research
- General knowledge

Those belong in Laboratory.

---

# ATLAS vs LABORATORY

## Atlas

Question:

How does the organization work?

Examples:

- Platform ownership
- Stakeholder maps
- Budget processes
- Team structures
- Organizational influence
- Project relationships

---

## Laboratory

Question:

What have I learned?

Examples:

- Market structure research
- Business frameworks
- Design patterns
- AI research
- Architectural principles
- Personal intellectual capital

Never blur these two systems.

---

# INFORMATION MODEL

Atlas contains four information layers.

## Layer 1: Evidence

Examples:

- Meetings
- Communications

Purpose:

Raw source material.

---

## Layer 2: Facts

Examples:

- People
- Teams
- Desks
- Platforms
- Projects
- Relationships

Purpose:

Durable organizational knowledge.

---

## Layer 3: Interpretation

Examples:

- Assessments

Purpose:

Current understanding and analysis.

---

## Layer 4: Action

Examples:

- Initiatives

Purpose:

Desired organizational outcomes.

---

# VAULT STRUCTURE

```text
Atlas/

00 Home/

01 Dashboards/

05 Reviews/
    Weekly/
    Monthly/
    Quarterly/
    Yearly/

06 Communications/
    Stakeholder Updates/

10 People/

20 Teams/

30 Desks/

40 Platforms/

50 Projects/

60 Meetings/

70 Relationships/

80 Institutional History/

85 Workbench/
    30 Assessments/
    40 Initiatives/

90 Incubation/

99 Inbox/

100 System/
    templates/
    fileclasses/
```

---

# DIRECTORY GOVERNANCE

Atlas directories represent durable organizational concepts.

Directories should not be created for convenience.

Agents must treat creation of a directory as an architectural decision.

---

## Rule 1: Prefer Existing Directories

Before creating a new directory, determine whether the information belongs in:

```text
People
Teams
Desks
Platforms
Projects
Relationships
Assessments
Initiatives
Communications
```

A new directory should be the last option.

---

## Rule 2: Evidence Before Structure

A new directory should only be considered when:

- Multiple notes already exist that do not fit existing entities
- The concept has its own lifecycle
- The concept requires dedicated metadata
- The concept requires a dedicated template
- The concept is expected to have significant future growth

---

## Rule 3: Every Directory Requires Infrastructure

Every new directory must have:

```text
Directory
Template
FileClass
QuickAdd Entry
Documentation
```

Example:

```text
15 Companies/

100 System/templates/Company.md

100 System/fileclasses/Company.md

QuickAdd:
New Company
```

---

## Rule 4: Use Incubation First

If uncertain:

```text
90 Incubation/
```

before creating a new permanent directory.

---

## Rule 5: No Convenience Directories

Avoid:

```text
Misc
Random Notes
Reference
Scratch
General
Temporary
```

These indicate the information model needs refinement.

---

# FOLDER PURPOSES

## 00 Home

Entry point to Atlas.

Contains:

- Navigation
- Dashboard links
- Recently modified content

---

## 01 Dashboards

Dataview and reporting layer.

Examples:

- Trusted Network
- Platform Portfolio
- Organizational Navigators
- People by Team
- Inbox Review

---

## 05 Reviews

Periodic reflection.

Contains:

- Weekly Reviews
- Monthly Reviews
- Quarterly Reviews
- Yearly Reviews

Purpose:

Track organizational learning over time.

---

## 06 Communications

Outbound communications.

Examples:

- Weekly stakeholder updates
- Leadership summaries
- Program communications

Purpose:

Capture narrative and messaging.

---

## 10 People

Stakeholders.

Examples:

- Managers
- Architects
- Traders
- SMEs
- Sponsors
- Influencers

Purpose:

Track people and organizational value.

---

## 20 Teams

Organizational groups.

Purpose:

Define ownership and responsibility.

---

## 30 Desks

Business domains.

Examples:

- Prime Services
- Credit Trading
- Repo
- Financing

Purpose:

Represent business functions.

---

## 40 Platforms

Technology assets.

Examples:

- Zeus
- Iron
- RTGen
- LeadFollow

Purpose:

Represent systems that matter.

Platform is a generic term and may represent:

- System
- Application
- Service
- Technology Product

---

## 50 Projects

Organizational initiatives.

Purpose:

Track significant efforts.

---

## 60 Meetings

Evidence repository.

Meetings are evidence.

Meetings are not knowledge.

Meeting notes should be processed and distilled into Atlas.

---

## 70 Relationships

High-value relationships only.

Do NOT create relationships for every person.

Create relationships for:

- Trusted Advisors
- Navigators
- Sponsors
- Historians
- Connectors

---

## 80 Institutional History

Historical organizational context.

Examples:

- Reorganizations
- Platform evolution
- Historical ownership

---

## 85 Workbench

Thinking layer.

Contains only:

- Assessments
- Initiatives

No Research.
No Discovery.
No Strategy.

---

## 90 Incubation

Temporary classification area.

Use when unsure where something belongs.

---

## 99 Inbox

Processing area.

Inbox is workflow.

Inbox is not storage.

---

# REQUIRED PLUGINS

Install:

- Dataview
- Templater
- Metadata Menu
- QuickAdd
- Excalibrain
- Homepage
- Periodic Notes
- Kanban

Plugin configuration intentionally omitted.

---

# ENTITY TYPES

Atlas contains:

- Person
- Team
- Desk
- Platform
- Project
- Relationship
- Assessment
- Initiative
- Meeting
- Stakeholder Update

---

# PERSON MODEL

## Person Properties

```yaml
fileClass: Person

type: person

title:

position:

company:

affiliation:

division:

group:

team:

desks: []

platforms: []

projects: []

roles: []

relationship_strength:

knowledge_capital:

network_capital:

execution_capital:

navigation_value:

can_help_with: []

introduced_by: []

trusted_connections: []

last_interaction:

status: active

created:
```

---

## Affiliation Values

```text
Employee
Contractor
Consultant
Vendor
Partner
Client
Former Employee
```

---

## Organizational Roles

```text
historian

navigator

connector

trusted-advisor

sponsor

decision-maker

architect

operator

sme

influencer
```

Roles describe organizational value.

Roles are not job titles.

---

# PLATFORM MODEL

Platforms should emphasize:

- Ownership
- Stakeholders
- Dependencies
- Projects

Recommended field:

```yaml
depends_on: []
```

Example:

```yaml
depends_on:
  - [[RTGen]]
  - [[LeadFollow]]
```

---

# PROJECT MODEL

Projects represent significant organizational efforts.

Track:

- Sponsors
- Stakeholders
- Platforms
- Teams
- Dependencies

---

# RELATIONSHIP MODEL

Relationships represent:

The value and evolution of a relationship.

Not the existence of a person.

---

# ASSESSMENT MODEL

Assessment answers:

"What do I think?"

Examples:

- Credit Platform Assessment
- Stakeholder Assessment
- Operating Model Assessment

Assessment stores:

- Risks
- Opportunities
- Recommendations
- Current understanding

---

# INITIATIVE MODEL

Initiative answers:

"What outcome am I trying to create?"

Examples:

- Stakeholder Development Initiative
- 90-Day Plan

---

# QUICKADD GOVERNANCE

Atlas assumes all durable entities are created through QuickAdd.

Every Atlas entity should have a corresponding QuickAdd workflow.

---

## Required QuickAdd Choices

```text
New Person

New Team

New Desk

New Platform

New Project

New Relationship

New Meeting

New Assessment

New Initiative

New Stakeholder Update
```

---

## New Person Example

Input:

```text
George Elsener
```

Creates:

```text
10 People/George Elsener.md
```

Template:

```text
Person.md
```

Expected frontmatter:

```yaml
fileClass: Person
type: person
```

---

## New Platform Example

Input:

```text
Zeus
```

Creates:

```text
40 Platforms/Zeus.md
```

Template:

```text
Platform.md
```

Expected frontmatter:

```yaml
fileClass: Platform
type: platform
```

---

## New Assessment Example

Input:

```text
AMER Credit Platform Assessment
```

Creates:

```text
85 Workbench/30 Assessments/AMER Credit Platform Assessment.md
```

Template:

```text
Assessment.md
```

---

## New Stakeholder Update Example

Input:

```text
2026-W44 Stakeholder Update
```

Creates:

```text
06 Communications/Stakeholder Updates/2026-W44 Stakeholder Update.md
```

Template:

```text
StakeholderUpdate.md
```

Expected frontmatter:

```yaml
fileClass: StakeholderUpdate
type: stakeholder-update
```

---

## QuickAdd Standard

Every Atlas QuickAdd workflow must:

1. Prompt for entity name
2. Create file
3. Apply template
4. Save to correct directory
5. Open note

Create first.

Enrich later.

---

# MEETING PROCESSING MODEL

Meetings follow a four-stage workflow.

---

## Stage 1: Capture

Store raw information.

Do not analyze.

---

## Stage 2: Distill

Extract:

- New people
- Teams
- Platforms
- Ownership information
- Dependencies
- Projects
- Relationships
- Organizational insights

Questions:

- Who matters?
- What changed?
- What surprised me?
- What should survive beyond this meeting?

---

## Stage 3: Assimilate

Update:

- People
- Teams
- Platforms
- Projects
- Relationships
- Assessments

Goal:

Move knowledge out of meetings.

---

## Stage 4: Archive

Keep meetings.

Meetings provide:

- Context
- History
- Provenance
- Verification

Meetings become evidence.

---

# COMMUNICATION MODEL

Location:

```text
06 Communications/
    Stakeholder Updates/
```

Communications answer:

```text
What was communicated?
```

Flow:

```text
Meetings
    ↓

Entities
    ↓

Assessments
    ↓

Stakeholder Updates
```

---

# REVIEW MODEL

## Weekly

Review:

- Stakeholders
- Meetings
- Platforms
- Open questions

---

## Monthly

Review:

- Knowledge gained
- Organizational understanding
- Relationship growth

---

## Quarterly

Review:

- Strategic understanding
- Platform landscape

---

## Yearly

Review:

- Institutional knowledge
- Network development
- Organizational evolution

---

# FILECLASS RULES

Every entity template MUST contain:

```yaml
fileClass:
type:
```

Example:

```yaml
fileClass: Person
type: person
```

Purpose:

```text
fileClass
→ Metadata Menu

type
→ Dataview
```

---

# EXTENDING ATLAS

When introducing a new entity:

---

## Step 1

Create directory.

Only after governance criteria are satisfied.

---

## Step 2

Create template.

Location:

```text
100 System/templates/
```

---

## Step 3

Create FileClass.

Location:

```text
100 System/fileclasses/
```

---

## Step 4

Template MUST include:

```yaml
fileClass:
type:
```

---

## Step 5

Add QuickAdd workflow.

---

## Step 6

Update AGENTS.md.

---

# AGENT VALIDATION RULES

Before modifying Atlas, validate decisions.

---

## Validation Rule 1: Classification

Classify information as:

```text
Evidence
Fact
Interpretation
Action
```

Mapping:

```text
Evidence
→ Meetings
→ Stakeholder Updates

Fact
→ People
→ Teams
→ Desks
→ Platforms
→ Projects
→ Relationships

Interpretation
→ Assessments

Action
→ Initiatives
```

---

## Validation Rule 2: Reuse Before Creation

Ask:

```text
Does this entity already exist?
```

If yes:

Update existing note.

Do not duplicate.

---

## Validation Rule 3: Atlas vs Laboratory

Reject:

```text
Research
Industry Analysis
Book Notes
Frameworks
General Learning
```

These belong in Laboratory.

---

## Validation Rule 4: Durability

Ask:

```text
Will this matter in six months?
```

If no:

Use:

```text
Meeting
Inbox
Incubation
```

instead of a permanent entity.

---

## Validation Rule 5: Meeting Knowledge Extraction

Ask:

```text
If this meeting were deleted tomorrow,
what knowledge would be lost?
```

Transfer that knowledge into:

```text
People
Teams
Platforms
Projects
Relationships
Assessments
```

before archiving.

---

## Validation Rule 6: Assessment Test

Use Assessments for:

- Opinions
- Interpretations
- Risks
- Opportunities
- Recommendations

---

## Validation Rule 7: Platform Modeling

Prefer:

```yaml
depends_on:
```

before:

```yaml
parent_platform:
```

Model dependencies early.

Model hierarchy late.

---

## Validation Rule 8: Directory Creation

Before creating a directory confirm:

```text
Template exists

FileClass exists

QuickAdd exists

Documentation exists
```

All must be true.

---

## Validation Rule 9: Simplicity First

Prefer:

```text
Update Existing Entity
```

over:

```text
Create New Entity
```

Prefer:

```text
Create Assessment
```

over:

```text
Create New Workbench Type
```

Prefer:

```text
Dependency
```

over:

```text
Hierarchy
```

---

# GOVERNANCE RULES

## Rule 1

Capture quickly.

Refine later.

---

## Rule 2

Do not optimize for perfection.

---

## Rule 3

Create notes when future reuse is likely.

---

## Rule 4

Repeated appearance indicates importance.

---

## Rule 5

Facts belong in entities.

Interpretation belongs in assessments.

Evidence belongs in meetings.

Narrative belongs in stakeholder updates.

---

## Rule 6

Do not allow organizational knowledge to remain trapped inside meeting notes.

---

# USER PROFILE

## Name

Luis Cota

---

## Current Context

Technology leader building organizational understanding within SocGen.

Primary objective:

Understand and influence organizational systems at scale.

---

## Working Style

- Analytical
- Systems-oriented
- Architecture-driven
- High signal-to-noise preference
- Favors durable operational frameworks
- Optimizes for long-term leverage

---

## Atlas Design Preferences

- Organizational intelligence over PKM
- Minimal maintenance overhead
- High reuse of captured information
- Strong separation between Atlas and Laboratory
- Entity-centric architecture
- Evidence → Facts → Interpretation → Action workflow

---

## Preferred Agent Behavior

Agents should:

- Preserve simplicity
- Prefer evolution over redesign
- Introduce hierarchy only when justified
- Prefer assessments over new note types
- Avoid proliferation of templates
- Avoid unnecessary metadata
- Prioritize organizational intelligence extraction
- Recommend updates to existing entities before creating new structures

---

# SUCCESS CRITERIA

Atlas is successful when it can answer:

- Who should I talk to?
- Who owns this?
- Who influences this?
- Which platforms matter?
- What should I learn next?
- Why was this decision made?

without relying on memory or searching through historical meeting notes.
