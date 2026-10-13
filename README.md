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

Pushing to `main` uploads the site to Hostinger over FTP with lftp
(`.github/workflows/deploy.yml`). It only touches files from this repo, so
other folders in `public_html` are left alone. Needs repo secrets
`FTP_SERVER`, `FTP_USERNAME`, `FTP_PASSWORD`.
