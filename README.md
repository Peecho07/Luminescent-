# Luminescent website

Coffee by day, cocktails by night. Static site: one HTML file plus assets. No build step.

## Files
- `index.html` - the full site (styles and scripts included)
- `assets/luminescent-interior.jpg` - Our Story image
- `assets/favicon.svg` - browser tab icon

## Edit business details
Open `index.html` and find `const CONFIG` near the bottom. Hours, address, email, Instagram,
Google rating, happy hour and the form endpoint all live there.

Menu items live in `const MENU` right below it.

## Turn on the pop-up form
The form runs in demo mode until `FORM_ENDPOINT` has a value.
1. Create a form at formspree.io using the client's email.
2. Paste the endpoint URL into `FORM_ENDPOINT: ""`.
3. Commit. Submissions go straight to that inbox.

## Deploy
### Netlify (recommended)
1. Push this folder to a GitHub repo (index.html at the root).
2. Netlify > Add new site > Import from Git > pick the repo.
3. Build command: leave blank. Publish directory: `/`.
4. Deploy, then add the custom domain under Domain management.

### GitHub Pages
1. Repo > Settings > Pages.
2. Source: Deploy from a branch > `main` > `/ (root)`.
3. Save. The site goes live at `https://<username>.github.io/<repo>/`.
