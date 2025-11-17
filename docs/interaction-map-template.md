# Interaction Map Template

## Purpose
Visualize cross-role workflows, dependencies, and communication paths to clarify how different roles collaborate throughout the project lifecycle. This template helps teams understand the flow of work and information across roles.

## When to Use
- Project kickoff to establish collaboration patterns
- Onboarding new team members to show their place in the workflow
- Process improvement initiatives to identify bottlenecks
- Cross-functional team formation
- Resolving unclear handoffs or communication breakdowns

---

## How to Use This Template

1. **Identify Roles**: List all roles involved in your project (from [Roles and Personas](./octoacme-roles-and-personas.md))
2. **Map Workflows**: For each major workflow, document how work flows between roles
3. **Define Touchpoints**: Specify when and how roles interact
4. **Clarify Handoffs**: Make explicit what is delivered and when
5. **Review Regularly**: Update as team or process changes

---

## Visual Interaction Map

Use this text-based representation or create a visual diagram using tools like Miro, Lucidchart, or draw.io.

```
Legend:
→  : Delivers work/information to
↔  : Collaborates bidirectionally with
⊙  : Reviews/Approves
◈  : Facilitates/Coordinates
```

### Example: Feature Development Workflow

```
Product Manager → Business Analyst → UX Designer → Developers → Technical Writer
        ↓              ↓                  ↓              ↓              ↓
    (Defines       (Refines        (Designs       (Implements    (Documents
     vision)      requirements)   interface)      feature)       feature)
        ↓              ↓                  ↓              ↓              ↓
        └──────────────┴──────────────────┴──────────────┴──────────────┘
                              ↑
                        Scrum Master (Facilitates entire flow)
                              ↑
                        Project Manager (Tracks progress, manages risks)
```

---

## Interaction Matrix

For each workflow phase, document which roles interact and how:

### Planning Phase

| From Role | To Role | Interaction Type | Deliverable/Output | Frequency |
|-----------|---------|------------------|-------------------|-----------|
| Product Manager | Business Analyst | Collaboration | Problem statement, goals | Weekly |
| Business Analyst | Product Manager | Review | User stories, requirements | Per story |
| Business Analyst | UX Designer | Collaboration | User flows, process maps | As needed |
| Product Manager | Project Manager | Information sharing | Priority changes, scope | Weekly |
| Scrum Master | All Roles | Facilitation | Sprint planning meeting | Per sprint |
| Project Manager | All Roles | Coordination | Project plan, timeline | Kickoff + updates |

### Design Phase

| From Role | To Role | Interaction Type | Deliverable/Output | Frequency |
|-----------|---------|------------------|-------------------|-----------|
| UX Designer | Product Manager | Review/Approval | Wireframes, prototypes | Per feature |
| UX Designer | Business Analyst | Validation | Design against requirements | Before handoff |
| UX Designer | Developers | Handoff | Design specs, assets | Per feature |
| UX Designer | Technical Writer | Collaboration | UI copy, terminology | As needed |
| Scrum Master | UX Designer | Coaching | Definition of done for design | Ongoing |

### Development Phase

| From Role | To Role | Interaction Type | Deliverable/Output | Frequency |
|-----------|---------|------------------|-------------------|-----------|
| Developers | Product Manager | Clarification | Questions on requirements | As needed |
| Developers | UX Designer | Clarification | Implementation questions | As needed |
| Developers | Business Analyst | Validation | Acceptance criteria review | Per story |
| Developers | Developers | Collaboration | Code reviews, pair programming | Daily |
| Developers | Technical Writer | Information sharing | Feature details, API changes | Per feature |
| Scrum Master | Developers | Support | Impediment removal | Daily standup |
| Project Manager | Developers | Monitoring | Status updates, risks | Weekly |

### Testing & Release Phase

| From Role | To Role | Interaction Type | Deliverable/Output | Frequency |
|-----------|---------|------------------|-------------------|-----------|
| Business Analyst | Developers | Validation | Test scenarios, edge cases | Before testing |
| Product Manager | All Roles | Approval | Go/no-go decision | Per release |
| Technical Writer | Product Manager | Review | Release notes, documentation | Per release |
| Technical Writer | Developers | Validation | Technical accuracy review | Per doc |
| Project Manager | All Roles | Coordination | Release checklist, comms plan | Per release |
| Scrum Master | All Roles | Facilitation | Sprint review, retrospective | Per sprint |

---

