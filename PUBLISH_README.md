How to share `qr.html` so it loads on every device
-------------------------------------------------

Two simple hosting options are listed below. Pick one and follow the steps — both are free and serve static sites reliably.

Option A — GitHub Pages (recommended for version control)
1. Create a new GitHub repository (public) named e.g. `invitation`.
2. Copy your files (`qr.html`, `index.html`, `office-photo.jpeg`, any fonts or assets) into the repo root.
3. Commit and push to GitHub.
4. In the repo Settings → Pages, set the Source to the `main` branch and `/ (root)` folder, then Save.
5. Your site will publish at `https://<your-username>.github.io/<repo>/` within a minute. Share that URL.

Quick commands (Git must be installed):
```
git init
git add .
git commit -m "Add invitation"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo>.git
git push -u origin main
```

Option B — Netlify (drag-and-drop, easiest)
1. Go to https://app.netlify.com/drop
2. Drag the folder containing `qr.html` and `index.html` into the page.
3. Netlify uploads and gives you a live URL instantly. You can rename the site and set a custom domain if desired.

Notes & tips
- Ensure `index.html` and `qr.html` are in the same folder and use relative paths (the launcher uses `href="qr.html"`).
- If you reference local fonts, consider using Google Fonts links instead so they always load.
- Test on mobile: open the published URL in an incognito mobile browser to confirm assets load.
- If you want me to create a GitHub repo and push the files for you, I can generate the repo contents and show the exact git commands — you'll need to paste a personal access token when pushing.

If you want, I can: (A) prepare a ZIP of the site ready to upload, (B) create the GitHub repo files and instructions, or (C) walk you through Netlify step-by-step. Which do you prefer?
