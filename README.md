# Donor Board (d3-cloud)

Two-page donor recognition board using BroadcastChannel + localStorage and a d3-cloud word cloud on the display page.

## Files
- `admin.html` – paste/type names (deduped). Broadcasts updates to the display.
- `display.html` – renders a centered word cloud using [d3-cloud](https://github.com/jasondavies/d3-cloud). A 300×300 centerpiece image sits in the middle; words are nudged to avoid it. New names pop in near the center.

## Run locally
```bash
python3 -m http.server 5500
# http://localhost:5500/admin.html
# http://localhost:5500/display.html
```
Optional center image via URL: `display.html?img=URL_TO_IMAGE`

## Deploy on GitHub Pages
1. Push this folder to a repo (e.g., `donorboard`).
2. Settings → Pages → Deploy from branch (main / root).
3. Visit:
   - https://<user>.github.io/donorboard/admin.html
   - https://<user>.github.io/donorboard/display.html

## Notes
- End state font sizes are uniform; d3-cloud is used to position names without overlap.
- New names re-run the layout; those words get a CSS `pop` animation (scale down to 1).
- The centerpiece avoidance uses a simple nudge; in dense layouts a full re-layout may shift other words slightly.
