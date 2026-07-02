# wenwen-site

Personal academic website for Wen Wen, Associate Professor at the McCombs School of Business, UT Austin. Migrated from Google Sites to a static site suitable for GitHub Pages.

## Files
- `index.html` — About / bio page
- `research.html` — Publications (journal articles + working papers)
- `styles.css` — Shared styles
- `script.js` — Mobile nav toggle + footer year

## Deploy to GitHub Pages

1. **Create a repository on GitHub.**
   - Go to github.com → New repository.
   - If you want the site at `https://<your-username>.github.io`, name the repo exactly `<your-username>.github.io`.
   - Otherwise, name it anything (e.g. `wenwen-site`) — your site will be published at `https://<your-username>.github.io/<repo-name>/`.

2. **Upload these files to the repo.**
   - Easiest way: on the repo's GitHub page, click **Add file → Upload files**, drag in `index.html`, `research.html`, `styles.css`, `script.js`, and drop them at the root of the repo (not inside a subfolder). Commit.
   - Or, from a terminal with git installed:
     ```
     git init
     git add .
     git commit -m "Initial site"
     git branch -M main
     git remote add origin https://github.com/<your-username>/<repo-name>.git
     git push -u origin main
     ```

3. **Turn on GitHub Pages.**
   - In the repo, go to **Settings → Pages**.
   - Under "Build and deployment," set **Source** to `Deploy from a branch`.
   - Set **Branch** to `main` and folder to `/ (root)`. Save.
   - GitHub will give you the live URL within a minute or two (Settings → Pages will show it, and also under the repo's "Environments" / a green checkmark on the commit).

4. **(Optional) Custom domain.**
   - If you want a custom domain instead of the github.io URL, add a `CNAME` file with your domain name, and configure your domain's DNS to point at GitHub Pages (see GitHub's "Managing a custom domain" docs).

## Updating content later
Just edit `index.html` / `research.html` (plain HTML — publications are list items inside `<ul class="pub-list">`), commit, and push. GitHub Pages redeploys automatically.
