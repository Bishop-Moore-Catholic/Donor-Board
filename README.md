# Donor Board — Themed build (Futura PT + global stylesheet)

**Global stylesheet**: `styles.css`
- Imports Adobe Fonts kit and applies **Futura PT** globally.
- Quick theming with CSS variables:
  - `--bg`, `--bg-image`
  - `--title-color`, `--title-size`, `--title-weight`
  - `--name-color`, `--name-weight`
  - `--emph-color`, `--emph-weight`, `--emph-scale`
  - Chip & button colors for the admin UI
- Title (`.db-title`) is **centered and larger**.

**Background image**
- Put a file in `assets/bg.jpg` and set in `:root`:
  ```css
  --bg-image: url('assets/bg.jpg') center/cover no-repeat fixed;
  ```

**Run**
```bash
python3 -m http.server 5500
# open admin.html and display.html
```
