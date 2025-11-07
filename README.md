# Donor Board — Admin-controlled Theme (push to Display)

**How it works**
- The **admin page** now includes a Theme panel for the *display*.
- When you click **Apply & Push**, the theme is saved to `localStorage` as `donorTheme.v1`
  **and** broadcast to the display via `BroadcastChannel('donors')` with `{ type: 'themeUpdate', theme }`.
- The **display page** listens for `themeUpdate`, applies the theme (CSS variables + background image), persists it, and reflows the cloud (so no collisions after weight/scale changes).

**What you can control from Admin**
- Background color (+ optional background image upload)
- Title color
- Name color & font-weight
- Emphasized color & font-weight
- Emphasized scale

**Defaults**
- `styles.css` defines default variables and loads **Futura PT** via your Adobe kit.

**Run locally**
```bash
python3 -m http.server 5500
# open admin.html and display.html
```
