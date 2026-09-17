# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Security/Compliance Leads

### Role Summary
Security/Compliance Leads protect customers and the business by embedding secure-by-default practices into delivery. They own security reviews, risk assessments, and compliance sign-offs across the project lifecycle.

### Responsibilities
- Run threat modeling and security reviews for new or changed functionality
- Assess security, privacy, and regulatory risks and record them in the risk register
- Define required controls, secure defaults, and remediation expectations
- Approve security and compliance readiness before release
- Support incident response and post-incident follow-up for security events

### Goals
- Prevent avoidable security and compliance issues
- Keep required controls lightweight and repeatable
- Ensure security risks have named owners and mitigation plans

### Decision Rights
- Approve or block release on unresolved high-severity security findings
- Decide which controls and evidence are mandatory for a given change

### Collaboration Points
- PM: adds security review milestones to the plan and tracks remediation work
- PdM: agrees on trade-offs between scope, timeline, and risk acceptance
- Developers: pairs on secure design, code review, and security scan findings
- QA: aligns security test cases with acceptance criteria
- Stakeholders: communicates residual risk and compliance status

### Typical Communication
- Security review notes and findings in PRs and design docs
- Risk register entries and weekly risk review updates
- Security incident notifications via the security incident runbook

---

## UX / Design Leads

### Role Summary
UX / Design Leads ensure solutions are usable, accessible, and grounded in real user needs. They translate problem statements into flows, prototypes, and design decisions the team can build against.

### Responsibilities
- Conduct user research and validate problems and solutions
- Produce flows, prototypes, and design specs for prioritized work
- Define accessibility requirements and review implementations against them
- Maintain design system consistency across features
- Feed usability findings back into the backlog

### Goals
- Deliver experiences customers can use without friction
- Meet accessibility standards by default
- Reduce rework by validating designs before build

### Decision Rights
- Own final interaction and visual design decisions within agreed scope
- Confirm accessibility and usability readiness for release

### Collaboration Points
- PM: sequences design work ahead of build and flags design dependencies
- PdM: co-defines problem statements, success metrics, and acceptance criteria
- Developers: reviews implementation fidelity and resolves design trade-offs
- QA: supplies design and accessibility criteria for validation
- Stakeholders: shares prototypes and research findings to build alignment

### Typical Communication
- Design reviews and prototype walkthroughs
- Design specs and accessibility notes linked from issues
- Research summaries shared at product alignment meetings

---

## Operations / SRE Leads

### Role Summary
Operations / SRE Leads make sure what the team builds can run reliably in production. They own production readiness, monitoring, and incident response planning.

### Responsibilities
- Define production readiness and observability requirements
- Review rollout, rollback, and capacity plans before release
- Set up monitoring, alerting, and on-call coverage for new services
- Lead incident response and blameless post-incident reviews
- Track operational risks and reliability follow-up actions

### Goals
- Maintain service reliability and fast recovery
- Make deployments low-risk and reversible
- Reduce unplanned operational work

### Decision Rights
- Approve production readiness and deployment windows
- Call for rollback or hold a release when reliability is at risk

### Collaboration Points
- PM: aligns deployment windows, dependencies, and operational readiness tasks
- PdM: clarifies reliability expectations against feature priorities
- Developers: reviews instrumentation, runbooks, and failure modes
- QA: coordinates staging smoke tests and post-deploy verification
- Stakeholders: reports availability impacts and incident status

### Typical Communication
- Production readiness reviews and deployment checklists
- Incident communications and post-incident retrospectives
- Reliability and monitoring updates at weekly delivery syncs

---

## Customer Success / Stakeholder Enablement Leads

### Role Summary
Customer Success / Stakeholder Enablement Leads prepare internal and external audiences for change. They own adoption readiness, release communications, and feedback loops back into the backlog.

### Responsibilities
- Maintain the stakeholder list and communication plan
- Prepare enablement materials, training, and support documentation
- Coordinate release announcements with support and customer-facing teams
- Collect and summarize customer and stakeholder feedback
- Track adoption blockers and route them to the right owner

### Goals
- Ensure customers and internal teams are ready before a release lands
- Shorten the loop between customer feedback and backlog decisions
- Keep stakeholders aligned and free of surprises

### Decision Rights
- Approve customer-facing communications and enablement readiness
- Decide the timing and channels for release announcements

