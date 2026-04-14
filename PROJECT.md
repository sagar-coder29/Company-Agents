# 🎯 HireMate Company Configuration

> **Single source of truth for all 26 agents. Fill once, reference everywhere.**

---

## 📋 How to Fill This

| Your Input | What Happens |
|-----------|--------------|
| Specific value | Your value is used |
| "yes" / "all" | Full default applied |
| "no" / "skip" | Feature removed |
| "don't know" / blank | Smart default applied |
| "not decided" | Default used, noted as TBD |

---

## 🏢 Company Basics

| Field | Value | Default If Unknown |
|-------|-------|-------------------|
| Company Name | HireMate | HireMate |
| Industry | service | service marketplace |
| Stage | pre-seed | pre-seed |
| Current Revenue | 0 | 0 |
| Target Revenue | 1 Cr | 1 Cr (₹10M) |

---

## 👔 Executive Configuration

### CEO (Defaults Applied)
| Question | Default |
|----------|---------|
| 3-year vision | "Become India's most trusted home services platform" |
| Top 3 OKRs | [Launch MVP, 100 users, 4.5+ rating] |
| Fundraising | Post-MVP (~6 months) |
| Key metrics | [Users, Bookings, Rating, Retention] |
| Blockers | [Trust, Supply, Awareness] |

### CFO (Defaults Applied)
| Question | Default |
|----------|---------|
| Monthly burn | Minimal |
| Runway | 12 months |
| Profitability | Month 18 |
| Cost centers | [Dev, Marketing, Ops] |

### COO (Defaults Applied)
| Question | Default |
|----------|---------|
| Headcount | 1-2 (lean) |
| Tools | [Notion, Slack, GitHub] |
| Bottleneck | Customer acquisition |

---

## 💻 Engineering Configuration

### Tech Stack (Applied Defaults)
```yaml
frontend:
  framework: React 18
  bundler: Vite
  styling: Tailwind CSS
  state: Context API + useState
  routing: React Router 6
  icons: Lucide React

backend:
  framework: Django 5 + DRF
  language: Python 3.11+
  auth: JWT + Google OAuth
  
database:
  dev: SQLite
  prod: PostgreSQL
  orm: Django ORM

infrastructure:
  frontend: Vercel
  backend: Railway
  cicd: GitHub Actions
```

### Scale Targets (Defaults)
| Metric | Target |
|--------|--------|
| Users (MVP) | 100+ |
| Transactions | 1000/month |
| Uptime | 99.5% |
| Latency | <200ms |
| Concurrent | 100+ |

### Security (Defaults Applied)
```yaml
auth:
  password_hashing: bcrypt
  jwt_expiry: 15 minutes
  refresh_token: rotation enabled
  google_oauth: enabled
  rate_limiting: enabled

protection:
  csrf: enabled
  xss: sanitization
  sql_injection: django_orm
  https: enforced
```

---

## 🎨 Design System (Defaults Applied)

```yaml
style: glassmorphism
colors:
  primary: "#8B5CF6"   # Purple - Trust
  secondary: "#10B981"  # Green - CTAs
  background: gray-900
  text: white/gray-400

effects:
  glass: backdrop-blur-xl bg-white/10
  border: border-white/20
  rounded: rounded-2xl
  shadows: shadow-xl

animations:
  hover: scale-105
  duration: 200-300ms
  easing: ease-out

accessibility:
  level: WCAG 2.1 AA
  contrast: 4.5:1 minimum
```

---

## 📢 Marketing Configuration (Defaults)

```yaml
channels:
  primary:
    - social_media
    - word_of_mouth
    - local_seo
    - referral_program
  secondary:
    - content_marketing
    - email_newsletter

budget:
  monthly: ₹5,000
  allocation:
    social_ads: ₹2,000
    content: ₹1,000
    tools: ₹1,000
    contingency: ₹1,000

competitors:
  - Urban Company
  - Practo
  - Local providers

content:
  social: 2-3 posts/week
  blog: 2 posts/month
```

---

## 💰 Sales Configuration (Defaults)

```yaml
pipeline:
  stages:
    - inquiry
    - booked
    - in_progress
    - completed

crm: None (MVP - spreadsheet)

metrics:
  avg_deal_size: tracked
  conversion_rate: tracked
  sales_cycle: 1 day to 1 week

commission:
  structure: 10% post-MVP
```

---

## 🔄 Agent Communication Protocol

### How They Talk
```yaml
types:
  REQUEST: "Need X from Y"
  INFO: "FYI, X is done"
  APPROVAL: "Approve X?"
  BLOCKER: "Can't proceed without Y"
  UPDATE: "Progress report"
```

### Default Checkpoints
```yaml
1. Requirements Review
   → PM, CTO, Designer
   
2. Design Review
   → Designer, Frontend Lead
   
3. Code Review
   → Tech Lead, Peer
   
4. Security Review
   → Auth Security Specialist
   
5. QA Review
   → QA or PM (MVP)
   
6. Launch Approval
   → CEO, CTO
```

---

## 🛡️ Feature Flags (Defaults)

### Enabled by Default
```yaml
✅ user_auth
✅ google_oauth
✅ worker_profiles
✅ booking_system
✅ ratings_reviews
✅ map_integration
✅ address_management
✅ price_calculator
✅ pay_after_service
✅ notifications_email
```

### Disabled by Default (Future)
```yaml
❌ payment_gateway
❌ real_time_chat
❌ admin_panel
❌ subscriptions
❌ api_partners
❌ mobile_app
```

---

## 📅 Project Phases (Defaults)

```yaml
phase_1_mvp:
  duration: 3_months
  features:
    - auth
    - profiles
    - booking
    - ratings
    - basic_ui

phase_2_growth:
  duration: 3_months
  features:
    - payments
    - notifications
    - analytics
    - referrals

phase_3_scale:
  duration: 6_months
  features:
    - advanced_filters
    - subscriptions
    - api_partners
    - multi_city
```

---

## 📊 Current Status

| Section | Status |
|---------|--------|
| Company Basics | ✅ Configured |
| Executive | ✅ Defaults Applied |
| Engineering | ✅ Defaults Applied |
| Design | ✅ Defaults Applied |
| Marketing | ✅ Defaults Applied |
| Sales | ✅ Defaults Applied |
| Operations | ⚠️ Not Configured |

---

*Update this file when company direction changes. All agents reference this.*
