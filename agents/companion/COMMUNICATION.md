# 💬 Agent Communication Hub

> **How agents talk to each other, share context, and collaborate**

---

## 🎯 What This Enables

| Capability | Description |
|------------|-------------|
| 🔗 Cross-team coordination | Agents share updates automatically |
| ✅ Quality gates | Security, design, performance checks |
| 📊 Context propagation | All agents see relevant decisions |
| 🚀 Faster execution | Parallel work with clear interfaces |

---

## 🏗️ Communication Architecture

```
                    ┌─────────────────┐
                    │   PROJECT.MD    │
                    │  (Source of     │
                    │    Truth)       │
                    └────────┬────────┘
                             │
        ┌────────────────────┼────────────────────┐
        │                    │                    │
        ▼                    ▼                    ▼
┌───────────────┐    ┌───────────────┐    ┌───────────────┐
│  EXECUTIVE    │◄──►│  ENGINEERING  │◄──►│   MARKETING   │
│  CEO, CFO, COO│    │  CTO, Devs    │    │  CMO, Growth  │
└───────┬───────┘    └───────┬───────┘    └───────┬───────┘
        │                    │                    │
        └────────────────────┼────────────────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │   PRODUCT       │
                    │   PM, Designer  │
                    └────────┬────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │   SALES & OPS   │
                    │ Sales, Support  │
                    └─────────────────┘
```

---

## 📨 Message Types

### 1. REQUEST
```markdown
TO: [Agent]
PRIORITY: [High/Medium/Low]

[Subject]

CONTEXT:
- [Background info]
- [Why this matters]

DELIVERABLES:
- [What you need]
- [By when]

DEADLINE: [Date]
```

### 2. APPROVAL
```markdown
FROM: [Agent]
TO: [Approver]
PRIORITY: [High/Medium/Low]

[Subject]: Ready for Approval

STATUS: [Ready]
REVIEWED BY: [List of agents who reviewed]

SUMMARY:
- [What was done]
- [Changes made from last version]

RECOMMENDATION: [Approve/Reject]

APPROVE? [Yes/No/Changes Needed]
```

### 3. INFO
```markdown
FROM: [Agent]
TO: [Relevant agents]
TYPE: FYI

[Subject]

KEY POINTS:
- [Point 1]
- [Point 2]

IMPACT:
- [Who this affects]
- [What they should know]

NO ACTION NEEDED
```

### 4. BLOCKER
```markdown
FROM: [Agent]
TO: [Relevant agents]
PRIORITY: [High/Medium/Low]

🚨 BLOCKER: [Description]

AFFECTED:
- [What is blocked]
- [Who is affected]

REASON:
- [Why it's blocked]
- [What's missing]

NEEDED:
- [Who can unblock]
- [What they need to provide]

SINCE: [Date/Time]
```

### 5. UPDATE
```markdown
FROM: [Agent]
TO: [Team/Stakeholders]
TYPE: Progress Update

SPRINT: [N]
DATE: [Date]

PROGRESS:
- ✅ Completed: [Items]
- 🔄 In Progress: [Items]
- ⏳ Planned: [Items]

BLOCKERS: [If any]
METRICS: [Key numbers]

NEXT: [What's coming up]
```

---

## 🔄 Conversation Flows

### Flow 1: New Feature (Complete)

```
👤 USER: Add worker verification feature

    │
    ▼
📋 PM: Scope the feature
    
    │
    ├──→ 🎨 Designer: Create verification badge UI
    │
    ├──→ 🧠 CTO: Design database schema
    │
    └──→ 🔐 Auth Security: Define verification requirements

    │
    ▼
⚛️ React Dev: Build verification components
🔌 API Dev: Create verification endpoints

    │
    ▼
✅ QA: Test verification flow

    │
    ▼
🚀 DevOps: Deploy to staging

    │
    ▼
👔 CEO: Approve for production

    │
    ▼
🚀 DevOps: Launch to production

    │
    ▼
📣 Marketing: Announce feature
```

### Flow 2: Bug Report (Complete)

```
👤 USER: App crashes when uploading photo

    │
    ▼
📋 PM: Log bug, prioritize

    │
    ▼
🐛 QA: Reproduce and document

    │
    ▼
⚛️ React Dev: Fix frontend validation
🔌 API Dev: Fix backend file handling

    │
    ▼
✅ QA: Verify fix

    │
    ▼
🚀 DevOps: Deploy hotfix

    │
    ▼
📋 PM: Close ticket, update users
```

