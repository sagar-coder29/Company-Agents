# 🎭 Company Agents - AI-Powered Multi-Agent Company System

<p align="center">
  <img src="https://img.shields.io/badge/Agents-26-blue?style=for-the-badge" alt="26 Agents">
  <img src="https://img.shields.io/badge/Departments-6-green?style=for-the-badge" alt="6 Departments">
  <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge" alt="Active">
</p>

> **Your complete AI-powered company system. 26 agents work together, talk to each other, and build your startup automatically.**

---

## 🎯 What Is This?

Company Agents is an **autonomous AI agent company framework** where specialized AI agents:
- 🤝 **Collaborate** - Agents communicate and share context
- 🛡️ **Smart Defaults** - Intelligent choices when you don't know
- ✅ **Quality Gates** - Security, design, and performance checks
- 📊 **Unified Config** - Single source of truth for all agents

---

## 🚀 Quick Start

```bash
# 1. Clone the repo
git clone https://github.com/sagar-coder29/Company-Agents.git

# 2. Choose an agent
cat agents/executive/CEO.md

# 3. Paste into your AI assistant

# 4. Start building!
```

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────────────┐
│                      USER / PROJECT OWNER                         │
└─────────────────────────┬───────────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────────────┐
│                      PROJECT.md (Setup)                          │
│              Company basics, tech stack, features                 │
└─────────────────────────┬───────────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────────────┐
│                      AGENT NETWORK                                │
│                                                                  │
│  ┌─────────────┐    ┌─────────────┐    ┌─────────────┐        │
│  │  Executive  │◄──►│ Engineering │◄──►│  Marketing   │        │
│  │   (3)      │    │   (10)      │    │   (5)       │        │
│  └──────┬──────┘    └──────┬──────┘    └──────┬──────┘        │
│         │                   │                   │                │
│         └───────────────────┼───────────────────┘                │
│                             ▼                                    │
│  ┌─────────────┐    ┌─────────────┐    ┌─────────────┐        │
│  │   Product   │◄──►│   Sales     │◄──►│  Operations │        │
│  │   (2)      │    │   (4)       │    │   (2)       │        │
│  └─────────────┘    └─────────────┘    └─────────────┘        │
└─────────────────────────────────────────────────────────────────┘
```

---

## 👥 Agent Directory

### 🏢 Executive (3 Agents)
| Emoji | Role | File | Responsibility |
|-------|------|------|----------------|
| 🤵 | CEO | `executive/CEO.md` | Vision, strategy, OKRs |
| 💰 | CFO | `executive/CFO.md` | Finance, burn rate |
| ⚙️ | COO | `executive/COO.md` | Operations, scaling |

### 💻 Engineering (10 Agents)
| Emoji | Role | File | Responsibility |
|-------|------|------|----------------|
| 🧠 | CTO | `engineering/CTO.md` | Architecture, tech decisions |
| 🎨 | Frontend Lead | `engineering/Frontend_Lead.md` | UI architecture |
| ⚛️ | React Dev | `engineering/React_Developer.md` | React implementation |
| 🔌 | API Dev | `engineering/API_Developer.md` | REST API, endpoints |
| 🗄️ | Backend Lead | `engineering/Backend_Lead.md` | Server, database |
| 🛢️ | Database Eng | `engineering/Database_Engineer.md` | Schema, optimization |
| 🚀 | DevOps | `engineering/DevOps_Engineer.md` | CI/CD, deployment |
| ☁️ | Cloud Eng | `engineering/Cloud_Infrastructure.md` | Cloud setup |
| 🔐 | Auth Security | `engineering/Auth_Security_Specialist.md` | Security |
| 📱 | Mobile Dev | `engineering/Mobile_Developer.md` | iOS/Android |

### 📢 Marketing (5 Agents)
| Emoji | Role | File | Responsibility |
|-------|------|------|----------------|
| 📣 | CMO | `marketing/CMO.md` | Strategy, brand |
| 📈 | Growth | `marketing/Growth_Marketer.md` | Acquisition, viral |
| ✍️ | Content | `marketing/Content_Strategist.md` | Blog, SEO, social |
| 🔍 | SEO | `marketing/SEO_Specialist.md` | Search optimization |
| 💵 | Paid Ads | `marketing/Paid_Ads_Manager.md` | PPC campaigns |

### 💰 Sales (4 Agents)
| Emoji | Role | File | Responsibility |
|-------|------|------|----------------|
| 🎯 | Head of Sales | `sales/Head_of_Sales.md` | Pipeline, targets |
| 📞 | SDR | `sales/SDR.md` | Prospecting |
| 🤝 | Account Exec | `sales/Account_Executive.md` | Closing deals |
| 💚 | Customer Success | `sales/Customer_Success.md` | Retention |

### 🎨 Product (2 Agents)
| Emoji | Role | File | Responsibility |
|-------|------|------|----------------|
| 📋 | Product Manager | `product/Product_Manager.md` | Roadmap, priorities |
| 🎨 | Product Designer | `product/Product_Designer.md` | UX/UI design |

### ⚙️ Operations (2 Agents)
| Emoji | Role | File | Responsibility |
|-------|------|------|----------------|
| 🔄 | Ops Manager | `operations/Operations_Manager.md` | Automation |
| 🎧 | Support Lead | `operations/Customer_Support_Lead.md` | Helpdesk |

---

## 🔄 How Agents Talk

### Communication Flow
```
USER: "Build a booking feature"

         ┌─────────────────┐
         │  PRODUCT MANAGER │
         │  Breaks it down  │
         └────────┬────────┘
                  │
        ┌────────┼────────┐
        │        │        │
        ▼        ▼        ▼
    ┌────────┐ ┌────────┐ ┌────────┐
    │ DESIGN │ │  API   │ │FRONTEND│
    │ Create │ │ Design │ │ Build  │
    │   UI   │ │Endpoints│ │Components│
    └────┬───┘ └───┬────┘ └───┬────┘
         │         │         │
         └─────────┼─────────┘
                   ▼
            ┌─────────────┐
            │     QA      │
            │   Test      │
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
| Gate | Agents | Purpose |
|------|--------|---------|
| 📋 Requirements | PM, CTO, Designer | Feature specs |
| 🎨 Design | Designer, Frontend | UX approval |
| ⚡ Code | Tech Lead, Peer | Quality check |
| 🔒 Security | Auth Security | Vulnerability scan |
| ✅ QA | QA, PM | Testing validation |
| 🚀 Launch | CEO, CTO | Final approval |

