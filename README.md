# 🦁 Singapore Day Planner

An interactive, mobile-friendly day-out planner for exploring Singapore. Add stops with times and costs, visualise your day on a timeline, and keep a packing checklist — all in a single HTML file.

**👉 [Try it live](https://lilyj8D.github.io/singapore-day-planner/)**

## Features

### Multi-Plan Support
- Create multiple day plans (e.g. "Marina Bay Explorer", "Sentosa Beach Day")
- Each plan has its own name, location, memo, stops, and checklist
- Switch between plans via tabs
- Edit or delete plans

### Itinerary Builder
- Add stops with: place name, category, start time, duration, and estimated cost (SGD)
- 7 colour-coded categories: Attraction, Food & Drink, Shopping, Nature, Transport, Entertainment, Other
- Optional notes field for tips or reminders
- Edit or delete existing stops
- Auto-sorts stops chronologically

### Visual Timeline
- Clean vertical timeline with coloured category dots and cards
- Day-at-a-glance bar (8 AM–10 PM) with proportional coloured segments
- Empty state with helpful prompt to get started

### Budget & Stats
- Running total in SGD displayed in the sticky stats bar
- Total number of stops and total time at a glance

### Things to Bring Checklist
- Per-plan checklist (independent for each itinerary)
- Add custom items, tick them off
- Progress counter
- Collapsible section

### Design
- Mobile-first responsive layout (works on phones, tablets, desktop)
- Friendly, colourful UI with smooth animations
- Sticky stats bar stays visible while scrolling
- Bottom-sheet modal pattern for adding stops (natural on mobile)
- Floating action button (+) for quick access
- No external dependencies beyond Google Fonts (Poppins)

## Quick Start

```bash
# Option 1: Just open it
open index.html

# Option 2: Serve locally
npx serve .
# → http://localhost:3000
