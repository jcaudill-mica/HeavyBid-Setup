# Data Governance Plan

## HeavyBid Setup Project

**Version:** v0.1
**Status:** Draft
**Project:** HB Setup
**Owner:** MICA Corporation / Estimating Department
**Prepared by:** James Caudill
**Date:** May 15, 2026

---

## 1. Purpose

The purpose of this Data Governance Plan is to define how data will be managed, controlled, documented, validated, and maintained during the HeavyBid Setup project.

HeavyBid will become a core estimating system for MICA Corporation. Because the system depends on structured data such as bid items, activities, resources, crews, production rates, cost codes, vendors, and quote folders, poor data governance could result in inaccurate estimates, inconsistent workflows, duplicated setup work, unreliable reporting, and downstream issues when transferring information into HeavyJob or other operational systems.

This document establishes the rules and responsibilities needed to keep HeavyBid setup data consistent, traceable, and useful.

---

## 2. Governance Objective

The objective of data governance for the HB Setup project is to ensure that HeavyBid data is:

* Accurate enough to support estimating decisions.
* Structured consistently across estimates and codebooks.
* Documented so future users understand how and why data was configured.
* Controlled so changes are intentional, reviewed, and traceable.
* Aligned with future HeavyJob integration and operational reporting needs.
* Practical enough to support real estimating work without overcomplicating the setup.

---

## 3. Scope

This Data Governance Plan applies to data created, reviewed, imported, modified, or standardized as part of the HB Setup project.

### In Scope

The following data areas are included:

* Bid Item Codebook
* Activity Codebook
* Material Codebook
* Equipment Codebook
* Labor Codebook
* Crew structures
* Production rates
* Quote folders and quote system setup
* Vendor and supplier reference data
* Subcontractor reference data
* Cost code structures
* Alternate cost code structures
* Estimate templates
* Assembly and calculation structures
* Standard estimate notes and assumptions
* HeavyBid-to-HeavyJob transfer-related data
* Supporting spreadsheets, exports, documentation, and mapping files

### Out of Scope

The following are outside the direct scope of this document unless later added through change control:

* Company-wide accounting master data governance
* Payroll system governance
* Enterprise-wide vendor master governance
* Full HeavyJob production data governance
* Corporate-wide document retention policy
* IT cybersecurity policy
* Formal ERP master data management

---

## 4. Data Governance Principles

The HB Setup project will follow these principles:

### 4.1 Code What It Is, Not What It Does

Codebook entries should represent the identity of the resource, activity, or item, not a temporary use case. This is especially important for materials, equipment, and activities that may be reused across multiple estimate types.

### 4.2 Build for Reuse

Data should be structured so that future estimates can reuse existing setup rather than rebuilding items manually.

### 4.3 Keep the Structure Simple Until It Breaks

The system should avoid unnecessary complexity. Additional hierarchy, fields, or controls should be added only when the existing structure no longer supports the work.

### 4.4 Preserve Estimator Judgment

Governance should standardize the data structure, not eliminate estimator judgment. Estimators must retain control over crew selection, means and methods, production assumptions, and estimate-specific decisions.

### 4.5 Make Assumptions Visible

Where calculations, production rates, crew assumptions, or quote adjustments are used, the logic should be documented clearly enough that another estimator can understand the estimate later.

### 4.6 Avoid Silent Changes

Changes to core setup data should be intentional and traceable. Important changes should be logged, especially when they affect reusable codebooks, templates, assemblies, or transfer behavior.

### 4.7 Align Estimating and Operations

HeavyBid data should be structured with consideration for HeavyJob transfer, field tracking, cost reporting, and operational usability.

---

## 5. Data Domains

The following data domains are recognized for the HB Setup project.

