# Functional Vision Lab — Website

Website for the Functional Vision Lab at IIT Gandhinagar, led by Dr. Mahalakshmi Ramamurthy.

Live site: https://functionalvisionlab.com

## What this is

A single-file static website. Everything — HTML, CSS, JavaScript, and images (base64-encoded) — lives in `index.html`. No build step, no dependencies. It's a single-page app: navigation between "pages" happens via JavaScript that shows/hides `<div class="page">` sections.

## Hosting

- **Hosting:** [Netlify](https://netlify.com) (free tier)
- **Domain:** `functionalvisionlab.com`, registered at Namecheap, DNS pointed at Netlify
- **Contact form:** Netlify Forms — submissions appear in the Netlify dashboard under Forms → `contact`, and are emailed to `zz.maha@gmail.com`

## How to edit

1. Open `index.html` in any text editor (VS Code, Sublime, even TextEdit).
2. Make your changes.
3. Save.
4. Preview locally by double-clicking `index.html` — it opens in your browser with no server needed.

Common edits:

- **Text content (bio, news, publications):** search the file for the text you want to change.
- **Images:** images are embedded as base64 data URLs. To replace one, convert the new image to base64 (e.g. via https://base64.guru/converter/encode/image) and replace the existing `data:image/...` string.
- **Contact form recipients:** change the notification email in the Netlify dashboard → Site settings → Forms → Form notifications.

## How to deploy changes

```
git add index.html
git commit -m "describe what changed"
git push
```

Netlify watches the `main` branch. It auto-deploys within ~1 minute of a push. Check the Netlify dashboard for deploy status.

## Files

- `index.html` — the entire site
- `README.md` — this file
- `.gitignore` — files git should ignore (OS/editor junk)
