# Aevum Intelligence — Landing Page

Static landing page for Aevum Intelligence LLC, hosted via GitHub Pages.

## Files

- `index.html` — single-page site
- `styles.css` — styles
- `CNAME` — custom domain (edit or delete if not using one)

## Deploy to GitHub Pages

1. Create a new GitHub repo (e.g. `aevum-intelligence/aevum-intelligence.github.io`
   for a user/org site, or any repo name for a project site).
2. Push these files to the default branch:
   ```bash
   cd ~/aevum/githubPage
   git init
   git add .
   git commit -m "Initial landing page"
   git branch -M main
   git remote add origin git@github.com:<org>/<repo>.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Build and deployment**
   - Source: **Deploy from a branch**
   - Branch: `main` / `/ (root)`
4. (Optional) Set a custom domain in the `CNAME` file and configure DNS:
   - `CNAME` record: `www.aevumintelligence.com` → `<org>.github.io`
   - `A` records for apex: see GitHub Pages docs.

## Local preview

```bash
cd ~/aevum/githubPage
python3 -m http.server 8000
# open http://localhost:8000
```
