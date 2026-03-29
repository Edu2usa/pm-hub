# Preferred Maintenance — Operations Hub

## Concept & Vision
A clean, professional operations hub that ties together all Preferred Maintenance web apps under one roof. Dark, modern, business-grade — the kind of dashboard a CEO uses to show investors. Fast, static, zero backend needed.

## Apps Linked
1. **Prometheus Dashboard** — Main agent/operations dashboard (prometheus-dashboard)
2. **Equipment Tracker** — Asset management (equipment-tracker)  
3. **LeadScout** — Lead generation
4. **Stock Screener** — Munger-style stock screening (4 tabs: Oversold, Analyze, How to Use, Watchlist)
5. **Telegram Bot** — OpenClaw agent interface

## Stock Screener (stocks.html) — Tabbed Interface

### Tabs
1. **🎯 Oversold Tab**
   - Pre-built scans: S&P 500, Popular Stocks, Tech Giants
   - Results table with Williams %R, RSI, Signal columns
   - "⭐ Save" button on each row to add to watchlist
   - Clear results option

2. **🔍 Analyze Tab**
   - Single ticker lookup with market selector (US/SET)
   - Detailed analysis: Price, Williams %R, RSI, Signal
   - "Add to Watchlist" button on results
   - Quick-add input for fast watchlist additions

3. **📖 How to Use Tab**
   - Williams %R explanation with zone colors
   - RSI explanation with thresholds
   - How to use each tab guide
   - Munger-style value strategy tips
   - Important limitations & disclaimers

4. **⭐ Watchlist Tab**
   - List of saved stocks with live prices
   - Refresh individual or all stocks
   - Export to CSV
   - Clear all option
   - localStorage persistence

### Technical Indicators
- **Williams %R**: -100 to 0 scale
  - Below -80: Oversold (buy zone)
  - -50 to -80: Neutral
  - Above -50: Overbought
- **RSI(14)**: 0-100 scale
  - Below 30: Oversold
  - 30-70: Neutral
  - Above 70: Overbought

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
