# David Xiao — Profile Site

A static personal profile / résumé site. No build step: plain HTML + CSS.

| File | Purpose |
|---|---|
| `index.html` | All page content (edit text here) |
| `style.css` | Look and feel (accent color is `--accent` at the top) |
| `David-Xiao-Resume.pdf` | Downloadable résumé (exported from `David-Xiao-Resume.docx`) |

## Preview locally
Double-click `index.html`, or run `start index.html` in this folder.

## Publish on GitHub Pages
1. Sign in at https://github.com (create a free account if needed).
2. Create a new **public** repository named exactly `<your-username>.github.io`
   (leave "Add a README" unchecked).
3. In this folder run:
   ```
   git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
   git push -u origin main
   ```
   The first push opens a browser window to sign in to GitHub.
4. In the repo on GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   branch `main`, folder `/ (root)` → Save.
5. After 1–2 minutes the site is live at `https://<your-username>.github.io`.

## Updating later
Edit the files, then:
```
git add -A
git commit -m "Update profile"
git push
```
To refresh the PDF, export the Word résumé to PDF with the same file name.

## Optional: custom domain
Buy a domain (e.g. davidxiao.ca), then in **Settings → Pages → Custom domain** enter it and
follow GitHub's DNS instructions.
