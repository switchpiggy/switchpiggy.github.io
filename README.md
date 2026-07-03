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

## Analytics

Every page loads [GoatCounter](https://www.goatcounter.com) (free, no cookies, so
no consent banner needed). Dashboard: **https://switchpiggy.goatcounter.com** —
shows pageviews, referrers, countries, and devices. It can't identify individual
visitors by name; no tool can.

One-time setup: sign up at goatcounter.com and register the code `switchpiggy`
(it must match the URL in the `<script data-goatcounter=...>` tag at the bottom
of each page — if that code is taken, pick another and update it in all three
HTML files).

Outbound links tagged with `data-goatcounter-click="some-name"` (see the contact
links in `index.html`) report each click as an event on the dashboard. Tag any
new external link the same way to track its clicks.

## Notes

- CDN caching means a change can take up to a minute to appear live — hard-refresh
  if you don't see it.
- All internal links are relative, so nothing breaks on the live domain.
- To add a custom domain: repo **Settings → Pages → Custom domain**, then add the
  matching DNS record with your registrar.