### Collaboration Points
- PM: supplies stakeholder updates and confirms communication milestones
- PdM: translates customer feedback into prioritization input
- Developers: clarifies behavior changes and migration steps for documentation
- QA: confirms known issues are documented before announcements
- Stakeholders: runs briefings, demos, and feedback sessions

### Typical Communication
- Release announcements and enablement guides
- Monthly stakeholder updates and adoption summaries
- Feedback digests shared at product alignment meetings

---

## Data / Analytics Leads

### Role Summary
Data / Analytics Leads make outcomes measurable. They define instrumentation, reporting, and analysis so decisions are evidence-based.

### Responsibilities
- Define success metrics and the instrumentation needed to measure them
- Validate data quality and tracking before and after release
- Build dashboards and reports for delivery and product outcomes
- Analyze results and report whether outcomes were achieved
- Flag data privacy considerations to the Security/Compliance Lead

### Goals
- Ensure every initiative has measurable success criteria
- Provide trustworthy, timely data for decisions
- Replace assumptions with evidence in planning and retrospectives

### Decision Rights
- Own metric definitions and the source of truth for reporting
- Confirm that tracking is in place before a feature is considered done

### Collaboration Points
- PM: reports delivery metrics and highlights measurement dependencies
- PdM: co-defines success metrics and validates outcomes after release
- Developers: specifies event tracking and reviews instrumentation in PRs
- QA: verifies tracking events as part of acceptance testing
- Stakeholders: presents outcome analysis at milestone and retrospective reviews

### Typical Communication
- Metric definitions and dashboards linked from the project board
- Outcome reports at milestone reviews and retrospectives
- Data quality alerts and tracking gaps raised at weekly syncs

---

## Cross-functional Participation by Lifecycle Phase

| Phase | Security/Compliance | UX / Design | Operations / SRE | Customer Success | Data / Analytics |
| --- | --- | --- | --- | --- | --- |
| Initiation | Flag security, privacy, and compliance constraints in the one-pager | Frame user needs and validate the problem statement | Raise operational constraints and capacity needs | Identify stakeholder groups and adoption risks | Define candidate success metrics |
| Planning | Schedule reviews and required controls | Deliver flows and accessibility requirements | Define production readiness and rollout needs | Draft the communication and enablement plan | Plan instrumentation and reporting work |
| Execution | Review designs, code, and scan findings | Review implementation fidelity and usability | Review observability, runbooks, and rollback plans | Prepare enablement materials and updates | Verify tracking and data quality |
| Release | Sign off on security and compliance readiness | Confirm usability and accessibility readiness | Approve production readiness and verify post-deploy | Announce the release and enable support | Confirm metrics are collecting correctly |
| Retrospective | Report security findings and follow-up actions | Share usability and accessibility learnings | Lead post-incident reviews and reliability actions | Summarize adoption and feedback themes | Report outcomes against success metrics |

## Coordination, Escalation, and Approval Paths
- Coordination: the PM is the single point of coordination across roles and keeps the project board and status source of truth current. Each lead brings their own risks, dependencies, and readiness status to the weekly delivery sync.
- Escalation: follow the standard path of Team-level -> PM -> Product Lead -> Sponsor. Security incidents follow the security incident runbook and notify Security on-call; production incidents follow the rollback and incident playbook and notify the Operations / SRE Lead on-call.
- Approvals before release: Security/Compliance (security and compliance readiness), Operations / SRE (production readiness), UX / Design (usability and accessibility), Data / Analytics (metrics instrumentation), and Customer Success (communications and enablement). The PdM resolves scope trade-offs; unresolved blocking concerns escalate to the Sponsor.

## Ownership and Handoffs
- Every risk, action item, and readiness check has one named owner; the PM records the owner in the risk register or project board.
- Initiation to planning: the PdM hands the approved one-pager to the PM, who confirms which cross-functional leads are engaged and named in the plan.
- Planning to execution: UX / Design hands off specs and accessibility requirements, Security/Compliance hands off required controls, and Data / Analytics hands off metric definitions, all linked from the relevant issues.
- Execution to release: Developers and QA hand off verified changes; Operations / SRE owns deployment and post-deploy verification; Customer Success owns the announcement once verification passes.
- Release to retrospective: each lead brings their findings and owned follow-up actions, which are tracked to closure like any other backlog item.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

