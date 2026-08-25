# F1 2026 Season Dashboard

## Goal
A web dashboard that shows the live/current status of the F1 2026 season — schedule, standings, results, and the big 2026 regulation changes (new power units, active aero, narrower/lighter cars) — styled as a bold, neo-brutalist web page (see [.claude/skills/neo-brutalist/SKILL.md](.claude/skills/neo-brutalist/SKILL.md)).

## Scope
- **Dashboard page**: at-a-glance season status
  - Next race countdown (name, circuit, date, session times)
  - Driver standings table (position, driver, team, points, gap to leader)
  - Constructor standings table
  - Last race result summary (podium, fastest lap)
  - Full season calendar with completed/upcoming race indicators
- **Web design page**: the neo-brutalist front-end presentation layer for the above
  - Hero section with headline season stat (e.g. championship leader, next race)
  - Standings tables restyled as brutalist cards/grids
  - Calendar as a chunky, high-contrast list or grid
  - Team/driver detail cards (color-coded by team)
- **Mobile-friendly**: fully responsive, not just a scaled-down desktop layout
  - Standings tables collapse to stacked cards below tablet width
  - Nav collapses to a brutalist hamburger/drawer, not hidden links
  - Touch targets sized for tap (buttons, checkboxes, nav items)
  - Borders/shadows/type scale down but stay chunky — never thin out to "normal" web weight

## Data
2026 season data (calendar, standings, results) needs a source — likely one of:
- A public F1 API (e.g. Ergast successor / Jolpica API, OpenF1)
- Manual/static JSON updated periodically
- Scraping is a fallback only if no API is available

Decision on data source is still open — pick this before building data-fetching logic.

## Tech Direction (proposed, not yet decided)
- Static site or lightweight frontend (plain HTML/CSS/JS or a small framework)
- Tailwind CSS for the brutalist utility classes already documented in the skill
- Data layer: fetch from chosen API at build/runtime, or read local JSON

## Design Direction
- Neo-brutalist: hard shadows, thick borders, high-contrast palette (see skill for palettes/fonts)
- Suggested palette: Electric Blue or Inverted (dark) to fit motorsport/night-race feel
- Team colors used as accent colors within brutalist card system
- Mobile-first responsive breakpoints: design for phone width first, scale up to tablet/desktop
- Reference: [neo-brutalist-reference.html](neo-brutalist-reference.html) for live component/color/type examples

## Open Questions
- [ ] Which data source/API for 2026 standings and calendar?
- [ ] Static build or needs live/auto-refreshing data?
- [ ] Single page or multi-page (dashboard + separate design showcase)?
- [ ] Hosting target (local only, Vercel/Netlify, GitHub Pages)?

## Next Steps
1. Confirm data source for F1 2026 season data
2. Scaffold project (index.html + Tailwind, or chosen framework)
3. Build dashboard components against real/sample data
4. Apply neo-brutalist skill styling
