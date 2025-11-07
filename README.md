# Donor Board (stable layout fix + scaling)

**Admin**
- Click-to-open chip menus (centered glyphs), emphasize/delete controls.

**Display**
- Rebuilt for stability: synchronous d3-cloud layout (no `timeInterval`/streaming).
- Smooth transitions on redraw; positions relax vertically to reduce overlaps.
- Font auto-scales after 50 names (down to ~60% by 250 names).
- Emphasize toggles persist via `localStorage` and survive redraws.

Run locally:
```bash
python3 -m http.server 5500
# http://localhost:5500/admin.html
# http://localhost:5500/display.html
```
