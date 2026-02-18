# OctoAcme Process Checklists

## Purpose
Provide quick reference checklists for common project management activities and decision gates.

---

## Project Initiation Checklist

Use this checklist when starting a new project or major initiative.

### Business Validation
- [ ] Problem statement defined and validated with stakeholders
- [ ] Business goals and success metrics documented (SMART format)
- [ ] Customer research or discovery completed
- [ ] Budget and resource approval obtained
- [ ] Strategic alignment confirmed with leadership

### Stakeholder Alignment
- [ ] Stakeholder list created and roles defined
- [ ] Sponsor identified and committed
- [ ] Executive briefing completed
- [ ] Communication plan documented
- [ ] Approval meeting completed

### Team & Scope
- [ ] Project Manager assigned
- [ ] Product Manager assigned
- [ ] Core team identified (developers, QA, designers, etc.)
- [ ] High-level scope documented
- [ ] Timeline and key milestones sketched
- [ ] Initial risk list created

### Setup
- [ ] Project repository or project board created
- [ ] Project charter/one-pager added to repo
- [ ] Issue templates configured
- [ ] First kickoff meeting scheduled
- [ ] Documentation templates prepared

### Decision Gate: Move to Planning?
- [ ] Problem and goals are clear ✓
- [ ] Stakeholder buy-in obtained ✓
- [ ] Success metrics defined ✓
- [ ] Team capacity confirmed ✓
- [ ] **Decision: APPROVE / DEFER / REJECT**

---

## Project Planning Checklist

Use this checklist during the planning phase.

### Kickoff & Alignment
- [ ] Kickoff meeting held with full team
- [ ] Project charter reviewed and confirmed
- [ ] Success metrics and acceptance criteria reviewed
- [ ] Team roles and responsibilities clarified
- [ ] Questions and concerns addressed

### Backlog & Scope
- [ ] Features broken down into shippable stories
- [ ] Acceptance criteria defined for each story
- [ ] Story points or effort estimates provided
- [ ] Dependencies identified and documented
- [ ] Cross-team dependencies flagged
- [ ] Backlog prioritized and sequenced

### Timeline & Milestones
- [ ] Release milestones and dates set
- [ ] Sprint/iteration length agreed (if applicable)
- [ ] Key decision points and gates identified
- [ ] Risk buffer included in timeline
- [ ] Dependencies with other projects identified

### Quality & Testing
- [ ] Definition of Done documented
- [ ] Test strategy and test plan drafted
- [ ] Acceptance criteria clear and testable
- [ ] Test environment requirements identified
- [ ] Accessibility and security requirements noted

### Resources & Capacity
- [ ] Team capacity confirmed for duration
- [ ] Roles and responsibilities documented
- [ ] Training or ramp-up time accounted for
- [ ] External dependencies (vendors, approvals) identified

### Execution Plan
- [ ] Team rhythm documented (standups, syncs, demos)
- [ ] Communication channels and cadence set
- [ ] Escalation paths and decision makers identified
- [ ] Risk register created and reviewed
- [ ] Retrospective schedule set

### Decision Gate: Ready to Execute?
- [ ] Backlog is defined and prioritized ✓
- [ ] Team is clear on goals and dependencies ✓
- [ ] Timeline and milestones are realistic ✓
- [ ] Resources are confirmed ✓
- [ ] All parties are aligned ✓
- [ ] **Decision: APPROVE / REVISE / DEFER**

---

## Execution & Tracking Checklist

Use this weekly during execution.

### Daily Activities
- [ ] Daily standup held (15 min, blockers identified)
- [ ] Project board updated (stories moved to correct status)
- [ ] PRs created with clear descriptions and acceptance criteria
- [ ] Code reviews completed (feedback provided within 24 hours)
- [ ] CI/CD tests passing before merge

### Weekly Activities
- [ ] Weekly PM/PdM sync held
  - [ ] Velocity and progress reviewed
  - [ ] Risks and blockers discussed
  - [ ] Dependencies and handoffs confirmed
  - [ ] Decisions made and documented
  
- [ ] Delivery or demo meeting held
  - [ ] Completed work demonstrated
  - [ ] Stakeholder feedback captured
  - [ ] Scope or timeline changes identified
  
- [ ] Risk register reviewed and updated
  - [ ] New risks added
  - [ ] Mitigations assessed
  - [ ] Escalation needed? (if so, escalate)

### Quality Gates
- [ ] Test coverage maintained at agreed level
- [ ] No critical defects in main branch
- [ ] Security scanning passed
- [ ] Performance benchmarks met
- [ ] Accessibility standards validated

### Communication
- [ ] Stakeholders received status update
- [ ] Decisions communicated to all parties
- [ ] Escalations tracked and resolved
- [ ] Documentation updated

### Tracking & Metrics
- [ ] Burndown or velocity tracked
- [ ] Success metrics collected
- [ ] Defect metrics recorded
- [ ] Team morale and blockers noted

---

## Code Review & PR Checklist

Use this for every pull request.

### Description & Context
- [ ] PR title is clear and descriptive
- [ ] Link to related issue included
- [ ] Description explains what and why
- [ ] Acceptance criteria listed
- [ ] Related PRs or dependencies noted

### Code Quality
- [ ] Code follows team style guide
- [ ] Comments explain complex logic
- [ ] No commented-out or debug code
- [ ] Variable names are clear and meaningful
- [ ] Functions are focused and testable

