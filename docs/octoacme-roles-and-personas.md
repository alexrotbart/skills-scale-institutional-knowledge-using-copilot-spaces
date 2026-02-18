# OctoAcme Personas & Roles

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Core Roles

### Developers

**Role Summary**
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

**Responsibilities**
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

**Goals**
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

**Typical Communication**
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

**Key Interactions**
- With QA Lead: Code review for testability, test coverage discussion
- With DevOps Engineer: Deployment readiness, CI/CD pipeline questions
- With UX Designer: Implementation feedback on wireframes and designs
- With Technical Writer: Technical documentation and API details

---

### Product Managers

**Role Summary**
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

**Responsibilities**
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics
- Review and approve feature acceptance criteria

**Goals**
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

**Typical Communication**
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

**Key Interactions**
- With Project Manager: Weekly sync on schedule, risks, and blockers
- With UX Designer: Requirements refinement and user feedback loops
- With Stakeholders: Priority alignment and business context
- With Technical Writer: User guide and release communication

---

### Project Managers

**Role Summary**
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

**Responsibilities**
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication
- Escalate blockers and manage escalation paths

**Goals**
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

**Typical Communication**
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

**Key Interactions**
- With Product Manager: Weekly alignment on priorities and outcomes
- With DevOps Engineer: Release coordination and deployment schedules
- With QA Lead: Quality metrics and testing timelines
- With Stakeholders: Status updates and milestone approvals

---

## Specialized Roles

### UX Designer

**Role Summary**
UX Designers ensure solutions meet user needs through research, design, and iterative testing. They collaborate with Product Managers on requirements and with Developers on implementation feasibility.

**Responsibilities**
- Conduct user research and validate problem statements
- Create wireframes, mockups, and prototypes
- Run usability tests and gather user feedback
- Document design decisions and rationale
- Collaborate with Developers on implementation details
- Ensure accessibility and consistency across features

**Goals**
- Deliver intuitive, user-centered solutions
- Reduce user friction and support burden
- Maintain design consistency across the product

**Typical Communication**
- Design reviews with Product Managers and Developers
- User research findings and recommendations
- Design documentation and handoff specs

**Key Interactions**
- With Product Managers: Requirements refinement and user feedback
- With Developers: Design feasibility and implementation questions
- With QA Lead: User acceptance testing and edge case validation
- With Technical Writer: User guide accuracy and terminology

**Example Workflow**
1. Kickoff: Review problem statement with Product Manager
2. Research: Conduct user interviews and validate assumptions
3. Design: Create wireframes and get developer feasibility feedback
4. Iterate: Run usability tests and refine based on feedback
5. Handoff: Document final design and acceptance criteria with Developers

---

### QA Lead

**Role Summary**
QA Leads champion quality and testing standards across the project. They own test strategy, coordinate manual and automated QA efforts, and monitor quality metrics.

**Responsibilities**
- Develop test strategy and test plans for features
- Coordinate manual and automated QA activities
- Track defect metrics and quality indicators
- Create and maintain test checklists and scripts
- Validate acceptance criteria before release
- Identify and escalate quality risks
- Collaborate with Developers on test coverage improvement

**Goals**
- Deliver high-quality features that meet acceptance criteria
- Reduce production defects and support burden
- Enable confident releases through comprehensive testing

**Typical Communication**
- Quality reports in weekly syncs
- Test plans and defect logs
- Release readiness sign-offs

**Key Interactions**
- With Developers: Test coverage review, build quality discussion
- With Project Manager: Quality metrics and timeline impact
- With DevOps Engineer: Test environment setup and deployment validation
- With UX Designer: User acceptance testing and edge cases

**Example Workflow**
1. Planning: Create test plan with acceptance criteria
2. Development: Collaborate with Developers on test coverage
3. Testing: Execute automated and manual QA
4. Validation: Verify acceptance criteria are met
5. Release: Conduct final regression and sign-off

---

### DevOps Engineer

**Role Summary**
DevOps Engineers maintain CI/CD pipelines, automate deployment processes, and ensure system reliability and observability. They enable rapid, safe releases.

**Responsibilities**
- Design and maintain CI/CD pipelines
- Automate deployment and release processes
- Monitor system health, performance, and observability
- Manage infrastructure and deployment environments
- Coordinate deployments and manage rollback processes
- Identify and resolve deployment-related risks

**Goals**
- Enable rapid, reliable deployments
- Maintain high system availability and performance
- Reduce mean time to recovery (MTTR) for incidents

**Typical Communication**
- Deployment readiness checks
- System health and incident alerts
- Infrastructure and pipeline documentation

