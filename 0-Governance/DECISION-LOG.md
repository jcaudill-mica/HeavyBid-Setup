# HB Setup Decision Log

**Project:** HeavyBid (HB) Setup
**Document Type:** Decision Log
**Version:** 0.1
**Status:** Draft
**Owner:** James Caudill
**Purpose:** Track key implementation decisions, rationale, alternatives considered, and follow-up actions for the HeavyBid setup project.

---

## 1. Document Purpose

The Decision Log provides a structured record of important decisions made during the HB Setup project. Its purpose is to preserve the reasoning behind configuration choices, design standards, governance rules, and implementation priorities.

This log helps prevent repeated debate, supports onboarding, and provides an audit trail for why the HeavyBid environment was built a certain way.

---

## 2. Decision Log Table

| ID     | Date | Decision Area            | Decision                                                                                                                       | Rationale                                                                                                                                                                                     | Alternatives Considered                                               | Impact                                                             | Status   | Owner         |
| ------ | ---- | ------------------------ | ------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------- | ------------------------------------------------------------------ | -------- | ------------- |
| DL-001 | TBD  | Project Structure        | Establish HB Setup as a formal implementation project with supporting documentation.                                           | The setup effort affects estimating standards, cost structure, project transfer, reporting, and future HeavyJob integration. Treating it as a project improves accountability and continuity. | Handle setup informally through ad hoc configuration changes.         | Creates a documentation baseline and supports governance.          | Proposed | James Caudill |
| DL-002 | TBD  | Documentation            | Maintain core project documents including README, Charter, Business Case, Governance, and Decision Log.                        | HeavyBid setup decisions have long-term operational consequences. Documentation reduces knowledge loss and supports executive communication.                                                  | Keep notes only in chat, OneNote, or informal working files.          | Improves traceability and provides reusable reference material.    | Proposed | James Caudill |
| DL-003 | TBD  | Implementation Approach  | Use an analysis-first setup approach rather than rushing directly into production use.                                         | HeavyBid configuration affects activity structure, resource coding, bid item mapping, quote workflows, and HeavyJob transfer. Premature use may lock in poor structures.                      | Configure quickly and refine after initial use.                       | Reduces rework and improves long-term system quality.              | Proposed | James Caudill |
| DL-004 | TBD  | Codebook Design          | Treat codebooks as governed master data rather than simple lookup lists.                                                       | Codebooks drive consistency, automation, estimating behavior, and reporting. Poor governance can create duplicate, inconsistent, or unusable records.                                         | Allow each estimator to freely create and modify codes as needed.     | Supports standardization, reporting, and future integration.       | Proposed | James Caudill |
| DL-005 | TBD  | Activity Structure       | Design Activities around meaningful estimating work packages, production logic, and cost tracking needs.                       | Activities should support how work is estimated, built, tracked, and analyzed. They should not merely mirror bid items or accounting codes.                                                   | Use bid items directly as the primary activity structure.             | Improves estimate reuse, crew production modeling, and reporting.  | Proposed | James Caudill |
| DL-006 | TBD  | Resource Structure       | Code resources according to what they are, not only what they are used for.                                                    | Materials, labor, equipment, and subcontract resources need stable identities across estimates. Usage context should be handled through activities and assemblies.                            | Create highly specific resources for every use case.                  | Reduces duplication and improves resource library maintainability. | Proposed | James Caudill |
| DL-007 | TBD  | Bid Item Mapping         | Use the Bid Item Codebook as a central automation and mapping layer between owner pay items and internal estimating structure. | Bid items are the bridge between external proposal requirements and internal estimating logic. A governed bid item codebook supports repeatability.                                           | Manually configure bid items estimate-by-estimate.                    | Improves consistency, speed, and future data analysis.             | Proposed | James Caudill |
| DL-008 | TBD  | Estimate Automation      | Build reusable estimate structures, assemblies, and calculation logic where repeatable work patterns exist.                    | Recurring work such as roadway illumination, conduit, trenching, and standard construction activities can benefit from reusable setup logic.                                                  | Continue using manual entry and spreadsheet-side calculations.        | Increases transparency, repeatability, and estimating efficiency.  | Proposed | James Caudill |
| DL-009 | TBD  | Calculation Transparency | Move important estimate calculations into HeavyBid where practical instead of leaving them only in external spreadsheets.      | Internal calculations improve visibility, reduce disconnects, and make estimates easier to review and transfer.                                                                               | Keep calculations in separate Excel files and manually enter results. | Improves auditability and knowledge transfer.                      | Proposed | James Caudill |
| DL-010 | TBD  | HeavyJob Integration     | Preserve HeavyBid-to-HeavyJob transfer readiness as a major design constraint.                                                 | The downstream handoff to HeavyJob is a key business objective. HeavyBid setup should avoid choices that make job costing, production tracking, or scheduling integration harder.             | Optimize only for estimating speed without considering HeavyJob.      | Reduces future integration risk.                                   | Proposed | James Caudill |
| DL-011 | TBD  | Governance               | Require review before making major changes to shared codebooks, assemblies, or templates.                                      | Shared setup elements affect multiple estimates and users. Uncontrolled edits can create inconsistency and hidden defects.                                                                    | Allow unrestricted edits by all users.                                | Protects system stability while still allowing improvement.        | Proposed | James Caudill |
| DL-012 | TBD  | Versioning               | Maintain version history for major setup documents, exports, and configuration reference files.                                | The project needs a way to compare setup changes over time and recover from mistakes.                                                                                                         | Rely on current-state files only.                                     | Improves change control and troubleshooting.                       | Proposed | James Caudill |
| DL-013 | TBD  | Executive Communication  | Develop executive summaries for HB Setup and related HCSS implementation work.                                                 | Leadership needs concise visibility into status, risks, decisions, and value without reviewing all technical detail.                                                                          | Communicate only through informal updates or meetings.                | Improves alignment and reduces misunderstanding.                   | Proposed | James Caudill |
| DL-014 | TBD  | Parallel Governance      | Compare HB Setup governance with the broader HCSS Implementation project governance.                                           | HeavyBid setup is one part of a larger HCSS ecosystem. Parallel documentation helps clarify boundaries, dependencies, and ownership.                                                          | Treat HB Setup and HCSS Implementation as unrelated efforts.          | Improves enterprise-level implementation clarity.                  | Proposed | James Caudill |

