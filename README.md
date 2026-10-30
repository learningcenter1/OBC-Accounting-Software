# OBC Indonesia ERP

Single-file ERP (`index.html`) hosted on GitHub Pages.

## Deploy
1. Create a **private** GitHub repo (e.g. `obc-erp`) and push these files to `main`.
2. Repo → **Settings → Pages → Build and deployment → Source: GitHub Actions**.
3. After the workflow finishes, open `https://<your-username>.github.io/obc-erp/`.

> Note: GitHub Pages sites are public by default, even from private repos, unless your
> plan supports private Pages. Anyone with the URL can load the app (login screen
> only, no data is in the file unless you auto-save into it). Do NOT commit a
> file containing real company data, and do not commit backup `.json` files.

## Important: where data lives
Data is stored in **each browser's IndexedDB** on each device. It is NOT shared
between users or devices. Two staff opening the URL will see two separate databases.
- Back up regularly: Settings → Backup & Restore → Download Backup.
- Restore a backup on another device with the same screen (admin only).
- "Automatic Saving" writes into a local file you pick; it does not write to GitHub.

## Default logins (change immediately)
- admin / admin123
- user / user123

## Updating the app
Edit `index.html`, commit to `main`; the workflow redeploys automatically.
Clearing browser site data erases local data, so back up first.
