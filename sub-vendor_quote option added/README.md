# Mazillo — Navtek Marine Services (Enquiry → Balance Sheet)

Latest build, ready to deploy as a static site (e.g. **GitHub Pages**).

## Files
| File | Purpose |
|---|---|
| `index.html` | The application (Enquiry → Quotation → Order → Invoice → Balance Sheet). Entry point. |
| `Navtek Product Document.dc.html` | The Product Operations Document, shown inside the app's **Help** tab and openable on its own. |
| `support.js` | Runtime required by both HTML files. |
| `navtek-logo.jpeg` | Logo used in the app login + sidebar. |

> Keep all files together in the same folder — the app loads `support.js`, the logo, and the Help document by relative path.

## Deploy on GitHub Pages
1. Create a new repository and add **all files in this folder** to its root (keep the file names exactly as-is).
2. Push to GitHub.
3. Repo **Settings → Pages** → Source: *Deploy from a branch* → Branch: `main` / root → **Save**.
4. After a minute the site is live at `https://<user>.github.io/<repo>/`.

The app opens at the root URL (`index.html`). The **Help** tab embeds the product document so any user can read it inside the app.

## Notes
- Data is stored per-browser (localStorage). Use **Settings → User Management → Data Backup &amp; Restore** to move data between machines.
- An internet connection is only needed the first time, to load the IBM Plex fonts.
