# Let It Out — Architecture of Catharsis

> **Single-Session Emotional Discharge Engine**
> An anonymous, zero-persistence digital release platform engineered for immediate catharsis, emotional reflection, and non-verbal resonance without the toxicity of traditional social networks.

---

## 🏛️ Core Philosophy & Architecture

Legacy confession apps fail because threaded comments, direct messages, and user profiles create vectors for harassment and cyberbullying. **Let It Out** solves this by establishing a **Bounded Single-Session Release Model**:

* **Zero Social Graph:** No user accounts, profiles, DMs, comments, likes, or search tools.
* **Automated PII Scrubbing:** Client-side scrubbing strips names, phone numbers, email addresses, and handles prior to submission.
* **Non-Directive AI Companion:** Governed by an enforced system prompt rail (Hear -> Validate -> Reframe) that holds empathetic space without offering unsolicited advice or making decisions for the user.
* **Pre/Post Mood Delta Tracking:** Tracks emotional heaviness on a 1–10 scale from session entry to completion.
* **Particle Burn Ritual:** Visual HTML5 canvas disintegration animating the destruction of typed text off-screen.

---

## 📁 Project Architecture

```
let-it-out/
├── index.html            # Single-page client UI (Tailwind CSS, Canvas particle burn)
├── api/
│   └── chat.js           # Vercel serverless proxy (protects API key)
├── shared/
│   └── emoSystemPrompt.js # Enforced v2.2 System Prompt & Safety Rails
├── package.json          # ES Module manifest
└── README.md             # Project documentation
```

---

## 🚀 Deployment Instructions

### 1. Import to Vercel
1. Go to [vercel.com/new](https://vercel.com/new).
2. Import the repository **Vitalchain76/let-it-out**.

### 2. Set Environment Variable
Under **Environment Variables**, add:
* **Key:** ANTHROPIC_API_KEY
* **Value:** your_anthropic_api_key_here

### 3. Deploy
Click **Deploy**. Vercel will automatically build the site and route all /api/chat requests to the serverless function.

---

## 🛡️ Safety & Duty of Care

* **Crisis Intervention:** Direct crisis line references (such as 988 Lifeline) built into the closing ritual.
* **API Security:** API keys and raw system prompt rails remain server-side in api/chat.js and shared/emoSystemPrompt.js, completely hidden from browser DevTools.

---
