# Project-Level Instructions Template

**Instructions:** Customize each section for your specific project. Sections marked [REQUIRED] apply to all projects. Sections marked [OPTIONAL] apply only if relevant to the project type.

---

## [REQUIRED] Project Context

**Project Name:** [Insert project name]

**Project Purpose:** [1-2 sentence description of what this project accomplishes]

**Timeline:** [Start date] to [Expected completion date]

**Current Phase:** [Brief description of current phase/focus]

---

## [OPTIONAL] Research Methodology (For Academic Projects)

**Methodology Type:** [e.g., Action Research, Qualitative Interview Study, Mixed Methods]

**Research Focus:** [1-2 sentence description of research question/focus]

**Key Frameworks:** [Theoretical frameworks or models guiding the work]

**Cycle/Phase Structure:** [If using iterative methodology, describe cycle structure]

---

## [REQUIRED] Temporal Context Protocol

**Date Provision:** David will always provide current date and timeline context at the start of sessions for this project. Do not make temporal inferences or assumptions about "when" things are happening. If date/timeline context is needed and not provided, ask David directly rather than inferring.

**Key Milestones:** [List major project milestones with dates]

---

## [REQUIRED] Chat Architecture

This project uses a two-tier chat system:

### TIER 1: Home Base Chat

- **Purpose:** Brainstorming, check-ins, exploratory thinking, meta-learning
- **Mode:** Primarily Discovery Mode (dialogic, exploratory)
- **Lifespan:** Long-running (months), retired only when unwieldy
- **Current Home Base:** [Chat name - will be updated as chats retire]

### TIER 2: Work Unit Chats

- **Purpose:** Specific deliverables with bounded scope
- **Mode:** Varies by work type (Discovery for design, Execution for development)
- **Lifespan:** Short (days to weeks), retired when work unit completes

**Decision Rule:**

- **Home Base:** Exploratory thinking, check-ins, learning, no defined deliverable
- **Work Unit:** Specific deliverable with clear done-state

---

## [REQUIRED] Chat Naming Conventions

### Home Base Chat Format:

```
[Project Name] - Home Base [Month Year]
Example: EdD Research - Home Base (Nov 2025)
```

When retired, add date range: `EdD Research - Home Base (Aug-Nov 2025)`

### Work Unit Chat Format:

```
[Category] - [Specific Deliverable] - [YYYY-MM-DD] - [Status]
Examples:
- DEV - Dissertation Website - 2025-10-15 - Active
- DATA - Cycle 1 Coding Framework - 2025-11-01 - Active
- WRITING - Methodology Chapter - 2026-02-10 - Active
- META - Project Overview Maintenance - 2025-11-07 - Active
```

### Category Codes:

- **DEV** = Development/Technical work
- **DATA** = Data collection/analysis
- **THEORY** = Theoretical synthesis/analysis
- **WRITING** = Writing/drafting
- **META** = System design/organizational work
- **[Custom]** = Project-specific categories as needed

### Status Options:

- **Active** = Currently working
- **Paused** = May return to, not complete
- **Complete** = Deliverable finished, chat retired
- **Archived** = Superseded or no longer relevant

---

## [REQUIRED] File Management Protocol

### Automatic File Access:

At the start of every conversation in this project, Claude will automatically read:

- **`Project Overview - Current.md`** for context about project status, active chats, and relevant files

### Project Overview Structure:

The Project Overview document serves as a routing system, indicating:

- Current project phase/status
- Active chats and their relevant files
- Recent updates and decisions
- Which files each chat type should reference

### File Organization:

- Only keep CURRENT version of Project Overview in project files
- Archive previous versions locally with dates for record-keeping
- Keep project files lean to minimize resource overhead

---

## [REQUIRED] Chat Retirement Protocol

### Home Base Retirement Triggers:

- Performance degradation (errors, confusion, slow responses)
- Major phase transition in project
- Token capacity approaching limits (Claude will warn)
- Natural break point (completion of major milestone)
- **Rule of thumb:** Every 2-3 months or at major phase shifts

### Work Unit Retirement Triggers:

- Deliverable complete
- Project abandoned or superseded
- Technical degradation accumulating
- **Rule of thumb:** When specific work is done

### Retirement Process:

1. Mark status in chat name (Active → Complete/Archived)
2. Create summary in Home Base if key decisions need preserving
3. Export chat if needed for methodology documentation
4. Start fresh chat for next work unit

---

## [REQUIRED] Cross-Chat Coherence Strategy

**Project Instructions + Project Overview maintain coherence:**

- These instructions provide "how we work together" protocols
- Project Overview provides "where we are now" context
- Individual chats don't need to repeat full context

**When starting any chat in this project:**

1. Claude reads these project instructions automatically
2. Claude reads Project Overview - Current.md automatically
3. David provides date and specific session focus
4. Claude has sufficient context to engage effectively

**Meta Chat for Maintenance:**

- Long-running META chat exists for updating Project Overview
- Every 2-4 weeks: consolidate updates into refreshed Overview
- Keeps all chats aligned on current project state

---

## [OPTIONAL] Project-Specific Protocols

[Add any protocols specific to this project type that don't fit above categories]

Examples for dissertation project:

- Academic integrity requirements
- Citation practices
- Data handling protocols
- IRB considerations

---

## [OPTIONAL] Key Resources & References

[List critical documents, frameworks, or resources Claude should be aware of]

Examples:

- Dissertation proposal
- Theoretical framework documents
- Interview protocols
- Coding schemes

---

## Example: EdD Research Project Implementation

**Project Name:** EdD Dissertation Research

**Project Purpose:** Doctoral dissertation on career development, organizational support structures, and self-directed learning in higher education administration.

**Timeline:** August 2024 - May 2027 (Defense)

**Current Phase:** Foundation building transitioning to Cycle 1 data collection (Nov 2025)

**Methodology Type:** Action Research with qualitative interviews

**Research Focus:** How do organizational support structures facilitate or constrain self-directed career development in higher education administration?

**Key Frameworks:** Hall's Protean Career Theory, Savickas' Career Construction Theory

**Cycle Structure:**

- Cycle 1 (Nov 2025 - April 2026): Data collection and analysis of current state
- Cycle 2 (May 2026 - Aug 2026): Intervention design and implementation
- Analysis and writing (Sept 2026 - May 2027)

**Key Milestones:**

- First interview: November 14, 2025
- Intensive data collection: January-February 2026
- Heavy data analysis: March-April 2026
- Cycle 2 implementation: May-August 2026
- Dissertation writing: September 2026 - February 2027
- Defense: May 2027

**Current Home Base:** EdD Research - Home Base (Nov 2025)

**Project-Specific Values:**

- Research must be accessible to non-academic audiences
- Transparent AI collaboration for methodological contribution
- Work should democratize knowledge about career development

---

## Contribution Report

**Human Contribution (40%):**

- Project-specific requirements
- Example implementation content
- Customization needs
- Usage context

**Claude Contribution (60%):**

- Template structure and sections
- Format organization
- Implementation examples
- Documentation standards
- Instruction clarity

**Collaboration Type:** Template development - human requirements with AI structure-heavy organization

Citation & Attribution

**Citation (APA 7th Edition):** Dawson, D. R., II. (2025). *Project-level instructions template for AI collaboration*. Northeastern University. https://github.com/drdawson2/ai-collaboration-reference-guide

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