| Domain                 | Description                                                    | Governance Concern                                       |
| ---------------------- | -------------------------------------------------------------- | -------------------------------------------------------- |
| Bid Items              | Owner/client pay items used in proposals                       | Consistent mapping, description standards, unit accuracy |
| Activities             | Internal estimating work tasks                                 | Logical organization, reusable production assumptions    |
| Materials              | Physical materials used in work                                | Clear naming, quote folders, supplier alignment          |
| Labor                  | Labor classifications and rates                                | Accuracy, rate control, estimating consistency           |
| Equipment              | Owned/rented equipment resources                               | Naming, cost rates, ownership/rental distinction         |
| Crews                  | Standard labor/equipment groupings                             | Consistency, production assumptions, reuse               |
| Production Rates       | Expected work output over time                                 | Documentation, validation, estimator review              |
| Cost Codes             | Internal accounting/operations structure                       | Alignment with reporting and HeavyJob                    |
| Alt Cost Codes         | Estimating detail mapped to simplified accounting or reporting | Transfer clarity, reporting bridge                       |
| Vendors/Subcontractors | Companies used for quotes and services                         | Naming consistency, quote tracking                       |
| Quote Folders          | Organization of quote requests and comparisons                 | Proper folder assignment, quote package clarity          |
| Templates/Assemblies   | Reusable estimating structures                                 | Versioning, review, documentation                        |
| Calculations           | Embedded or supporting estimate calculations                   | Transparency, formula review, avoid hidden logic         |

---

## 6. Roles and Responsibilities

### 6.1 Project Sponsor

The Project Sponsor provides direction and approves major decisions affecting the HeavyBid setup.

Responsibilities include:

* Approving major configuration direction.
* Resolving conflicts between estimating, operations, and accounting priorities.
* Supporting governance enforcement when required.
* Approving go-live readiness at the business level.

### 6.2 Project Lead / Setup Coordinator

The Project Lead coordinates the setup effort and maintains the governance structure.

Responsibilities include:

* Maintaining project documentation.
* Coordinating codebook review.
* Tracking decisions and changes.
* Identifying data quality risks.
* Preparing summary recommendations for leadership.
* Ensuring setup choices are documented.

### 6.3 Estimating Lead / Senior Estimators

Estimating leadership provides subject matter expertise for estimating workflows.

Responsibilities include:

* Reviewing activity structures.
* Validating production assumptions.
* Approving estimating templates and assemblies.
* Confirming that setup supports real estimating workflows.
* Identifying areas where standardization would help or hurt estimating accuracy.

### 6.4 Accounting / Cost Reporting Representative

Accounting or cost reporting stakeholders provide input on cost structure alignment.

Responsibilities include:

* Reviewing cost code and alternate cost code logic.
* Confirming reporting requirements.
* Identifying downstream impacts of cost structure decisions.
* Supporting HeavyBid-to-HeavyJob alignment where needed.

### 6.5 Operations / HeavyJob Representative

Operations or HeavyJob stakeholders provide input on field usability and transfer needs.

Responsibilities include:

* Reviewing how estimate data may transfer into HeavyJob.
* Identifying field tracking requirements.
* Providing feedback on cost code usability.
* Confirming whether estimate structure supports job execution.

### 6.6 Data Steward

A Data Steward may be formally assigned or functionally handled by the Project Lead during the setup phase.

Responsibilities include:

* Reviewing new codebook entries for duplication or inconsistency.
* Maintaining naming standards.
* Monitoring data quality issues.
* Flagging governance risks.
* Supporting cleanup and standardization work.

---

## 7. Data Standards

### 7.1 Naming Standards

Data names should be clear, consistent, and recognizable to estimators and operations users.

Naming should avoid:

* Unexplained abbreviations.
* Duplicate names for the same item.
* Overly specific names that prevent reuse.
* Temporary project-specific labels in reusable codebooks.
* Naming based only on one estimate’s context.

Naming should favor:

* Plain language.
* Consistent word order.
* Logical grouping.
* Clear distinction between general and specific items.
* Reusable descriptions.

Example principle:

> “Concrete Riprap, 5 IN” is more reusable than “West Side Culvert Concrete.”

---

### 7.2 Code Structure Standards

Code structures should be designed to support sorting, grouping, searching, and reporting.

Codes should be:

* Consistent in length where practical.
* Grouped by logical category.
* Designed to allow future expansion.
* Avoided from being overly dense or cryptic.
* Documented when the structure has meaning.

Any use of leading zeros, delimiters, or advanced copy conventions should be documented.

---

### 7.3 Unit of Measure Standards

Units of measure must be consistent and reviewed carefully because mismatched units can distort estimate quantities, prices, and production calculations.

Governance expectations:

* Use standard units where possible.
* Confirm unit conversions before reuse.
* Avoid creating duplicate unit descriptions.
* Document conversion assumptions.
* Review bid quantity versus takeoff quantity behavior when relevant.

