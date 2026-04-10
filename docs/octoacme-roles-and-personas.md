# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

## How to use this document

Each persona entry includes a **Role Summary**, **Responsibilities**, **Goals**, **Typical Communication**, and an **Interactions with existing roles** section describing handoffs and escalation paths. Use these entries to:
- Assign clear ownership during project planning.
- Onboard new team members to role expectations quickly.
- Set up role-specific Copilot Spaces prompts for guided assistance.

For a compact at-a-glance responsibility assignment, see the [Roles & Personas RACI Matrix](./roles-and-personas-matrix.md).

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

### Interactions with existing roles
- **PdM**: Receive acceptance criteria and clarify requirements; flag technical constraints that affect scope.
- **PM**: Report progress and blockers in standups; provide estimates and input for planning.
- **QA**: Hand off completed features for testing; address bugs surfaced during QA cycles.
- **DevOps**: Collaborate on CI/CD configuration, deployment scripts, and environment issues.
- **Stakeholders**: Participate in demos to gather direct feedback.

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

### Interactions with existing roles
- **PM**: Align on scope, timeline, and priority changes; jointly manage trade-off decisions.
- **Developers**: Provide clear acceptance criteria; review completed work for business fit.
- **QA**: Review test scenarios to confirm coverage of business requirements.
- **UX Designer**: Co-define user experience goals; review prototypes before development begins.
- **Business Analyst**: Receive detailed requirements analysis; collaborate on backlog refinement.
- **Stakeholders**: Present roadmap updates and gather approval or feedback.

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

### Interactions with existing roles
- **PdM**: Align scope and priority; jointly manage change requests.
- **Developers**: Surface blockers and dependencies; ensure work is planned and tracked.
- **QA**: Coordinate test cycles and acceptance sign-off timing.
- **DevOps**: Schedule deployment windows; notify of production-risk items during Level 2 escalations.
- **Customer Support Lead**: Notify of upcoming releases; receive post-release customer feedback.
- **Stakeholders**: Provide status reports and escalate issues requiring sponsor-level decisions.

---

## QA / Testing

### Role Summary
QA engineers validate that features meet acceptance criteria and quality standards before release. They own test plans, defect tracking, and go/no-go sign-off.

### Responsibilities
- Create and maintain test plans and test cases
- Execute manual and automated tests
- Log, track, and verify resolution of defects
- Provide go/no-go sign-off for releases
- Contribute to CI/CD quality gates

### Goals
- Ensure releases are stable and meet acceptance criteria
- Reduce defect escape rate to production
- Provide fast, reliable feedback to developers

### Typical Communication
- Test status reports and defect logs
- Go/no-go decisions communicated to PM before release
- Participation in sprint reviews and retrospectives

### Interactions with existing roles
- **Developers**: Receive completed features; report defects and verify fixes.
- **PM**: Communicate test status and risks; flag blockers that affect release schedule.
- **PdM**: Confirm acceptance criteria coverage; escalate ambiguous requirements.
- **DevOps**: Coordinate test environment stability; align on deployment readiness.
- **Tech Writer**: Validate that documentation reflects tested behavior.

---

## UX Designer

### Role Summary
UX Designers ensure that features are usable, accessible, and aligned with user needs. They translate requirements into wireframes, prototypes, and design specifications.

### Responsibilities
- Conduct user research and usability testing
- Create wireframes, mockups, and interactive prototypes
- Define and maintain design standards and component libraries
- Provide design specifications to developers
- Iterate on designs based on user feedback and metrics

### Goals
- Deliver intuitive, accessible user experiences
- Reduce usability issues discovered post-release
- Keep design assets organized and reusable

### Typical Communication
- Design reviews and prototype walkthroughs
- Annotated design specs shared with developers
- Participation in sprint planning and retrospectives

### Interactions with existing roles
- **PdM**: Co-define user experience goals; review prototypes for alignment with product vision.
- **PM**: Communicate design milestone status and flag scope changes.
- **Developers**: Provide detailed design specs and answer implementation questions.
- **QA**: Validate that implemented UI matches approved designs and accessibility requirements.
- **Stakeholders**: Present design concepts and incorporate feedback before development.

---

## Technical Writer

### Role Summary
Technical Writers create and maintain clear, accurate documentation for users and internal teams. They ensure knowledge is captured, organized, and easy to find.

### Responsibilities
- Write and update user guides, API docs, and internal runbooks
- Collaborate with developers and PdMs to document new features
- Review documentation for accuracy and completeness before release
- Maintain the documentation site or knowledge base
- Define documentation standards and templates

### Goals
- Ensure documentation is accurate, current, and useful
- Reduce support tickets caused by unclear documentation
- Streamline onboarding with well-structured knowledge resources

### Typical Communication
- Documentation review cycles linked to sprint milestones
- Collaborative editing with developers and PdMs
- Release notes published ahead of each release

### Interactions with existing roles
- **PdM**: Receive feature context and acceptance criteria to document new capabilities.
- **PM**: Align on documentation milestones within the project schedule.
- **Developers**: Obtain technical accuracy reviews for API and implementation docs.
- **QA**: Confirm documented behavior matches tested behavior before release.
- **Customer Support Lead**: Incorporate common support questions into knowledge base articles.

---

## DevOps Engineer

