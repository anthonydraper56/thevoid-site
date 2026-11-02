# The Void — website

Static site. Three files, no build step.

- index.html — landing page
- archive.html — every issue + contents
- books.html — books
- submit.html — submission guidelines

## Deploying (GitHub + Vercel)

1. Create a new GitHub repo (e.g. `thevoid-site`) and upload these files to the repo root.
2. Go to vercel.com, "Add New… → Project", import the repo.
3. Framework preset: **Other**. Leave build command and output directory empty. Deploy.
4. Add your domain under Project → Settings → Domains, and follow the DNS instructions.

Every push to `main` redeploys automatically.

## Updating each quarter

Ask Claude to update the source design files, re-bundle, and replace these three files in the repo (GitHub web UI: "Add file → Upload files", overwrite, commit). Vercel redeploys in ~30 seconds.

## Share previews (Open Graph)

Each page carries its own `<title>`, description, favicon, and Open Graph / Twitter card tags pointing at `og.png`. These use absolute URLs on `https://welcometothevoid.net` — if the live domain changes, the `og:*` URLs in each HTML file must be updated to match, or link previews will break.

`og.png` (1200×630) and `favicon.png` must sit in the repo root alongside the HTML files.

Caching: X, iMessage, Slack, and Substack cache previews aggressively. After deploying, re-scrape with a debugger (e.g. cards-dev.twitter.com/validator, developers.facebook.com/tools/debug) or append `?v=2` to the URL once to force a fresh fetch.
