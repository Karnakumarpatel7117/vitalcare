# VitalCare AI — Family Medicine Manager

> **AI in Action FY27 Q2 — AI @ Home Category**

A mobile-first web app that helps Indian families manage medicines for elderly parents and family members. Built entirely with AI.

## The Problem
Every Indian household has this problem. Elderly parents take 5–8 medicines at different times. Someone always forgets. There's no easy way to track who took what, generate doctor reports, or get reminded before it's too late.

## The Solution
**VitalCare AI** — take a photo of any medicine box → AI reads the label → adds to daily schedule automatically.

## Features

| Feature | Description |
|---|---|
| 📸 **AI Medicine Recognition** | Photo a medicine box — Gemini reads the name, dosage and instructions |
| 👨‍👩‍👧 **Multi-member tracking** | Separate profiles for each family member |
| ⏰ **Daily Schedule** | Morning / Afternoon / Evening / Night view |
| ✅ **One-tap mark taken** | Tap to mark — instantly updates adherence |
| 📊 **7-day history** | Visual grid showing adherence per day per member |
| 📋 **Doctor report** | 30-day adherence report ready to share with doctor |
| 🔴 **Missed medicine alerts** | Auto-alerts if medicines not taken after cutoff time |

## Tech Stack
- **Frontend**: Pure HTML/CSS/JavaScript (single file, no frameworks)
- **AI**: Google Gemini 1.5 Flash (free tier)
- **Storage**: Browser localStorage
- **Hosting**: Any static host (Netlify, GitHub Pages, Vercel)

## Getting Started

### Option 1 — Run locally
```bash
# Just open the file in Chrome
open index.html
```

### Option 2 — Deploy to Netlify
1. Drag `index.html` to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Get your live URL in 30 seconds

### Option 3 — GitHub Pages
1. Fork this repo
2. Go to Settings → Pages → Deploy from main branch
3. Your app is live at `https://yourusername.github.io/vitalcare`

## Setup (One-time)
1. Get a free Gemini API key at [aistudio.google.com](https://aistudio.google.com)
2. Open the app → tap ⚙️ Setup → paste your key → Save & Test
3. Start adding family members and medicines

## How It Works

```
User taps + → Takes photo of medicine box
         ↓
Gemini AI reads: medicine name, dosage, timing
         ↓
Form pre-fills automatically → User verifies
         ↓
Medicine added to daily schedule
         ↓
Daily: tap each medicine as taken
         ↓
Weekly: history grid shows adherence
         ↓
Monthly: one-tap doctor report
```

## Demo

**Add a medicine manually:**
1. Tap **+** → Add Medicine
2. Select family member
3. Enter medicine name, dosage
4. Select timing (Morning/Night/etc) and food instruction
5. Save

**Use AI to read a medicine box:**
1. Tap **+** → Add Medicine
2. Tap the camera area → take a photo
3. Gemini reads the label and fills the form
4. Verify and save

## Privacy
- All data stored locally in your browser (localStorage)
- No server, no database, no accounts
- Gemini API only processes the photo you take — nothing else is sent

## Roadmap
- [ ] Push notifications for medicine reminders
- [ ] Export data to Google Sheets
- [ ] Share reports via WhatsApp
- [ ] Caregiver mode (monitor remotely)
- [ ] Refill reminders based on stock

---

Built with Claude AI for the p44 AI in Action FY27 Q2 Challenge — "From Insight to Impact"
