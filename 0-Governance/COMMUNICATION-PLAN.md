# HeavyBid Setup Project — Communication Plan

**Document Status:** Draft v0.1
**Project:** HeavyBid Setup / HB Setup
**Prepared For:** MICA Corporation
**Prepared By:** James Caudill
**Purpose:** Define how project information, decisions, risks, updates, and deliverables will be communicated during the HeavyBid setup effort.

---

## 1. Purpose

The Communication Plan establishes a consistent method for keeping stakeholders aligned during the HeavyBid Setup project.

The goal is to reduce confusion, prevent duplicated effort, document key decisions, and make sure project progress is visible to both operational users and leadership.

This plan supports the broader project governance structure by defining:

* Who needs to know what
* When communication should occur
* Which channels should be used
* How decisions and risks should be documented
* How issues should be escalated

---

## 2. Communication Objectives

The communication objectives for the HB Setup project are:

1. Keep leadership informed of progress, risks, and key decisions.
2. Keep estimators and operational users aware of setup changes that may affect their work.
3. Maintain a clear record of project direction, assumptions, and implementation choices.
4. Support coordination between HeavyBid, HeavyJob, accounting, scheduling, and field operations.
5. Prevent informal decisions from becoming undocumented system rules.
6. Create enough visibility to support trust, adoption, and accountability.

---

## 3. Communication Principles

Communication for this project should follow these principles:

### Clarity Over Volume

Project communication should be useful, direct, and tied to action. The goal is not to flood stakeholders with updates, but to make sure the right people receive the right information at the right time.

### Document Decisions, Not Just Conversations

Verbal discussions are expected, but important decisions should be captured in the project Decision Log or supporting documentation.

### Separate Working Notes from Approved Direction

Exploratory notes, analysis, and draft ideas should be clearly distinguished from approved configuration decisions.

### Escalate Risks Early

Risks involving system design, go-live readiness, data structure, HeavyBid-to-HeavyJob transfer, cost codes, accounting alignment, or leadership expectations should be raised early.

### Maintain a Single Source of Truth

Project documents should be stored in a known location so stakeholders are not relying on scattered emails, chat messages, or memory.

---

## 4. Stakeholder Communication Matrix

| Stakeholder Group                          | Communication Need                                                  |                      Frequency | Channel                      | Owner                             |
| ------------------------------------------ | ------------------------------------------------------------------- | -----------------------------: | ---------------------------- | --------------------------------- |
| Company Leadership                         | Progress, risks, strategic decisions, go-live readiness             |            Weekly or as needed | Meeting, summary memo, Teams | Project Lead                      |
| Estimating Team                            | Setup changes, HeavyBid workflow impacts, testing needs             | Weekly / during active changes | Teams, working sessions      | Project Lead / Estimating Lead    |
| HeavyJob / Operations Users                | Transfer requirements, cost code impacts, operational handoff needs |                      As needed | Meetings, Teams              | Project Lead                      |
| Accounting / Admin                         | Cost structure, coding, reporting, accounting alignment             |                      As needed | Meeting, documented summary  | Project Lead / Accounting Contact |
| Scheduling / Project Transfer Stakeholders | Estimate-to-job transfer expectations and responsibilities          |                      As needed | Meeting, Teams               | Project Lead                      |
| HCSS Support / Vendor Contacts             | Technical questions, configuration guidance, issue resolution       |                      As needed | HCSS support channels, email | Assigned Contact                  |
| Project Documentation Owner                | Updates to charter, decision log, risk register, governance docs    |                        Ongoing | Document repository          | Project Lead                      |

---

## 5. Communication Channels

### Microsoft Teams

Teams should be the primary day-to-day communication channel for project coordination.

Recommended uses:

* Status updates
* Meeting coordination
* Quick questions
* File links
* Discussion threads
* Stakeholder notifications

### Meetings

Meetings should be used for:

* Decision-making
* Design review
* Process alignment
* Risk review
* Go-live readiness review
* HeavyBid-to-HeavyJob workflow discussion

Meetings should produce either notes, action items, or updates to the Decision Log / Risk Register when appropriate.

### Email

Email should be used when communication needs a more formal record or when communicating with external parties.

Recommended uses:

* Vendor communication
* Formal leadership updates
* Distribution of approved documents
* Meeting summaries for major decisions

### Project Documentation Repository

The documentation repository should serve as the long-term record of the project.

Recommended contents:

* Project Charter
* Business Case
* Communication Plan
* Decision Log
* Risk Register
* README
* Setup notes
* Configuration summaries
* Governance documents
* Meeting summaries
* Process maps
* Training or handoff material

---

