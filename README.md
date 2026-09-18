# Endless Car Chase

A browser-based endless car chase game built with Unity WebGL.

## Play

Since this is a Unity WebGL build, it must be served over HTTP(S) — opening `index.html` directly as a local file will fail due to browser restrictions on loading `.wasm`/`.data` files via `file://`.

### Option 1: GitHub Pages (recommended)

1. Go to the repo's **Settings → Pages**
2. Set source to the `main` branch, root folder
3. Visit the generated URL (e.g. `https://game-hub-code.github.io/endless-car-chase/`)

### Option 2: Run locally

```bash
git clone https://github.com/game-hub-code/endless-car-chase.git
cd endless-car-chase
npx serve
```

Then open the URL printed in the terminal (e.g. `http://localhost:3000`).

## Project Structure
