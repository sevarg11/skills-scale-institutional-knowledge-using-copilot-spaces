# Decision Log Template

## Purpose
Track important project decisions, the people who made them, the rationale, and the date. A decision log helps distributed or cross-functional teams stay aligned on *why* things were decided, reduces revisiting settled decisions, and provides an audit trail for future reference.

## When to use
- During planning, when a significant scope, design, or process choice is made.
- When a stakeholder trade-off is agreed upon.
- Whenever a decision affects multiple roles or teams.
- During post-mortems or retrospectives to review past decisions.

---

## Log Table

| # | Date | Decision | Owner | Rationale | Alternatives Considered | Status | Related Links |
|---|------|----------|-------|-----------|------------------------|--------|---------------|
| 1 | YYYY-MM-DD | Short description of the decision | Role / Name | Why this option was chosen | Other options explored and why they were rejected | Active / Superseded / Reversed | Link to issue/PR/doc |

---

## Field Definitions

| Field | Description |
|-------|-------------|
| **#** | Sequential decision number for reference |
| **Date** | Date the decision was finalized |
| **Decision** | Concise statement of what was decided |
| **Owner** | Role and/or name of the person accountable for the decision |
| **Rationale** | Key reasons supporting the decision |
| **Alternatives Considered** | Other options that were evaluated and why they were rejected |
| **Status** | `Active` (current), `Superseded` (replaced by a later decision), or `Reversed` |
| **Related Links** | GitHub issue, PR, design doc, or meeting notes where more context lives |

---

## Sample Entries

| # | Date | Decision | Owner | Rationale | Alternatives Considered | Status | Related Links |
|---|------|----------|-------|-----------|------------------------|--------|---------------|
| 1 | 2025-06-10 | Use PostgreSQL for the new reporting database | Developers (Tech Lead) | Team familiarity, strong JSON support, aligns with existing infrastructure | MySQL (less JSON flexibility), MongoDB (more ops overhead) | Active | [#42](../../issues/42) |
| 2 | 2025-06-15 | Delay v2.3.0 release by one sprint to complete security review | PM + PdM | Security Champion identified two medium-severity findings requiring fixes | Ship with known findings (rejected — risk too high) | Active | [Release Planning Doc](../octoacme-release-and-deployment.md) |
| 3 | 2025-07-01 | Retire legacy API v1 endpoint after 90-day deprecation window | PdM | Reduces maintenance burden; customer adoption of v2 is at 95% | Keep v1 indefinitely (rejected — high maintenance cost) | Active | [#55](../../issues/55) |

---

## Tips

- Keep decision descriptions brief — link to full context rather than duplicating it.
- Record decisions as they are made, not weeks later.
- When a decision is superseded, update the **Status** column and add a reference to the new decision number.
- Review the decision log at sprint retrospectives to capture any undocumented decisions from the previous cycle.

---

## Related resources
- [Roles & Personas RACI Matrix](../roles-and-personas-matrix.md)
- [Execution & Tracking](../octoacme-execution-and-tracking.md)
- [Role Onboarding Checklist](./role-onboarding-checklist.md)