### Testing
- [ ] New logic has unit tests
- [ ] Tests cover happy path and edge cases
- [ ] No test regressions
- [ ] CI/CD tests pass
- [ ] Manual testing completed (if needed)

### Performance & Security
- [ ] No obvious performance regressions
- [ ] SQL queries are optimized (if applicable)
- [ ] Security scanning passed
- [ ] No hardcoded secrets or credentials
- [ ] Dependencies are up-to-date

### Documentation
- [ ] Code comments are clear and helpful
- [ ] API documentation updated (if applicable)
- [ ] README or guides updated (if applicable)
- [ ] Migration steps documented (if applicable)

### Readiness for Merge
- [ ] At least one approval from reviewer
- [ ] All requested changes addressed
- [ ] Ready for production (not draft or WIP)
- [ ] No merge conflicts

---

## Release Readiness Checklist

Use this before every release.

### Scope & Content
- [ ] All committed features are complete
- [ ] Acceptance criteria met for each feature
- [ ] No unplanned scope changes
- [ ] All PRs merged and tested in main

### Quality Assurance
- [ ] QA Lead sign-off obtained
- [ ] Regression testing passed
- [ ] Critical path testing completed
- [ ] Performance testing passed
- [ ] Accessibility testing passed
- [ ] Security scanning passed
- [ ] No critical or high severity defects

### Documentation & Communication
- [ ] Release notes drafted and reviewed
- [ ] User guides updated
- [ ] API documentation updated
- [ ] Migration steps documented (if applicable)
- [ ] Customer communication prepared

### Deployment Preparation
- [ ] Deployment runbook reviewed
- [ ] Rollback plan documented and tested
- [ ] Staging deployment successful
- [ ] Staging smoke tests passed
- [ ] Database migrations tested (if applicable)
- [ ] Environment variables and config confirmed
- [ ] On-call engineer confirmed

### Stakeholder Readiness
- [ ] Product Manager approval obtained
- [ ] Sponsor aware of release (if major)
- [ ] Support team trained on new features
- [ ] Sales/marketing briefed (if customer-facing)
- [ ] Customer success notified

### Final Go/No-Go
- [ ] All checklist items completed ✓
- [ ] Quality metrics acceptable ✓
- [ ] Stakeholders approve ✓
- [ ] No blocking risks ✓
- [ ] **Decision: GO FOR RELEASE / HOLD**

---

## Post-Release Verification Checklist

Use this immediately after deployment.

### Deployment Verification
- [ ] Deployment completed successfully
- [ ] No errors in deployment logs
- [ ] Application is healthy (status page, monitoring)
- [ ] Core functionality working
- [ ] Database migrations successful (if applicable)

### Smoke Tests
- [ ] Login/authentication working
- [ ] Happy path user flows working
- [ ] Critical features accessible
- [ ] Error handling functioning
- [ ] Performance metrics normal

### Monitoring & Alerting
- [ ] Monitoring dashboards showing normal metrics
- [ ] Error rates normal
- [ ] Performance metrics normal
- [ ] Alerts configured and active
- [ ] On-call engineer on watch

### Communication
- [ ] Release announcement sent to stakeholders
- [ ] Users notified (if customer-facing)
- [ ] Support team notified of changes
- [ ] Success metrics collection started

### Rollback Readiness
- [ ] Rollback plan is ready if needed
- [ ] On-call engineer aware of rollback process
- [ ] Previous version accessible for quick rollback
- [ ] Decision criteria for rollback documented

---

## Retrospective Checklist

Use this after every sprint, release, or milestone.

### Preparation
- [ ] Retrospective scheduled for 45-75 minutes
- [ ] Team members confirmed attending
- [ ] Anonymous feedback tool set up (optional)
- [ ] Previous action items reviewed

### Facilitation
- [ ] "What went well?" ideas captured (10 min)
- [ ] "What could be improved?" ideas captured (15 min)
- [ ] Root causes discussed (10 min)
- [ ] Top 2-3 action items prioritized (10 min)
- [ ] Owners and due dates assigned (5 min)

### Action Items
- [ ] Each action item has: title, owner, due date, success criteria
- [ ] Action items are realistic and specific (not vague)
- [ ] No more than 3-5 action items per retrospective
- [ ] Owner confirmed they can take on action

### Follow-up
- [ ] Action items added to project backlog or issue tracker
- [ ] Retrospective notes shared with team
- [ ] Previous action items reviewed in next retrospective
- [ ] Improvements from action items celebrated and communicated

---

## Risk & Blocker Escalation Checklist

Use this when a risk or blocker needs escalation.

### Risk Documentation
- [ ] Risk ID and description documented
- [ ] Impact (High/Med/Low) assessed
- [ ] Likelihood (High/Med/Low) assessed
- [ ] Current owner assigned
- [ ] Mitigation plan drafted

### Escalation Decision
- [ ] Is this a team-level issue (can be resolved in standup)?
- [ ] Or PM-level escalation needed?
- [ ] Or sponsor-level escalation needed?

### Escalation Message
- [ ] Clear description of issue
- [ ] Business impact explained
- [ ] Proposed solutions identified
- [ ] Timeline/urgency communicated
- [ ] Decision/approval being requested

### Follow-up
- [ ] Decision communicated to team
- [ ] Risk register updated with status
- [ ] Mitigation plan assigned to owner
- [ ] Next review date scheduled
- [ ] All stakeholders notified
