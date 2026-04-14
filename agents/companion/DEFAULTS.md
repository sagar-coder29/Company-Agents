# 🛡️ HireMate Defaults - Smart Configuration

> **What happens when you don't know or say "no"**

---

## 🎯 Philosophy

When you don't specify something, agents apply **intelligent defaults** based on:
- Industry best practices
- Lean startup principles
- Proven patterns from 100+ projects
- Security-first approach
- User trust priorities

---

## 📊 Default Quick Reference

### Company Defaults
| Input | Default |
|-------|---------|
| Company name | HireMate |
| Industry | service marketplace |
| Stage | pre-seed |
| Revenue | 0 |
| Target | 1 Cr (₹10M INR) |

### Tech Stack Defaults
| Component | Default |
|-----------|---------|
| Frontend | React + Tailwind CSS |
| Backend | Django + Python |
| Database | SQLite (dev) → PostgreSQL (prod) |
| Auth | JWT + Google OAuth |
| API | REST |
| Hosting | Vercel + Railway |
| CI/CD | GitHub Actions |

### Design Defaults
| Element | Default |
|---------|---------|
| Style | Glassmorphism |
| Primary color | #8B5CF6 (purple) |
| CTA color | #10B981 (green) |
| Background | Dark (gray-900) |
| Animations | 200-300ms transitions |
| Accessibility | WCAG 2.1 AA |

### Feature Defaults
| Feature | Default |
|---------|---------|
| User auth | ✅ Included |
| Google OAuth | ✅ Included |
| Worker profiles | ✅ Included |
| Booking system | ✅ Included |
| Ratings/reviews | ✅ Included |
| Map integration | ✅ Included |
| Payment gateway | ❌ Skipped (MVP) |
| Real-time chat | ❌ Skipped (Future) |

---

## 🚫 When You Say "No"

| Input | Result |
|-------|--------|
| "no payment" | Payment gateway disabled |
| "no social login" | Email/password only |
| "no map" | Manual address entry |
| "no ratings" | Reviews disabled |
| "no analytics" | No tracking (privacy-first) |
| "no notifications" | Email notifications disabled |

## ✅ When You Say "Yes" / "All"

| Input | Result |
|-------|--------|
| "yes auth" | Full auth (email + social + MFA) |
| "all features" | Everything in spec |
| "yes payments" | Payment gateway integrated |
| "yes notifications" | Email + SMS + Push |

---

## 💬 Default Conversation Examples

### Example 1: Unknown Feature
```
USER: Add something for trust

AGENT: "Applying trust defaults:

🔒 Trust Features:
├── Verified badges on workers
├── 5-star rating system
├── Customer reviews
├── Background verification badge
├── Secure payment (pay after)
└── 24/7 support option

These are standard for marketplaces.
Want to customize?"
```

### Example 2: Unknown Timeline
```
USER: How long will this take?

AGENT: "Applying timeline defaults:

📅 Default Timeline:
├── MVP Core: 3 months
├── Launch prep: 2 weeks
├── First 100 users: 1 month
└── Series A ready: 12-18 months

Per feature:
├── Simple: 1 week
├── Medium: 2 weeks
└── Complex: 1 month
```

### Example 3: Unknown Budget
```
USER: What's this going to cost?

AGENT: "Applying cost defaults:

💰 Monthly Costs (Pre-seed):
├── Development: ₹0 (team)
├── Hosting: ₹0-500 (free)
├── Domain: ₹800/year
├── Tools: ₹0-2000 (free)
├── Marketing: ₹5000
└── Total: ~₹7000/month
```

---

## 🛠️ How to Override

```markdown
# Use specific value
USER: Use PostgreSQL (not SQLite)
USER: Budget ₹50,000/month

# Remove feature
USER: No payment gateway for now
USER: Skip the review system

# Change priority
USER: This is critical
USER: Wait until phase 2
```

---

## 🔄 Agent Communication Defaults

When agents collaborate:

```
1. REQUEST → "Need X from Y"
2. INFO → "FYI, X is done"
3. APPROVAL → "Approve X?"
4. BLOCKER → "Can't proceed without Y"
5. UPDATE → "Progress report"
```

### Default Checkpoints
| Phase | Agents | Purpose |
|-------|--------|---------|
| Requirements | PM, CTO, Designer | Validate specs |
| Design | Designer, Frontend | UX approval |
| Code | Tech Lead, Peer | Quality check |
| Security | Auth Security | Vulnerability scan |
| QA | QA, PM | Testing validation |
| Launch | CEO, CTO | Final approval |

---

## 📋 Decision Matrix

```
INPUT           → DEFAULT APPLIED
─────────────────────────────────
specific value  → USE IT
"yes/all/sure"  → FULL DEFAULT
"no/not needed" → REMOVE FEATURE
"I don't know"  → SMART DEFAULT
blank/no answer → SMART DEFAULT
```

---

## 🎓 Philosophy

| Principle | Default Behavior |
|-----------|------------------|
| YAGNI | MVP features only |
| Security-first | Safe defaults always |
| Lean | Minimal viable for pre-seed |
| User trust | Trust features enabled |
| Scalability | Architecture supports growth |

---

*Defaults exist to help you move fast. Customize when you know better.*