### Role Summary
DevOps Engineers manage infrastructure, CI/CD pipelines, deployment processes, and environment reliability. They enable teams to ship software safely and quickly.

### Responsibilities
- Build and maintain CI/CD pipelines and deployment automation
- Manage cloud infrastructure, environments, and configuration
- Monitor system health, alerts, and on-call escalations
- Coordinate and execute production deployments
- Lead incident response and post-incident reviews

### Goals
- Maximize deployment frequency while minimizing failure rate
- Keep environments stable and observable
- Reduce mean time to recovery (MTTR) for incidents

### Typical Communication
- Deployment schedule coordination with PM and QA
- Incident alerts and post-mortem reports
- Infrastructure change notifications to the development team

### Interactions with existing roles
- **PM**: Confirm deployment windows; receive notification of production-risk items during Level 2 escalations.
- **Developers**: Collaborate on pipeline configuration and environment troubleshooting.
- **QA**: Provide stable test environments; coordinate release readiness.
- **Security Champion**: Implement security controls and remediate pipeline vulnerabilities.
- **Customer Support Lead**: Notify of incidents that may affect customers; coordinate status page updates.

---

## Customer Support Lead

### Role Summary
Customer Support Leads act as the voice of the customer inside the team. They surface recurring issues, communicate product pain points, and ensure support teams are prepared for releases.

### Responsibilities
- Aggregate and prioritize customer-reported issues and feature requests
- Communicate high-impact bugs and patterns to PM and Developers
- Prepare support teams for upcoming feature releases
- Manage escalated customer cases and coordinate resolution
- Contribute to post-release retrospectives with customer feedback data

### Goals
- Reduce customer-impacting incidents and unresolved issues
- Ensure support teams are always release-ready
- Close the feedback loop between customers and product teams

### Typical Communication
- Weekly support summaries shared with PM and PdM
- Pre-release briefings for support teams
- Escalation notifications for high-impact customer issues

### Interactions with existing roles
- **PdM**: Share top customer pain points to influence roadmap prioritization.
- **PM**: Provide post-release feedback; receive advance notice of release dates.
- **Developers**: Escalate reproducible bugs with customer context and priority.
- **DevOps**: Coordinate status page updates and incident communications for customers.
- **Tech Writer**: Contribute to knowledge base articles based on common support questions.

---

## Security Champion

### Role Summary
Security Champions promote secure development practices within the team. They review designs for security risks, educate teammates, and coordinate security incident response.

### Responsibilities
- Review technical designs and PRs for security vulnerabilities
- Champion secure coding standards and practices
- Participate in threat modeling exercises during planning
- Monitor security scanning tools and triage findings
- Lead security-related retrospectives and remediations

### Goals
- Reduce security vulnerabilities in delivered features
- Build security awareness across the team
- Ensure compliance with security policies and standards

### Typical Communication
- Security findings shared with Developers and PM
- Risk Register contributions for security-related items
- Security review sign-off documented before releases

### Interactions with existing roles
- **PdM**: Flag security risks that affect scope or timeline; advise on privacy and compliance requirements.
- **PM**: Contribute security items to the Risk Register; escalate critical vulnerabilities.
- **Developers**: Conduct code and design security reviews; provide remediation guidance.
- **DevOps**: Collaborate on pipeline security controls and infrastructure hardening.
- **QA**: Align on security test cases for high-risk features.

---

## Business Analyst

### Role Summary
Business Analysts bridge the gap between business stakeholders and the delivery team. They gather, document, and clarify requirements to ensure the team builds the right thing.

### Responsibilities
- Elicit and document business and functional requirements
- Analyze workflows and identify process improvement opportunities
- Create process diagrams, user stories, and acceptance criteria
- Validate delivered features against documented requirements
- Support backlog refinement and prioritization with data

### Goals
- Ensure requirements are unambiguous and complete before development
- Reduce rework caused by misunderstood scope
- Align stakeholder expectations with team delivery capacity

### Typical Communication
- Requirements documents and user story workshops
- Stakeholder interviews and analysis reports
- Backlog refinement sessions with PM and PdM

### Interactions with existing roles
- **PdM**: Translate high-level goals into detailed requirements and acceptance criteria.
- **PM**: Provide scoping input for planning; flag requirement gaps that affect timelines.
- **Developers**: Answer requirement questions during development; review implementations for accuracy.
- **Stakeholders**: Conduct requirements workshops and validate that delivered features meet business needs.
- **QA**: Provide detailed acceptance criteria to inform test case development.

---

## RACI Guidance

When assigning accountability for project activities, use a RACI model:
- **R (Responsible)** — Does the work.
- **A (Accountable)** — Owns the outcome; approves or signs off.
- **C (Consulted)** — Provides input before decisions or actions.
- **I (Informed)** — Kept in the loop after decisions or actions.

For a ready-to-use RACI matrix across common project activities, see [Roles & Personas RACI Matrix](./roles-and-personas-matrix.md).

**Tips for using RACI on your project:**
- Record specific owners (by name) in the project one-pager or README.
- Limit **Accountable** to one person per activity to avoid diffusion of responsibility.
- Review the matrix during project kickoff and before major releases.
- Adjust the matrix to match your team's actual composition — not all projects require all roles.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- When onboarding a new team member to a role, use the [Role Onboarding Checklist](./templates/role-onboarding-checklist.md).

