# SITE2GYM Mobile App

Interactive high-fidelity prototype of the SITE2GYM fitness app — dark theme, neon-lime accents, 6 screens, gamification (streak / XP / leaderboard).

## Run

No build step. Just serve statically:

```bash
npx serve -l 5199 .
```

Open http://localhost:5199/app.html.

## Screens

1. **Onboarding** — welcome → user type (member / employee) → home gym picker
2. **Home** — streak, XP, membership hero, quick actions, weekly chart, up-next classes
3. **Booking** — calendar strip, filter chips, timeline with class slots
4. **Gym Access** — animated QR scanner with scan → unlock flow
5. **Membership** — Elite Global Pass card, benefits, billing
6. **Profile** — XP ring, tabs for stats / badges / leaderboard

## Stage

Single HTML file, 1360×768 dark stage, iPhone frame centered (scaled 0.82). React 18 via UMD + Babel-standalone — zero dependencies to install.

## Design tokens

- Colors: ink `#000`, surface `#0A0B0C`, lime `#D0FF00`, cyan `#00F0FF`, amber `#FFB020`, magenta `#FF2E88`
- Type: Inter Tight (400–800) + JetBrains Mono (400–600)
- Motion: page-fade 280ms, scan loop 1.5s, tap scale 0.97, toast drop-in 300ms

## Gamification

- Streak: 7-day ribbon
- XP: `+10` enter gym · `+50` book class · `+40–80` FAB quick-book
- Leaderboard: HSR Layout weekly ranking
