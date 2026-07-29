# Pat's Mythic Tier List — Season 2

A World of Warcraft: Midnight fan-made tier list site for **Mythic+ Season 2** (Patch 12.1 / Curse of Ula'tek).

Compare every DPS, Tank, and Healer specialization across S–C tiers, with per-spec rationale and utility notes, plus a rundown of the Season 2 dungeon pool.

## Features

- **Role switcher** — toggle between DPS, Tank, and Healer with an animated gold slider.
- **Cinematic hero panels** — each role shows a themed cinematic image (swap in your own screenshots easily).
- **Tier lists per role** — S / A+ / A / B / C rows with class-colored spec chips and icons.
- **Hover tooltips** — every spec explains *why* it's ranked there and lists its key Mythic+ utility.
- **Season 2 dungeon pool** — all 8 dungeons (5 new Midnight + 3 returning) with their tuning notes.
- **Class icons + favicon** — WoW-themed, generated locally.
- Fully static — no build step, no dependencies, works offline.

## How the rankings were built

Rankings are a **Season 2 projection**, combining:

- **End-of-Season-1 standings** (Icy Veins, Patch 12.0.7)
- **Patch 12.1 PTR class changes**, including:
  - +25% player health / enemy damage system
  - DPS cooldown smoothing (power moved from burst windows into filler)
  - Per-spec reworks (notably Marksmanship Hunter, Protection Paladin, Restoration Druid, Elemental Shaman, Unholy Death Knight)

> PTR numbers are **not final** and will shift before launch. Bring the better player, not just the better spec.

## Run locally

Open a terminal in this folder and start a simple server:

```powershell
python -m http.server 8000
```

Then visit **http://localhost:8000**.

Or just double-click `index.html` to open it directly in a browser.

## Deploy

This is a static site — host it anywhere:

- **GitHub Pages:** push to a `main` branch and enable Pages in repo Settings → Pages.
- **Netlify Drop:** drag this folder onto https://app.netlify.com/drop.
- **Cloudflare Pages:** direct upload via the dashboard.

## Customizing

- **Cinematic images:** replace `cinematic-dps.jpg`, `cinematic-tank.jpg`, `cinematic-healer.jpg` (keep the same filenames; ~1600x560 works best).
- **Class icons:** replace any `icon-<class>.png` with a real WoW class crest (keep the filename).
- **Rankings:** edit the `DATA` object near the bottom of `index.html`.
- **Spec notes:** edit the `SPECS` object.

## Credits & disclaimer

- Tier list data informed by **Icy Veins** Mythic+ rankings and Blizzard's Patch 12.1 PTR notes.
- World of Warcraft and all related art are © Blizzard Entertainment. This is a non-commercial fan project.
- Class icons and cinematic placeholder art are generated locally; replace them with your own assets as desired.
