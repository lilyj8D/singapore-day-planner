# Singapore Day Planner
An interactive, mobile-friendly day-out planner for exploring Singapore. Create multiple itineraries, add stops with times and costs, visualise your day on a timeline, and keep a packing checklist — all in a single HTML file.
## Screenshots
| Timeline | Add Stop | Plan Switcher |
|----------|----------|---------------|
| Colour-coded stops with travel gaps | Bottom-sheet form with category picker | Tabs to switch between plans |
## Features
### Multi-Plan Support
- Create unlimited day plans (e.g. "Marina Bay Explorer", "Sentosa Beach Day")
- Each plan has its own name, location, memo, stops, and checklist
- Switch between plans instantly via tabs
- Edit or delete plans at any time
### Itinerary Builder
- Add stops with: place name, category, start time, duration, and estimated cost (SGD)
- 7 colour-coded categories: Attraction, Food & Drink, Shopping, Nature, Transport, Entertainment, Other
- Optional notes field for tips, booking links, or reminders
- Auto-sorts stops chronologically
- Smart start-time pre-fill (picks up where your last stop ends)
### Visual Timeline
- Clean vertical timeline with coloured dots and cards
- Travel gap indicators between stops (shows walk/transit time available)
- "Back-to-back" badges when stops are consecutive
- Red dashed connectors for overlapping stops
- Day-at-a-glance bar (8 AM–10 PM) with proportional coloured segments
### Budget Tracker
- Running total in SGD displayed in the sticky stats bar
- Per-stop cost badges (or "Free" label)
- End-of-day summary with total time + total spend
### Smart Warnings
- Overpacked day alert (> 10 hours of activities)
- Overlapping stops detection with specific timing
- Late-finish warning (past 10 PM)
### Things to Bring Checklist
- Per-plan checklist (independent for each itinerary)
- Pre-loaded with 10 Singapore essentials (EZ-Link card, sunscreen, umbrella, etc.)
- Add custom items, tick them off, delete what you don't need
- Progress bar and counter — turns green when everything is packed
### Design
- Mobile-first responsive layout (works on phones, tablets, desktop)
- Friendly, colourful UI with smooth animations
- Sticky stats bar stays visible while scrolling
- Bottom-sheet modal pattern for adding stops (natural on mobile)
- No external dependencies beyond Google Fonts (Poppins)
## Quick Start
```bash
# Option 1: Just open it
open index.html
# Option 2: Serve locally
npx serve .
# → http://localhost:3000
```
No build step. No `npm install`. No framework. Just one HTML file.
## Deploy to GitHub Pages
1. Create a new repository on GitHub
2. Upload `index.html` (drag-and-drop works)
3. Go to **Settings > Pages**
4. Source: **Deploy from a branch** → `main` → `/ (root)`
5. Your planner will be live at:
   ```
   https://<your-username>.github.io/<repo-name>/
   ```
## File Structure
```
singapore-day-planner/
├── index.html   ← entire app (HTML + CSS + JS, ~1100 lines)
├── README.md    ← this file
└── LICENSE      ← MIT
```
## Technical Details
| Aspect | Detail |
|--------|--------|
| Size | ~35 KB (single file) |
| Dependencies | None (Google Fonts loaded via CDN) |
| Framework | Vanilla JS |
| Storage | In-memory (refreshing resets data) |
| Browser support | Modern browsers (Chrome, Safari, Firefox, Edge) |
| Offline | Works offline once loaded (except font) |
## Customisation Ideas
- Swap the default checklist items in the `DEFAULT_CHECKLIST` array
- Change the colour palette via CSS custom properties (`:root` block)
- Add `localStorage` persistence by saving/loading `plans` array
- Extend to other cities by changing the header and default data
## License
MIT
