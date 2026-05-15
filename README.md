# HeavyBid Setup Project

## Project Purpose

The HeavyBid Setup Project is focused on building, organizing, documenting, and governing the company’s HCSS HeavyBid estimating environment.

The goal is not simply to “get HeavyBid working,” but to create a maintainable estimating system that supports consistent bid development, reliable cost structure, useful reporting, and future integration with HeavyJob and other operational systems.

This project treats HeavyBid as a business system, not just estimating software.

---

## Executive Summary

The HeavyBid Setup Project establishes the estimating foundation for consistent, repeatable, and maintainable bid development. The project includes codebook design, estimate templates, resource setup, quote organization, governance documentation, and HeavyBid-to-HeavyJob transfer planning.

The intent is to create a system that supports both day-to-day estimating and longer-term organizational improvement through better structure, cleaner data, and more transparent estimating logic.

---

## Primary Objectives

- Establish a clean and usable HeavyBid setup for active estimating work.
- Build logical codebooks for bid items, activities, materials, crews, equipment, labor, subcontractors, and other estimating resources.
- Align estimating structure with how work is actually performed, tracked, transferred, and reviewed.
- Support HeavyBid-to-HeavyJob transfer workflows.
- Improve transparency of estimating assumptions, calculations, and production logic.
- Document setup decisions so the system can be maintained and improved over time.
- Create governance practices that prevent uncontrolled drift in codebooks, assemblies, templates, and estimating standards.

---

## Project Scope

This project includes the setup and documentation of the HeavyBid estimating environment, including but not limited to:

- Bid Item Codebook
- Activity Codebook
- Material Codebook
- Labor setup
- Equipment setup
- Crew setup
- Subcontractor/vendor setup
- Quote folders and quote organization
- Estimate templates
- Standard calculations
- Assemblies and reusable estimating logic
- HeavyBid-to-HeavyJob transfer considerations
- Governance documentation
- Security and access considerations
- Process documentation for estimators and support users

This project may reference HeavyJob, HCSS Credentials, accounting structures, scheduling, and field operations where those systems affect HeavyBid setup or downstream workflow.

---

## Out of Scope

The following items are related but not primary deliverables of this project unless explicitly added later:

- Full HeavyJob implementation
- Accounting system redesign
- Company-wide ERP replacement
- Field production tracking redesign
- Payroll system configuration
- Formal IT infrastructure design
- Full enterprise data warehouse implementation

These areas may be considered dependencies, constraints, or future integration points.

---

## Current Project Focus

The current phase is focused on building the base document structure and initial governance framework for the HeavyBid Setup project.

Key areas of attention include:

- Understanding the current state of the HeavyBid setup.
- Identifying what has already been configured.
- Separating usable configuration from items that may need redesign.
- Developing executive-level summaries of project status.
- Building governance documents that explain how decisions should be made and maintained.
- Creating parallel documentation with the HCSS Implementation project where appropriate.

---

## Documentation Structure

The project documentation is organized into a simple numbered folder structure. The intent is to separate governance, planning, working notes, technical design, reporting, and archived materials while keeping the root project directory clean.

The active project structure is:

```text
HB-Setup/
│
├── README.md
├── .gitignore
│
├── 0-Governance/
│   ├── PROJECT-CHARTER.md
│   ├── BUSINESS-CASE.md
│   ├── STAKEHOLDER-REGISTER.md
│   ├── COMMUNICATION-PLAN.md
│   ├── DECISION-LOG.md
│   ├── RISK-REGISTER.md
│   ├── ISSUE-LOG.md
│   ├── CHANGE-LOG.md
│   ├── DATA-GOVERNANCE.md
│   ├── SECURITY-ASSESSMENT.md
│   └── AI-GOVERNANCE-POLICY.md
│
├── 1-Planning/
│   ├── ROADMAP.md
│   ├── BACKLOG.md
│   ├── REQUIREMENTS.md
│   └── MILESTONES.md
│
├── 2-Working-Docs/
│   ├── MEETING-NOTES.md
│   ├── WORKING-NOTES.md
│   └── RESEARCH-NOTES.md
│
├── 3-Technical/
│   ├── SYSTEM-OVERVIEW.md
│   ├── DATA-MODEL.md
│   ├── WORKFLOW-DESIGN.md
│   └── INTEGRATION-NOTES.md
│
├── 4-Reports/
│   ├── STATUS-REPORTS.md
│   └── LESSONS-LEARNED.md
│
└── 9-Archive/
    └── README.md
```
---

## Guiding Principles

### 1. Build for Maintainability

HeavyBid should be configured in a way that future users can understand, maintain, and extend. A setup that only works because one person remembers why it was built that way is fragile.

### 2. Estimate the Way the Work Is Built

Activities, resources, crews, and production logic should reflect actual construction means and methods wherever practical.

### 3. Separate Detail from Summary

The estimating system should support detailed estimating while still allowing summarized reporting, cost-code mapping, and transfer to downstream systems.

### 4. Document Decisions

Important setup decisions should be captured in a decision log. This includes decisions about codebook structure, naming conventions, transfer logic, bid item strategy, activity design, and governance rules.

### 5. Avoid Uncontrolled Drift

Codebooks and templates should not evolve through undocumented one-off edits. Changes should be reviewed, documented, and applied deliberately.

