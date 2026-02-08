# Valentines Game — Sliding Puzzle

This is a small static sliding-puzzle page. It expects two optional image files placed next to the HTML:

- `puzzle.jpg` — the square image used for the puzzle (default path `./puzzle.jpg`).
- `prize.png` — the image downloaded when the puzzle is completed (default `./prize.png`).

How to run locally

1. Quick (open file): double-click `index.html` in File Explorer. This opens as `file://` — good for quick checks.
2. Recommended (local server):

```powershell
Set-Location -Path 'd:\Personal\Coding\Valentines Game'
python -m http.server 8000
# Then open: http://localhost:8000/index.html
```

Host on GitHub Pages

1. Rename `Untitled-1.html` → `index.html` (already done).
2. Commit and push to a GitHub repo, then enable Pages from the `main` branch → `/ (root)`.

Netlify (drag-and-drop)

1. Zip the folder contents (or use the ZIP included: `valentines-game-netlify.zip`).
2. Drag the zip into Netlify Sites → "Drag & drop your site output folder here".

Vercel (CLI)

```powershell
npm i -g vercel
Set-Location -Path 'd:\Personal\Coding\Valentines Game'
vercel
# follow the prompts
```

Git commands (prepare & push)

Run these locally to create a repo and push (replace the remote URL):

```powershell
Set-Location -Path 'd:\Personal\Coding\Valentines Game'
git init
git add .
git commit -m "Initial puzzle site"
# Add remote and push (replace URL):
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git branch -M main
git push -u origin main
```

Notes

- Use a square image for `puzzle.jpg` (e.g., 600×600) for best results.
- Serve via HTTP/HTTPS for reliable downloads and cross-origin behavior.
- If you want me to push to your GitHub repo, provide the repo URL and confirm and I can run the push commands here.
