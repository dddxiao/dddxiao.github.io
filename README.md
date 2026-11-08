# David Xiao — Executive Profile Site

Live at **https://dddxiao.github.io**. A static site with no build step and no framework.
GitHub Pages serves the `main` branch from the repository root.

| File | Purpose |
|---|---|
| `index.html` | All page content, SEO and Open Graph tags, structured data |
| `style.css` | Design: palette tokens at the top (light + dark), layout, print styles |
| `main.js` | ~2 KB of optional enhancements: mobile menu, active-section nav, scroll reveals, count-up metrics. The page works fully without it. |
| `David-Xiao-Resume.pdf` | Downloadable résumé (exported from the Word file) |
| `og-image.png` | 1200×627 preview image shown when the link is shared on LinkedIn |
| `robots.txt`, `sitemap.xml` | Search-engine hints |

## Preview locally
Double-click `index.html`.

## Change the profile photo
Overwrite `images/david-xiao.jpg` with a square or portrait headshot under 100 KB
(e.g. compress with https://squoosh.app, MozJPEG at quality ~75). The page crops it to 4:5.
If the new image isn't 550×550, update the `width`/`height` on the `<img>` in the hero of `index.html`.

## Publish changes
```
git add -A
git commit -m "Update profile"
git push
```
Live in about a minute.

## Refresh the LinkedIn preview
LinkedIn caches previews. After changing `og-image.png` or the title or description, paste the URL into
https://www.linkedin.com/post-inspector/ to refresh it.

## Optional: custom domain
Buy a domain (e.g. davidxiao.ca), then in **Settings → Pages → Custom domain** enter it and follow
GitHub's DNS instructions. Then update the `https://dddxiao.github.io/` URLs in `index.html`,
`robots.txt` and `sitemap.xml`.
