# Donor Board — CSV Import + Threshold Emphasize

**New on Admin**
- Drag‑and‑drop (or browse) a **OneCause CSV**.
- We parse **Column B** (amount) and **Column M** (name).
- Set an **emphasize threshold** (default **$1000**). Anyone with amount ≥ threshold is auto‑emphasized.
- Keep using the existing textarea — both inputs work together. Duplicates are ignored.

**How to use**
1. Open **admin.html**.
2. Drop your `.csv` onto the dashed box (or click **Browse…**).
3. (Optional) adjust **threshold**.
4. Click **Preview first 10** to verify (check console), or **Import all rows**.
5. Display updates live via `BroadcastChannel`.

**Notes**
- Currency like `$1,234.56` is parsed automatically.
- Header rows are skipped.
- Everything else remains: chip menu/actions, `+` emphasize in text input, theme push to display, collision‑reduced cloud with cap 350.
