# OctoAcme Role Interactions & Collaboration Workflows

## Purpose
This document provides detailed workflows showing how different roles collaborate throughout the project lifecycle.

---

## Feature Development Workflow

### Participants
Product Manager → UX Designer → Developer → QA Lead → Technical Writer → Project Manager → Stakeholder

### Phase 1: Discovery & Definition (Week 1)
**Lead: Product Manager**

1. **Product Manager** defines the problem statement and success metrics
   - Creates feature brief with customer problem and business context
   - Identifies success metrics (adoption, engagement, cost savings, etc.)
   - Shares with Stakeholder for business approval

2. **Stakeholder** reviews and approves business case
   - Confirms alignment with organizational priorities
   - Approves resource allocation and timeline expectations

3. **Product Manager** kicks off with UX Designer
   - Shares problem statement, success metrics, and constraints
   - Discusses user personas and research needs
   - Identifies timeline and dependencies

### Phase 2: User Research & Design (Weeks 2-3)
**Lead: UX Designer**

1. **UX Designer** conducts user research
   - Interviews users and validates problem statement
   - Documents findings and recommendations
   - Shares insights with Product Manager for refinement

2. **Product Manager** refines requirements based on research
   - Adjusts scope and acceptance criteria
   - Validates solution direction with users
   - Prepares for Developer handoff

3. **UX Designer** creates design artifacts
   - Develops wireframes and prototypes
   - Validates design with Developer for feasibility
   - Gets feedback from Product Manager and Stakeholder
   - Creates final design spec and handoff document

### Phase 3: Implementation Planning (Week 4)
**Lead: Project Manager & Developer**

1. **Project Manager** schedules kickoff meeting
   - Invites Developers, QA Lead, Technical Writer, DevOps Engineer
   - Prepares project timeline and milestones

2. **Developer** reviews design and creates technical plan
   - Assesses feasibility and technical risks
   - Estimates effort and identifies dependencies
   - Discusses test strategy with QA Lead

3. **QA Lead** creates test plan
   - Reviews acceptance criteria and edge cases
   - Plans manual and automated testing approach
   - Identifies test environment needs

4. **Technical Writer** gathers requirements
   - Reviews design and acceptance criteria
   - Identifies documentation needs (user guide, API docs, etc.)
   - Plans documentation timeline

5. **DevOps Engineer** prepares CI/CD
   - Ensures pipeline supports the feature
   - Prepares staging environment for testing
   - Plans deployment steps

### Phase 4: Development & Testing (Weeks 5-7)
**Lead: Developer & QA Lead**

1. **Developer** implements feature
   - Opens PR with design doc reference and acceptance criteria
   - Coordinates with QA Lead on test coverage
   - Updates Technical Writer on implementation details

2. **QA Lead** conducts testing
   - Executes test plan (automated and manual)
   - Reports defects with clear reproduction steps
   - Works with Developer on test coverage improvements

3. **Technical Writer** creates documentation
   - Writes user guides based on implementation
   - Documents API endpoints and technical details
   - Gets feedback from QA Lead on edge cases

4. **Project Manager** tracks progress
   - Updates risk register weekly
   - Escalates blockers to Product Manager or Stakeholder
   - Coordinates between teams for dependencies

### Phase 5: Validation & Sign-off (Week 8)
**Lead: Product Manager & QA Lead**

1. **QA Lead** conducts final acceptance testing
   - Verifies all acceptance criteria are met
   - Conducts regression testing
   - Signs off on quality for release

2. **Product Manager** validates solution
   - Tests feature against success metrics
   - Gets user feedback if needed
   - Approves feature for release

3. **Technical Writer** finalizes documentation
   - Prepares release notes
   - Creates user communication if needed
   - Finalizes all related documentation

4. **DevOps Engineer** prepares release
   - Runs smoke tests in staging
   - Prepares deployment runbook
   - Coordinates with Project Manager on release window

### Phase 6: Release & Communication (Week 9)
**Lead: DevOps Engineer & Project Manager**

1. **DevOps Engineer** deploys to production
   - Follows deployment checklist
   - Monitors system health during and after deployment
   - Is ready to rollback if needed

2. **Project Manager** coordinates communication
   - Announces release to stakeholders
   - Communicates success metrics
   - Schedules retrospective

