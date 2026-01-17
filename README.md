# SentinelPulse

![Status](https://img.shields.io/badge/status-early%20development-yellow)
![Focus](https://img.shields.io/badge/focus-reliability%20%26%20privacy-blue)
![AI](https://img.shields.io/badge/AI-optional%20%26%20bounded-lightgrey)
![License](https://img.shields.io/badge/license-TBD-lightgrey)

> A quiet signal that you're still here.

**SentinelPulse** is a web-based personal safety check-in system.  
It helps people quietly confirm they are okay — and responsibly notifies trusted contacts **only when silence lasts too long**.

This project is intentionally built **without urgency theatrics, without diagnosis, and without AI making life-or-death decisions**.

---

## 🧭 Project Intent

SentinelPulse started from a simple question:

> *“What if checking in felt calm, private, and respectful — instead of alarming?”*

This project is designed for:
- people who live alone
- people who are often offline or overwhelmed
- people who want **control over how and when others are notified**

It is **not** built to monitor behavior, analyze mental health, or predict outcomes.

---

## 🧠 Design Philosophy

- **Human-first**  
  Calm language, no fear-driven UX.

- **Privacy by default**  
  Minimal data, explicit consent, preview before sharing.

- **Reliable over clever**  
  A stable reminder system matters more than complex intelligence.

- **AI as assistance, never authority**  
  AI may help format or suggest — never decide.

---

## ✨ Core Features

### ✅ Check-in System
- Manual check-in (“Still here”, “I’m okay”)
- Flexible schedules (daily, custom)
- Grace periods to prevent false alarms

### ⏰ Reminder & Escalation
- Gentle reminders before escalation
- Multi-step escalation logic
- User-controlled thresholds

### 👥 Emergency Contacts
- Explicit consent per contact
- Channel-based delivery (email, push, etc.)
- Cancel window before final escalation

---

## 📝 Notes & Mood (Planned)

SentinelPulse includes a **note-first approach**, not analysis.

- Personal notes / journaling
- Optional mood tags (non-diagnostic)
- Notes are **private by default**
- Users decide if notes may be shared during escalation

No automatic psychological interpretation is performed.

---

## 📄 Emergency History Export

If a user does not confirm their status for an extended period (e.g. >30 days):

- Trusted contacts may receive:
  - last known check-in time
  - a calm status message
  - an optional `.txt` file containing:
    - check-in history
    - user-approved notes

Everything is previewable and consent-based.

---

## 🤖 AI Usage (Future, Optional)

AI is **not part of the MVP**.

If introduced, AI will only assist with:
- suggesting reminder schedules
- summarizing user-written notes (opt-in)
- adjusting message tone (neutral / gentle / firm)
- formatting exported text files

AI will **never**:
- diagnose mental health
- provide therapy or medical advice
- predict self-harm or death
- trigger emergency escalation autonomously

> SentinelPulse does not delegate human safety decisions to AI.

---

## 🛡️ Safety & Ethics

- No behavioral scoring
- No emotional inference
- No hidden data sharing
- Clear disclaimers and user control

SentinelPulse aims to be **supportive, not intrusive**.

---

## 🧱 Planned Tech Stack

**Frontend**
- React / Next.js
- PWA (installable, offline-tolerant)
- Tailwind CSS

**Backend**
- Node.js or Bun
- RESTful API
- Background jobs & schedulers

**Data**
- PostgreSQL
- Redis (queues & rate limiting)

**Notifications**
- Web Push
- Email
- Optional: WhatsApp / Telegram

---

## 📁 Repository Structure (Draft)

```
sentinelpulse/
├─ apps/
│  ├─ web/        # UI & PWA
│  └─ api/        # Core API & scheduler
├─ packages/
│  ├─ core/       # Domain logic
│  ├─ notifier/   # Notification channels
│  ├─ scheduler/  # Reminder & escalation
│  └─ ai/         # Reserved for future use
├─ docs/
│  ├─ product.md
│  ├─ roadmap.md
│  └─ ai-ideas.md
```

---

## 🚧 Project Status

🟡 **Early development / exploration phase**

- Architecture & domain modeling in progress
- No production deployment yet
- API & scheduler logic under design

This repository represents **intentional groundwork**, not a finished product.

---

## ⚠️ Disclaimer

SentinelPulse is **not a medical or mental health service**.  
If you or someone else is in immediate danger, contact local emergency services or trusted individuals.

---

## 🤝 Contributions

Thoughtful discussion and feedback are welcome — especially around:
- reliability
- ethical boundaries
- privacy design
- UX clarity

---

> Built quietly.  
> Designed to care.
