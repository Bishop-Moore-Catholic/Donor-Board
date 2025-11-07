# Donor Board (d3-cloud streaming updates)

- `display.html` streams words in during layout via the d3-cloud **`word`** event, then does a gentle reconcile on **`end`** so redraws aren't jarring.
- `admin.html` accepts newline, comma, and tab separated names; deduped case-insensitively.

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
