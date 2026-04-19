# SITE2GYM Mobile App

Interactive high-fidelity prototype of the SITE2GYM fitness app — dark theme, neon-lime accents, 6 screens, gamification (streak / XP / leaderboard).

## Files

- **`app.html`** — the mobile-app prototype. A 1360×768 dark stage with a single centered iPhone frame (scaled 0.82) running the full interactive React app.
- **`index.html`** — marketing landing page for SITE2GYM.

## Running

No build step. Just serve the folder statically:

```bash
npx serve -l 5199 .
```

Then open:

- http://localhost:5199/app.html — mobile-app prototype
- http://localhost:5199/index.html — landing page

## Mobile-app prototype (`app.html`)

Self-contained single-file React 18 app via UMD + Babel-standalone. No dependencies to install.

### Screens

1. **Onboarding** — 3 steps: welcome → user type (member / employee) → home gym picker
2. **Home** — streak, XP, membership hero, quick actions, weekly chart, up-next classes
3. **Booking** — calendar strip, filter chips, timeline with class slots
4. **Gym Access** — animated QR scanner with scan → unlock flow
5. **Membership** — Elite Global Pass card, benefits, billing
6. **Profile** — XP ring, tabs for stats / badges / leaderboard

### Gamification

- **Streak**: 7-day ribbon, 5 days active
- **XP**: `+10` enter gym · `+50` book class · `+40–80` FAB quick-book
- **Leaderboard**: HSR Layout weekly ranking, user at rank #3

### Design tokens

- **Colors**: ink `#000`, surface `#0A0B0C`, lime `#D0FF00`, cyan `#00F0FF`, amber `#FFB020`, magenta `#FF2E88`
- **Type**: Inter Tight (400–800) + JetBrains Mono (400–600)
- **Motion**: page-fade 280ms, scan loop 1.5s, tap scale 0.97, toast drop-in 300ms
