# Donor Board (Click menus + vertical spacing + scaling)

**Admin**
- Tooltip replaced with **click-to-open menu** (stays open until you click elsewhere).
- Larger buttons and **centered glyphs** (flexbox).

**Display**
- Adds **more vertical separation** in a post-layout relaxation pass that prioritizes Y movement.
- **Dynamic font scaling**: after 50 names, size scales down linearly to 65% at 250 names.
- Keeps streaming-in animation and persistent emphasize toggle.

Tune spacing in `display.html`:
- `dynamicPadding()` – increases base padding
- `relaxPositions()` – adjust `passes`, `pushY`, `minRowGap`

Run locally:
```bash
python3 -m http.server 5500
# http://localhost:5500/admin.html
# http://localhost:5500/display.html
```
