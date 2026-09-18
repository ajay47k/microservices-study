# Microservices Study Notes — static site

A single-page, client-side web app (no backend) built from `microservices.docx`. It renders the notes with a sticky contents sidebar, live search, light/dark themes, and all diagrams.

## Files

- `index.html` — the page (references `images/`).
- `images/` — the 18 diagrams.
- `.nojekyll` — tells GitHub Pages to serve every file as-is.

A single-file version (all images inlined into one `.html`, nothing external) can also be generated if you want a copy you can open by double-click with no server.

## Deploy to GitHub Pages (free, easiest)

1. Create a new repo on GitHub, e.g. `microservices-notes`.
2. From this `site/` folder:
   ```
   git init
   git add .
   git commit -m "Microservices study notes site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/microservices-notes.git
   git push -u origin main
   ```
3. On GitHub: **Settings -> Pages -> Build and deployment -> Source: Deploy from a branch**, pick `main` and `/ (root)`, Save.
4. Wait about a minute. Your site is live at `https://<your-username>.github.io/microservices-notes/`.

## Alternatives (also free, also drag-and-drop)

- **Netlify Drop** (app.netlify.com/drop): drag this `site/` folder onto the page, instant URL.
- **Cloudflare Pages** / **Vercel**: connect the repo, framework preset "None", output directory `/`.

All three are free for a static site this size. GitHub Pages is the simplest if the notes already live in a GitHub repo.