**Key Interactions**
- With Developers: Build pipeline support, deployment questions
- With Project Manager: Release scheduling and deployment coordination
- With QA Lead: Test environment setup and staging validation
- With Technical Writer: Deployment runbooks and incident procedures

**Example Workflow**
1. Planning: Review deployment requirements and environment needs
2. Preparation: Ensure CI/CD pipeline is ready, conduct smoke tests
3. Coordination: Coordinate deployment window with Project Manager
4. Execution: Deploy to staging, validate, then production
5. Monitoring: Monitor system health and be ready for rollback

---

### Technical Writer

**Role Summary**
Technical Writers maintain accurate, accessible documentation of features, APIs, and processes. They collaborate with Developers, Product Managers, and QA to ensure clarity and completeness.

**Responsibilities**
- Document features, APIs, and user guides
- Create and maintain operational runbooks and procedures
- Collaborate with Developers on technical accuracy
- Review and approve release notes and communication
- Ensure consistency in terminology and style
- Manage documentation version control and updates

**Goals**
- Reduce support burden through clear documentation
- Enable rapid onboarding for new team members
- Maintain single source of truth for feature information

**Typical Communication**
- Documentation reviews with subject matter experts
- Release notes and API documentation
- User guide and operational procedure updates

**Key Interactions**
- With Developers: Technical details, API documentation, code comments
- With Product Managers: User guide content and business context
- With QA Lead: Edge case documentation and FAQ updates
- With DevOps Engineer: Runbooks and incident procedures

**Example Workflow**
1. Kickoff: Review feature requirements and acceptance criteria
2. Research: Gather technical details from Developers
3. Draft: Create user guides, API docs, and release notes
4. Review: Get feedback from Developers and Product Managers
5. Publish: Release documentation alongside feature

---

### Stakeholder / Business Sponsor

**Role Summary**
Stakeholders represent business interests, provide strategic context, and make go/no-go decisions. They ensure projects align with organizational goals and priorities.

**Responsibilities**
- Define business goals and success metrics
- Provide budget and resource approval
- Make go/no-go and priority decisions
- Review and approve major milestones
- Communicate project status to leadership
- Remove blockers at the organizational level

**Goals**
- Ensure projects deliver business value
- Maintain strategic alignment across initiatives
- Enable rapid decision-making and resource allocation

**Typical Communication**
- Monthly or milestone-based status updates
- Decision meetings for major decisions
- Executive summaries and business case reviews

**Key Interactions**
- With Project Manager: Status updates and escalations
- With Product Manager: Priority alignment and success metrics
- With Executives: Strategic context and business impact

**Example Workflow**
1. Initiation: Review business case and approve go-ahead
2. Planning: Approve scope, timeline, and resource allocation
3. Execution: Receive regular status updates
4. Decisions: Make priority and trade-off decisions as needed
5. Close: Assess delivery against success metrics

---

## Role Interaction Matrix

| | Developers | Product Mgr | Project Mgr | UX Designer | QA Lead | DevOps | Tech Writer | Stakeholder |
|---|---|---|---|---|---|---|---|---|
| **Developers** | Daily collab | PR reviews | Standups | Design feedback | Test coverage | Build support | Tech docs | N/A |
| **Product Mgr** | Requirements | Alignment | Weekly sync | User research | Acceptance | N/A | Release notes | Priority align |
| **Project Mgr** | Standups | Weekly sync | Daily updates | Timeline impact | QA timeline | Deployment coord | N/A | Status & escalation |
| **UX Designer** | Implementation | Requirements | Timeline impact | Design reviews | User acceptance | N/A | User guide | Approval |
| **QA Lead** | Test coverage | Acceptance | QA timeline | User acceptance | Test strategy | Test env setup | Edge cases | N/A |
| **DevOps** | Build support | N/A | Deployment coord | N/A | Test env | Deployment | Runbooks | N/A |
| **Tech Writer** | Tech details | User guides | Release comms | User guide | FAQ/edge cases | Runbooks | Documentation | N/A |
| **Stakeholder** | N/A | Priority | Escalations | Approval | N/A | N/A | N/A | Strategic align |

---

## How to Use These Personas

### For Project Setup
- Identify which personas are involved in your project
- Clarify roles and responsibilities with the team
- Use the interaction matrix to plan communication touchpoints

### For Collaboration
- Reference typical communication patterns when planning meetings
- Use interaction workflows to understand expected handoffs
- Escalate to the appropriate role based on the issue type

### For Onboarding
- Share relevant persona descriptions with new team members
- Use role descriptions to clarify expectations
- Reference workflows for step-by-step guidance

### For Copilot Spaces
- Use persona prompts to get role-specific guidance
- Reference interactions to understand collaboration patterns
- Use workflows as templates for your project