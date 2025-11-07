# Donor Board (Better padding + chip actions)

## New
- **D3-cloud dynamic padding**: uses a padding function based on font size and name length to reduce overlaps.
- **Chip hover actions**: hover any chip in `admin.html` to reveal two buttons:
  - ⭐ Emphasize — pulses the name once on the display.
  - 🗑️ Delete — removes the donor and updates the display.

## Use
- Serve locally:
  ```bash
  python3 -m http.server 5500
  # http://localhost:5500/admin.html
  # http://localhost:5500/display.html
  ```
- Deploy on GitHub Pages (root of repo).

## Notes
- Tweak the padding by editing `dynamicPadding()` in `display.html`.
- Emphasize reorders SVG to top (bring-to-front) and scales then returns to stored position.
