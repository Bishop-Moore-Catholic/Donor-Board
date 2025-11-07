# Donor Board (cap 350 + auto‑emphasize with '+')

**Admin**
- Adding names: include a `+` anywhere in a token to **auto‑emphasize** that donor.
  - `John +Doe`, `+Jane Smith`, `Family+Foundation` → all become emphasized.
  - `+` is stripped from the stored/displayed name.
- Emphasis is **persisted** and **broadcast** immediately.
- Chips for emphasized donors are **highlighted** (pale gold) with a ★ badge.
- Clear All clears donors **and** emphasis.

**Display**
- Default cap is **350** donors. You can change (or lift) it via `?max=NNNN` (soft cap 10k).
- Keeps dense packing, seeded RNG, quadtree collision resolution.

**Examples**
- `display.html?bias=denser&max=350`
- `display.html?bias=larger&max=500`

Run locally:
```bash
python3 -m http.server 5500
# open admin.html and display.html
```
