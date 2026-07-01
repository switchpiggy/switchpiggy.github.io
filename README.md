# Personal site

Static personal site for Alan Xiao, hosted on GitHub Pages.

**Live:** https://switchpiggy.github.io/

## Files

| File | Purpose |
| --- | --- |
| `index.html` | Landing page (intro, work, classes, links) |
| `blog.html` | Writing index |
| `post-empirical-likelihood.html` | A blog post |
| `style.css` | All styling |

No build step, no dependencies — just static HTML/CSS.

## Editing

### Locally (recommended)

```bash
git add -A
git commit -m "describe your change"
git push
```

Pages redeploys automatically within ~30–60s of each push. To preview before
committing, just open `index.html` in a browser.

### In the browser (quick tweaks)

On GitHub, open any file → pencil icon → edit → **Commit changes**. It redeploys
on save, and every change is versioned so you can always roll back.

## Notes

- CDN caching means a change can take up to a minute to appear live — hard-refresh
  if you don't see it.
- All internal links are relative, so nothing breaks on the live domain.
- To add a custom domain: repo **Settings → Pages → Custom domain**, then add the
  matching DNS record with your registrar.
