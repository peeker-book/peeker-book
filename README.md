# Peeker — book landing page

This folder contains one file: `index.html`. It's a complete, self-contained
web page (images included) for the book *Peeker*. Publishing it on GitHub
Pages turns it into a free, permanent URL you can text or post anywhere.

## What you need
- A free GitHub account: https://github.com/join
- The `index.html` file from this download

## Option A — no command line (easiest)

1. Go to https://github.com/new and create a new repository.
   - Name it something like `peeker-book`
   - Set it to **Public** (Pages requires this on free accounts)
   - Don't add a README/gitignore/license — leave it empty
   - Click **Create repository**
2. On the new repo's page, click **"uploading an existing file"**
   (or the **Add file → Upload files** button).
3. Drag `index.html` into the upload box, then click **Commit changes**.
4. Go to the repo's **Settings** tab → **Pages** (left sidebar).
5. Under "Build and deployment," set **Source** to **Deploy from a branch**,
   branch **main**, folder **/ (root)**, then **Save**.
6. Wait about 1 minute, then refresh the page. GitHub will show your live
   URL, something like:

   ```
   https://YOUR-USERNAME.github.io/peeker-book/
   ```

That URL is what you share/text — it will always point at the current
version of `index.html` in the repo.

## Option B — command line (git)

From the folder containing `index.html`:

```bash
git init
git add index.html
git commit -m "Add Peeker landing page"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/peeker-book.git
git push -u origin main
```

Then enable Pages the same way as step 4–5 above (Settings → Pages →
Deploy from branch → main → / root → Save).

## Updating the page later

- **Option A:** Settings aside, just open the file in the repo on GitHub,
  click the pencil (edit) icon, paste in the new version, and commit.
  Or delete and re-upload.
- **Option B:** Edit `index.html` locally, then:
  ```bash
  git add index.html
  git commit -m "Update page"
  git push
  ```
  The live URL updates automatically within a minute or two.

## Notes
- Because everything (cover images, styling) is embedded directly in
  `index.html`, this is the only file you need — no extra assets to upload.
- The file is fairly large (~500KB) because of the embedded cover images;
  that's normal and GitHub Pages has no problem serving it.
- If you'd rather use a different free host (Netlify, Vercel, Cloudflare
  Pages), the same `index.html` file works there too — most of them let
  you connect the same GitHub repo with a couple of clicks.