## 6. Standard Communication Types

### Project Status Update

**Purpose:** Provide leadership and stakeholders with a concise summary of progress.

**Recommended Frequency:** Weekly during active setup.

**Suggested Format:**

```markdown
# HB Setup Weekly Status Update

## Summary
Brief overview of current project status.

## Completed This Period
- 

## In Progress
- 

## Key Decisions Needed
- 

## Risks / Issues
- 

## Next Steps
- 
```

---

### Meeting Summary

**Purpose:** Capture important discussion points, decisions, and action items.

**Recommended Use:** After design, governance, or decision meetings.

**Suggested Format:**

```markdown
# Meeting Summary

**Date:**  
**Topic:**  
**Participants:**  

## Purpose
Brief reason for the meeting.

## Discussion Summary
- 

## Decisions
- 

## Action Items
| Action | Owner | Due Date | Status |
|---|---|---:|---|

## Follow-Up Needed
- 
```

---

### Decision Communication

**Purpose:** Make sure major system decisions are visible and traceable.

Any major decision should be entered into the Decision Log.

Examples include:

* Cost code structure
* Activity codebook design
* Bid item mapping approach
* Resource naming standards
* Quote folder structure
* HeavyBid-to-HeavyJob transfer method
* Go-live readiness criteria
* Estimator workflow rules
* Use of assemblies, templates, or library estimates

**Minimum decision record should include:**

* Decision date
* Decision title
* Context
* Options considered
* Final decision
* Owner
* Impact
* Follow-up actions

---

### Risk Communication

**Purpose:** Raise project risks before they become implementation failures.

Risks should be added to the Risk Register when they affect:

* Schedule
* Setup quality
* Estimate accuracy
* HeavyBid-to-HeavyJob transfer
* Accounting alignment
* User adoption
* Training readiness
* Data quality
* Reporting confidence
* Leadership expectations

Risk updates should include:

* Risk description
* Probability
* Impact
* Mitigation
* Owner
* Current status

---

### Change Communication

**Purpose:** Communicate meaningful changes to setup, process, or workflow.

A change should be communicated when it affects how users estimate, transfer, report, or manage work.

Examples:

* New activity structure
* Revised cost code format
* Updated quote folder logic
* Changes to bid item mapping
* Revised resource naming
* New library estimate process
* Revised estimate review procedure

Change communication should answer:

1. What changed?
2. Why did it change?
3. Who is affected?
4. When does it take effect?
5. What action is required?

---

## 7. Meeting Cadence

| Meeting Type                  | Purpose                                                    |                             Frequency | Participants                                        |
| ----------------------------- | ---------------------------------------------------------- | ------------------------------------: | --------------------------------------------------- |
| Project Check-In              | Review progress, blockers, and near-term priorities        |                    Weekly or biweekly | Project Lead, key stakeholders                      |
| Design / Configuration Review | Review setup structure and technical decisions             |                             As needed | Project Lead, estimators, relevant department leads |
| Leadership Update             | Communicate status, risks, decisions, and support needs    |                   Weekly or as needed | Leadership, Project Lead                            |
| Risk / Readiness Review       | Evaluate implementation risks and go-live readiness        |           Before major rollout points | Leadership, Project Lead, affected users            |
| Training / Adoption Session   | Prepare users for workflow changes                         | Before launch or major process change | Estimators, operations users, Project Lead          |
| Post-Implementation Review    | Review what worked, what failed, and what needs refinement |                 After initial rollout | Project stakeholders                                |

---

## 8. Escalation Path

Issues should be escalated when they cannot be resolved at the working level or when they create risk to project success.

### Escalation Triggers

Escalation is appropriate when:

* A decision is blocking progress.
* System setup conflicts with business process.
* HeavyBid setup may not support HeavyJob transfer.
* Accounting or cost code alignment is unclear.
* Go-live pressure may compromise quality.
* Stakeholders disagree on implementation direction.
* A configuration decision creates downstream reporting risk.
* User adoption or training readiness is at risk.

### Escalation Levels

| Level   | Description               | Example                                                          |
| ------- | ------------------------- | ---------------------------------------------------------------- |
| Level 1 | Working team resolution   | Estimator and project lead resolve setup detail                  |
| Level 2 | Department-level decision | Estimating / operations / accounting alignment needed            |
| Level 3 | Leadership decision       | Strategic tradeoff, schedule pressure, or major process impact   |
| Level 4 | Vendor / HCSS support     | Technical issue or product limitation requires external guidance |

---

## 9. Documentation Standards

All major project documentation should use consistent structure and naming.

### Recommended Naming Convention

