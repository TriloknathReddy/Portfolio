# MyPortfolio

This is a Vite + React portfolio site ready for deployment.

Build locally:

```bash
npm install
npm run build
```

Deploy to Netlify:

- Option A (connect repo): In Netlify, create a new site from GitHub. Set build command `npm run build` and publish directory `dist`.
- Option B (drag & drop): Build locally then drag the `dist` folder to Netlify's drag-and-drop deploy area.

Files of interest:
- `netlify.toml` — Netlify build/publish settings and SPA redirect.
- `public/certificates/*` — certificate image assets.
- `public/resume/*` — resume PDF used by the site.

Useful local git commands to push to GitHub (run from project root):

```bash
# initialize and push
git init
git branch -M main
git add .
git commit -m "Initial commit: Deploy-ready portfolio with assets and netlify.toml"

# create remote and push (replace URL)
git remote add origin <YOUR_GITHUB_REPO_URL>
git push -u origin main
```

Or use GitHub CLI (if installed):

```bash
gh repo create <your-username>/<repo-name> --public --source=. --remote=origin --push
```

Once pushed, connect the repo to Netlify (build command `npm run build`, publish `dist`).
<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://ai.google.dev/static/site-assets/images/share-ais-513315318.png" />
</div>

# Run and deploy your AI Studio app

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio/apps/4d698bf8-a1f6-4ba8-86c6-84a7e4a8b8b4

## Run Locally

**Prerequisites:**  Node.js


1. Install dependencies:
   `npm install`
2. Set the `GEMINI_API_KEY` in [.env.local](.env.local) to your Gemini API key
3. Run the app:
   `npm run dev`