### Flow 3: Security Check (Complete)

```
🔌 API Dev: Implementing file upload

    │
    ▼
🔐 Auth Security: Security requirements
    
    │
    ├──→ File type validation
    ├──→ Size limits (10MB)
    ├──→ Virus scanning
    └──→ Secure storage

    │
    ▼
🔌 API Dev: Implement security measures

    │
    ▼
🔐 Auth Security: Review implementation

    │
    ▼
✅ APPROVED (or fixes requested)

    │
    ▼
🧠 CTO: Note security patterns for future
```

---

## 🎯 Quality Gates

### Gate 1: Requirements Review
```
CHECKED BY: PM, CTO, Designer
PURPOSE: Ensure feature is well-defined
PASS CRITERIA:
✓ Clear user story
✓ Acceptance criteria defined
✓ Design reference provided
✓ Technical feasibility confirmed
```

### Gate 2: Design Review
```
CHECKED BY: Designer, Frontend Lead
PURPOSE: Ensure UX consistency
PASS CRITERIA:
✓ Follows design system
✓ Mobile responsive
✓ Accessible (WCAG 2.1)
✓ Usability tested
```

### Gate 3: Code Review
```
CHECKED BY: Tech Lead, Peer Developer
PURPOSE: Ensure code quality
PASS CRITERIA:
✓ Tests written
✓ No security issues
✓ Performance considered
✓ Clean code
```

### Gate 4: Security Review
```
CHECKED BY: Auth Security Specialist
PURPOSE: Ensure application security
PASS CRITERIA:
✓ No injection vulnerabilities
✓ Auth properly implemented
✓ Data encrypted
✓ GDPR compliance ready
```

### Gate 5: QA Review
```
CHECKED BY: QA (or PM for MVP)
PURPOSE: Ensure quality
PASS CRITERIA:
✓ All acceptance criteria met
✓ No critical bugs
✓ Edge cases handled
✓ Cross-browser tested
```

### Gate 6: Launch Approval
```
CHECKED BY: CEO, CTO
PURPOSE: Business readiness
PASS CRITERIA:
✓ All gates passed
✓ Rollback plan ready
✓ Monitoring active
✓ Support trained
```

---

## 📋 Agent Meeting Templates

### Daily Standup
```markdown
## Daily Standup - [Date]

### [Agent 1]
- Yesterday: [What done]
- Today: [What's planned]
- Blockers: [If any]

### [Agent 2]
- Yesterday: [What done]
- Today: [What's planned]
- Blockers: [If any]

### Decisions Needed
- [Decision 1]
- [Decision 2]

### Parking Lot
- [Items to discuss later]
```

### Sprint Planning
```markdown
## Sprint Planning - Sprint [N]

### Goal: [Sprint Goal]

### Stories Committed
| Story | Points | Owner |
|-------|--------|-------|
| [S1]  | [N]    | [X]   |
| [S2]  | [N]    | [X]   |

### Capacity
- Team: [N] points
- Committed: [N] points
- Buffer: [N] points

### Dependencies
- [Dep 1]
- [Dep 2]

### Risks
- [Risk 1] → Mitigation
```

### Retrospective
```markdown
## Sprint Retrospective - Sprint [N]

### What Went Well
- [Good thing 1]
- [Good thing 2]

### What Could Improve
- [Improvement 1]
- [Improvement 2]

### Action Items
- [ ] [Action 1] → Owner: [X]
- [ ] [Action 2] → Owner: [X]

### Metrics
- Velocity: [N] points
- Quality: [N] bugs
- Satisfaction: [N]/5
```

---

## 🔔 Notification Matrix

| Event | Notify | Method |
|-------|--------|--------|
| Feature deployed | CEO, PM, Marketing | Message |
| Security issue | CTO, CEO | Urgent message |
| Bug escalated | PM, QA | Message |
| Design approved | PM, Dev | Message |
| New user feedback | PM, CEO | Daily digest |
| Milestone reached | All agents | Announcement |

---

## ✅ Checklist: Agent Communication

Before finishing any task, agent should:

- [ ] Update relevant agents on progress
- [ ] Flag blockers immediately
- [ ] Request reviews from quality gates
- [ ] Document decisions in PROJECT.md
- [ ] Handoff cleanly to next agent

---

*Good communication is the difference between a team and a group of individuals working on the same project.*