## Communication Channels by Interaction Type

### Synchronous (Real-time)
- **Daily Standups**: All development team + Scrum Master
- **Sprint Planning**: Product Manager, Business Analyst, UX Designer, Developers, Scrum Master
- **Design Reviews**: UX Designer, Product Manager, Developers, Business Analyst
- **Code Reviews**: Developers (via PR comments or pair programming)
- **Ad-hoc Problem Solving**: Any relevant roles as needed

### Asynchronous (Documentation-based)
- **Requirements Documentation**: Business Analyst → Developers
- **Design Specifications**: UX Designer → Developers
- **Technical Documentation**: Technical Writer → All roles
- **Status Reports**: Project Manager → Stakeholders
- **User Stories**: Product Manager/Business Analyst → All team
- **Release Notes**: Technical Writer → Product Manager → Stakeholders

### Review & Approval Workflows
- **Design Approval**: UX Designer → Product Manager (approval) → Developers
- **Requirements Sign-off**: Business Analyst → Product Manager → Stakeholders
- **Code Review**: Developer → Developer(s) (approval) → Merge
- **Documentation Review**: Technical Writer → Subject Matter Experts → Publication
- **Release Approval**: Project Manager + Product Manager → Go/No-Go

---

## Key Handoff Points

Document critical handoffs where work transitions between roles:

### Handoff: Requirements to Design
- **From**: Business Analyst
- **To**: UX Designer
- **Trigger**: User stories accepted and prioritized
- **Deliverable**: User stories with acceptance criteria, process flows
- **Validation**: Design kickoff meeting
- **Risks**: Unclear requirements, missing edge cases

### Handoff: Design to Development
- **From**: UX Designer
- **To**: Developers
- **Trigger**: Design approved by Product Manager
- **Deliverable**: Design specs, mockups, assets, interaction patterns
- **Validation**: Design handoff meeting, developer Q&A
- **Risks**: Implementation feasibility, missing states or error cases

### Handoff: Development to Documentation
- **From**: Developers
- **To**: Technical Writer
- **Trigger**: Feature complete and tested
- **Deliverable**: Feature description, API changes, UI flows
- **Validation**: Documentation review with developer
- **Risks**: Late notification, incomplete technical details

### Handoff: Feature Complete to Release
- **From**: Developers, Technical Writer
- **To**: Product Manager, Project Manager
- **Trigger**: All acceptance criteria met, docs complete
- **Deliverable**: Tested feature, release notes, user docs
- **Validation**: Release readiness review
- **Risks**: Undiscovered bugs, incomplete documentation

---

## Escalation Paths

When issues arise, follow these escalation patterns:

```
Blocker or Issue Identified
        ↓
1. Raise in Daily Standup (for team-level issues)
        ↓
2. Scrum Master attempts resolution
        ↓
3. If unresolved → Project Manager (for schedule/resource issues)
                 → Product Manager (for scope/priority issues)
                 → Technical Lead (for technical decisions)
        ↓
4. If still unresolved → Steering Committee or Leadership
```

---

## Customization Guide

Adapt this template for your team:

1. **Add/Remove Roles**: Modify based on your team composition
2. **Define Your Workflows**: Replace example workflows with your actual processes
3. **Specify Tools**: Add specific tools used for each interaction (Slack channels, boards, etc.)
4. **Add Timings**: Document expected response times or SLAs for each interaction
5. **Include Examples**: Add real examples from your projects for clarity

---

## Tips for Effective Interaction Mapping

**Do:**
- Keep it simple—focus on the most important workflows first
- Make it visual when possible—diagrams are easier to understand
- Review and update regularly—teams and processes evolve
- Use it in onboarding—new team members benefit most
- Post it somewhere visible—wiki, project board, team space

**Don't:**
- Document every possible interaction—focus on critical paths
- Make it too rigid—allow flexibility for team collaboration
- Create it in isolation—involve all roles in the mapping exercise
- Let it get stale—outdated maps cause confusion
- Use it as a control mechanism—it's for clarity, not micromanagement

---

## Related Resources

- [Roles and Personas](./octoacme-roles-and-personas.md) - Detailed role descriptions
- [Role Alignment Checklist](./role-alignment-checklist.md) - Ensure role clarity during onboarding
- [Project Management Overview](./octoacme-project-management-overview.md) - Overall project approach
- [Communication Plan Template](./octoacme-risks-and-communication.md) - Detailed communication strategies
