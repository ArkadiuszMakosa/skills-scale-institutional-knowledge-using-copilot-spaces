# OctoAcme — Cross-Functional Checklists & Process Templates

## Purpose
Provide lightweight, reusable checklists and templates to improve accountability, reduce ambiguity, and support repeatable project execution across the full delivery lifecycle.

---

## Definition of Ready (DoR)

A backlog item is **Ready** to be pulled into a sprint when all of the following are true:

- [ ] Problem statement / user story is clearly written and understood by the team
- [ ] Acceptance criteria are defined and reviewed by the Product Manager and QA Lead
- [ ] UX designs or wireframes are available and signed off (if applicable)
- [ ] Business Analyst has resolved any outstanding requirement ambiguities
- [ ] Dependencies on other teams or services are identified and tracked
- [ ] Story is estimated (T-shirt size or story points)
- [ ] No blocking risks are unmitigated

> **Owners:** Product Manager defines criteria; Business Analyst validates completeness; QA Lead confirms testability.

---

## Definition of Done (DoD)

A backlog item is **Done** when all of the following are true:

- [ ] All acceptance criteria are met and verified by QA Lead
- [ ] Code reviewed and merged (PR approved per team policy)
- [ ] Automated tests (unit / integration) written and passing in CI
- [ ] No open critical or high-severity defects related to the item
- [ ] UX Designer has reviewed implementation against design spec (if applicable)
- [ ] Documentation updated (Technical Writer sign-off if docs-impacting)
- [ ] Feature flagged or release-ready as appropriate
- [ ] Product Manager has accepted the item

> **Owners:** QA Lead verifies; Product Manager accepts; Developer, UX Designer, and Technical Writer contribute sign-offs as applicable.

---

## Cross-Functional Handoff Checklist

Use this checklist at each major handoff point to ensure continuity and reduce dropped context.

### Design → Development Handoff

- [ ] Design files (wireframes, prototypes) finalized and accessible to Developers
- [ ] Design specifications annotated with interaction details, edge cases, and accessibility notes
- [ ] Open design questions documented and resolved with the Product Manager
- [ ] UX Designer available for questions during implementation sprint
- [ ] Acceptance criteria include UX-specific checks (e.g., responsive behavior, error states)

> **Handoff Owners:** UX Designer hands off to Developers; Business Analyst confirms requirements are reflected.

### Development → QA Handoff

- [ ] Feature branch merged to integration/staging environment
- [ ] Developer has completed self-testing and resolved known issues
- [ ] Test environment configured and accessible to QA Lead
- [ ] Acceptance criteria provided to QA Lead in ticket or PR description
- [ ] Any known risks or edge cases flagged to QA Lead

> **Handoff Owners:** Developer hands off to QA Lead; Project Manager confirms environment readiness.

### QA → Release Handoff

- [ ] All acceptance criteria verified and documented by QA Lead
- [ ] No open critical or high-severity defects blocking release
- [ ] Regression test suite passed
- [ ] Release notes drafted and reviewed (Technical Writer / Product Manager)
- [ ] Rollback plan documented (Project Manager / DevOps)
- [ ] Product Manager sign-off on release readiness

> **Handoff Owners:** QA Lead hands off to Project Manager and Product Manager for release approval.

---

## RACI Mini-Matrix

Quick reference for key activities across the project lifecycle. **R** = Responsible, **A** = Accountable, **C** = Consulted, **I** = Informed.

| Activity | Project Manager | Product Manager | Developer | UX Designer | QA Lead | Technical Writer | Business Analyst |
|---|---|---|---|---|---|---|---|
| Define project charter | A | C | I | I | I | I | C |
| Prioritize backlog | C | A | C | C | C | I | R |
| Write acceptance criteria | I | A | C | C | C | I | R |
| UX design & wireframes | I | C | C | A/R | I | I | C |
| Implementation | C | I | A/R | C | C | I | I |
| Test planning & execution | C | C | C | I | A/R | I | C |
| Documentation updates | C | C | C | I | I | A/R | C |
| Risk management | A/R | C | C | I | C | I | C |
| Release sign-off | A | C | C | I | R | I | I |
| Retrospective facilitation | A/R | C | C | C | C | C | C |

---

## Stakeholder Update Template

Use this template for regular stakeholder communications (weekly or milestone-based).

```
## Stakeholder Update — [Project Name] | [Date]

**Owner:** [Project Manager name]

### Summary
[1–2 sentence status: on track / at risk / blocked]

### Progress This Period
- [Key accomplishment 1]
- [Key accomplishment 2]

### Upcoming Next Steps
- [Next milestone or deliverable + target date]

### Risks & Blockers
| Risk / Blocker | Impact | Owner | Mitigation |
|---|---|---|---|
| [Description] | High/Med/Low | [Name] | [Action] |

### Decisions Needed
- [Decision or approval required, with deadline]

### Notes
[Any additional context for stakeholders]
```

> **Owner:** Project Manager drafts and sends; Product Manager reviews before distribution.

---

## See Also
- [Roles & Personas](octoacme-roles-and-personas.md) — full role definitions and interaction notes
- [Project Planning](octoacme-project-planning.md) — backlog and sprint planning guidance
- [Execution & Tracking](octoacme-execution-and-tracking.md) — day-to-day delivery workflows
- [Release & Deployment](octoacme-release-and-deployment.md) — release checklists and deployment guide
- [Risks & Communication](octoacme-risks-and-communication.md) — risk register and communication templates
