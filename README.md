# Blockchain Explorer – Audited Ledger (Static Demo) — Custom Domain Variant

This folder is identical but includes a `CNAME` file for the custom domain: `www.blockchain-simulation.com`.

## How to publish (with custom domain)
1. Push these files to a public repo.
2. In **Settings → Pages**, set **Source → Deploy from a branch** (Branch `main`, Folder `/ (root)`) and under **Custom domain**, enter `www.blockchain-simulation.com` and save.
3. At your DNS provider, create:
   - **CNAME** for `www` → `<your-username>.github.io` (exactly).
   - **A** records for apex `blockchain-simulation.com` → GitHub Pages IPs (optional but recommended for root domain redirect).
4. After DNS propagates, return to **Settings → Pages** and **Enforce HTTPS**.

Files included:
- `index.html` — explorer UI (self‑contained HTML, CSS, JS).
- `CNAME` — `www.blockchain-simulation.com`
- `.nojekyll` — disables Jekyll so assets load as-is.
- `404.html` — fallback page.