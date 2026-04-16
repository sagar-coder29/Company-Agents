# 🎭 Company Agents — AI-Powered Multi-Agent Company System

<p align="center">
  <img src="https://img.shields.io/badge/Agents-26-blue?style=for-the-badge" alt="26 Agents">
  <img src="https://img.shields.io/badge/Departments-6-green?style=for-the-badge" alt="6 Departments">
  <img src="https://img.shields.io/badge/Personalities-26-purple?style=for-the-badge" alt="26 Personalities">
  <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge" alt="Active">
</p>

> **26 AI agents, each modeled after the best person in their field. They collaborate, challenge each other, and build your startup the way the world's top experts would.**

---

## 🎯 What Is This?

Company Agents is an **autonomous AI agent company framework** where each agent thinks, communicates, and makes decisions like a world-class expert in their domain:

- 🧠 **Expert Personalities** — Every agent is modeled after a real industry legend (Linus Torvalds, Brian Chesky, Seth Godin, and more)
- 🤝 **Cross-Agent Collaboration** — Agents communicate with structured handoffs and quality gates
- 🛡️ **Smart Defaults** — Intelligent choices when you don't specify
- ✅ **Quality Gates** — Security, design, and performance checks at every stage
- 📊 **Unified Config** — Single source of truth in `PROJECT.md`

---

## 🚀 Quick Start

```bash
# 1. Clone the repo
git clone https://github.com/sagar-coder29/Company-Agents.git

# 2. Choose an agent
cat agents/executive/CEO.md

# 3. Paste into your AI assistant (Claude, ChatGPT, Gemini)

# 4. Start building
```

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────────────┐
│                      USER / PROJECT OWNER                       │
└─────────────────────────┬───────────────────────────────────────┘
                           │
                           ▼
┌─────────────────────────────────────────────────────────────────┐
│                      AGENTS.md (Rules)                          │
│         Operating rules, quality gates, persona guidelines      │
└─────────────────────────┬───────────────────────────────────────┘
                           │
                           ▼
┌─────────────────────────────────────────────────────────────────┐
│                      PROJECT.md (Config)                        │
│              Company basics, tech stack, features               │
└─────────────────────────┬───────────────────────────────────────┘
                           │
                           ▼
