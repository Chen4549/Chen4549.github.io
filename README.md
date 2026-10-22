# Neil (Hsuan-Chih) Chen — personal website

A single static page (`index.html`), no build step. Hosted on GitHub Pages.

## Edit content

Everything is in `index.html`:

- **Headshot**: put your photo at `images/headshot.jpg`, then replace the
  `<div class="portrait glass" ...>...</div>` block with
  `<img class="portrait glass" src="images/headshot.jpg" alt="Neil Chen" style="object-fit:cover">`.
- **CV**: the CV button links to `CV.pdf` in the repo root; replace that file to
  update it.
- **GitHub button**: commented out in the hero section (search for `Add links here`).
  Fill in the URL and remove the `<!--` `-->`.
- **Publications**: each project is one `<article class="pub">` block. Status
  pill classes: `s-rev` (under revision), `s-prep` (in preparation), `s-run` (ongoing).

Preview locally by double-clicking `index.html`.

## Publish on GitHub Pages (first time)

1. Create a GitHub account if needed, then create a **new public repository** named
   exactly `<your-username>.github.io` (no README, no license).
2. In this folder, run:
   ```
   git init -b main
   git add .
   git commit -m "Personal website"
   git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
   git push -u origin main
   ```
3. On GitHub: repository **Settings → Pages → Build and deployment**, set Source to
   **Deploy from a branch**, branch `main`, folder `/ (root)`, Save.
4. After a minute the site is live at `https://<your-username>.github.io`.

## Update later

```
git add .
git commit -m "Update site"
git push
```
