# Project Charter

## HeavyBid Setup Project

**Document Status:** Draft v0.2
**Project Name:** HeavyBid Setup Project
**Short Name:** HB Setup
**Organization:** MICA Corporation
**Prepared By:** James Caudill
**Date:** May 15, 2026

---

## 1. Project Purpose

The purpose of the HeavyBid Setup Project is to establish a structured, reliable, and scalable estimating environment within HCSS HeavyBid that supports MICA Corporation’s estimating, bidding, cost development, and future HeavyJob integration needs.

This project is intended to move HeavyBid from an initial implementation state into a governed production-ready estimating system. The focus is not merely software configuration, but the creation of a repeatable estimating framework that improves consistency, transparency, knowledge capture, bid preparation efficiency, and downstream project handoff.

---

## 2. Project Background

MICA Corporation is implementing HCSS HeavyBid as part of a broader modernization of estimating and project execution workflows. Initial setup work has begun, including exploration of bid items, activities, resources, cost structures, and estimate automation. However, the system requires deliberate organization before it can serve as a dependable foundation for estimating operations.

Key implementation concerns include:

* Existing setup elements may not fully reflect MICA’s estimating logic, field operations, or reporting needs.
* HeavyBid must support both detailed estimating and practical project execution handoff.
* HeavyBid setup decisions may affect HeavyJob integration, cost tracking, reporting, and future analytics.
* Governance is needed to prevent uncontrolled changes, duplicated structures, inconsistent naming, and unclear ownership.
* Documentation is needed so the system can be maintained, explained, trained, and improved over time.

This charter establishes the formal purpose, scope, objectives, governance expectations, and success criteria for the HB Setup Project.

---

## 3. Business Need

MICA requires an estimating system that can support:

* Consistent bid preparation across estimators and project types.
* Reliable activity, resource, labor, equipment, subcontractor, and material structures.
* Transparent estimate calculations and assumptions.
* Better linkage between bid items, production activities, crews, and cost codes.
* More effective handoff from estimating to operations.
* Future integration between HeavyBid and HeavyJob.
* Improved reporting, analysis, and institutional knowledge retention.

Without a structured setup approach, HeavyBid risks becoming a digital version of fragmented estimating practices rather than a controlled estimating system.

---

## 4. Project Objectives

The HB Setup Project will pursue the following objectives:

1. **Establish a governed HeavyBid structure**
   Define the core setup logic for bid items, activities, resources, cost codes, crews, quote folders, and related estimating components.

2. **Create a reliable estimating foundation**
   Build structures that support repeatable bid development, reduce rework, and improve estimate consistency.

3. **Support HeavyBid-to-HeavyJob integration**
   Prepare HeavyBid structures so estimate data can transfer cleanly into HeavyJob where practical and appropriate.

4. **Improve transparency of estimating logic**
   Move critical calculations, assumptions, and production logic into visible, explainable estimate structures where possible.

5. **Document system design decisions**
   Create governance and reference documents that explain how HeavyBid is configured and why key decisions were made.

6. **Enable future analytics and reporting**
   Structure estimating data in a way that supports future analysis of bid history, production rates, resource usage, cost trends, and estimate performance.

---

## 5. Project Scope

### In Scope

The project includes the review, design, setup, documentation, and governance of core HeavyBid estimating structures, including but not limited to:

* Bid Item Codebook structure
* Activity Codebook structure
* Resource Codebook structure
* Labor, equipment, material, subcontract, and crew setup
* Quote folder structure
* Estimate templates and library estimates
* Assemblies and reusable estimate logic
* Cost code alignment
* Alternate cost code strategy, where applicable
* Naming conventions
* Unit-of-measure standards
* Production rate assumptions
* HeavyBid-to-HeavyJob handoff considerations
* Setup documentation
* Governance procedures for future changes
* Initial executive summaries and project status reporting

### Out of Scope

The following items are not part of the initial project scope unless later added through change control:

* Full HeavyJob implementation
* Full accounting system redesign
* Company-wide ERP redesign
* Complete historical bid data warehouse development
* Full automation of all estimating functions
* Final production deployment without management approval
* Training program rollout beyond initial documentation and internal knowledge transfer
* Replacement of estimator judgment with automated logic

---

## 6. Key Deliverables

The project should produce the following deliverables:

### Governance and Planning Deliverables

* Project Charter
* Business Case
* README / project overview
* Communication Plan document
* Decision log
* Risk register
* Change control process
* Stakeholder summary
* Executive summary

