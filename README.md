# 👔 HireMate Multi-Agent System

> 🤖 **26 AI Agents | 6 Departments | 1 Vision**

Your complete AI-powered company system where agents collaborate, talk to each other, and build your startup automatically.

---

## 🎯 What Is This?

HireMate is an **autonomous AI agent company** with 26 specialized agents that:
- 🤝 **Collaborate** - Agents talk to each other
- 🛡️ **Apply Smart Defaults** - When you don't know, they decide
- ✅ **Quality Gates** - Security, design, performance checks
- 📋 **Share Context** - All agents see the same project data

---

## 🏗️ Quick Start

### 1️⃣ Choose Your Agent
```bash
# Copy any agent file and paste into your AI assistant

agents/executive/CEO.md        # Vision & strategy
agents/engineering/CTO.md       # Tech decisions
agents/product/Product_Manager.md # Features
agents/marketing/CMO.md        # Marketing
```

### 2️⃣ Answer (or Skip) Setup Questions
```
Company Name: [Your Name]
Tech Stack: [Your choice or default]

# If you say "don't know" → Smart defaults applied
# If you say "yes/all" → Full features included
# If you say "no" → Minimal version
```

### 3️⃣ Start Building
```
You: Build our auth system
Agent: Applying defaults... (JWT + Google OAuth)
      Notifying other agents...
```

---

## 👥 Agent Directory

### 🏢 Executive (3)
| Emoji | Role | Does |
|--------|------|-------|
| 🤵 | CEO | Vision, strategy, OKRs |
| 💰 | CFO | Finance, burn rate |
| ⚙️ | COO | Operations, scaling |

### 💻 Engineering (10)
| Emoji | Role | Does |
|--------|------|-------|
| 🧠 | CTO | Architecture, tech stack |
| 🎨 | Frontend Lead | UI, components |
| ⚛️ | React Dev | React implementation |
| 🔌 | API Dev | REST API, endpoints |
| 🗄️ | Backend Lead | Server, database |
| 🛢️ | Database Eng | Schema, optimization |
| 🚀 | DevOps | CI/CD, deployment |
| ☁️ | Cloud Eng | AWS/GCP setup |
| 🔐 | Auth Security | Security, compliance |
| 📱 | Mobile Dev | iOS/Android |

### 📢 Marketing (5)
| Emoji | Role | Does |
|--------|------|-------|
| 📣 | CMO | Strategy, brand |
| 📈 | Growth | Acquisition, viral |
| ✍️ | Content | Blog, SEO, social |
| 🔍 | SEO | Search rankings |
| 💵 | Paid Ads | PPC campaigns |

### 💰 Sales (4)
| Emoji | Role | Does |
|--------|------|-------|
| 🎯 | Head of Sales | Pipeline, targets |
| 📞 | SDR | Prospecting |
| 🤝 | Account Exec | Closing deals |
| 💚 | Customer Success | Retention |

### 🎨 Product (2)
| Emoji | Role | Does |
|--------|------|-------|
| 📋 | Product Manager | Roadmap, priorities |
| 🎨 | Product Designer | UX/UI |

### ⚙️ Operations (2)
| Emoji | Role | Does |
|--------|------|-------|
| 🔄 | Ops Manager | Efficiency, automation |
| 🎧 | Support Lead | Helpdesk, SLAs |

---

## 🔄 How Agents Talk

```
👤 USER: "Add booking feature"

         ┌─────────────────┐
         │  PRODUCT MANAGER │
         │  Breaks it down  │
         └────────┬────────┘
                  │
    ┌─────────────┼─────────────┐
    │             │             │
    ▼             ▼             ▼
┌────────┐  ┌────────┐  ┌────────┐
│ DESIGN │  │  API   │  │ FRONTEND│
│ Create │  │ Design │  │ Build   │
│  UI    │  │ Endpoints│  │ Components│
└───┬────┘  └───┬────┘  └───┬────┘
    │           │           │
    └───────────┴───────────┘
                │
                ▼
         ┌─────────────┐
         │    QA       │
         │   Test      │
         └─────────────┘
```

---

## 🛡️ Smart Defaults

