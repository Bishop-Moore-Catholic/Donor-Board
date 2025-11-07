# Donor Board (clear-emphasize + adaptive + seeded)

**Admin**
- `Clear All` now also clears **emphasized** names and sends a `clearEmph` broadcast.

**Display**
- Clears emphasized names on `reset`, `clearEmph`, and when removed individually.
- Adaptive sizing tries several (font, padding) combos; accepts when ≥85% placed (up to 400 cap).
- **Seeded RNG** for stable layouts (per viewport + count) and **rectangular** spiral for tighter packing.
- Keeps debug logs of totals and each attempt.

Run:
```bash
python3 -m http.server 5500
# open admin.html and display.html
```
