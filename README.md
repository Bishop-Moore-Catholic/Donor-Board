# Donor Board (d3-cloud streaming — FIXED)

Fixes:
- **Admin**: Template literals now evaluate correctly; chips show actual names (no `${...}`).
- **Display**: `viewBox` is set via string concat (prevents `${W} ${H}` parsing warning). Streaming render + safe keyed data join prevents the `d.text` null error.

## Run locally
```bash
python3 -m http.server 5500
# http://localhost:5500/admin.html
# http://localhost:5500/display.html
```

## GitHub Pages
Enable Pages on the repo and visit:
- https://<your-username>.github.io/<repo>/admin.html
- https://<your-username>.github.io/<repo>/display.html