When you **don't know** or say **"no"**:

| You Say | Default Applied |
|---------|----------------|
| Tech stack | React + Tailwind + Django |
| Design | Glassmorphism (purple/green) |
| Auth | JWT + Google OAuth |
| Database | SQLite → PostgreSQL |
| Budget | Minimal (lean startup) |
| Timeline | 3-month MVP |
| Features | Core MVP (YAGNI) |
| Security | Standard protection |
| Marketing | Organic + social only |

### Examples

```
USER: "Build the backend (don't know tech)"
AGENT: ✅ Django + Python
       ✅ SQLite dev, PostgreSQL prod
       ✅ REST API
       ✅ JWT auth

USER: "Skip the review system"
AGENT: ❌ Reviews disabled

USER: "We want everything"
AGENT: ✅ Full auth (email + social + MFA)
       ✅ All features
       ✅ Premium design
```

---

## 💬 Conversation Flow

### New Feature Request
```
CEO: "New feature: Worker video portfolio"
     │
     ├──→ PM: Scope it
     ├──→ CTO: Plan infrastructure
     ├──→ Designer: Create video UI
     └──→ Security: Content safety
```

### Unknown Tech Question
```
USER: "What should we use for auth?"
AGENT: Applying defaults:
       ✅ Email/Password
       ✅ Google OAuth
       ✅ JWT tokens
       ✅ Standard security
```

### Quality Gate Check
```
API Dev: Implementing file upload
        │
        ▼
Auth Security: Review security
              │
              ▼
Security Issues: [ ] File validation
                 [ ] Size limits
                 [ ] Virus scan
              │
              ▼
✅ APPROVED (or fixes requested)
```

---

## 📁 File Structure

```
hiremate2/
├── 📄 README.md              ← You are here
├── 📋 PROJECT.md             ← Setup (fill once)
│
├── 👔 executive/            ← CEO, CFO, COO
├── 💻 engineering/          ← CTO, Devs
├── 📢 marketing/            ← CMO, Growth
├── 💰 sales/                ← Sales team
├── 🎨 product/              ← PM, Designer
├── ⚙️ operations/          ← Ops, Support
│
├── 🔧 companion/            ← Utilities
│   ├── COMMUNICATION.md     ← How agents talk
│   └── DEFAULTS.md         ← Smart defaults
│
└── 🌐 hiremate-website/    ← Built website
```

---

## 🚀 Commands

| Command | Agent | What Happens |
|---------|-------|--------------|
| `status` | Any | Report current work |
| `architecture` | CTO | Show tech stack |
| `roadmap` | PM | Show 3-month plan |
| `marketing-plan` | CMO | Show strategy |
| `defaults` | Any | Show applied defaults |

---

## 📊 Stats

| Metric | Count |
|--------|-------|
| 🤖 Total Agents | 26 |
| 🏢 Departments | 6 |
| 📁 Agent Files | 26 |
| 📝 Companion Files | 2 |

---

## 🎓 Usage Examples

### Single Agent (Quick Task)
```markdown
1. Copy React_Developer.md
2. Paste into AI assistant
3. Ask your question
```

### Multi-Agent (Complex)
```markdown
1. Start with CEO (vision)
2. Add CTO (architecture)
3. Bring in specialists
4. Agents coordinate
```

### Full Company (Startup)
```markdown
1. CEO sets OKRs
2. CTO builds roadmap
3. CMO creates launch plan
4. PM manages priorities
5. Weekly syncs
```

---

## 🛠️ Built With

- **AI**: Claude, GPT, any LLM
- **Frontend**: React + Tailwind + Vite
- **Backend**: Django + Python
- **Database**: SQLite → PostgreSQL
- **Design**: Glassmorphism

---

## 🤝 Contributing

1. Fork the repo
2. Copy an agent as template
3. Customize for your role
4. Update this README
5. Submit changes

---

## 📄 License

MIT - Use freely!

---

<p align="center">
  <strong>HireMate - Your AI-Powered Company</strong>
  <br>
  🤖 26 Agents | 🏢 6 Departments | 🎯 1 Vision
</p>
