# Ray Joseph — personal website

A single-page static academic-style site (no build tools). Just HTML + CSS.

```
ray-website/
├── index.html          ← all the content (edit here)
└── assets/
    ├── style.css        ← styling / colors
    ├── profile.jpg      ← YOUR photo (add this — see step 1)
    └── Ray_Joseph_CV.pdf ← your resume, linked as "CV"
```

## 1. Add your photo
Drop a square photo named **`profile.jpg`** into the `assets/` folder. (Until you do,
the avatar shows a blank placeholder — the site still works.)

## 2. Fill in your real links
Open `index.html` and search for `data-social` and `data-press`. Replace each
`href="#"` with your real URL:
- LinkedIn profile
- GitHub profile
- Google Scholar profile
- Forbes / press article links

## 3. Preview it locally (optional)
Double-click `index.html` — it opens in your browser. That's it. No server needed.

## 4. Put it on GitHub Pages (free hosting)

GitHub Pages serves a personal site at `https://<username>.github.io`. Steps:

1. **Make a GitHub account** at https://github.com (if you don't have one). Note your
   username — say it's `rayjoseph`.
2. **Create a new repository** named exactly **`<username>.github.io`**
   (e.g. `rayjoseph.github.io`). This exact name is what makes it your main site.
   Set it to **Public**.
3. **Upload the files.** Easiest way (no command line):
   - On the new repo page, click **“uploading an existing file.”**
   - Drag in `index.html`, the `assets/` folder, and `README.md`.
   - Click **Commit changes**.
4. **Wait ~1 minute**, then visit `https://<username>.github.io`. Done.

   (If it doesn't appear: repo **Settings → Pages** → set **Source = Deploy from a
   branch**, **Branch = main / (root)**, Save.)

### Command-line alternative (if you prefer)
From inside this folder:
```bash
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/<username>/<username>.github.io.git
git push -u origin main
```

## 5. Updating later
Edit `index.html`, then re-upload it (or `git commit` + `git push`). Changes go live
in about a minute.

## Custom domain (optional)
Buy a domain, then in repo **Settings → Pages → Custom domain** enter it and follow
the DNS instructions GitHub shows.
