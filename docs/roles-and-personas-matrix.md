# OctoAcme — Roles & Personas RACI Matrix

## Purpose
Provide a compact, at-a-glance reference for assigning responsibility across common project activities. Use this matrix at project kickoff, during planning, and before major releases to confirm ownership is clear.

## When to use
- **Project kickoff** — walk through the matrix with your team and fill in named owners.
- **Sprint planning** — verify accountability before committing work.
- **Release planning** — confirm all pre- and post-release activities have an Accountable owner.
- **Onboarding** — help new team members quickly understand their scope of responsibility.

## RACI Key

| Symbol | Meaning |
|--------|---------|
| **R** | Responsible — does the work |
| **A** | Accountable — owns the outcome; approves/signs off |
| **C** | Consulted — provides input before decisions or actions |
| **I** | Informed — kept in the loop after decisions or actions |

---

## Matrix

| Activity | PdM | PM | Developers | QA | UX Designer | DevOps | Tech Writer | Support Lead | Security Champion | Business Analyst | Stakeholders |
|---|---|---|---|---|---|---|---|---|---|---|---|
| Requirements gathering | A | C | C | C | C | I | I | C | C | R | C |
| Backlog prioritization | A | C | C | I | C | I | I | C | C | C | C |
| UX design & prototyping | C | I | C | C | A/R | I | I | I | I | C | C |
| Technical design | C | I | A/R | C | C | C | I | I | R | C | I |
| Implementation | C | I | A/R | C | C | C | I | I | C | I | I |
| Code review | I | I | A/R | C | I | C | I | I | C | I | I |
| QA / Testing | C | I | R | A/R | C | C | C | I | C | C | I |
| Security review | C | I | C | C | I | C | I | I | A/R | I | I |
| Documentation | C | I | C | C | C | I | A/R | C | I | C | I |
| Release execution | I | A | R | C | I | R | C | C | C | I | I |
| Release go/no-go | C | A | C | R | I | C | I | C | C | I | C |
| Incident response | I | A | R | C | I | R | I | C | C | I | I |
| Stakeholder communication | C | A | I | I | I | I | I | I | I | C | I |
| Post-release retrospective | C | A | R | R | C | R | C | C | C | C | C |
| Onboarding new team member | C | A | C | C | C | C | C | C | C | C | I |

> **Note:** A/R in the same cell means the role is both Accountable and Responsible (common for small teams or specialist roles).

---

## How to adapt this matrix

1. **Copy this table** into your project README or one-pager.
2. **Replace role labels** with real names for your project (e.g., "DevOps → Alex Chen").
3. **Add or remove rows** for activities unique to your project (e.g., localization, compliance review).
4. **Limit Accountable to one person** per row — if two people share accountability, clarify the boundary.
5. **Review at kickoff and before each major release** to ensure assignments are current.

## Related resources
- [Roles & Personas detail](./octoacme-roles-and-personas.md)
- [Role Onboarding Checklist](./templates/role-onboarding-checklist.md)
- [Release Checklist (Compact)](./templates/release-checklist-compact.md)