### HeavyBid Setup Deliverables

* HeavyBid setup assessment
* Bid Item Codebook design guidance
* Activity Codebook design guidance
* Resource Codebook design guidance
* Cost code alignment notes
* Quote folder structure
* Crew/resource setup standards
* Naming convention guide
* Unit-of-measure standards
* Estimate template strategy
* Library estimate strategy
* Assembly development standards

### Integration and Handoff Deliverables

* HeavyBid-to-HeavyJob handoff considerations
* Cost tracking alignment notes
* Estimating-to-operations handoff workflow
* Known integration risks and constraints

### Documentation and Knowledge Deliverables

* Setup documentation repository
* Glossary of HeavyBid/MICA estimating terms
* Process notes from setup sessions
* Current-state and future-state summaries
* Training/reference notes for future users

---

## 7. Project Stakeholders

### Executive / Leadership Stakeholders

* Company President
* Senior leadership involved in estimating, operations, and implementation decisions

### Business Stakeholders

* Estimators
* Project managers
* Schedulers
* Operations leadership
* Accounting or cost tracking stakeholders
* Administrative staff supporting bid setup or project setup

### Technical / System Stakeholders

* HeavyBid users
* HeavyJob users
* HCSS support or implementation contacts
* Internal staff responsible for system governance, reporting, or analytics

### Project Contributor

* James Caudill — Assistant Estimator / HeavyBid setup contributor / documentation and analytics support

---

## 8. Roles and Responsibilities

| Role                           | Responsibility                                                              |
| ------------------------------ | --------------------------------------------------------------------------- |
| Project Sponsor                | Provides direction, priority, and approval for major setup decisions        |
| Project Lead / Coordinator     | Organizes setup work, documentation, issue tracking, and progress summaries |
| Estimating Stakeholders        | Provide estimating logic, workflow requirements, and validation feedback    |
| Operations Stakeholders        | Provide input on field execution, cost tracking, and handoff requirements   |
| Accounting / Cost Stakeholders | Provide input on cost code alignment and reporting constraints              |
| HCSS Support / Consultants     | Provide product-specific guidance and best-practice clarification           |
| Documentation Owner            | Maintains project documentation, decision logs, and governance records      |

---

## 9. Project Governance

The HB Setup Project should be governed as a controlled configuration and business process project.

Key governance expectations include:

* Major setup decisions should be documented.
* Changes to codebooks, templates, and reusable structures should be intentional.
* Naming conventions and structural standards should be followed.
* New setup elements should be reviewed before becoming standard.
* Temporary test structures should be clearly identified and either promoted, archived, or removed.
* Project documentation should remain current enough to support future users and leadership review.
* Risks, assumptions, open questions, and unresolved decisions should be tracked.

The goal of governance is not to slow implementation, but to prevent confusion, rework, and uncontrolled system drift.

---

## 10. Success Criteria

The HB Setup Project will be considered successful when:

* HeavyBid has a documented base structure that reflects MICA’s estimating needs.
* Core codebooks are organized, explainable, and usable.
* Estimators can build estimates using repeatable structures rather than ad hoc setup.
* Bid item, activity, resource, and cost code relationships are clear enough to support estimating and handoff.
* Reusable estimate logic exists for common work types.
* HeavyBid-to-HeavyJob handoff requirements are understood and partially validated.
* Leadership can review an executive summary of current state, risks, progress, and next steps.
* Future users can understand the setup through documentation without relying entirely on tribal knowledge.
* The system is stable enough to support controlled production use and future improvement.

---

## 11. Initial Risks

| Risk                             | Description                                                      | Potential Impact                                     |
| -------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------- |
| Premature go-live                | HeavyBid may be pushed into production before setup is stable    | Inconsistent estimates, rework, poor downstream data |
| Unclear ownership                | No single owner for codebook structure or governance             | Conflicting changes and setup drift                  |
| Over-customization               | System may become too complex too early                          | Difficult maintenance and user adoption issues       |
| Under-documentation              | Decisions may be made verbally without durable records           | Loss of knowledge and repeated debate                |
| Misaligned cost codes            | Estimating detail may not align with operations/accounting needs | Poor handoff and reporting gaps                      |
| HeavyJob integration assumptions | HeavyBid setup may not transfer cleanly into HeavyJob            | Failed or limited integration value                  |
| User resistance                  | Estimators or operations users may avoid structured workflows    | Reduced adoption and inconsistent use                |
| Scope creep                      | Setup project may expand into full ERP/process redesign          | Loss of focus and delayed deliverables               |

