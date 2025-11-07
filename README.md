# Donor Board (Admin SyntaxError fix + better parsing)

**Fixes**
- Removed problematic template/escape usage in `admin.html` (now DOM-builds chips).
- Robust delimiter parsing using `new RegExp('[,\t\r\n]+','g')`.
- Persistent event delegation for chip actions (no `{ once:true }` pitfall).

**Display**
- Same d3-cloud streaming + padded layout as previous package.

## Run locally
```bash
python3 -m http.server 5500
# http://localhost:5500/admin.html
# http://localhost:5500/display.html
```
