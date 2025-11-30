# Annie's Journal Marketing Website

## Project Overview

This is the marketing/brochureware website for Annie's Journal, hosted at www.anniesjournal.com.

The main application lives in a separate repo and is hosted at app.anniesjournal.com.

## Tech Stack

- **Framework**: Astro (static site generator)
- **Styling**: Tailwind CSS v4
- **Hosting**: Cloudflare Pages (free tier)
- **Analytics**: Cloudflare Web Analytics (privacy-friendly)

## Related Repositories

- **Main App**: https://github.com/lawrab/annies-health-journal
  - Frontend: React + TypeScript + Tailwind
  - Backend: Express + MongoDB
  - Hosted on Railway

## Domain Architecture

```
anniesjournal.com (Cloudflare DNS)
├── www.anniesjournal.com → Cloudflare Pages (this repo)
├── app.anniesjournal.com → Railway (main app)
└── @ redirect → www
```

## Design System

Colors are synced with the main app:
- **Primary**: Indigo (#4f46e5) - professional, trustworthy
- **Secondary**: Teal (#0d9488) - calm, healing
- **Font**: Inter

## Pages

| Page | Path | Status |
|------|------|--------|
| Home | `/` | ✅ Created |
| Features | `/features` | 📋 Planned |
| How It Works | `/how-it-works` | 📋 Planned |
| About | `/about` | 📋 Planned |
| Privacy | `/privacy` | 📋 Planned |

## Story & Dedication

Annie's Journal is dedicated to Annie Rabbets. The project was created to help people with complex or undiagnosed conditions track their symptoms and communicate better with healthcare providers.

Key messaging:
- "Your voice. Your health. Your journal."
- Voice-first symptom tracking
- Pattern recognition over time
- Prepared for doctor appointments
- Privacy-first, open source (AGPL-3.0)

## Development

```bash
# Install dependencies
npm install

# Start dev server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Deployment

Cloudflare Pages auto-deploys from the `main` branch.

Build settings:
- Build command: `npm run build`
- Build output directory: `dist`
- Node version: 18+