### 6. Support Integration

HeavyBid setup decisions should consider downstream impact on HeavyJob, accounting, scheduling, reporting, and project management.

### 7. Favor Practical Standards Over Perfect Theory

The system should be structured enough to provide consistency but flexible enough to support real estimating work.

---

## Key System Areas

### Bid Item Codebook

The Bid Item Codebook serves as a central bridge between owner pay items and internal estimating logic. It should support consistency across estimates while allowing flexibility for project-specific requirements.

Key concerns:

* Client pay item structure
* Internal item organization
* Bid item descriptions
* Units of measure
* Reusable bid item logic
* Mapping to activities and resources
* Future reporting value

---

### Activity Codebook

The Activity Codebook should describe work in a way that supports production-based estimating and downstream understanding.

Key concerns:

* Activity naming conventions
* Cost code structure
* Relationship to bid items
* Relationship to crews and resources
* Quantity and unit conversions
* Compatibility with HeavyJob transfer
* Avoiding excessive fragmentation or oversimplification

---

### Material Codebook

The Material Codebook should describe what the material is, not merely what it is used for.

Key concerns:

* General-to-specific organization
* Vendor quote support
* Quote folder mapping
* Reusable material descriptions
* Avoiding duplicate or near-duplicate materials
* Supporting both estimating and purchasing workflows

---

### Quote System

The quote system should support organized vendor and subcontractor comparison.

Key concerns:

* Quote folders
* Material and subcontractor quote organization
* Side-by-side comparison
* Plug numbers
* Late quote adjustments
* Traceability of selected quotes
* Clear review process

---

### Estimate Templates and Assemblies

Templates and assemblies should reduce repetitive work while preserving estimator control and transparency.

Key concerns:

* Standard estimate structure
* Reusable assemblies
* Roadway illumination assemblies
* Signalization assemblies
* Conduit calculations
* Crew/productivity assumptions
* Template governance

---

## Governance Approach

Governance is required so that the HeavyBid setup remains stable, understandable, and useful.

Recommended governance documents include:

* Project Charter
* Executive Summary
* Decision Log
* Risk Register
* Issue Log
* Change Control Procedure
* Data Governance Document
* Security Assessment
* User Roles and Access Matrix
* Codebook Maintenance Guidelines
* Estimate Template Maintenance Guidelines

Governance should answer:

* Who can change shared codebooks?
* Who approves structural changes?
* How are changes tested?
* How are changes documented?
* How are old versions preserved?
* How are estimate templates reviewed?
* How are downstream impacts checked?

---

## Risks and Constraints

Known or likely project risks include:

* Moving too quickly to production before setup decisions are fully understood.
* Carrying forward flawed early configuration because it appears to work in a simple test.
* Creating codebooks without clear naming or maintenance standards.
* Overbuilding detail that becomes difficult for estimators to use.
* Underbuilding detail that weakens reporting and HeavyJob transfer.
* Lack of documentation around key setup decisions.
* Misalignment between estimating structure and accounting or field tracking structures.
* Limited organizational understanding of how HeavyBid setup affects downstream systems.

---

## Current Deliverables

Initial deliverables should include:

* README.md
* Project Charter
* Executive Summary
* Current State Assessment
* Data Governance Document
* Security Assessment
* Decision Log
* Risk Register
* Codebook Review Notes
* Target State Overview
* HeavyBid-to-HeavyJob Transfer Strategy

---

## Working Status

This project is currently in an active setup and documentation phase.

The immediate priority is to establish the base documentation structure and begin creating governance documents that describe how the HeavyBid environment should be built, maintained, reviewed, and improved.

This README should be updated as the project matures.

---

## Suggested Next Steps

1. Create the project folder structure.
2. Add this README as the project root document.
3. Draft the Project Charter.
4. Draft the Executive Summary.
5. Create the Decision Log and Risk Register.
6. Review the current HeavyBid setup against the target documentation structure.
7. Begin documenting codebook-specific findings.
8. Align HeavyBid Setup documentation with the broader HCSS Implementation documentation.

---

## Project Owner / Stewardship

This project should have a clearly identified owner or steward responsible for documentation quality, governance discipline, and alignment between setup decisions and business needs.

The project steward is not necessarily the only person making decisions, but should ensure that decisions are visible, traceable, and connected to the larger implementation strategy.

---

## README Maintenance Notes

This README should be reviewed and updated when:

* Major setup milestones are completed.
* Governance documents are added or revised.
* Codebook strategy changes.
* HeavyBid-to-HeavyJob workflow assumptions change.
* New project risks are identified.
* The documentation structure changes.
* The project moves from setup into production support.

## Change Log

| Version | Date | Author | Description of Change |
|---|---:|---|---|
| v0.1 | 2026-05-15 | James Caudill | Initial README draft created for the HeavyBid Setup project. Included project purpose, objectives, scope, guiding principles, key system areas, governance approach, risks, deliverables, working status, and suggested next steps. |
| v0.2 | 2026-05-15 | James Caudill | Updated the Documentation Structure section to align with the approved numbered project folder structure: `0-Governance`, `1-Planning`, `2-Working-Docs`, `3-Technical`, `4-Reports`, and `9-Archive`. |