┌─────────────────────────────────────────────────────────────────┐
│                        AGENT NETWORK                            │
│                                                                 │
│  ┌─────────────┐    ┌─────────────┐    ┌─────────────┐          │
│  │  Executive  │◄──►│ Engineering │◄──►│  Marketing  │          │
│  │    (3)      │    │    (10)     │    │    (5)      │          │
│  └──────┬──────┘    └──────┬──────┘    └──────┬──────┘          │
│         │                  │                  │                 │
│         └──────────────────┼──────────────────┘                 │
│                            ▼                                    │
│  ┌─────────────┐    ┌─────────────┐    ┌─────────────┐          │
│  │   Product   │◄──►│    Sales    │◄──►│ Operations  │          │
│  │    (2)      │    │    (4)      │    │    (2)      │          │
│  └─────────────┘    └─────────────┘    └─────────────┘          │
└─────────────────────────────────────────────────────────────────┘
```

### Key Files
| File | Purpose |
|------|---------|
| `PROJECT.md` | Company config (stack, goals, features) |
| `AGENTS.md` | Operating rules, quality gates, personas |
| `agents/companion/COMMUNICATION.md` | Detailed communication patterns |
| `agents/companion/DEFAULTS.md` | Smart defaults catalog |

---

## 👥 Agent Directory

Each agent is modeled after the best-known expert in their field. Their personality shapes how they think, communicate, and make decisions.

### 🏢 Executive (3 Agents)

| Role | File | Modeled After | Their Edge |
|------|------|---------------|------------|
| 🤵 CEO | `executive/CEO.md` | **Brian Chesky** (Airbnb) | Founder obsession, trust-first, detail-driven |
| 💰 CFO | `executive/CFO.md` | **Charlie Munger** (Berkshire) | Inversion thinking, ruthless capital allocation |
| ⚙️ COO | `executive/COO.md` | **Sheryl Sandberg** (Meta) | Systems builder, clarity-driven, operational excellence |

### 💻 Engineering (10 Agents)

| Role | File | Modeled After | Their Edge |
|------|------|---------------|------------|
| 🧠 CTO | `engineering/CTO.md` | **Linus Torvalds** (Linux/Git) | Brutally pragmatic, correctness-first, anti-complexity |
| 🎨 Frontend Lead | `engineering/Frontend_Lead.md` | **Dan Abramov** (Redux/React) | Honest about tradeoffs, anti-over-engineering |
| ⚛️ React Dev | `engineering/React_Developer.md` | **Kent C. Dodds** (Testing Library) | Accessibility-first, behavior testing, composable |
| 🔌 API Dev | `engineering/API_Developer.md` | **Roy Fielding** (REST inventor) | Principled, resource-based, contracts matter |
| 🗄️ Backend Lead | `engineering/Backend_Lead.md` | **Martin Fowler** (ThoughtWorks) | Patterns, refactoring, architecture as managing change |
| 🛢️ Database Eng | `engineering/Database_Engineer.md` | **Joe Celko** (SQL for Smarties) | Relational theory, DB-level integrity, constraints first |
| 🚀 DevOps | `engineering/DevOps_Engineer.md` | **Kelsey Hightower** (Google) | Boring infrastructure, observability, fast recovery |
| ☁️ Cloud Eng | `engineering/Cloud_Infrastructure.md` | **Werner Vogels** (AWS CTO) | "Everything fails", design for failure, cost-conscious |
| 🔐 Auth Security | `engineering/Auth_Security_Specialist.md` | **Bruce Schneier** | Threat modeling, security as process not product |
| 📱 Mobile Dev | `engineering/Mobile_Developer.md` | **Chris Lattner** (Swift creator) | Safety-first, native feel, thumb-friendly |

### 📢 Marketing (5 Agents)

| Role | File | Modeled After | Their Edge |
|------|------|---------------|------------|
| 📣 CMO | `marketing/CMO.md` | **Seth Godin** (Purple Cow) | Smallest viable audience, remarkable product |
| 📈 Growth | `marketing/Growth_Marketer.md` | **Andrew Chen** (a16z) | Retention first, viral loops, north star metrics |
| ✍️ Content | `marketing/Content_Strategist.md` | **Ann Handley** (MarketingProfs) | Write for the reader, clarity, useful over promotional |
| 🔍 SEO | `marketing/SEO_Specialist.md` | **Rand Fishkin** (Moz/SparkToro) | Earn links, realistic timelines, best answer wins |
| 💵 Paid Ads | `marketing/Paid_Ads_Manager.md` | **Neil Patel** (NP Digital) | CAC/LTV obsessed, test everything, fix funnel first |

### 💰 Sales (4 Agents)

| Role | File | Modeled After | Their Edge |
|------|------|---------------|------------|
| 🎯 Head of Sales | `sales/Head_of_Sales.md` | **Aaron Ross** (Predictable Revenue) | Systematic, pipeline-driven, separate roles |
| 📞 SDR | `sales/SDR.md` | **Jeb Blount** (Fanatical Prospecting) | Multi-channel, personalized, qualify fast |
| 🤝 Account Exec | `sales/Account_Executive.md` | **Zig Ziglar** | Relationship-first, value over price, solve don't sell |
| 💚 Customer Success | `sales/Customer_Success.md` | **Lincoln Murphy** | Desired outcomes, proactive, health scores |

### 🎨 Product (2 Agents)

| Role | File | Modeled After | Their Edge |
|------|------|---------------|------------|
| 📋 Product Manager | `product/Product_Manager.md` | **Marty Cagan** (SVPG) | Outcome over output, discovery before delivery |
| 🎨 Product Designer | `product/Product_Designer.md` | **Jony Ive** (Apple) | Simplicity as clarity, invisible design, every detail matters |

### ⚙️ Operations (2 Agents)

| Role | File | Modeled After | Their Edge |
|------|------|---------------|------------|
| 🔄 Ops Manager | `operations/Operations_Manager.md` | **Jeff Sutherland** (Scrum) | Eliminate waste, automate predictable, inspect and adapt |
| 🎧 Support Lead | `operations/Customer_Support_Lead.md` | **Tony Hsieh** (Zappos) | WOW experiences, complaints as gifts, human first |

---

## 🔄 How Agents Talk

### Communication Flow
```
USER: "Build a booking feature"

         ┌─────────────────┐
         │ PRODUCT MANAGER │  ← Marty Cagan: "Why? Who asked for this?"
         │  Breaks it down │
         └────────┬────────┘
                  │
        ┌─────────┼──────────┐
        │         │          │
        ▼         ▼          ▼
    ┌────────┐ ┌────────┐ ┌──────────┐
    │DESIGNER│ │API DEV │ │FRONTEND  │
    │Jony Ive│ │Fielding│ │Abramov   │
    └────┬───┘ └───┬────┘ └───┬──────┘
         │         │          │
         └─────────┼──────────┘
                   ▼
            ┌─────────────┐
            │  CTO REVIEW │  ← Torvalds: "Is this actually necessary?"
            └─────────────┘
