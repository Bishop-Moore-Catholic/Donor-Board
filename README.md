# Donor Board (D3-cloud basic, no animations)

- `admin.html`: now accepts newline, comma **and tab** separated names (deduped).
- `display.html`: returns to the basic d3-cloud layout, **no animations**, **no center image**. Also sets `viewBox` and correct center translation to avoid the "stuck in the corner" issue.

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
