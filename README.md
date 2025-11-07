# Donor Board (dense packing + no overlaps)

**What’s new**
- **Max 300 names** (configurable via `?max=NNN`, capped 300).
- **Bias**: `?bias=larger|balanced|denser` (default balanced). This sets the placement acceptance ratio (80%, 95%, 97%).  
- **Adaptive attempts** down to 0.70 font scale & padding.
- **Accurate text measurement** using an offscreen canvas to estimate true label widths.
- **Quadtree collision resolution** pass ensures *no overlaps* while keeping a dense look.
- Keeps **seeded RNG** and **rectangular spiral**.

**Run**
```
python3 -m http.server 5500
# open admin.html and display.html
# for maximal density:
# http://localhost:5500/display.html?bias=denser&max=300
```
