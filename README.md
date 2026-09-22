# RINGFORGE // NEXUS

Ring capability truth layer.  
**NEXUS** — NExtended Xperimental USers  
**DoubleA · AntManThePro** × Ring Bot

Live (after Pages deploy): https://antmanthepro.github.io/ringforge-nexus/

## What this is

A verified contract console for Ring Developer Platform docs as of **2026-09-10 CT**.  
Force-graph topology, capability matrix, mock event bus with temporal + BFS correlation, OAuth/scope registry, endpoint/webhook catalog, open-verification tracker.

Not a live home dashboard. Partner OAuth is **not linked**. Runtime source facts are **unavailable**. Mock streams are labeled **MOCK ADAPTER**.

Not affiliated with Ring or Amazon.

## Wanderer gate

Client-side SHA-256 check. Stops casual traffic. **Not a vault** — contracts remain in page source.

Mission key is issued by DoubleA (not printed in this public README).  
Rotate by editing `GATE_HASH` in `app.js` (`SHA-256("rf.v2|" + password)`).

Lockout: 6 failed attempts → 60 seconds.

## Controls

| Key | Action |
|---|---|
| `/` | Search |
| `1–7` | Panels |
| `Space` | Pause mock bus |
| `Esc` | Close overlays |
| LOCK | Clear session + reload |

## Truth labels

- RING DOCUMENTATION FACT
- RING SOURCE FACT (runtime) — UNAVAILABLE
- RINGFORGE DERIVED
- AI INTERPRETATION
- MOCK ADAPTER

Rule: never sacrifice truth for features.

## Repo layout

- `index.html` — shell + embedded contracts
- `app.js` — kernel
- `data.json` — same contracts, exportable
- `sw.js` / `manifest.webmanifest` / `icons/icon.svg` — PWA + home-screen sigil
- `.github/workflows/pages.yml` — GitHub Pages

## Local

Open `index.html` over http (service worker needs a host). Gate first, then Space/tap through boot.