---

## 12. Assumptions

This charter assumes:

* HeavyBid will become a central estimating system for MICA.
* HeavyJob integration is a meaningful long-term objective.
* Existing estimating knowledge must be preserved and translated into the system.
* Setup should support both practical bidding and future data analysis.
* Documentation is a necessary part of implementation, not an optional afterthought.
* The initial project will evolve through discovery as current setup conditions become clearer.

---

## 13. Constraints

Known constraints include:

* Business operations and active estimating work must continue during setup.
* Time available for structured analysis may be limited.
* Leadership may expect rapid validation of HeavyBid functionality.
* HCSS configuration options may constrain ideal process design.
* Existing cost structures, accounting practices, or operational workflows may limit redesign options.
* Some decisions may need to be made before all downstream impacts are fully known.

---

## 14. Project Approach

The HB Setup Project should proceed through iterative documentation, assessment, setup, validation, and refinement.

### Phase 1 — Foundation and Documentation

* Establish project charter, business case, README, and governance structure.
* Identify current state of HeavyBid setup.
* Document known assumptions, risks, and open questions.

### Phase 2 — Current-State Assessment

* Review existing codebooks, templates, resources, and estimate structures.
* Identify inconsistencies, gaps, duplicates, and unclear design decisions.
* Summarize current state for leadership and project stakeholders.

### Phase 3 — Base Structure Design

* Define preferred structure for bid items, activities, resources, crews, and cost codes.
* Establish naming conventions and organizational rules.
* Clarify how estimating detail should connect to project execution needs.

### Phase 4 — Prototype and Validation

* Build or refine sample structures in HeavyBid.
* Test with real or representative estimates.
* Validate usefulness with estimating and operations stakeholders.

### Phase 5 — Governance and Controlled Expansion

* Formalize change control and maintenance practices.
* Promote validated structures into standard use.
* Continue improving documentation, templates, and reusable assemblies.

---

## 15. Open Questions

The following questions should be tracked and resolved as the project matures:

* Who has final approval authority for HeavyBid setup standards?
* What level of estimating detail should be transferred into HeavyJob?
* How should MICA balance detailed estimating structures with simplified accounting cost codes?
* Which work types should receive reusable assemblies first?
* What naming conventions should be mandatory?
* What setup changes require review before implementation?
* How should temporary testing structures be managed?
* What is the minimum viable setup required before HeavyBid can be considered production-ready?
* What reports or analytics should the system support in the future?

---

## 16. Approval

Approval of this charter authorizes the HB Setup Project to proceed as a structured setup, governance, and documentation effort.

| Name | Role                      | Approval | Date |
| ---- | ------------------------- | -------- | ---- |
|      | Project Sponsor           |          |      |
|      | Estimating Lead           |          |      |
|      | Operations Representative |          |      |
|      | Project Contributor       |          |      |

---

## 17. Charter Summary

The HeavyBid Setup Project exists to transform HeavyBid from a software implementation into a governed estimating system. The project will define, organize, document, and validate the structures needed for consistent estimating, practical project handoff, and future analytics.

The immediate priority is to establish a clear foundation: understand the current state, document key decisions, define setup standards, and build enough structure to support controlled progress without locking the company into poorly understood assumptions.

---

## Document Change Log

| Version |       Date | Author        | Change Summary                                                                                            | Reason / Notes                                                                                                                                                       |
| ------- | ---------: | ------------- | --------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| v0.1    | 2026-05-15 | James Caudill | Initial draft of the Project Charter created.                                                             | Established the baseline charter structure, including purpose, scope, objectives, deliverables, stakeholders, risks, assumptions, constraints, and approval section. |
| v0.2    | 2026-05-15 | James Caudill | Updated Key Deliverables section: changed “Project Governance Document” to “Communication Plan document.” | Revision clarifies that the project requires a dedicated communication planning artifact as part of the core governance/documentation package.                       |

### Change Log Maintenance Notes

* Add a new row each time the document is materially revised.
* Increment the version number for meaningful content changes.
* Minor spelling, formatting, or punctuation edits may be recorded only when useful.
* Use the **Change Summary** field to describe what changed.
* Use the **Reason / Notes** field to explain why the change was made or what decision it reflects.
