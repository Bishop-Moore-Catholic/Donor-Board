# Donor Board

A browser-based donor recognition board that uses the BroadcastChannel API and localStorage.

## Usage

- `admin.html` — enter names (deduped, case-insensitive).
- `display.html` — projector page showing the live word cloud.

## Run locally

```bash
python3 -m http.server 5500
# then visit:
# http://localhost:5500/admin.html
# http://localhost:5500/display.html
```

## Deploy on GitHub Pages

1. Push this folder to a repo (e.g., `donorboard`).
2. Enable GitHub Pages (Settings → Pages → Deploy from branch → main → root).
3. Visit:
   - https://yourusername.github.io/donorboard/admin.html
   - https://yourusername.github.io/donorboard/display.html
