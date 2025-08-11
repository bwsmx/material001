# People Counter (Material)

## Overview
A zero-training, offline-first people counter for events. Supports multiple counters (e.g., Main Entrance, Terrace Stairs), per-counter capacity/lockout, offline queue + optional sync to a Google Apps Script endpoint. CSV export included.

## Live URL
https://bwsmx.github.io/material001/

## Run locally
```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Configure
Open the ⚙️ menu (PIN 1234) to add counters, set capacity, or configure an optional Google Apps Script endpoint.

## Privacy
All data is stored locally in your browser. If you configure an endpoint, counts are queued locally and sent to that endpoint when online.

## Deployment
Static HTML; host index.html on any static file server. Pushes to the `main` branch are automatically deployed to GitHub Pages.

