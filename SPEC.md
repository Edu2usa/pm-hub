# Preferred Maintenance — Operations Hub

## Concept & Vision
A clean, professional operations hub that ties together all Preferred Maintenance web apps under one roof. Dark, modern, business-grade — the kind of dashboard a CEO uses to show investors. Fast, static, zero backend needed.

## Apps Linked
1. **Prometheus Dashboard** — Main agent/operations dashboard (prometheus-dashboard)
2. **Equipment Tracker** — Asset management (equipment-tracker)  
3. **LeadScout** — Lead generation
4. **Stock Screener** — Munger-style stock screening
5. **Telegram Bot** — OpenClaw agent interface

## Tech
- Vite + React + TypeScript
- Tailwind CSS (CDN for simplicity)
- Static — deploys to Vercel, no server needed
- Deployed repo: github.com/Edu2usa/pm-hub

## Design
- Dark navy gradient background
- Card-based layout with hover effects
- App cards with emoji icons, names, descriptions
- "View App" buttons linking to each deployed URL
- Status indicators (live/deprecated)
- Responsive grid (1-3 columns)
- Footer with company name + timestamp