---

## 3. Decision Status Definitions

| Status      | Meaning                                                        |
| ----------- | -------------------------------------------------------------- |
| Proposed    | Decision has been suggested but not formally accepted.         |
| Accepted    | Decision has been agreed to and should guide project work.     |
| Deferred    | Decision is not ready and requires more information or timing. |
| Rejected    | Decision was considered but not adopted.                       |
| Superseded  | Decision has been replaced by a later decision.                |
| Implemented | Decision has been acted on and incorporated into the setup.    |

---

## 4. Decision Categories

The HB Setup Decision Log should track decisions in the following areas:

| Category              | Description                                                                                         |
| --------------------- | --------------------------------------------------------------------------------------------------- |
| Project Governance    | Charter, scope, ownership, documentation standards, decision rights.                                |
| Codebook Management   | Activity, material, equipment, labor, subcontractor, bid item, and cost code design.                |
| Estimate Structure    | Templates, library estimates, assemblies, folders, and reusable setup patterns.                     |
| Calculation Logic     | Internal HeavyBid calculations, external spreadsheet use, quantity conversions, production factors. |
| Quote System          | Quote folders, material/subfolder standards, vendor comparison practices, plug numbers.             |
| HeavyJob Integration  | Transfer structure, job costing compatibility, scheduling handoff, cost code alignment.             |
| Reporting & Analytics | Data extraction, reporting expectations, future dashboards, performance analysis.                   |
| Security & Access     | User roles, permissions, setup control, administrative authority.                                   |
| Change Management     | Training, rollout timing, review procedures, documentation updates.                                 |

---

## 5. Review Process

Decisions should be reviewed when:

* A shared codebook or template is changed.
* A setup standard affects more than one estimate.
* A configuration choice affects HeavyJob transfer.
* A manual workaround becomes a recurring process.
* Leadership direction conflicts with technical setup recommendations.
* A decision creates downstream reporting, accounting, or production-tracking consequences.

---

## 6. Recommended Immediate Decisions to Confirm

The following decisions should probably be reviewed early:

| Priority | Decision Needed                                                       | Why It Matters                              |
| -------- | --------------------------------------------------------------------- | ------------------------------------------- |
| High     | Who has authority to approve shared codebook changes?                 | Prevents uncontrolled setup drift.          |
| High     | What is the minimum setup required before production use?             | Reduces risk of premature go-live.          |
| High     | What HeavyBid structures must support HeavyJob transfer?              | Keeps estimating aligned with operations.   |
| Medium   | What documentation set is required for the project baseline?          | Establishes governance and continuity.      |
| Medium   | How should reusable assemblies and library estimates be managed?      | Supports repeatability and standardization. |
| Medium   | What calculations belong inside HeavyBid vs. outside in spreadsheets? | Improves transparency and reviewability.    |

---

## 7. Notes

This document should remain practical rather than bureaucratic. The goal is not to document every small preference, but to capture decisions that affect system structure, repeatability, governance, integration, reporting, or long-term maintainability.
