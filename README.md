# haltriedman.com

Plain HTML. No build step, no JavaScript, no framework.

- `index.html` — the whole site
- `resume.pdf` — CV (replace this file to update it)
- `style.css` — the only styling
- `papers/` — old PDFs
- `.htaccess` — redirects from the old WordPress URLs

## Editing

Open `index.html` in a text editor. To post an update, add a line to the top
of the "Recent updates" list. Bump the "Last updated" line at the bottom.

Preview locally: `open index.html`

## Deploying

Pushing to `main` deploys to Hostinger (hPanel → Websites → Advanced → Git,
with Auto Deployment webhook added to this repo's GitHub webhooks).
