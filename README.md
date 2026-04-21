# CARP Planner v1.2.0
**Computed Air Release Point Planning Tool for Microsoft Flight Simulator**

CARP Planner computes the release point for airdrop missions using the procedures defined in AFMAN 11-231. Enter your drop zone details, fetch real-world weather data, and the tool calculates where to release your cargo so it lands on the Point of Impact. Supports CDS, Personnel, and Heavy Equipment drop types.

---

## Installation
1. Place **CARP_Planner.exe** in any folder on your PC
2. Double-click to run

No additional software is required. The application will check for updates automatically on startup and notify you when a new version is available.

> **Windows SmartScreen:** On first run, right-click the EXE → Properties → tick **Unblock** → OK.

---

## Quick Start
1. Enter the **Point of Impact** coordinates and **Drop Zone** dimensions
2. Select your **Drop Type** (CDS, Personnel, or Heavy Equipment) and set the item count
3. Enter the **Load Weight** (lbs), or 0 to use the default rate of fall
4. Select your **aircraft** — IAS will auto-populate with the default drop speed
5. Adjust **IAS**, **drop altitude**, and other parameters as required
6. Click **FETCH WEATHER** to retrieve current or forecast wind data
7. Click **COMPUTE CARP** to calculate the release point
8. Use the **tactical map** and **steering compass** to plan your run
9. Click **EXPORT** to save a printable HTML data card

---

## Key Features

### Computation
- Full AF Form 4018 CARP computation (all 35 items) per AFMAN 11-231
- Three drop types: **CDS**, **Personnel**, and **Heavy Equipment**
- Weight-indexed ballistic interpolation (RoF, VD, TFC, DQ) from AFMAN 11-231 ATTLA tables
- Parachute automatically assigned by drop type (G-12D / T-10C / G-11B)
- Load weight gross error check — warns if entry is outside valid ballistic range
- Multi-pass handling with racetrack turn direction

### Weather
- Real-world weather from Open-Meteo with forecast support (Time on Target)
- WMM-2025 magnetic declination
- Manual wind override for simulator-known conditions

### Tactical Map
- **Schematic mode** — dark tactical overlay, works offline
- **OSM tile mode** — live OpenStreetMap background, toggled via the 🗺 Map button
  - Tiles pre-loaded on Compute (zoom levels 9–19 around CARP, APDIP, and EODP)
  - Progressive tile loading — tiles appear as they arrive
  - Zoom via **+** / **−** buttons (discrete OSM zoom steps; overlay and tiles always in sync)
- Personnel drops: 400-yard safety margin zone drawn in amber ahead of PI
- HUD overlays (wind barb, north arrow, scale bar) with dark backing for legibility over map tiles
- Pan (click+drag), Reset View

### Navigation & Export
- Steering compass with heading bug and drift correction
- Waypoints: APDIP (4 NM prior), CARP, and EODP (end of drop)
- Save and load Drop Zone mission profiles
- HTML data card export (printable from browser)
- Aircraft IAS auto-updates to default drop speed on aircraft or drop type change

### General
- Adjustable font size (A+/A− buttons or Ctrl+=/Ctrl+−)
- Automatic update checking with in-app download
- Dark tactical theme for cockpit use alongside MSFS

---

## Updates
The application checks for updates automatically on startup. You can also check manually by clicking the **⟳ Updates** button in the top-right corner of the title bar.

When an update is available, you can choose to:
- **Download & Install** — downloads the new version and restarts the application automatically
- **Download Only** — saves the update to a location of your choice for manual installation
- **Skip** — continue using the current version

---

## Keyboard Shortcuts
| Key | Action |
|-----|--------|
| Enter / F9 | Compute CARP |
| F5 | Fetch Weather |
| Ctrl+S | Save Mission |
| Ctrl+O | Load Mission |
| Ctrl+E | Export Data Card |
| Ctrl+= / Ctrl+− | Increase / Decrease font size |
| + / − buttons | Zoom tactical map in / out |
| Click + Drag | Pan tactical map |

---

## Further Information
Refer to the **CARP Planner User Manual** (PDF) for detailed instructions on all features, input parameters, weather integration, multi-pass operations, and troubleshooting.

---

## Support Development
If you find CARP Planner useful, consider supporting its development:

☕ **[Buy me a coffee on Ko-fi](https://ko-fi.com/phoenixegmh)**

Your support helps fund continued development, new features, and Phase 2 (SimConnect integration).

---

## Disclaimer
**FOR SIMULATION USE ONLY.** This application is designed for use with Microsoft Flight Simulator. It is not certified for actual airdrop operations. Parachute ballistic data is approximate and may not reflect current USAF ATTLA tables.

---

*Reference: AFMAN 11-231, Computed Air Release Point Procedures (18 Nov 2020)*
