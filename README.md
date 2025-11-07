# Donor Board — Chip Click Fix

- Added a dedicated **⋯ handle** on each chip to open/close its menu.
- Switched to event delegation on `#chips` for reliable click routing.
- Ensured SVG icons don't swallow clicks via `pointer-events: none` on `svg`.
- Added console logs for actions (`[chips]` and `[theme]`) to help debug.

Everything else remains the same (theme push from admin, display applies & persists).
