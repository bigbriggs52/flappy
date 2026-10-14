# Flappy

A simple Flappy Bird-style game that runs in any browser, built to be played on a phone.

## Play

Open `index.html` in a browser, or host it with GitHub Pages (see below).

**Controls**
- Phone: tap the screen to flap
- Desktop: click, or press Space / Up Arrow

**Scoring**
- Each pipe you fly past is +1
- Your best score is saved on the device

## Host on GitHub Pages

1. Create a new repository on GitHub (for example, `flappy`).
2. Upload `index.html` and `README.md` to the repository root, or push them with git:
   ```bash
   git init
   git add .
   git commit -m "Add Flappy game"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/flappy.git
   git push -u origin main
   ```
3. On GitHub, go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose `main` and `/ (root)`, then save.
5. After a minute or two, the game is live at `https://YOUR-USERNAME.github.io/flappy/`.
6. Open that link on your phone. To add it to your home screen, use the browser's share menu ("Add to Home Screen").

## Tweaking

All of the difficulty settings are at the top of the `<script>` section in `index.html`:
- `GRAVITY` and `FLAP_VY` control how the bird falls and jumps
- `PIPE_GAP` controls the opening size (smaller is harder)
- `PIPE_SPEED` and `PIPE_SPACING` control how fast and how often pipes appear
