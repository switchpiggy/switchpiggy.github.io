# Personal site

Static personal site for Alan Xiao, hosted on GitHub Pages.

**Live:** https://switchpiggy.github.io/

## Current state

The site is currently a single "work in progress" placeholder (`index.html`,
self-contained, no stylesheet or analytics). The previous full site is preserved
in git history and tagged `old-site`.

### Restoring the old site

```bash
git checkout old-site -- index.html blog.html post-empirical-likelihood.html style.css README.md
git commit -m "Restore site"
git push
```

## Editing

No build step, no dependencies — just static HTML/CSS.

```bash
git add -A
git commit -m "describe your change"
git push
```

Pages redeploys automatically within ~30–60s of each push. To preview before
committing, just open `index.html` in a browser.

## Notes

- CDN caching means a change can take up to a minute to appear live — hard-refresh
  if you don't see it.
- GoatCounter analytics (dashboard: https://switchpiggy.goatcounter.com) was on
  every page of the old site; re-add the `<script data-goatcounter=...>` tag when
  the full site returns. See the `old-site` tag for the exact snippet.
- To add a custom domain: repo **Settings → Pages → Custom domain**, then add the
  matching DNS record with your registrar.
