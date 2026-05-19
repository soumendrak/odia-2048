<p align="center">
  <img src="https://img.shields.io/badge/୨୦୪୮-Odia_2048-FF6B35?style=for-the-badge&logo=javascript&logoColor=white" alt="Odia 2048">
</p>

<p align="center">
  <b>Play 2048 with Odia numerals (୦ ୧ ୨ ୩ ୪ ୫ ୬ ୭ ୮ ୯)</b><br>
  Vanilla JS · Dark & Light mode · Touch & Keyboard
</p>

<p align="center">
  <a href="https://2048.openodia.com/"><img src="https://img.shields.io/badge/Play-Now-FF6B35?style=for-the-badge&logo=playstation&logoColor=white" alt="Play Now"></a>
</p>

<p align="center">
  <img src="https://img.shields.io/github/languages/top/soumendrak/odia-2048?style=flat-square&logo=javascript&logoColor=white" alt="JavaScript">
  <img src="https://img.shields.io/github/languages/code-size/soumendrak/odia-2048?style=flat-square" alt="Code Size">
  <img src="https://img.shields.io/github/license/soumendrak/odia-2048?style=flat-square" alt="License">
  <img src="https://img.shields.io/github/last-commit/soumendrak/odia-2048?style=flat-square&logo=git&logoColor=white" alt="Last Commit">
  <img src="https://img.shields.io/github/deployments/soumendrak/odia-2048/Production?style=flat-square&logo=cloudflare&logoColor=white" alt="Cloudflare">
</p>

---

## About

The classic 2048 puzzle game, localized for the Odia language. Every tile value is displayed in Odia numerals (୨, ୪, ୮, ୧୬, ୩୨, ...).

Built as a single HTML file — no frameworks, no build tools, no dependencies. Deployed in under a minute.

### Features

- **Odia numerals** — all tile values displayed in Odia script
- **Dark & Light mode** — toggles with one click, persists in localStorage
- **Keyboard support** — arrow keys to move tiles
- **Touch support** — swipe on mobile (no page refresh)
- **Score tracking** — current score + best score saved locally
- **Animations** — smooth tile pop-in for new tiles
- **Responsive** — works on any screen size

---

## Play

→ [2048.openodia.com](https://2048.openodia.com/)

No install needed. Open in any browser and play.

---

## Local Development

### Prerequisites

- A web browser (Chrome, Firefox, Safari, Edge)

### Run locally

```bash
# Clone the repo
git clone https://github.com/soumendrak/odia-2048.git
cd odia-2048

# Open in browser
open index.html
```

That is it. No npm install, no build step, no server required. Just open `index.html` in any browser.

### Deploy

```bash
# Deploy to Cloudflare Pages
npx wrangler pages deploy . --project-name odia-2048 --branch main
```

---

## Project Structure

```
odia-2048/
├── index.html    # Single-file game (HTML + CSS + JS)
├── LICENSE       # MIT license
└── README.md     # This file
```

Everything is in one file. The game logic, styling, touch handling, theme toggle — all self-contained.

---

## How It Works

Core mechanics:

1. **Board**: 4x4 grid of tiles, represented as a 2D array
2. **Moves**: Each direction slides all tiles and merges adjacent equal values
3. **New tile**: A random 2 (90%) or 4 (10%) appears after each move
4. **Win**: Reach a 2048 tile
5. **Lose**: No empty cells and no possible merges

---

## License

[MIT](LICENSE) — free to use, modify, and share.

---

<p align="center">
  Made by <a href="https://soumendrak.com">Soumendra Kumar Sahoo</a> · <a href="https://openodia.com">OpenOdia</a>
</p>
