# FEA Lab Admin Portal — GitHub Pages

Includes the 16 supplied students and random allocation into groups P, Q, R and S (exactly four students per group).

## Files
- `index.html` — portal interface
- `app.js` — student roster, allocation logic and password configuration

## Publish
1. Create a new GitHub repository, for example `fea-lab-portal`.
2. Upload `index.html` and `app.js` to the repository root.
3. Open **Settings → Pages**.
4. Select **Deploy from a branch**, branch `main`, folder `/ (root)`, then Save.
5. GitHub will show the published URL, typically `https://YOUR-USERNAME.github.io/fea-lab-portal/`.

## Change the initial password
Edit `ADMIN_PASSWORD` at the top of `app.js` before uploading. Initial value: `FEAAdmin2026!`.

## Important security limitation
GitHub Pages is static hosting. A password embedded in JavaScript is visible to anyone who inspects the site's source, so this is only a convenience gate and does not provide genuine admin-only security. For real access control, use server-side authentication (e.g. Firebase Authentication or Supabase Auth) and protected data storage. The roster is also public in the static source.

## Data
Allocation is saved in browser localStorage and is not shared across devices. Download CSV or print/save as PDF for a durable copy.