```text
HB_Setup_[DocumentName]_v0.1.md
HB_Setup_[DocumentName]_v0.2.md
HB_Setup_[DocumentName]_v1.0.md
```

Examples:

```text
HB_Setup_Project_Charter_v0.1.md
HB_Setup_Business_Case_v0.1.md
HB_Setup_Communication_Plan_v0.1.md
HB_Setup_Decision_Log_v0.1.md
HB_Setup_Risk_Register_v0.1.md
```

### Version Guidance

| Version | Meaning                         |
| ------- | ------------------------------- |
| v0.1    | Initial draft                   |
| v0.x    | Working draft / under review    |
| v1.0    | Approved baseline               |
| v1.x    | Minor revisions                 |
| v2.0    | Major revision or restructuring |

---

## 10. Communication Roles and Responsibilities

| Role                               | Responsibility                                                                |
| ---------------------------------- | ----------------------------------------------------------------------------- |
| Project Lead                       | Maintains communication plan, prepares updates, tracks decisions and risks    |
| Leadership Sponsor                 | Provides direction, resolves escalated decisions, reinforces project priority |
| Estimating Stakeholders            | Provide workflow input, test setup, identify practical issues                 |
| Operations / HeavyJob Stakeholders | Validate transfer requirements and downstream job setup needs                 |
| Accounting Stakeholders            | Validate cost structure, reporting needs, and financial alignment             |
| Documentation Owner                | Maintains document repository, version control, and project records           |
| HCSS / Vendor Support              | Provides technical guidance and product-specific answers when needed          |

---

## 11. Information Flow

The preferred information flow should be:

```text
Working Discussion
        ↓
Meeting Notes / Working Notes
        ↓
Decision Log, Risk Register, or Action Item
        ↓
Project Documentation Update
        ↓
Stakeholder Communication
```

This keeps the project from relying on memory or scattered conversations.

---

## 12. Communication Risks

| Risk                                           | Impact                                      | Mitigation                                   |
| ---------------------------------------------- | ------------------------------------------- | -------------------------------------------- |
| Decisions are made verbally but not documented | Setup logic becomes unclear later           | Maintain Decision Log                        |
| Leadership receives only partial visibility    | Misalignment on readiness or scope          | Provide regular status summaries             |
| Users are surprised by workflow changes        | Resistance or incorrect usage               | Communicate changes before implementation    |
| Teams use different assumptions                | Conflicting setup decisions                 | Maintain shared documentation                |
| Go-live pressure skips communication steps     | Poor adoption or setup rework               | Use readiness reviews                        |
| Technical issues are discussed informally only | Repeated troubleshooting and knowledge loss | Capture vendor questions and answers         |
| Documentation becomes stale                    | Project record loses value                  | Review and update during weekly status cycle |

---

## 13. Communication Success Criteria

The Communication Plan is working if:

* Stakeholders know where to find current project information.
* Major decisions are captured in the Decision Log.
* Risks are captured before they become emergencies.
* Leadership understands progress and tradeoffs.
* Estimators understand changes affecting their workflow.
* HeavyBid-to-HeavyJob transfer issues are identified early.
* Project documentation reflects actual implementation direction.
* Meetings result in clear decisions or action items.
* The project can be explained clearly to someone who was not present for every discussion.

---

## 14. Initial Communication Priorities

The first communication priorities for the HB Setup project should be:

1. Establish the project documentation location.
2. Confirm the primary Teams channel or communication space.
3. Identify recurring status update cadence.
4. Begin maintaining the Decision Log.
5. Begin maintaining the Risk Register.
6. Identify stakeholders who need periodic updates.
7. Define what decisions require leadership approval.
8. Define what setup changes require user communication.
9. Prepare a simple weekly status update format.
10. Establish a go-live readiness communication process.

---

## 15. Open Questions

The following questions should be resolved as the project matures:

1. Who is the formal project sponsor?
2. Who has final approval authority for HeavyBid setup structure?
3. What project documentation location will serve as the source of truth?
4. Will the Teams channel be the official communication hub?
5. What cadence does leadership want for status updates?
6. What HeavyBid changes require formal approval before implementation?
7. Who must sign off before HeavyBid-to-HeavyJob transfer is considered ready?
8. What level of documentation is expected before go-live?
9. How will training communication be handled?
10. Who owns long-term maintenance of the HeavyBid setup after initial implementation?

---

## 16. Recommended Next Step

Adopt this Communication Plan as a working draft and use it to support the first round of HB Setup governance.

The most immediate action should be to establish the project communication hub, confirm the stakeholder list, and begin issuing regular status summaries tied to the Decision Log and Risk Register.
