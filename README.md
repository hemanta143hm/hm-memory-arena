# HM Memory Arena

A standalone, mobile-friendly neon memory matching game created for Hemanta Malik's portfolio.

## Features
- Easy (8 pairs), Medium (10 pairs), Hard (18 pairs)
- Responsive neon UI
- Timer, move counter, matches, score and progress
- Match streak bonuses and end-game score bonuses
- Personal best score saved locally in the browser
- Pause, restart, new game and sound toggle
- No backend, build tools, external game libraries or API keys required

## Run locally
Open `index.html` in a modern browser, or use a local static server:
```bash
python -m http.server 8080
```
Then visit `http://localhost:8080`.

## Deploy to GitHub Pages
1. Create a GitHub repository, for example `hm-memory-arena`.
2. Keep your main portfolio repository private. This game can be in its own repository; choose public only if you want the GitHub Pages URL publicly accessible.
3. Upload `index.html` to the root of the game repository.
4. In repository Settings → Pages, select Deploy from a branch → `main` → `/ (root)` → Save.
5. Wait for the Pages URL, typically `https://YOUR-USERNAME.github.io/hm-memory-arena/`.

## Add to the portfolio Admin CMS
Use the actual URLs after publishing:
- Title: `HM Memory Arena`
- Slug: `hm-memory-arena`
- Short description: `A neon memory matching challenge. Flip cards, find pairs, build streaks and beat your personal best across three difficulty levels.`
- Additional data JSON:
```json
{
  "repoUrl": "https://github.com/YOUR-USERNAME/hm-memory-arena",
  "playUrl": "https://YOUR-USERNAME.github.io/hm-memory-arena/",
  "displayMode": "embed",
  "gameType": "external",
  "iframeEnabled": true
}
```
Replace `YOUR-USERNAME` with your actual GitHub username and use the exact deployed URL.

Important: This is a static browser game. The current version stores personal bests in the player's own browser using localStorage; it does not send player data to a server.