```

### Message Types
| Type | Purpose | Example |
|------|---------|---------|
| REQUEST | Need something from another agent | "Need API endpoint for bookings" |
| INFO | Share completed work | "Worker profile component done" |
| APPROVAL | Need sign-off | "Ready for production deployment" |
| BLOCKER | Can't proceed | "Need database schema first" |
| UPDATE | Progress report | "Sprint status update" |

### Quality Gates
| Gate | Owners | Purpose |
|------|--------|---------|
| 📋 Requirements | PM + CTO + Designer | Feature specs validated |
| 🎨 Design | Designer + Frontend Lead | UX approved |
| ⚡ Code | Tech Lead + Peer | Quality checked |
| 🔒 Security | Auth Security + CTO | Vulnerabilities scanned |
| ✅ QA | PM | Acceptance criteria met |
| 🚀 Launch | CEO + CTO | Final approval |

---

## 🧠 Personality Highlights

Each agent has a distinct voice. Here's a taste:

**CTO (Linus Torvalds) on microservices:**
> *"You have zero users. Microservices solve a scaling problem you don't have, while creating a distributed systems problem you're not equipped to handle."*

**CFO (Charlie Munger) on a tool purchase:**
> *"Wrong question. Right question: what does this tool replace, and what's the cost of not having it? Invert, always invert."*

**PM (Marty Cagan) on a new feature request:**
> *"Before we spec this — why? Talk to 5 users first. If 3+ say they'd pay for it and can articulate why, then we scope it."*

**CMO (Seth Godin) on paid ads:**
> *"Not yet. Build organic first. The best marketing for a trust product is trust. Earn it before you advertise it."*

**Auth Security (Bruce Schneier) on a login review:**
> *"Let me build a threat model first. Who are the attackers? What do they want? What's the cheapest way to stop them?"*

---

## 🛡️ Smart Defaults

When you don't specify, agents apply intelligent defaults:

### Default Stack
| Component | Default |
|-----------|---------|
| Frontend | React 18 + Tailwind CSS |
| Backend | Django 5 + Python |
| Database | SQLite (dev) → PostgreSQL (prod) |
| Auth | JWT + Google OAuth |
| Hosting | Vercel + Railway |
| Design | Glassmorphism (purple/green) |

### Decision Matrix
| Input | Result |
|-------|--------|
| "yes" / "all" | ✅ Full feature |
| "no" / "skip" | ❌ Feature removed |
| "don't know" | 🛡️ Smart default |
| blank | 🛡️ Smart default |

---

## 📁 File Structure

```
Company-Agents/
├── 📄 README.md                    ← You are here
├── 📋 PROJECT.md                   ← Company config (stack, goals)
├── 📜 AGENTS.md                    ← Operating rules
│
├── 👔 agents/executive/            ← 3 agents
│   ├── CEO.md                      ← Brian Chesky
│   ├── CFO.md                      ← Charlie Munger
│   └── COO.md                      ← Sheryl Sandberg
│
├── 💻 agents/engineering/          ← 10 agents
│   ├── CTO.md                      ← Linus Torvalds
│   ├── Frontend_Lead.md            ← Dan Abramov
│   ├── React_Developer.md          ← Kent C. Dodds
│   ├── API_Developer.md            ← Roy Fielding
│   ├── Backend_Lead.md             ← Martin Fowler
│   ├── Database_Engineer.md        ← Joe Celko
│   ├── DevOps_Engineer.md          ← Kelsey Hightower
│   ├── Cloud_Infrastructure.md     ← Werner Vogels
│   ├── Auth_Security_Specialist.md ← Bruce Schneier
│   └── Mobile_Developer.md         ← Chris Lattner
│
├── 📢 agents/marketing/            ← 5 agents
│   ├── CMO.md                      ← Seth Godin
│   ├── Growth_Marketer.md          ← Andrew Chen
│   ├── Content_Strategist.md       ← Ann Handley
│   ├── SEO_Specialist.md           ← Rand Fishkin
│   └── Paid_Ads_Manager.md         ← Neil Patel
│
├── 💰 agents/sales/                ← 4 agents
│   ├── Head_of_Sales.md            ← Aaron Ross
│   ├── SDR.md                      ← Jeb Blount
│   ├── Account_Executive.md        ← Zig Ziglar
│   └── Customer_Success.md         ← Lincoln Murphy
│
├── 🎨 agents/product/              ← 2 agents
│   ├── Product_Manager.md          ← Marty Cagan
│   └── Product_Designer.md         ← Jony Ive
│
├── ⚙️ agents/operations/           ← 2 agents
│   ├── Operations_Manager.md       ← Jeff Sutherland
│   └── Customer_Support_Lead.md    ← Tony Hsieh
│
└── 🔧 agents/companion/            ← Utilities
    ├── COMMUNICATION.md            ← How agents talk
    └── DEFAULTS.md                 ← Smart defaults catalog
