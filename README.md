# Swachh Track

**Smart real-time waste reporting and collection platform**

Problem Statement ID `SIH26195`, Theme: *Clean & Green Technology*, Category: Software.
Team: **CleanCoders**

---

## The Problem

Nearly 65% of municipal waste is collected on schedule, but the remaining **35% goes uncollected** — not because of a shortage of trucks, but because there's no real-time way for municipalities to know where waste is piling up between scheduled rounds. Complaints, when they happen, are slow, untracked, and rarely followed up on.

## The Idea

Swachh Track lets any resident **photograph and pin** uncollected waste in their area. The report goes straight onto a live map that municipal drivers use, so the nearest vehicle can act on it without waiting for the next scheduled sweep. Once collected, the report closes and the reporter earns points — with a separate payout system for residents who hand over sorted recyclables directly.

## How It Works

1. **Sign in** — Residents register with name, phone number, and ward.
2. **Photograph the waste** — A photo taken on-site is enough; no long description needed.
3. **Mark the location** — Captured automatically via device GPS, adjustable on the map.
4. **Vehicle is notified** — The report appears on the driver's live map with the photo attached.
5. **Collected & rewarded** — Once cleared, the report is marked done and the reporter earns points.

## Features

- 📍 **Report waste** — photo upload + live geolocation capture
- 🗺️ **Live map** — all open and resolved reports shown with status (Pending / En route / Collected) via Leaflet + OpenStreetMap
- 🏆 **Rewards** — points for reporting, bonus points for confirmed collection, and a separate cash-payout guide for recyclables (paper, plastic, metal)
- 👷 **Municipal dashboard** — a driver/admin login to view incoming reports and update their status
- 📱 Fully responsive, single-page interface — no backend or database required for the demo

## Tech Stack

**Frontend (this prototype):** HTML5, CSS3, vanilla JavaScript, [Leaflet.js](https://leafletjs.com/) for mapping, browser `localStorage` for demo data persistence

**Proposed full-stack build:**
| Layer | Technology |
|---|---|
| Frontend | HTML, CSS, JavaScript, React JS |
| Backend | Java |
| Database | SQL, MongoDB |
| IoT (waste-sorting bins) | Nano Arduino v3, Ultrasonic fill sensor, Soil moisture sensor |

## Impact & Benefits

- **Environment** — faster, targeted collection reduces improperly disposed waste
- **Regulatory compliance** — timestamped records support compliance with environmental disposal standards
- **Public health** — reduces breeding grounds for vector-borne disease from uncollected waste
- **Individual residents** — a direct, visible link between reporting waste and being rewarded for it

## Feasibility & Challenges

| Challenge | Mitigation |
|---|---|
| User adoption & engagement | In-app onboarding and a visible feedback loop on report outcomes |
| Sustaining user interest | Regular feature updates and a running rewards balance |
| Technical integration | Lightweight interface compatible with low-end Android devices |
| Municipality collaboration | Pilot with a single ward's drivers before wider rollout |

## Getting Started

This is a static, single-file website — no build step or server required.

1. Clone or download this repository
2. Open `index.html` directly in a browser, **or**
3. Deploy it as-is to any static host (see below)

```bash
git clone https://github.com/<your-username>/swachh-track.git
cd swachh-track