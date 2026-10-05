# SCROLL

A TikTok/Reels-style short-video app prototype for the cloud computing assignment.

## Contents
- `index.html` — the single-page app (mobile phone frame, endless feed, sign-in, upload)
- `logo.jpeg` — app logo
- `videos/` — sample clips used in the feed

## Run locally
Just open `index.html` in a browser. For file-upload to work reliably, serve the folder:
```
npx serve .
# or
python -m http.server 8000
```

## Deploy to GitHub Pages
1. Create a new GitHub repository (e.g. `scroll`).
2. Copy **everything in this folder** (`index.html`, `logo.jpeg`, `videos/`) into the repo root.
3. Commit and push.
4. Repo → Settings → Pages → Source: `Deploy from a branch` → Branch: `main` → `/ (root)`.
5. Your site is live at `https://<username>.github.io/<repo>/`.

Note: GitHub Pages is static hosting — the Floci backend, SQS worker, and DynamoDB demo
from `tiktok-demo/` run locally only and are not part of the deployed site.