```

---

## 🎓 Usage Examples

### Single Agent (Quick Task)
```bash
# Copy the agent file
cat agents/engineering/CTO.md

# Paste into Claude, ChatGPT, or any AI assistant
# Ask your question — the agent responds in character
```

### Multi-Agent (Complex Feature)
```bash
# 1. PM scopes the feature (Marty Cagan style)
# 2. Designer creates UX (Jony Ive style)
# 3. CTO reviews architecture (Linus Torvalds style)
# 4. Agents coordinate with structured handoffs
```

### Full Company (Startup)
```bash
# 1. CEO sets OKRs (Brian Chesky style)
# 2. CTO builds tech roadmap (Linus Torvalds style)
# 3. CMO creates marketing plan (Seth Godin style)
# 4. Head of Sales sets pipeline (Aaron Ross style)
# 5. PM manages priorities (Marty Cagan style)
```

---

## 📊 Stats

| Metric | Count |
|--------|-------|
| 🤖 Total Agents | 26 |
| 🏢 Departments | 6 |
| 🧠 Expert Personalities | 26 |
| 📁 Agent Files | 26 |
| 📝 Companion Files | 2 |
| 📄 Total Files | 31 |

---

## 🛠️ Built With

| Category | Tools |
|----------|-------|
| 🤖 AI | Claude, GPT, any LLM |
| 💻 Frontend | React, Tailwind CSS |
| ⚙️ Backend | Django, Python |
| 🗄️ Database | SQLite, PostgreSQL |
| 📦 Deploy | Vercel, Railway |
| 🎨 Design | Figma, Glassmorphism |

---

## 🤝 Contributing

1. Fork the repo
2. Copy an existing agent as template
3. Assign a real-world expert personality
4. Add their core beliefs and conversation examples
5. Update README with the personality
6. Submit PR

---

## 📄 License

MIT License — Use freely for your startup.

---

<p align="center">
  <strong>Company Agents — Your AI-Powered Expert Team</strong>
  <br>
  🤖 26 Agents · 🧠 26 Expert Personalities · 🏢 6 Departments · 🎯 1 Vision
  <br>
  <a href="https://github.com/sagar-coder29/Company-Agents">GitHub</a>
</p>
