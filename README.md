# drewhall-site

Static portfolio site. Plain HTML/CSS/JS, no build step.

## Files
- `index.html` — all content
- `styles.css` — styling (light and dark mode follow the visitor's system setting)
- `main.js` — mobile menu, header border on scroll, footer year
- `.nojekyll` — tells GitHub Pages to serve files as-is

## Publish on GitHub Pages
1. Create a new repo. Name it `<your-username>.github.io` if you want it at that address, or any name to get `<your-username>.github.io/<repo>`.
2. Upload these files to the root of the `main` branch.
3. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, pick `main` and `/ (root)`, then Save.
4. The site goes live in a minute or two at the URL shown on that page.

## Use your own domain (thedrewhall.com)
1. In **Settings → Pages → Custom domain**, enter `thedrewhall.com` and save. GitHub adds a `CNAME` file to the repo.
2. At your domain registrar, point DNS to GitHub Pages:
   - `A` records for `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` record for `www`: `<your-username>.github.io`
3. Once DNS resolves, tick **Enforce HTTPS**.

Check GitHub's Pages docs for current IPs before changing DNS.

## Editing
- Placeholders are marked `<!-- TODO -->` in `index.html` (Avant dates/title, contact links, extra coursework).
- **Projects** and **Writing** are built but hidden. To show them, remove the `hidden` attribute from both the nav link and the section.