---

### 7.4 Production Rate Standards

Production rates should be treated as controlled estimating assumptions, not casual defaults.

Production rates should include enough context to understand:

* What work is being performed.
* What crew is assumed.
* What equipment is assumed.
* What conditions are assumed.
* Whether the rate is historical, estimated, vendor-provided, or judgment-based.

Where possible, reusable production rates should be reviewed before being added to templates or assemblies.

---

### 7.5 Quote Folder Standards

Quote folders should support efficient vendor solicitation and quote comparison.

Governance expectations:

* Quote folders should be assigned consistently.
* Materials and subcontract items should route to logical quote folders.
* Folder structure should support common estimating workflows.
* Folder assignments should be reviewed during codebook setup.
* Quote folder logic should be documented for future users.

---

## 8. Data Quality Management

### 8.1 Data Quality Dimensions

The HB Setup project will use the following data quality dimensions:

| Dimension    | Description                                                                 |
| ------------ | --------------------------------------------------------------------------- |
| Accuracy     | Data correctly represents the intended item, cost, unit, or relationship    |
| Completeness | Required fields and relationships are present                               |
| Consistency  | Similar data is structured and named the same way                           |
| Uniqueness   | Duplicate or redundant entries are avoided                                  |
| Validity     | Data follows approved formats, units, and code structures                   |
| Usability    | Data can be understood and used by estimators without excessive explanation |
| Traceability | Important setup decisions can be traced to a source or decision record      |

---

### 8.2 Data Quality Review Activities

Data quality will be reviewed through:

* Codebook cleanup sessions.
* Sample estimate testing.
* Review of duplicate or near-duplicate entries.
* Unit of measure checks.
* Quote folder assignment checks.
* HeavyBid-to-HeavyJob transfer testing.
* Review of production assumptions.
* Review of template and assembly behavior.
* Feedback from estimators during active use.

---

### 8.3 Common Data Quality Risks

Known data quality risks include:

* Duplicate material or activity codes.
* Misaligned bid item descriptions.
* Inconsistent quote folder assignments.
* Production rates copied without context.
* Cost codes that do not align with operations reporting.
* Data built for one estimate that becomes accidentally reused as a standard.
* Too much setup work performed without review.
* HeavyBid structures that transfer poorly into HeavyJob.
* Estimators bypassing codebooks due to lack of trust or usability.

---

## 9. Change Control for Data

Changes to controlled HeavyBid data should follow the project Change Control Plan when the change affects reusable setup, reporting, integration, or standard workflows.

### 9.1 Controlled Data Changes

The following changes should be logged or reviewed:

* New codebook structures.
* Major changes to activity coding.
* Major changes to material coding.
* Cost code or alternate cost code structure changes.
* Crew template changes.
* Standard production rate changes.
* Estimate template changes.
* Assembly logic changes.
* HeavyBid-to-HeavyJob transfer configuration changes.
* Quote folder structure changes.
* Vendor/subcontractor naming cleanup.

### 9.2 Minor Data Changes

Minor corrections may not require formal approval but should still be made carefully.

Examples include:

* Typo corrections.
* Minor description cleanup.
* Removal of obvious duplicates after review.
* Formatting cleanup.
* Adding missing notes or documentation.

### 9.3 Change Log Expectations

A data change log should capture:

| Field                 | Description                                          |
| --------------------- | ---------------------------------------------------- |
| Date                  | Date of change                                       |
| Area Affected         | Codebook, template, assembly, etc.                   |
| Description of Change | What changed                                         |
| Reason                | Why the change was made                              |
| Requested By          | Person requesting the change                         |
| Approved By           | Person approving the change, if required             |
| Impact                | Expected effect on estimates, reporting, or transfer |
| Status                | Proposed, approved, implemented, rejected            |

---

## 10. Data Ownership and Stewardship

Data ownership should be assigned by business function.

