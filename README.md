# Dr. Harish Chandra Verma — Tribute Site

A single-page tribute site for your brother, built as a plain static site
(`index.html` + `style.css` + `script.js` + `images/`). No build tools, no
dependencies — this means it works immediately on Vercel with zero config,
which matters since you're deploying from your phone.

## What's inside
```
index.html     → page content
style.css      → all styling + animations
script.js      → scroll-reveal animation
images/        → the 8 photos, already renamed and referenced
```

## 1. Push it to GitHub from your phone

**Easiest option — GitHub mobile app:**
1. Open the GitHub app → tap **+** → **New repository**. Name it something
   like `harish-tribute`, keep it **Public**, and create it.
2. In the new repo, tap the **+** / **Add file** option and upload each file
   (`index.html`, `style.css`, `script.js`) one at a time.
3. For the `images` folder: GitHub's mobile app doesn't support folder
   upload well. Easiest fix — use GitHub's web upload in your phone's
   browser instead:
   - Go to `github.com/<your-username>/harish-tribute` in Chrome/Safari
   - Tap **Add file → Upload files**
   - Select all 8 images from your photos — GitHub will let you type the
     path `images/` before committing, or you can drag them into a folder
     if the mobile browser UI allows it. If it uploads them to the root
     instead, just rename each one afterward to `images/filename.jpg` using
     GitHub's "rename" (pencil) option on each file.
4. Commit each upload with a short message like "add site files."

**Alternative (if you get stuck on step 3):** request "desktop site" in
your mobile browser when on github.com — the drag-and-drop uploader works
much better in desktop mode, even on a phone.

## 2. Deploy on Vercel

1. Open the Vercel app or **vercel.com** in your mobile browser.
2. Sign in with your GitHub account.
3. Tap **Add New → Project**, then select the `harish-tribute` repo.
4. Framework preset: choose **Other** (it's a static site — no build
   command needed, no output directory needed).
5. Tap **Deploy**. It finishes in under a minute.
6. Vercel gives you a live URL like `harish-tribute.vercel.app` — that's
   your live site, shareable with anyone.

Every time you push a new commit to GitHub after this, Vercel redeploys
automatically.

## Customizing later
- Swap or add photos in `images/`, then update the matching `<img src="...">`
  line in `index.html`.
- Copy (the notes, the letter, the bio) all lives directly in `index.html` —
  search for the text you want to change and edit it there.
- Colors and fonts are defined once at the top of `style.css` under
  `:root { ... }` if you want to adjust the palette.