3. **Technical Writer** publishes documentation
   - Updates production docs
   - Announces new features to users
   - Provides training if needed

4. **Stakeholder** receives completion notification
   - Reviews success metrics against goals
   - Provides feedback for future iterations

---

## Risk & Blocker Escalation Workflow

### Scenario: Technical Risk Identified During Development

**Initial Detection** (Developer)
- Developer identifies a technical constraint that affects timeline or scope
- Documents issue in risk register with: risk ID, description, impact, likelihood, owner

**Level 1: Team Triage** (Daily Standup)
- Developer presents in standup
- QA Lead and Project Manager discuss mitigation options
- If resolvable by team: assign owner and close in standup
- If unresolvable: escalate to Level 2

**Level 2: PM Escalation** (Within 24 hours)
- Project Manager escalates to Product Manager
- Product Manager evaluates business impact
- Discusses with Stakeholder if scope change needed
- Options: delay feature, reduce scope, increase resources, accept risk
- Document decision in risk register

**Level 3: Sponsor Escalation** (If critical)
- If business impact is severe: Project Manager escalates to Stakeholder
- Stakeholder makes final go/no-go decision
- All parties notified of decision
- Execution plan adjusted accordingly

**Resolution & Follow-up**
- Owner tracks mitigation progress
- Risk status updated weekly in sync meetings
- Risk closed when mitigation complete

---

## Weekly Sync Workflow

### Participants
Project Manager, Product Manager, Engineering Lead (optional), QA Lead

### Duration
30-45 minutes

### Agenda
1. **Project Status** (10 min)
   - % complete toward milestones
   - Velocity and burndown
   - Any scope changes or new requests

2. **Risks & Blockers** (10 min)
   - Review risk register
   - Discuss any new or escalating risks
   - Review blockers from previous week

3. **Dependencies & Handoffs** (5 min)
   - Cross-team dependencies
   - Upcoming handoffs (design to dev, dev to QA, etc.)
   - External dependencies

4. **Decisions Needed** (10 min)
   - Priority conflicts or trade-offs
   - Resource allocation questions
   - Timeline adjustments

5. **Next Steps** (5 min)
   - Owner for each action item
   - Due dates
   - Communication plan

### Decision Log
After the meeting, Project Manager:
- Documents all decisions and action items
- Updates risk register
- Communicates decisions to broader team
- Schedules follow-ups if needed

---

## Incident Response Workflow

### Discovery Phase (Developer or DevOps)
1. **DevOps Engineer** or **Developer** discovers production issue
2. Immediately notifies **Project Manager** and on-call engineer
3. Gathers initial triage info: what broke, when, impact

### Response Phase (Immediate)
1. **DevOps Engineer** assesses options:
   - Can issue be fixed quickly (hotfix)?
   - Should we rollback?
   - Is workaround possible?

2. **Project Manager** notifies Stakeholder
   - Brief description of issue and impact
   - Expected timeline for resolution
   - Status update frequency

3. **Developer** or **DevOps** works on fix or rollback
4. **Technical Writer** prepares customer communication if needed

### Recovery Phase (Within incident window)
1. If hotfix: Developer creates PR, QA validates, DevOps deploys
2. If rollback: DevOps executes rollback, validates stability
3. Monitor system metrics to confirm stability
4. Update Stakeholder on resolution

### Post-Incident Phase (Within 24 hours)
1. **Project Manager** schedules blameless retrospective
2. **Developer** + **DevOps** + **QA Lead** participate
3. Document:
   - Root cause
   - Timeline of what happened
   - What we'll do differently next time
   - Owner for each action item

4. **Project Manager** shares summary with Stakeholder
   - Key learnings
   - Preventive actions
   - Timeline for improvements

---

## How to Use These Workflows

### During Project Setup
- Map your actual team to these personas
- Identify which workflows apply to your project
- Adjust timeline and phases as needed

### During Execution
- Use workflows as a checklist for handoffs
- Refer to interaction patterns when collaborating
- Escalate following the documented escalation paths

### For New Team Members
- Share relevant workflows with new roles
- Use workflows to explain expected collaboration patterns
- Reference for questions about "who should I talk to?"