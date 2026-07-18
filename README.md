# Free Gift Card CPA Landing Page

A single-file, high-conversion CPA gift card landing page. All HTML, CSS, and
JavaScript are inline in one file — no build step, no dependencies.

## Files
- `index.html` — the landing page (GitHub Pages serves this automatically)
- `generator.html` — identical copy (open directly in any browser)

## What it does
1. Shows a grid of 20 gift-card brands with urgency + social proof.
2. Tapping any card plays a branded loading animation.
3. On completion it opens the CPA content locker (singingfiles.com id=1903196)
   inside a fullscreen iframe so the locker's `document.write()` runs correctly.

Images load remotely from `getagiftcards.com`, so the single HTML file works
anywhere with no extra assets.

## Deploy to GitHub Pages
1. Create a new GitHub repo and upload `index.html` (and optionally `generator.html`).
2. Repo **Settings → Pages → Source: Deploy from branch → main / root → Save**.
3. Your site goes live at `https://<username>.github.io/<repo>/` in ~1 minute.

## Change the content locker
Edit the `LOCKER_SRC` value in the `<script>` near the bottom of the HTML.

## Change gift cards / values
Edit the `CARDS` array in the same script block (name, file, value, claimed count, color).
