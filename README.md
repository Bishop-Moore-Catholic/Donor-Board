# Donor Board (adaptive sizing + single-flight)

- **display.html**: Adaptive loop tries smaller font/padding if too few words placed. Logs each attempt with font size, pad scale, and words placed.
- Prevents overlapping concurrent layouts with a single-flight guard.
- Still keeps emphasize toggle + vertical relaxation.
- **admin.html**: `.action-btn` width removed per request.

Check your console for lines like:

```
[DonorBoard] total donors: 180
[DonorBoard] attempt 1 fontPx 28.0 padScale 1 placed 72
[DonorBoard] attempt 2 fontPx 25.2 padScale 0.95 placed 121
[DonorBoard] attempt 3 fontPx 23.0 padScale 0.9 placed 156
```
