# ATLAS_AGENT_CONTEXT_v1

Version: 1.0

Status: Canonical

Purpose: Define the Atlas Organizational Intelligence System so it can be recreated, extended, governed, or operated consistently across environments.

---

# CORE DIRECTIVE

Atlas is an Organizational Intelligence System.

Atlas exists to map:

- People
- Teams
- Desks
- Platforms
- Projects
- Relationships
- Institutional Knowledge

Atlas does NOT exist to manage:

- Tasks
- Personal learning
- Research
- Book notes
- Career planning
- Personal knowledge management

The primary question Atlas answers is:

"How does the organization work?"

---

# SYSTEM BOUNDARY

## Atlas

Atlas stores organization-specific intelligence.

Examples:

- Stakeholders
- Organizational structures
- Platforms
- Business domains
- Projects
- Key relationships
- Institutional history
- Organizational assessments

Atlas is employer specific.

---

## Laboratory

Laboratory is external to Atlas.

Laboratory stores:

- Research
- Principles
- Frameworks
- Learning
- Writing
- Intellectual capital

Laboratory answers:

"What have I learned?"

Atlas answers:

"How does the organization work?"

Never blur these two systems.

---

# INFORMATION HIERARCHY

Atlas organizes information into four layers.

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

# FOLDER STRUCTURE

Atlas/

00 Home/

01 Dashboards/

05 Reviews/
    Weekly/
    Monthly/
    Quarterly/
    Yearly/

06 Communications/
    Weekly Updates/

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

- Weekly leadership updates
- Stakeholder summaries
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

Plugin configuration intentionally omitted from this document.

---

# CORE ENTITY TYPES

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
- Communication

---

# PERSON MODEL

Purpose:

Represent stakeholders.

Track both:

- Formal structure
- Informal influence

---

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

Purpose:

Represent meaningful technology assets.

Platform properties should emphasize:

- Ownership
- Stakeholders
- Dependencies
- Related Projects

Recommended field:

```yaml
depends_on: []
```

Model dependencies immediately.

Model hierarchy only after it naturally emerges.

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

Relationship notes are reserved for:

- Key advisors
- Sponsors
- Navigators
- Mentors
- Connectors

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

Assessments are interpretation.

Not source material.

---

# INITIATIVE MODEL

Initiative answers:

"What outcome am I trying to create?"

Examples:

- Stakeholder Development Initiative
- 90-Day Plan

---

# MEETING PROCESSING MODEL

Meetings follow a four-stage lifecycle.

---

## Stage 1

Capture

Goal:

Preserve raw information.

Do not analyze.

---

## Stage 2

Distill

Extract:

- People
- Teams
- Platforms
- Projects
- Relationships
- Organizational insights

Questions:

- Who matters?
- What changed?
- Who owns this?
- What surprised me?
- Who should I meet next?

---

## Stage 3

Assimilate

Update Atlas.

Potential updates:

- People
- Teams
- Platforms
- Projects
- Relationships
- Assessments

---

## Stage 4

Archive

Keep meeting notes.

Never treat meetings as primary knowledge.

Purpose:

- Provenance
- Context
- History
- Verification

Meetings become archived evidence.

---

# COMMUNICATION WORKFLOW

Communications belong in Atlas.

Communications represent:

"What was communicated?"

Not:

"What happened?"

Flow:

Meetings
    ↓

Atlas Entities
    ↓

Assessments
    ↓

Communications

---

# PERIODIC REVIEW MODEL

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
- Organizational influence
- Platform coverage

---

## Yearly

Review:

- Institutional knowledge
- Network development
- Organizational evolution

---

# GOVERNANCE RULES

## Rule 1

Create notes early.

Enrich later.

---

## Rule 2

Optimize for usefulness.

Not completeness.

---

## Rule 3

A note should exist before it is perfect.

---

## Rule 4

Meetings are evidence.

Entities are knowledge.

Assessments are interpretation.

Communications are narrative.

---

## Rule 5

Create an entity when you expect it to appear again.

Repeated appearance indicates importance.

---

## Rule 6

Model dependencies early.

Model hierarchy late.

---

# DECISION FRAMEWORK

When new information arrives:

Step 1

Determine whether it belongs in Atlas or Laboratory.

---

Step 2

Determine whether it is:

- Evidence
- Fact
- Interpretation
- Action

---

Step 3

Place it in the correct Atlas entity.

---

Step 4

Update Assessments as your understanding changes.

---

# SUCCESS CRITERIA

Atlas is successful when it helps answer:

- Who should I talk to?
- Who owns this?
- Who influences this?
- Which platforms matter?
- What projects matter?
- Why was this decision made?
- What should I learn next?

without requiring searches through historical meeting notes.

That is the primary purpose of Atlas.