| Data Area        | Primary Owner           | Stewardship Support                    |
| ---------------- | ----------------------- | -------------------------------------- |
| Bid Items        | Estimating              | Project Lead / Data Steward            |
| Activities       | Estimating              | Project Lead / Senior Estimators       |
| Materials        | Estimating / Purchasing | Project Lead / Data Steward            |
| Labor            | Estimating / Accounting | Project Lead                           |
| Equipment        | Estimating / Operations | Project Lead                           |
| Crews            | Estimating              | Senior Estimators                      |
| Production Rates | Estimating              | Senior Estimators                      |
| Cost Codes       | Accounting / Operations | Project Lead                           |
| Alt Cost Codes   | Estimating / Accounting | Project Lead                           |
| Quote Folders    | Estimating / Purchasing | Project Lead                           |
| Templates        | Estimating              | Project Lead                           |
| Assemblies       | Estimating              | Project Lead                           |
| Transfer Data    | Estimating / Operations | Project Lead / HeavyJob Representative |

---

## 11. Documentation Requirements

The HB Setup project should maintain documentation for major setup decisions and structures.

Documentation should include:

* Project Charter
* Business Case
* Communication Plan
* Risk Register
* Decision Log
* Change Control Plan
* Data Governance Plan
* Codebook structure notes
* HeavyBid-to-HeavyJob transfer notes
* Template and assembly documentation
* Known issues list
* Data cleanup notes
* Testing notes
* Executive summaries

Documentation should be stored in a consistent project folder structure and should use clear file names, version numbers, and dates where appropriate.

---

## 12. Version Control and File Management

Supporting files should be managed so that project history can be reconstructed.

### 12.1 File Naming

Recommended file naming pattern:

```text
HB_Setup_[DocumentName]_v0.1_YYYY-MM-DD
```

Example:

```text
HB_Setup_Data_Governance_v0.1_2026-05-15.md
```

### 12.2 Versioning

Version numbers should follow a simple pattern:

| Version | Meaning                        |
| ------- | ------------------------------ |
| v0.x    | Draft versions before approval |
| v1.0    | First approved baseline        |
| v1.x    | Minor updates after approval   |
| v2.0    | Major revision or restructure  |

### 12.3 Source of Truth

The project should define where the official version of each document and data file lives.

Possible locations include:

* Project documentation folder.
* Microsoft Teams project channel.
* OneDrive or SharePoint location.
* Local working folder for draft analysis.
* Git repository for markdown, CSV, or structured data files if used.

Only one location should be treated as the official source of truth for approved documents.

---

## 13. Access and Security

Access to HeavyBid setup data should be limited based on business need.

Governance expectations:

* Users should have access appropriate to their role.
* Reusable setup data should not be casually modified by all users.
* Sensitive cost, labor, vendor, and estimate data should be protected.
* Exported files should be stored in approved locations.
* Draft analysis files should not become uncontrolled copies of official data.
* Permissions should be reviewed before go-live.

This Data Governance Plan does not replace company IT or cybersecurity policies.

---

## 14. Data Retention

Project data should be retained long enough to support setup history, future troubleshooting, and auditability of decisions.

Recommended retention categories:

| Data Type                     | Retention Recommendation                            |
| ----------------------------- | --------------------------------------------------- |
| Approved governance documents | Retain indefinitely or per company policy           |
| Decision logs                 | Retain for life of system plus historical reference |
| Change logs                   | Retain for life of system plus historical reference |
| Setup exports                 | Retain by major milestone                           |
| Temporary working files       | Archive or delete after validation                  |
| Test estimates                | Retain if useful for setup reference                |
| Obsolete drafts               | Archive when superseded                             |

---

## 15. Data Issue Management

Data issues should be captured when they are discovered and tracked until resolved.

Examples of data issues include:

* Duplicate codebook entries.
* Incorrect unit of measure.
* Missing quote folder.
* Invalid cost code mapping.
* Confusing activity description.
* Incorrect production assumption.
* HeavyBid-to-HeavyJob transfer mismatch.
* Template or assembly calculation issue.

Issue tracking should include:

| Field             | Description                            |
| ----------------- | -------------------------------------- |
| Issue ID          | Unique identifier                      |
| Date Found        | Date issue was identified              |
| Data Area         | Codebook, template, quote folder, etc. |
| Issue Description | What is wrong                          |
| Impact            | Why it matters                         |
| Owner             | Person responsible for resolution      |
| Priority          | Low, Medium, High, Critical            |
| Status            | Open, In Review, Resolved, Deferred    |
| Resolution Notes  | How the issue was handled              |

---

## 16. Testing and Validation

Data governance depends on testing the setup in realistic estimating scenarios.

Validation activities should include:

