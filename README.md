# Nova Drift: Horizon Rush

An original 3D arcade racing game built with three.js. Fictional cars, tracks and branding.
Single static page, no build step.

## Features
- Home screen, garage (3 cars, paint, credit upgrades), race HUD, results screen
- 3-lap race vs 4 AI rivals, countdown start, checkpoints, live positions, minimap
- Two tracks: Neon Harbor (rainy night city) and Sunset Coast (ocean, palms, lighthouse)
- Drifting, nitro, tire smoke, sparks, crash shake, speed lines, cinematic cameras
- Keyboard and touch controls; automatic resolution scaling and a no-WebGL message

## Controls
| Action | Keyboard | Touch |
|---|---|---|
| Accelerate / Brake | W / S or Up / Down | GAS / BRAKE |
| Steer | A / D or Left / Right | arrow buttons |
| Nitro | Space | NITRO |
| Drift | Shift | DRIFT |
| Mute engine | M | - |

## Run locally
Open `index.html` in a modern browser, or serve the folder:

```bash
python3 -m http.server 8080
# then visit http://localhost:8080
```

An internet connection is needed once for three.js (cdnjs) and the Orbitron font (Google Fonts).

## Deploy to GitHub Pages
1. Create a new GitHub repository and push these files to the `main` branch.
2. In the repo go to **Settings > Pages > Build and deployment > Source** and choose **GitHub Actions**.
3. The included workflow (`.github/workflows/pages.yml`) publishes the site on every push.
   Your game will be live at `https://<username>.github.io/<repo>/`.

```bash
git init && git add . && git commit -m "Nova Drift"
git branch -M main
git remote add origin https://github.com/<username>/<repo>.git
git push -u origin main
```
