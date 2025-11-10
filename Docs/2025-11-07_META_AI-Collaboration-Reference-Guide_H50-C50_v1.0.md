# AI Collaboration System: Comprehensive Reference Guide

**Purpose:** Complete implementation guide for sustainable long-term AI collaboration in doctoral research and professional projects.

---

## System Requirements & Context

**Designed For:**

- **Claude Pro, Teams, or Enterprise accounts**
- **Model:** Claude Sonnet 4.5 (claude-sonnet-4-5-20250929)
- **Date Created:** November 7, 2025

**Important:** This system was developed specifically for Claude Sonnet 4.5 with Pro/Teams/Enterprise features (Projects, custom instructions, file upload). It may be adaptable to other AI models or Claude tiers, but functionality may vary. The protocols assume access to Claude's Project system and persistent file storage.

---

## Document Information

**Version:** 1.0 (Living Document)

**Status:** Active - This is a living document that evolves with implementation experience and methodological refinement.

**Research Context:** This system is part of an EdD dissertation methodology examining AI-human collaboration in doctoral research at Northeastern University's Graduate School of Education.

**Related Resources:**

- [AI-Assisted Dissertation Management System](https://drdawson2.github.io/dissertation-guide/)

**Contribution Ratio:** H50-C50 (Equal collaboration between human design and AI implementation)

---

## Table of Contents

1. [System Overview](#system-overview)
2. [Architecture: Where Everything Goes](#architecture-where-everything-goes)
3. [Naming Conventions](#naming-conventions)
4. [Two-Tier Chat System](#two-tier-chat-system)
5. [Decision Frameworks](#decision-frameworks)
6. [Session Protocols](#session-protocols)
7. [File Management](#file-management)
8. [Chat Retirement Protocol](#chat-retirement-protocol)
9. [META Chat Maintenance](#meta-chat-maintenance)
10. [Human/AI Responsibility Matrix](#humanai-responsibility-matrix)
11. [Implementation Guide](#implementation-guide)
12. [Troubleshooting Guide](#troubleshooting-guide)
13. [Quick Reference](#quick-reference)

---

## System Overview

### Core Principles

**Discovery vs. Execution Modes:**

- **Discovery Mode:** Exploratory dialogue, questions develop thinking, multiple perspectives
- **Execution Mode:** Directive guidance, efficient implementation, minimal back-and-forth

**Progressive Autonomy:**

- Collaboration patterns evolve over time
- Support scaffolds independence rather than creating dependency
- Strategic delegation based on capability development

**Resource Management:**

- Token monitoring prevents mid-work disruption
- Proactive chat retirement at natural breakpoints
- Lean file structures optimize performance

**Transparency & Integrity:**

- Contribution ratios track human/AI collaboration
- Academic integrity through documentation
- Methodological transparency for research validity

### System Goals

- Reduce scope creep through clear boundaries
- Provide decision frameworks for chat management
- Support 18+ month collaboration timelines
- Balance structure with flexibility
- Enable both technical and narrative work modes
- Scale sustainably as projects progress

---

## Architecture: Where Everything Goes

### CRITICAL DISTINCTION

Understanding where things live prevents confusion and ensures the system works correctly.

### Account-Level Custom Instructions

**Location:** Settings → Personalization → Custom Instructions

**What Lives Here:**

- Identity and context (universal across all Claude use)
- Communication mode protocols (Discovery vs. Execution)
- Collaboration values (transparency, accessibility, integrity)
- Token monitoring protocol
- Contribution tracking system (H[X]-C[Y])
- Artifact preferences and naming conventions
- Content placement rules
- Context gathering protocols

**Purpose:** Universal "how David works with Claude" protocols that apply everywhere

**When to Update:** Rarely - only when universal work patterns change

---

### Project-Level Instructions

**Location:** Project Settings → Custom Instructions (within specific project)

**What Lives Here:**

- Project-specific context (research focus, timeline, methodology)
- Temporal context protocol (date provision requirements)
- Chat architecture explanation (Home Base + Work Unit system)
- Chat naming conventions for this project
- Chat retirement triggers
- File management protocol
- Cross-chat coherence strategy
- Project-specific protocols or requirements

**Purpose:** "How this specific project works" configuration

**When to Update:** When project structure changes significantly

---

### Project Files

**Location:** Project → Files (uploaded documents within project)

**What Lives Here:**

**System Files (Required):**

- `Project Overview - Current.md` - Dynamic working document, read automatically by all chats
- `Project Overview Template.md` - Static format reference for META chat

**Content Files:**

- Research documents, frameworks, protocols
- Data collection tools, coding schemes
- Design specifications, technical documentation
- Progress tracking dashboards, timeline documents
- Reference materials specific to the project

**Purpose:** Searchable knowledge base accessible to all chats in project

**When to Update:** Continuously as project evolves; Project Overview every 2-4 weeks

---

### Individual Chat Context

**Location:** Within specific chat conversations

**What Lives Here:**

- Conversation history for THIS chat only
- Session-specific context and updates
- Work-in-progress for this deliverable
- Decisions made within this chat

**What Does NOT Live Here:**

- Context from other chats (must be explicitly bridged)
- Project-wide decisions (should go in Project Overview)

**Purpose:** Focused workspace for specific deliverable or ongoing dialogue

---

### Visual Summary

```
ACCOUNT LEVEL (Universal)
└── Custom Instructions: How David works with Claude always

PROJECT LEVEL
├── Project Instructions: How THIS project works
├── Project Files
│   ├── Project Overview - Current.md (auto-read by all chats)
│   ├── Project Overview Template.md (reference for META)
│   └── All other project documents
└── Individual Chats
    ├── Home Base Chat (long-running dialogue)
    └── Work Unit Chats (specific deliverables)
```

---

## Naming Conventions

### 1. Chat Naming Convention

#### Home Base Format

```
[Project Name] - Home Base [Month Year]

Example: EdD Research - Home Base (Nov 2025)

When retired: EdD Research - Home Base (Aug-Nov 2025)
```

**Purpose:** Long-running exploratory and accountability chat

---

#### Work Unit Format

```
[Category] - [Specific Deliverable] - [YYYY-MM-DD] - [Status]

Examples:
- DEV - Dissertation Website - 2025-10-15 - Active
- DATA - Cycle 1 Coding Framework - 2025-11-01 - Active
- THEORY - Hall-Savickas Integration - 2025-09-20 - Complete
- WRITING - Methodology Chapter - 2026-02-10 - Active
- META - Project Overview Maintenance - 2025-11-07 - Active
```

**Category Codes:**

- **DEV** = Development/Technical work
- **DATA** = Data collection/analysis
- **THEORY** = Theoretical synthesis/analysis
- **WRITING** = Writing/drafting
- **META** = System design/organizational work
- **[Custom]** = Project-specific categories as needed

**Status Options:**

- **Active** = Currently working
- **Paused** = May return to, not complete
- **Complete** = Deliverable finished, chat retired
- **Archived** = Superseded or no longer relevant

**Purpose:** Time-stamped, scannable identification of focused work

---

### 2. Artifact Naming Convention

```
[Descriptive Title] - [Contribution Ratio]

Examples:
- Account-Level Custom Instructions - H30-C70
- Project Overview Template - H20-C80
- Dissertation Timeline Dashboard - H95-C5
- Career Conversation Toolkit - H60-C40
- Website Homepage Code - H10-C90
```

**Components:**

- **Descriptive Title:** Clear indication of artifact content
- **Contribution Ratio:** H[X]-C[Y] tracking human/AI work

**Purpose:** Scannable artifact menu with transparent contribution tracking

---

### 3. File Naming Convention

```
yyyy-mm-dd_[Type]_[Document Title]_[H/C Ratio]_[Version]

Examples:
- 2025-11-07_META_System-Design-Session_H50-C50_v1.0.md
- 2025-10-15_DEV_Website-Structure-Specs_H40-C60_v2.0.md
- 2025-11-01_DATA_Interview-Protocol_H90-C10_v1.0.md
- 2025-09-20_THEORY_Framework-Synthesis_H70-C30_v1.5.md
- 2025-12-01_WRITING_Methodology-Draft_H85-C15_v1.0.md
```

**Components:**

- **yyyy-mm-dd:** ISO date format for chronological sorting
- **[Type]:** Category code (same as chat categories: DEV, DATA, THEORY, WRITING, META, etc.)
- **[Document Title]:** Descriptive title with hyphens (no spaces)
- **[H/C Ratio]:** Human/Claude contribution ratio (use H100-C0 for fully human-created documents)
- **[Version]:** Version number in v1.0 format

**Purpose:** Chronological organization, scannable by type, transparent contribution tracking, version control

**Special Cases:**

- Fully human documents: Include H100-C0 for consistency
- Multi-version tracking: Increment version (v1.0 → v1.5 → v2.0)
- Major vs minor changes: v1.0 → v1.1 (minor), v1.0 → v2.0 (major)

---

### 4. Contribution Ratio System

```
H[X]-C[Y]

Where:
- H = Human contribution percentage
- C = Claude (AI) contribution percentage
- Total always equals 100

Examples:
- H90-C10: 90% human work, 10% AI assistance
- H50-C50: Equal collaboration
- H10-C90: Primarily AI-generated with human direction
- H100-C0: Fully human-created (no AI involvement)
```

**Application:**

- All artifacts created in chat
- All files that involve AI collaboration
- Methodology documentation
- Academic integrity tracking

**Purpose:** Transparent contribution tracking for academic integrity and methodological rigor

---

## Two-Tier Chat System

### Architecture Overview

```
PROJECT
├── HOME BASE CHAT (Tier 1)
│   └── Long-running, exploratory, accountability
│
└── WORK UNIT CHATS (Tier 2)
    ├── DEV - Specific Deliverable - Active
    ├── DATA - Specific Deliverable - Active
    ├── WRITING - Specific Deliverable - Complete
    └── META - Project Overview Maintenance - Active
```

### Tier 1: Home Base Chat

**Purpose:**

- Brainstorming and exploratory thinking
- Check-ins and accountability tracking
- Learning discovery through dialogue
- Generative thinking without defined deliverables

**Communication Mode:** Primarily Discovery Mode

**Lifespan:** Long-running (months), retired only when:

- Performance degrades significantly
- Major phase transition occurs
- Token capacity approaching limits
- Natural break point (semester end, major milestone)

**Characteristics:**

- Loose structure, flexible topics
- Can prototype simple ideas
- Weekly check-ins and progress updates
- Meta-reflection on process and learning

---

### Tier 2: Work Unit Chats

**Purpose:**

- Specific deliverables with defined outcomes
- Focused project work (development, analysis, writing)
- Bounded scope with clear completion criteria

**Communication Mode:** Varies by work type (Discovery for design, Execution for development)

**Lifespan:** Short (days to weeks), retired when:

- Deliverable complete
- Project abandoned or superseded
- Technical degradation accumulating

**Characteristics:**

- Clear scope and outcome
- Focused on execution
- Minimal scope drift
- Retired upon completion

---

### Special Case: META Chat

**Purpose:** Maintain Project Overview document

**Type:** Work Unit chat, but long-running

**Usage:** Revisit every 2-4 weeks for Project Overview updates

**Lifespan:** Persistent throughout project, used periodically

---

## Decision Frameworks

### When to Use Home Base vs. Work Unit Chat

#### USE HOME BASE IF:

- ✓ Brainstorming/exploring without defined deliverable
- ✓ Weekly check-in or accountability tracking
- ✓ Learning through dialogue (discovering connections)
- ✓ Generative thinking about next steps
- ✓ Cannot yet articulate concrete outcome
- ✓ Rapid prototyping (1-2 sessions, single artifact)

#### CREATE WORK UNIT CHAT IF:

- ✓ Specific deliverable with defined done-state
- ✓ Work requires sustained focus over multiple sessions
- ✓ Primarily technical/development requiring Execution mode
- ✓ Can name it clearly using naming convention
- ✓ Will generate multiple artifacts or files
- ✓ Prototype "graduates" to full development

---

### Mode Transitions: Prototyping to Development

**PROTOTYPE IN HOME BASE:**

- Single session or ~2 sessions max
- Single artifact exploration
- Testing if concept works
- "Let's see if this could work" energy

**GRADUATE TO WORK UNIT WHEN:**

- Prototype works and you want to expand it
- Becomes multi-artifact (multiple files, interconnected)
- Shifts from "exploring if" to "making it work well"
- Needs multiple development sessions with technical focus

**Example:** Single HTML page guide (Home Base) → Multi-page website (New Work Unit chat)

**Signal to transition:** "Am I now committed to building this out?" → Create Work Unit chat

---

### Communication Mode Selection

#### DISCOVERY MODE Indicators:

- Figuring out WHAT you want
- Questions help develop thinking
- Multiple perspectives useful
- Theory synthesis, creative exploration, research design
- Music composition ideas, career direction, conceptual development

#### EXECUTION MODE Indicators:

- You KNOW what you want
- Need specific HOW-TO guidance
- Questions slow you down
- Coding implementation, software settings, workflow optimization
- Photography technique, specific edits, technical parameters

#### MODE SWITCHING:

Can switch within conversation (creative reverb ideas → technical Ableton settings)

**When unclear, Claude asks:** "Are we exploring possibilities or executing something specific?"

---

## Session Protocols

### Opening Protocol: Starting a Session

**Your Opening:** "I'm ready to start."

**Claude's Response Prompts:**

```
Welcome back! Let me orient to where we are:

1. What's today's date?
2. When was our last check-in?
3. What have you accomplished since then?
4. What's your focus for today's session?
5. What mode are we working in - Discovery or Execution?
```

**You Provide:**

```
Today is [Day, Date]
Last check-in: [X days ago]
Accomplished since then:
- [bullet list]

Today's focus: [specific goal or question]
Mode: [Discovery/Execution/Will switch between]
```

---

### Closing Protocol: Ending a Session

**Your Closing:** "I'm ready to close this session."

**Claude's Response Prompts:**

```
Let's capture what happened in this session:

1. What did we accomplish today?
2. What artifacts or decisions were created?
3. What's the contribution ratio for today's work?
4. What's your next step or focus for next session?
5. Any open questions or parking lot items?
6. Should anything be documented in Project Overview?
```

**You Provide:**

```
Accomplished:
- [bullet list]

Artifacts created:
- [artifact name - H[X]-C[Y]]

Next session focus:
- [what comes next]

For Project Overview:
- [anything META should know about]
```

---

### Check-In Protocol (Home Base)

**Frequency:** Weekly or bi-weekly

**Standard Check-In Structure:**

1. **Orientation:** Date, time since last check-in
2. **Progress Report:** What you've accomplished
3. **Challenges:** What's blocking or confusing you
4. **Planning:** Next steps and priorities
5. **Mode Declaration:** Discovery or Execution for this session

**Purpose:** Maintain momentum, prevent drift, track progress

---

## File Management

### Project Files Best Practices

**Keep Lean:**

- Only CURRENT version of Project Overview in project
- Archive superseded versions locally (not in project)
- Upload only files relevant to active work

**Naming Consistency:**

- Use full file naming convention: `yyyy-mm-dd_[Type]_[Title]_[H/C]_[Version]`
- Even fully human documents include H100-C0
- Easy to reference by exact filename

**Cross-Chat References:**

- Provide exact filename when asking Claude to check a file
- Example: "Review 2025-11-07_META_System-Design_H50-C50_v1.0.md"
- Most resource efficient approach

---

### Version Control

**Local/Cloud Storage:**

- Maintain version history outside project
- Archive format: `yyyy-mm-dd_[Type]_[Title]_[H/C]_[Version].md`
- Only current version in project files

**Version Incrementing:**

- **Minor updates:** v1.0 → v1.1 (small edits, clarifications)
- **Major updates:** v1.0 → v2.0 (significant changes, restructuring)
- **Iteration:** v1.0 → v1.5 → v2.0 (progressive development)

**Artifacts Inventory:**

- Track all artifacts with versions in Project Overview
- Shows evolution of deliverables
- Supports methodology documentation

---

### File Upload Strategy

**Rely on Project Files First:**

- Don't re-upload files already in project
- Reference by exact filename
- Only upload if file not yet in project

**When to Upload New Files:**

- New data or analysis documents
- Updated protocols or frameworks
- Session outputs that should be preserved
- Reference materials for specific work unit

**Avoid Duplication:**

- Check Project Files before uploading
- Update existing file vs. create new version
- Keep file inventory clean

---

## Chat Retirement Protocol

### Home Base Retirement Triggers

**When to retire Home Base:**

- Performance degradation (errors, date confusion, slower responses)
- Major phase transition (foundation → data collection → writing)
- Token capacity approaching limits (Level 3 warning from Claude)
- Natural break point (semester end, major milestone completion)

**Rule of Thumb:** Every 2-3 months or at major research phase shifts

**Process:**

1. Update chat name with date range: "Home Base (Aug-Nov 2025)"
2. Start new Home Base with current month
3. Update Project Overview to reflect new Home Base
4. First session in new Home Base: Brief orientation summary

---

### Work Unit Retirement Triggers

**When to retire Work Unit:**

- Deliverable complete and working
- Project abandoned (decided not to pursue)
- Superseded by different approach
- Technical degradation (batch failures, corruption)

**Rule of Thumb:** When the specific work is done

**Process:**

1. Mark status: Active → Complete (or Archived)
2. Document outcome in Project Overview
3. List in "Recently Completed Work Units" section
4. Add artifacts to Artifacts Inventory
5. Export chat if needed for methodology documentation

---

### Proactive vs. Reactive Retirement

**PROACTIVE (Preferred):**

- Retire at natural completion points
- Before token limits hit
- When phase transition occurs
- Planned and strategic

**REACTIVE (Avoid):**

- Waiting until chat breaks down
- Mid-work token limit disruption
- Error accumulation forces retirement
- Unplanned and disruptive

**Claude's Role:** Provide token warnings at three levels to enable proactive retirement

---

## META Chat Maintenance

### Purpose

Periodic consolidation of project progress into optimized Project Overview document that serves as automatic context for all chats.

### Workflow

**Frequency:** Every 2-4 weeks or after major milestones

**Process:**

1. Open META chat
2. Copy appropriate prompt template from `Project Overview Template.md`
3. Fill in updates (completed work, new chats, new files, phase changes, decisions)
4. META produces updated `Project Overview - Current.md`
5. Download artifact
6. Archive old Project Overview locally with date
7. Upload new version to project files (replaces old one)

---

### Prompt Templates

**Three templates available in `Project Overview Template.md`:**

1. **Initial Creation** - First-time setup when no Current file exists
2. **Regular Update** - Comprehensive update every 2-4 weeks
3. **Quick Reference Update** - Minor changes between major updates

**Claude's Role:**

- Reference `Project Overview Template.md` for structure
- Maintain format consistency
- Incorporate updates into proper sections
- Optimize for AI consumption (concise, structured)

---

### What to Include in Updates

**Completed Work:**

- Work units finished since last update
- Major milestones achieved
- Deliverables completed

**New Active Work:**

- New chats started
- New focus areas
- Shifted priorities

**Progress on Active Work:**

- Updates on ongoing work units
- Phase progressions
- Timeline adjustments

**New Files/Artifacts:**

- Files added to project
- Artifacts created with contribution ratios
- Version updates

**Retired/Archived:**

- Chats completed or abandoned
- Files superseded

**Key Decisions:**

- Important frameworks adopted
- Methodological choices
- Strategic directions

---

## Human/AI Responsibility Matrix

### David's Responsibilities

**Strategic Direction:**

- Define project goals and deliverables
- Make final decisions on direction
- Determine when work is complete
- Maintain research integrity

**Context Provision:**

- Provide date and timeline information
- Share relevant background and updates
- Clarify ambiguities
- Define session focus and mode

**File Management:**

- Upload files to project
- Archive versions locally
- Maintain clean file structure
- Update Project Overview regularly

**Session Structure:**

- Initiate sessions ("I'm ready to start")
- Close sessions ("I'm ready to close")
- Provide opening/closing information
- Track progress externally (Obsidian, dashboards)

**Quality Control:**

- Review outputs for accuracy
- Validate contribution ratios
- Ensure academic integrity
- Make final editing decisions

---

### Claude's Responsibilities

**Communication Adaptation:**

- Match mode (Discovery vs. Execution)
- Ask clarifying questions when needed
- Adjust tone and style appropriately
- Request files/context when necessary

**Resource Management:**

- Monitor conversation length
- Provide three-level token warnings
- Flag performance issues
- Recommend retirement timing

**Output Quality:**

- Follow naming conventions
- Provide complete artifacts (no truncation)
- Include contribution ratio estimates
- Maintain structure and clarity

**Context Maintenance:**

- Read Project Overview automatically
- Reference project files appropriately
- Track decisions within chat
- Flag inconsistencies or confusion

**System Adherence:**

- Follow established protocols
- Use correct artifact formats
- Apply naming conventions
- Respect mode distinctions

---

### Shared Responsibilities

**Scope Management:**

- Both recognize when focus drifts
- Collaboratively decide on chat boundaries
- Signal when mode needs shifting

**Learning & Adaptation:**

- Both notice what works and what doesn't
- Iterative improvement of protocols
- Flexibility within structure

**Documentation:**

- Maintain transparency about collaboration
- Track contributions accurately
- Create methodology trail

---

## Implementation Guide

### Phase 1: Account Setup (15 minutes)

**Step 1:** Copy Account-Level Custom Instructions

- Open Settings → Personalization → Custom Instructions
- Paste content from "Account-Level Custom Instructions - H30-C70" document
- Save

**Result:** Universal collaboration protocols now active across all Claude use

---

### Phase 2: Project Setup (30 minutes)

**Step 2:** Create Project (if not exists)

- Click "Projects" in sidebar
- Create new project (e.g., "EdD Research")
- Name clearly and descriptively

**Step 3:** Configure Project Instructions

- Open Project Settings → Custom Instructions
- Customize "Project-Level Instructions Template - H40-C60" for your project
- Fill in all [Required] sections
- Add [Optional] sections as relevant
- Save

**Step 4:** Upload Core Files

- Upload `Project Overview Template.md` to Project Files
- Upload any existing project documents
- Organize with clear file naming convention

**Result:** Project structure configured, ready for chat creation

---

### Phase 3: Initial Project Overview (45 minutes)

**Step 5:** Create META Chat

- Create new chat within project
- Name: `META - Project Overview Maintenance - [Today's Date] - Active`
- Example: `META - Project Overview Maintenance - 2025-11-07 - Active`

**Step 6:** Generate Initial Project Overview

- In META chat, use "Initial Creation" prompt template from `Project Overview Template.md`
- Provide current project context (active chats, files, phase, etc.)
- META produces first `Project Overview - Current.md`
- Download artifact

**Step 7:** Upload Project Overview

- Upload `Project Overview - Current.md` to Project Files
- This file will be auto-read by all future chats

**Result:** Project Overview system operational

---

### Phase 4: Create Home Base (15 minutes)

**Step 8:** Create Home Base Chat

- Create new chat within project
- Name: `[Project Name] - Home Base [Current Month Year]`
- Example: `EdD Research - Home Base (Nov 2025)`

**Step 9:** First Home Base Session

- Start with opening protocol
- Verify Project Overview is being read correctly
- Conduct normal check-in or exploratory work

**Result:** Home Base operational for ongoing work

---

### Phase 5: Create Work Unit Chats as Needed (Ongoing)

**Step 10:** Identify Need for Work Unit

- Use decision framework (specific deliverable + defined outcome)
- Determine appropriate category (DEV, DATA, THEORY, WRITING, META, etc.)

**Step 11:** Create Work Unit Chat

- Create new chat within project
- Name: `[Category] - [Deliverable] - [YYYY-MM-DD] - Active`
- Example: `DATA - Cycle 1 Coding Framework - 2025-11-01 - Active`

**Step 12:** Conduct Focused Work

- Mode: Discovery or Execution as appropriate
- Create deliverables
- Retire when complete

**Result:** Focused work units complete deliverables efficiently

---

### Phase 6: Maintain System (Ongoing)

**Step 13:** Regular META Updates

- Every 2-4 weeks, open META chat
- Use "Regular Update" prompt template
- Provide updates on progress, new chats, completed work
- Upload refreshed `Project Overview - Current.md`

**Step 14:** Monitor and Retire Chats

- Watch for Claude's token warnings
- Retire chats proactively at natural breakpoints
- Update Project Overview when chats retire
- Archive locally as needed

**Step 15:** Iterate and Improve

- Notice what works and what doesn't
- Adjust protocols as needed
- Document changes in META chat
- Update system documentation

**Result:** Sustainable long-term collaboration system

---

## Troubleshooting Guide

### Known Issues and Solutions

#### Issue: Chat Shows Incorrect Date

**Symptoms:**

- Claude references wrong date
- Cannot correct even after prompting
- Timeline confusion

**Causes:**

- Token capacity reached
- Context degradation
- Too many temporal inferences

**Solutions:**

1. Explicitly provide date at session start (always)
2. If persists, retire chat proactively
3. Start fresh chat with clear date context
4. Update Project Overview with correct timeline

**Prevention:**

- Always use opening protocol with date
- Don't rely on Claude to track time
- Provide temporal context explicitly

---

#### Issue: Batch Creation/Corruption

**Symptoms:**

- Updating multiple files simultaneously
- Files corrupted or incomplete
- Work needs redoing

**Causes:**

- System limitation with concurrent updates
- Complexity overload

**Solutions:**

1. NEVER update multiple files in one go
2. Work one file at a time
3. Wait for confirmation before next file
4. Test each change before proceeding

**Prevention:**

- Request single-file updates only
- Sequential workflow, not parallel
- Explicit: "Update only [specific file]"

---

#### Issue: Scope Creep Within Chat

**Symptoms:**

- Chat topic drifting
- Multiple projects bleeding together
- Unclear focus

**Causes:**

- No clear deliverable boundary
- Mode mixing (Discovery when Execution needed)
- Missing decision framework application

**Solutions:**

1. Reassess: Is this still same deliverable?
2. If scope expanded significantly, consider new Work Unit chat
3. Explicitly declare mode and focus at session start
4. Use Home Base for exploration, Work Unit for execution

**Prevention:**

- Clear deliverable definition for Work Units
- Recognize mode transitions
- Apply decision framework consistently

---

#### Issue: Context Loss Across Chats

**Symptoms:**

- Repeating information constantly
- Claude doesn't know decisions from other chats
- Fragmented understanding

**Causes:**

- Project Overview not updated
- Missing cross-chat documentation
- Claude cannot access other chat history

**Solutions:**

1. Update Project Overview more frequently
2. Document key decisions in Project Overview
3. Explicitly reference files in Project Files
4. Provide brief context when referencing other chats

**Prevention:**

- Regular META updates (every 2-4 weeks)
- Document major decisions immediately
- Use Project Files for shared knowledge

---

#### Issue: Token Warnings Ignored

**Symptoms:**

- Hitting token limits mid-work
- Forced disruption at bad moment
- Loss of context/progress

**Causes:**

- Ignoring Level 2 warnings
- Not planning retirement
- Pushing chat too long

**Solutions:**

1. Treat Level 2 warnings seriously
2. Plan retirement at next natural break
3. Don't wait for Level 3 (action alert)
4. Retire proactively, not reactively

**Prevention:**

- Listen to Claude's warnings
- Plan ahead for chat transitions
- Shorter work units when possible
- Lean file structure

---

#### Issue: Unclear Communication Mode

**Symptoms:**

- Questions when you want direct answers
- Technical detail when you want exploration
- Frustration with pacing

**Causes:**

- Mode not declared
- Mode transition not signaled
- Ambiguous request

**Solutions:**

1. Explicitly state mode at session start
2. Signal when switching modes
3. Claude will ask if unclear

**Prevention:**

- Use opening protocol
- Declare mode: "We're in Execution mode"
- Signal switches: "Switching to Discovery mode now"

---

#### Issue: Artifact Naming Inconsistent

**Symptoms:**

- Artifacts titled "Unknown"
- Hard to scan artifact menu
- Missing contribution ratios

**Causes:**

- Claude not following convention
- Account-level settings not applied
- Unclear deliverable description

**Solutions:**

1. Verify Account-Level instructions saved
2. Remind: "Use artifact naming convention"
3. Provide clear title suggestion

**Prevention:**

- Account-level settings properly configured
- Clear deliverable names
- Review artifact titles before accepting

---

### When to Seek Help

**Contact Anthropic Support if:**

- Persistent technical failures
- Account-level settings not applying
- Project files not accessible
- Systematic errors across conversations

**Revise System if:**

- Consistent friction points
- Protocols not serving purpose
- Better patterns emerging
- Project needs evolve

**Document in META if:**

- New issue discovered
- Solution found
- Pattern identified
- System improvement needed

---

## Quick Reference

### Daily Use Checklist

**Starting Any Session:**

1. ☑ Say "I'm ready to start"
2. ☑ Provide date and last check-in
3. ☑ State today's focus
4. ☑ Declare mode (Discovery/Execution)

**During Session:**

1. ☑ Stay focused on deliverable (Work Unit) or exploration (Home Base)
2. ☑ Signal mode switches if needed
3. ☑ Save artifacts with proper naming
4. ☑ Note any decisions for Project Overview

**Closing Any Session:**

1. ☑ Say "I'm ready to close"
2. ☑ Document accomplishments
3. ☑ Note contribution ratios
4. ☑ Identify next steps

---

### Weekly Maintenance

**Home Base Check-In:**

1. ☑ Date and time since last check-in
2. ☑ Progress report
3. ☑ Challenges or blocks
4. ☑ Next steps planning

---

### Bi-Weekly/Monthly Maintenance

**META Chat Update:**

1. ☑ Open META chat
2. ☑ Use update prompt template
3. ☑ Provide comprehensive updates
4. ☑ Download new Project Overview
5. ☑ Archive old version locally
6. ☑ Upload new version to Project Files

---

### Decision Quick Reference

**Home Base or Work Unit?**

- Exploring with no defined outcome → **Home Base**
- Specific deliverable with done-state → **Work Unit**

**Discovery or Execution?**

- Figuring out what I want → **Discovery**
- Know what I want, need how-to → **Execution**

**New Chat or Continue Current?**

- Same deliverable, same focus → **Continue**
- Different deliverable or major scope change → **New Chat**

**Retire Chat or Keep Going?**

- Level 2 token warning + natural break → **Retire**
- Performance issues or phase change → **Retire**
- Work flowing well and focused → **Keep Going**

---

### File Location Quick Reference

**Account-Level Instructions:**
Settings → Personalization → Custom Instructions

**Project-Level Instructions:**
Project Settings → Custom Instructions

**Project Files:**
Project → Files (upload documents)

**Project Overview - Current.md:**
Project Files (auto-read by all chats)

**Project Overview Template.md:**
Project Files (reference for META)

**Archived Versions:**
Local storage (not in Claude project)

---

### Naming Pattern Quick Reference

**Chats:**

- Home Base: `[Project] - Home Base [Month Year]`
- Work Unit: `[Category] - [Deliverable] - [YYYY-MM-DD] - [Status]`

**Artifacts:**

- Format: `[Title] - [H/C Ratio]`

**Files:**

- Format: `yyyy-mm-dd_[Type]_[Title]_[H/C]_[Version]`

**Contribution Ratios:**

- Format: `H[X]-C[Y]` (totals 100)
- Even fully human: `H100-C0`

---

### Emergency Protocols

**Chat Completely Broken:**

1. Don't panic
2. Retire current chat immediately
3. Start fresh chat with opening protocol
4. Provide brief context recap
5. Update Project Overview in META

**Lost Important Work:**

1. Check artifact menu in conversation
2. Check Project Files
3. Check local archives
4. Reconstruct from session notes
5. Document in Project Overview for prevention

**System Not Working:**

1. Review this guide
2. Check Account and Project settings
3. Verify file locations
4. Update Project Overview
5. Revise protocols if needed

---

## Citation

**APA Format:**

Dawson, D. R., II. (2025). *AI collaboration system: Comprehensive reference guide*. Northeastern University. https://drdawson2.github.io/dissertation-guide/

**Note:** Update URL with specific GitHub repository location when published.

---

## Document Version History

**v1.0 - November 7, 2025**

- Initial comprehensive reference guide created
- Two-tier chat system architecture defined
- Complete naming conventions established
- Session protocols developed
- META maintenance workflow documented
- Implementation guide created
- Troubleshooting guide added

---

## About This Document

This reference guide was developed through AI-human collaboration following the framework documented herein. The system represents an iterative, action research approach to designing sustainable protocols for long-term AI collaboration in academic research contexts.

**Methodology Note:** This document serves as both a practical implementation guide and a methodological artifact for examining AI-human collaboration practices in doctoral research. The development process itself demonstrates the protocols it describes.

---

## Footer

**Copyright & Licensing**

© 2025 David R. Dawson II | Northeastern University

Licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)

**Attribution:**

- **Author:** David R. Dawson II
- **ORCID:** [0009-0001-4719-4370](https://orcid.org/0009-0001-4719-4370)
- **Institution:** Northeastern University, Graduate School of Education
- **Contact:** [davidrobertodawsonii@outlook.com](mailto:davidrobertodawsonii@outlook.com)

**Quick Links:**
[Research Context](https://drdawson2.github.io/dissertation-guide/) | [Contact](mailto:davidrobertodawsonii@outlook.com) | Versions (Coming Soon)

**Last Updated:** November 7, 2025

---

**END OF REFERENCE GUIDE**



---

## Contribution Report

**Human Contribution (50%):**

- All architectural decisions (two-tier system)
- All organizational requirements
- All naming conventions concepts
- All protocol requirements
- All strategic direction

**Claude Contribution (50%):**

- Documentation structure and formatting
- Implementation guide development
- Troubleshooting guide compilation
- Decision frameworks organization
- Quick reference synthesis

**Collaboration Type:** Equal partnership - human design with AI documentation

Citation & Attribution

**Citation (APA 7th Edition):** Dawson, D. R., II. (2025). *AI collaboration system: Comprehensive reference guide*. Northeastern University. https://github.com/drdawson2/ai-collaboration-reference-guide

**Author Information:**

* **Name:** David R. Dawson II
* **ORCID:** [0009-0001-4719-4370](https://orcid.org/0009-0001-4719-4370)
* **Institution:** Northeastern University, Graduate School of Education
* **Email:** davidrobertodawsonii@outlook.com

**License:** This work is licensed under a [Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/).

**You are free to:**

* Share — copy and redistribute the material in any medium or format
* Adapt — remix, transform, and build upon the material

**Under the following terms:**

* **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made.
* **NonCommercial** — You may not use the material for commercial purposes.

**Suggested Attribution:**"Based on [Document Title] by David R. Dawson II (2025), available at https://github.com/drdawson2/ai-collaboration-reference-guide. Licensed under CC BY-NC 4.0."

* * *

**Last Updated:** 2025-11-09
