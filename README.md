# Gridwise — Intelligent EV Charging Network Optimization

Gridwise is a browser-based prototype dashboard for exploring EV charging network planning. It includes an overview, illustrative station directory, GPS map view, charging-time/cost calculator, analytics, charging-session examples, transport profiles, and demo settings.

## Run the dashboard
Open `index.html` in a modern web browser. The map uses Leaflet and OpenStreetMap tiles, which require an internet connection. Live GPS requires browser location permission and a secure context (HTTPS or localhost).

## Project files
- `index.html` — main interactive dashboard.
- `data/demo_stations.csv` — illustrative station examples for documentation/testing.
- `docs/PROJECT_NOTES.md` — scope, features, and known limitations.
- `.gitignore` — common files to exclude from Git.

## Important limitations
- Station records, prices, queues, savings, analytics, and map pins shown in this prototype are illustrative demo data, not verified live charger data.
- The optimizer currently estimates required energy, approximate charging duration, and cost using entered values. It is a rule-based calculator, not a production-grade global scheduling solver.
- It does not control real chargers or connect to a live grid operator, payment system, or live station availability API.
- Verify the official TechForge challenge statement and dataset before claiming full challenge compliance.

## Suggested next steps
1. Confirm the official challenge requirements and evaluation metrics.
2. Replace demo station data with an approved dataset.
3. Separate HTML, CSS, and JavaScript into maintainable files if desired.
4. Add tests for energy/time/cost calculations and grid-capacity constraints.
5. Measure performance against a documented baseline and report only measured results.
