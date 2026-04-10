# Release Checklist (Compact)

## Purpose
Provide a concise, role-aware checklist to ensure all pre-release, release, and post-release verification steps are completed with clear ownership.

## When to use
Before every production release. Adapt the checklist to match your release scope (hotfix, minor, major).

---

## Pre-Release

### Product & Planning
- [ ] **PdM** — Confirm all planned features have accepted acceptance criteria
- [ ] **PM** — Verify release scope is finalized and communicated to all stakeholders
- [ ] **PM** — Risk Register reviewed; open risks acknowledged or mitigated
- [ ] **PM** — Review [Roles & Personas RACI Matrix](../roles-and-personas-matrix.md) to confirm owners for this release

### Development & Quality
- [ ] **Developers** — All feature branches merged to release branch; no outstanding merge conflicts
- [ ] **Developers** — Code reviewed and approved (min. 1 approval per PR per team policy)
- [ ] **QA** — Test plan completed and all critical/blocking defects resolved
- [ ] **QA** — End-to-end smoke tests passed on staging environment
- [ ] **Security Champion** — Security review completed; no unresolved high/critical findings
- [ ] **DevOps** — Staging environment mirrors production configuration

### Documentation & Support
- [ ] **Tech Writer** — Release notes drafted and reviewed for accuracy
- [ ] **Tech Writer** — User-facing documentation updated for new or changed features
- [ ] **Support Lead** — Support team briefed on new features and known issues
- [ ] **Support Lead** — FAQ / knowledge base articles updated if needed

---

## Release

- [ ] **PM** — Go/no-go decision made and communicated to all stakeholders
- [ ] **DevOps** — Deployment executed in agreed maintenance window
- [ ] **DevOps** — Deployment logs and health checks reviewed immediately post-deploy
- [ ] **QA** — Production smoke test executed and passed
- [ ] **Developers** — On-call engineer confirmed available for 1 hour post-release
- [ ] **PM** — Release announcement sent to stakeholders

---

## Post-Release Verification

- [ ] **DevOps** — Monitoring dashboards checked for anomalies (errors, latency, resource usage)
- [ ] **QA** — Any new defects triaged and assigned
- [ ] **Support Lead** — Customer-facing channels monitored for unexpected issues
- [ ] **PM** — Post-release summary documented (what shipped, known issues, next steps)
- [ ] **PM** — Retrospective scheduled if release included significant challenges
- [ ] **Tech Writer** — Confirm documentation is live and accessible

---

## Rollback Criteria

Initiate rollback if any of the following occur within 1 hour post-release:
- Error rate increases by >5% over baseline
- Critical customer-impacting bug reported
- Core user flow broken (confirmed by smoke tests)
- Security incident triggered by release

**Rollback owner:** DevOps Engineer (notifies PM immediately)

---

## Sample Completed Entry

**Release:** v2.3.0 — Customer Dashboard Update  
**Release date:** 2025-07-15  
**Release manager (PM):** Morgan Smith  

| Step | Owner | Status |
|------|-------|--------|
| Scope finalized | Morgan Smith (PM) | ✅ Done |
| QA smoke tests passed | Jamie Reyes (QA) | ✅ Done |
| Security review | Alex Park (Security Champion) | ✅ Done |
| Deployment executed | Taylor Wu (DevOps) | ✅ Done |
| Production smoke test | Jamie Reyes (QA) | ✅ Done |
| Support team briefed | Casey Nguyen (Support Lead) | ✅ Done |

---

## Related resources
- [Roles & Personas RACI Matrix](../roles-and-personas-matrix.md)
- [Role Onboarding Checklist](./role-onboarding-checklist.md)
- [Execution & Tracking](../octoacme-execution-and-tracking.md)
