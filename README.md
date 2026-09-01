# mylesgoins.com

Personal site + blog. Jekyll on GitHub Pages, Flexoki colors, no build tools needed on your machine.

## Publishing a new post

1. Create a file in `_posts/` named `YYYY-MM-DD-short-title.md` (the date controls ordering; the title part becomes the URL).
2. Start it with front matter, then write markdown:

   ```
   ---
   layout: post
   title: "Your actual title"
   ---

   First paragraph doubles as the excerpt.
   ```

3. Commit/push (or paste it into GitHub's web editor). The site rebuilds automatically in ~1 minute — homepage list, archive, and RSS all update themselves.

## One-time setup (already done or documented in chat)

- Repo Settings → Pages → deploy from `main` branch, `/ (root)`.
- Custom domain `mylesgoins.com` (the `CNAME` file in this repo handles the domain claim; DNS lives at Cloudflare).
- "Enforce HTTPS" checked once the certificate is issued.

## Structure

```
_config.yml         site settings (title, description, plugins)
_layouts/           page skeletons (default = header/footer/theme, post = article)
_posts/             one markdown file per post
assets/css/style.css   all styling; Flexoki palette variables at the top
index.html          homepage (bio + recent posts)
writing.html        archive of all posts by year
about.md            about page
CNAME               custom domain for GitHub Pages
```

## Local preview (optional, not required)

With Ruby installed: `bundle install && bundle exec jekyll serve`, then open http://localhost:4000. Pushing to GitHub is the only thing that's actually necessary.