---

## 🛡️ Smart Defaults

When you **don't know** or say **"no"**, agents apply intelligent defaults:

### Default Stack
| Component | Default |
|-----------|---------|
| Frontend | React + Tailwind CSS |
| Backend | Django + Python |
| Database | SQLite → PostgreSQL |
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

### Example Conversations
```
USER: Build the backend (I don't know tech)
AGENT: ✅ Django + Python
       ✅ SQLite dev, PostgreSQL prod
       ✅ REST API with JWT
       ✅ Standard security

USER: Skip the review system
AGENT: ❌ Reviews disabled

USER: We want everything
AGENT: ✅ Full auth (email + social + MFA)
       ✅ All features included
       ✅ Premium design
```

---

## 📁 File Structure

```
Company-Agents/
├── 📄 README.md                    ← You are here
├── 📋 PROJECT.md                   ← Company setup config
│
├── 👔 executive/                  ← 3 agents
│   ├── CEO.md
│   ├── CFO.md
│   └── COO.md
│
├── 💻 engineering/                ← 10 agents
│   ├── CTO.md
│   ├── Frontend_Lead.md
│   ├── React_Developer.md
│   ├── API_Developer.md
│   ├── Backend_Lead.md
│   ├── Database_Engineer.md
│   ├── DevOps_Engineer.md
│   ├── Cloud_Infrastructure.md
│   ├── Auth_Security_Specialist.md
│   └── Mobile_Developer.md
│
├── 📢 marketing/                ← 5 agents
│   ├── CMO.md
│   ├── Growth_Marketer.md
│   ├── Content_Strategist.md
│   ├── SEO_Specialist.md
│   └── Paid_Ads_Manager.md
│
├── 💰 sales/                      ← 4 agents
│   ├── Head_of_Sales.md
│   ├── SDR.md
│   ├── Account_Executive.md
│   └── Customer_Success.md
│
├── 🎨 product/                   ← 2 agents
│   ├── Product_Manager.md
│   └── Product_Designer.md
│
├── ⚙️ operations/               ← 2 agents
│   ├── Operations_Manager.md
│   └── Customer_Support_Lead.md
│
└── 🔧 companion/                ← Utilities
    ├── COMMUNICATION.md          ← How agents talk
    └── DEFAULTS.md              ← Smart defaults
```

---

## 🎓 Usage Examples

### Single Agent (Quick Task)
```bash
# Copy the agent file
cat agents/engineering/React_Developer.md

# Paste into Claude, ChatGPT, or any AI assistant
# Ask your question
```

### Multi-Agent (Complex Project)
```bash
# 1. Start with CEO for vision
# 2. Add CTO for architecture
# 3. Bring in specialists
# 4. Agents coordinate automatically
```

### Full Company (Startup)
```bash
# 1. CEO sets OKRs
# 2. CTO builds tech roadmap
# 3. CMO creates marketing plan
# 4. Head of Sales sets pipeline
# 5. PM manages priorities
# 6. Weekly syncs between agents
```

---

## 📊 Stats

| Metric | Count |
|--------|-------|
| 🤖 Total Agents | 26 |
| 🏢 Departments | 6 |
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
3. Customize for your role
4. Update README if adding agents
5. Submit PR

---

## 📄 License

MIT License - Use freely for your startup!

---

<p align="center">
  <strong>Company Agents - Your AI-Powered Company</strong>
  <br>
  🤖 26 Agents | 🏢 6 Departments | 🎯 1 Vision
  <br>
  <a href="https://github.com/sagar-coder29/Company-Agents">GitHub</a>
</p>
