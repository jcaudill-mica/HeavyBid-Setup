# HB Setup Project — Risk Register

**Project:** HeavyBid Setup / HB Setup
**Version:** v0.1 Draft
**Date:** 05.15.26
**Owner:** Estimating / HCSS Implementation Team
**Purpose:** Identify, track, and manage risks that could affect the successful setup, governance, adoption, and long-term maintainability of HeavyBid.

---

## 1. Risk Rating Scale

### Probability

| Rating | Meaning                                |
| ------ | -------------------------------------- |
| Low    | Unlikely to occur                      |
| Medium | Possible / already showing early signs |
| High   | Likely or already occurring            |

### Impact

| Rating | Meaning                                                                 |
| ------ | ----------------------------------------------------------------------- |
| Low    | Minor inconvenience or rework                                           |
| Medium | Affects schedule, consistency, or user confidence                       |
| High   | Could compromise implementation quality, adoption, or operational value |

### Status

| Status     | Meaning                             |
| ---------- | ----------------------------------- |
| Open       | Active risk being monitored         |
| Mitigating | Response actions are underway       |
| Accepted   | Risk is known and tolerated for now |
| Closed     | Risk is no longer active            |

---

## 2. Risk Register

| ID    | Risk                                                                                                                                      |                 Category | Probability | Impact | Overall Risk | Mitigation / Response                                                                                                       | Owner                                | Status     |
| ----- | ----------------------------------------------------------------------------------------------------------------------------------------- | -----------------------: | ----------: | -----: | -----------: | --------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ | ---------- |
| R-001 | HeavyBid may be pushed toward go-live before setup, governance, and validation are mature enough.                                         |    Schedule / Governance |        High |   High |     Critical | Define phased rollout criteria, document minimum viable setup, and separate “testable” from “production-ready.”             | Project Lead / Estimating Leadership | Open       |
| R-002 | Initial setup decisions may become permanent by default if they are not documented and reviewed.                                          |               Governance |        High |   High |     Critical | Maintain decision log, setup notes, and change history for major configuration choices.                                     | HB Setup Lead                        | Mitigating |
| R-003 | Activity, resource, material, and bid item structures may drift without a formal naming and coding standard.                              |     Data / Configuration |        High |   High |     Critical | Create codebook governance document and enforce review before new codes are added.                                          | HB Setup Lead / Estimators           | Open       |
| R-004 | Leadership may focus on proving HeavyBid-to-HeavyJob transfer rather than building a sustainable estimating system.                       |      Strategic Alignment |      Medium |   High |         High | Frame implementation around both short-term transfer testing and long-term estimating reliability.                          | Project Sponsor / HB Setup Lead      | Open       |
| R-005 | Estimators may lose confidence if early HeavyBid outputs appear inconsistent, incomplete, or difficult to explain.                        |                 Adoption |      Medium |   High |         High | Use pilot estimates, document assumptions, and validate outputs against known bid examples.                                 | Estimating Team                      | Open       |
| R-006 | Lack of role clarity may cause confusion between estimator setup tasks, administrator tasks, and management decisions.                    |       Governance / Roles |      Medium | Medium |       Medium | Create RACI or responsibility matrix for setup, review, approval, and maintenance.                                          | Project Lead                         | Open       |
| R-007 | Quote folder and material setup may become inconsistent if materials are coded by use case instead of by what they are.                   |         Data / Materials |      Medium | Medium |       Medium | Apply the rule: “Code what it is, not what it does.” Use quote folder standards and review exceptions.                      | Materials / Estimating               | Open       |
| R-008 | Over-customization may create a system that is powerful but difficult for others to maintain.                                             |          Maintainability |      Medium |   High |         High | Prefer simple, explainable structures; document automation logic; avoid clever setup that only one person understands.      | HB Setup Lead                        | Open       |
| R-009 | Insufficient testing of assemblies, activities, and production rates may produce inaccurate estimate outputs.                             |     Quality / Estimating |      Medium |   High |         High | Build test estimates, compare against historical estimates, and review major assemblies before production use.              | Estimating Team                      | Open       |
| R-010 | Cost code structure may not align well between detailed estimating needs and simplified accounting or HeavyJob tracking needs.            |              Integration |      Medium |   High |         High | Use Alt Cost Codes or mapping structures where needed; document the bridge between estimate detail and job cost reporting.  | Estimating / Accounting / Operations | Open       |
| R-011 | HeavyBid setup knowledge may remain concentrated with one or two people.                                                                  |           Knowledge Risk |        High | Medium |         High | Maintain setup documentation, weekly notes, decision logs, and cross-train users.                                           | HB Setup Lead                        | Open       |
| R-012 | Existing undocumented preferences from leadership or senior estimators may conflict with formalized governance.                           |              Stakeholder |      Medium | Medium |       Medium | Capture preferences as assumptions or design constraints; review conflicts openly before locking standards.                 | Project Sponsor / HB Setup Lead      | Open       |
| R-013 | Inconsistent use of templates, library estimates, and assemblies may lead to duplicate or conflicting estimating methods.                 |                  Process |      Medium | Medium |       Medium | Establish approved library estimate structure and versioning procedure.                                                     | Estimating Team                      | Open       |
| R-014 | Bid item mapping may become unreliable if TxDOT/spec item changes are not clearly handled.                                                |     Data / Specification |      Medium |   High |         High | Maintain bid item mapping documentation and test against known spec families before relying on automation.                  | HB Setup Lead                        | Open       |
| R-015 | The project may lack a clear executive summary, making it harder to communicate progress and value to leadership.                         |            Communication |      Medium | Medium |       Medium | Maintain current project charter, business case, README, and periodic executive summaries.                                  | HB Setup Lead                        | Mitigating |
| R-016 | Setup fatigue may lead to shortcuts, abandoned documentation, or inconsistent governance practices.                                       |                Execution |      Medium | Medium |       Medium | Use lightweight documentation, daily planning, and defined stopping points. Keep standards useful rather than bureaucratic. | HB Setup Lead                        | Open       |
| R-017 | Users may bypass HeavyBid standards if the system feels slower than existing methods.                                                     |       Adoption / Process |      Medium |   High |         High | Identify friction points early, simplify workflows, and provide clear examples of time savings and consistency benefits.    | Estimating Leadership                | Open       |
| R-018 | HCSS ecosystem interactions may be misunderstood if HeavyBid, HeavyJob, credentials, scheduling, and accounting workflows are not mapped. |    Integration / Process |      Medium | Medium |       Medium | Develop ecosystem diagrams and clarify user roles, handoffs, and permissions.                                               | HCSS Implementation Team             | Open       |
| R-019 | Reporting and analytics opportunities may be lost if setup does not preserve useful estimating structure.                                 | Analytics / Future Value |      Medium |   High |         High | Design codebooks and estimate structures with future reporting, benchmarking, and forecasting in mind.                      | HB Setup Lead / Analytics            | Open       |
| R-020 | Documentation may become fragmented across Teams, OneNote, ChatGPT, local files, and project folders.                                     |            Documentation |        High | Medium |         High | Define a canonical project folder, naming conventions, and document index. Use README files for navigation.                 | HB Setup Lead                        | Open       |