* Building sample estimates from standard bid items.
* Testing reusable assemblies.
* Reviewing crew and production behavior.
* Testing quote folder routing.
* Reviewing cost code mappings.
* Testing HeavyBid-to-HeavyJob transfer.
* Comparing estimate output to expected reporting needs.
* Reviewing setup with estimators before approval.

Testing should focus on whether the setup supports real work, not just whether the software technically allows the configuration.

---

## 17. Governance Review Cadence

During the HB Setup project, data governance should be reviewed regularly.

Recommended cadence:

| Review Type              | Frequency                             |
| ------------------------ | ------------------------------------- |
| Informal setup review    | As needed during active configuration |
| Codebook review          | Weekly or at major setup milestones   |
| Data issue review        | Weekly during active buildout         |
| Decision log review      | Weekly or before leadership updates   |
| Change control review    | As changes are proposed               |
| Go-live readiness review | Before production use                 |

After initial implementation, governance review may shift to a monthly or quarterly maintenance cycle.

---

## 18. Go-Live Data Readiness Criteria

Before HeavyBid is considered ready for broader production use, the following governance items should be reviewed:

* Core codebooks have been reviewed for major duplicates and inconsistencies.
* Standard naming conventions are documented.
* Bid item mapping approach is defined.
* Activity structure is usable by estimators.
* Material structure supports quote folder routing.
* Cost code and alternate cost code logic is documented.
* Key assemblies and templates have been tested.
* HeavyBid-to-HeavyJob transfer behavior has been tested.
* Known data issues are documented.
* High-priority data issues are resolved or accepted.
* Estimators understand how to use the governed data.
* A process exists for requesting setup changes after go-live.

---

## 19. Risks and Controls

| Risk                                              | Potential Impact                                  | Control                                    |
| ------------------------------------------------- | ------------------------------------------------- | ------------------------------------------ |
| Codebooks become cluttered with duplicate entries | Estimators lose trust in the system               | Periodic duplicate review                  |
| Setup is rushed before structure is validated     | Rework, bad transfer data, inconsistent estimates | Go-live readiness checklist                |
| Production rates are reused without context       | Inaccurate estimates                              | Document rate assumptions                  |
| HeavyBid setup does not align with HeavyJob       | Transfer and reporting issues                     | Early integration testing                  |
| Too many users modify setup data                  | Loss of control and consistency                   | Role-based access and change process       |
| Documentation is not maintained                   | Future users cannot understand setup logic        | Decision log and change log                |
| Governance becomes too restrictive                | Estimators bypass the system                      | Keep rules practical and estimator-focused |

---

## 20. Success Measures

Data governance will be considered successful if:

* Estimators can find and reuse standard data without excessive searching.
* Duplicate entries are reduced over time.
* Codebooks support consistent estimate structure.
* Quote folders work predictably.
* HeavyBid-to-HeavyJob transfer is understandable and usable.
* Major setup decisions are documented.
* Leadership can understand the current state of the setup.
* Future changes can be made without losing the reasoning behind prior decisions.
* The system improves estimating consistency without reducing estimator flexibility.

---

## 21. Open Questions

The following items require further discussion or confirmation:

1. Who will have authority to approve permanent codebook changes?
2. What will be the official source of truth for project documentation?
3. Should HeavyBid setup files be exported and versioned on a recurring schedule?
4. What level of detail should be carried into HeavyJob?
5. How should alternate cost codes be structured for estimating versus accounting needs?
6. Who will own quote folder structure after initial setup?
7. What data fields are required before an item can be considered reusable?
8. How should obsolete codebook entries be retired or hidden?
9. What naming conventions should be formally adopted?
10. What is the minimum data quality standard required before go-live?

---

## 22. Approval

| Role                                 | Name | Approval Date | Signature / Confirmation |
| ------------------------------------ | ---- | ------------- | ------------------------ |
| Project Sponsor                      |      |               |                          |
| Project Lead                         |      |               |                          |
| Estimating Lead                      |      |               |                          |
| Accounting / Cost Representative     |      |               |                          |
| Operations / HeavyJob Representative |      |               |                          |

---

## 23. Revision History

| Version | Date       | Author        | Description                                    |
| ------- | ---------- | ------------- | ---------------------------------------------- |
| v0.1    | 2026-05-15 | James Caudill | Initial draft of HB Setup Data Governance Plan |
