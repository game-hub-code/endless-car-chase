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

```
endless-car-chase/
├── Build/                          # Unity WebGL build output
│   ├── Endless_Car_Chase.data
│   ├── Endless_Car_Chase.framework.js
│   ├── Endless_Car_Chase.loader.js
│   └── Endless_Car_Chase.wasm
├── TemplateData/                   # Static assets (styles, images)
│   ├── css/
│   │   └── style.css
│   └── img/
│       ├── background.png
│       ├── favicon.ico
│       ├── Logo.png
│       ├── progressEmpty.png
│       └── progressFull.png
├── game.js                         # Game/loader glue script
└── index.html                      # Entry point
```

## Tech Stack

- Unity (WebGL export)
- HTML / CSS / JavaScript

## Notes

- Requires a modern browser with WebAssembly support.
- Large asset sizes (`.data` ~8 MB, `.wasm` ~21 MB) — initial load may take a few seconds depending on connection speed.
