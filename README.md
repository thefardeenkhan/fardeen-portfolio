# Portfolio Deployment

This folder is ready to deploy as a static website.

## What is included

- `index.html` — the portfolio page
- `Profile/`, `designs/`, `music/`, `photos/`, `videos/` — asset folders
- `.nojekyll` — prevents GitHub Pages from skipping files because of Jekyll
- `.gitignore` — ignores system files like `.DS_Store`

## Recommended free deployment options

### Option 1: GitHub Pages (best for static sites)

1. Create a GitHub account if you do not have one.
2. Create a new repository named e.g. `fardeen-portfolio`.
3. Upload all files and folders from this `portfolio-assets` folder.
4. In the repository settings, open `Pages`:
   - Branch: `main`
   - Folder: `/ (root)`
   - Save.
5. GitHub will publish your site at `https://<username>.github.io/<repo>/`.

### Option 2: Cloudflare Pages (also free and very fast)

1. Create a Cloudflare account.
2. Create a new Pages project.
3. Connect your GitHub repository or upload the site manually.
4. Set the build command to blank and the build output directory to `/`.
5. Deploy.

## Performance tips

- `index.html` now uses `loading="lazy"` for images and `preload="none"` for videos so the page loads faster on mobile.
- Keep the page root structure exactly like this repository so asset paths stay correct.
- If the site still loads slowly, compress large image and video files before deployment.

## Notes

- The site will work even when your computer is off once it is deployed to GitHub Pages or Cloudflare Pages.
- Do not use Netlify if you prefer a faster setup and fewer upload delays.