---

## 3. Highest-Priority Risks

The top risks that need active attention are:

1. **Premature go-live before setup maturity**
2. **Undocumented setup decisions becoming permanent**
3. **Codebook drift across activities, resources, materials, and bid items**
4. **Mismatch between detailed estimating structure and HeavyJob/accounting needs**
5. **Knowledge concentration in one person**
6. **Loss of future analytics value due to poor setup structure**

---

## 4. Immediate Mitigation Actions

| Action                                       | Purpose                                                             | Priority |
| -------------------------------------------- | ------------------------------------------------------------------- | -------: |
| Create a formal Decision Log                 | Prevent undocumented setup choices from becoming hidden assumptions |     High |
| Define Minimum Viable HeavyBid Setup         | Separate “demo-ready” from “production-ready”                       |     High |
| Draft Codebook Governance Standards          | Reduce drift and duplicate structures                               |     High |
| Build Executive Summary                      | Communicate project status and value clearly                        |   Medium |
| Create Documentation Index                   | Keep project artifacts findable                                     |   Medium |
| Identify Pilot Estimate(s)                   | Validate setup against real estimating work                         |     High |
| Define HeavyBid-to-HeavyJob Mapping Approach | Protect integration quality                                         |     High |

---

## 5. Risk Themes

### Governance Risk

The project needs enough structure to prevent drift, but not so much structure that setup slows down or becomes bureaucratic.

### Adoption Risk

HeavyBid must feel useful to estimators, not like an administrative burden. Early wins and clear examples matter.

### Integration Risk

HeavyBid cannot be treated as an isolated estimating tool. Its value depends on how well it connects to HeavyJob, accounting, scheduling, permissions, reporting, and operational workflows.

### Data Quality Risk

The codebooks are not just setup tables. They are the foundation for consistency, reporting, estimating logic, and future analytics.

### Strategic Risk

There is a risk that the project gets judged only by whether a bid can transfer into HeavyJob, rather than whether the system is durable, explainable, and scalable.

---

## 6. Recommended Register Maintenance

The Risk Register should be reviewed:

* Weekly during active setup
* After major HeavyBid configuration decisions
* Before any pilot estimate is treated as a production model
* Before HeavyBid-to-HeavyJob transfer testing
* Before leadership review or go-live discussion

Each review should update:

* Probability
* Impact
* Status
* Mitigation progress
* Newly discovered risks
* Risks that can be closed or accepted
