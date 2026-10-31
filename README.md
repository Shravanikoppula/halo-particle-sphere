# Halo — hand-controlled particle sphere

A 3D particle sphere (Three.js) steered by your hand via webcam (Google MediaPipe Hands). Open palm = explode, fist = collapse, move = steer. Falls back to mouse/touch if the camera is unavailable. All processing happens in your browser.

## Run locally
Camera access needs `localhost` or HTTPS (opening the file directly may be blocked).

```bash
python3 -m http.server 8000   # then open http://localhost:8000
```

## Push to GitHub
```bash
git init && git add . && git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo>.git
git push -u origin main
```

## Deploy (pick one, all free, all HTTPS)
- **GitHub Pages:** repo → Settings → Pages → Source: **GitHub Actions**. The included workflow deploys on every push to `main`. Live at `https://<user>.github.io/<repo>/`.
- **Vercel:** import the repo, framework "Other", no build command.
- **Netlify:** import the repo, no build command, publish directory `.`.

## Tech
Tailwind CSS 3.4.17 (CDN), Three.js r128, MediaPipe Hands 0.4.1675469240 — all version-pinned.

## License
MIT
