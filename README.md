# ⚡ PokeBattles — Cyber Arena

> A neon cyberpunk-styled Pokémon PvP battle arena — built as a single-page, front-end-only web app.

[![Made with HTML5](https://img.shields.io/badge/Made%20with-HTML5-orange?style=for-the-badge&logo=html5)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=for-the-badge)](CONTRIBUTING.md)
[![Deploy to Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-blue?style=for-the-badge&logo=github)](.github/workflows/deploy-pages.yml)

[🐛 Report Bug](../../issues/new?template=bug_report.md) · [💡 Request Feature](../../issues/new?template=feature_request.md) · [📖 Game Guide](docs/GAME-GUIDE.md)

---

## 📌 About

**PokeBattles** is a self-contained, single-file web app that simulates a Pokémon-style PvP battle arena with a dark, cyber/neon aesthetic. It includes a home screen, matchmaking/lobby flow, live turn-based battles with HP bars and move effects, a results overlay, and match history — all rendered client-side with plain HTML, CSS, and JavaScript.

It also demonstrates calling the **Anthropic Claude API** directly from the browser to generate dynamic AI battle narration (hype announcer lines, victory/defeat commentary).

## 🚀 Quick Start

### Option 1 — Just open it

No build step, no dependencies. Simply open [`index.html`](index.html) in your browser.

### Option 2 — Run locally with a dev server

```bash
git clone https://github.com/<your-username>/pokebattles-cyber-arena.git
cd pokebattles-cyber-arena

# Any static server works, e.g.:
python -m http.server 8080
# then visit http://localhost:8080
```

### Option 3 — Deploy with GitHub Pages (automatic)

This repo already ships with a GitHub Actions workflow ([`.github/workflows/deploy-pages.yml`](.github/workflows/deploy-pages.yml)) that auto-deploys on every push to `main`.

1. Push this repo to GitHub.
2. Go to **Settings → Pages → Build and deployment → Source** and select **GitHub Actions**.
3. Push to `main` (or run the workflow manually) — your game will be live at `https://<your-username>.github.io/<repo-name>/`.

## ✨ Features

| Feature | Description |
|---|---|
| 🎮 Home / Menu screen | Animated logo, online player counter, mode selection |
| ⚔️ Turn-based battles | HP bars, move selection, type effectiveness, hit effects |
| 🏆 Matchmaking & Lobby | Ranked / casual flow with lobby entries |
| 📜 Match history & leaderboard | Track past results |
| 🤖 AI battle narration | Dynamic commentary generated via the Claude API |
| 🎨 Cyber/neon UI | Custom fonts, particle effects, scanlines, glassmorphism |

## 🗂️ Project Structure

```
pokebattles-cyber-arena/
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.md
│   │   └── feature_request.md
│   ├── workflows/
│   │   └── deploy-pages.yml   # Auto-deploy to GitHub Pages
│   └── PULL_REQUEST_TEMPLATE.md
├── docs/
│   ├── GAME-GUIDE.md          # Screens & architecture walkthrough
│   └── CHANGELOG.md
├── index.html                  # The entire app (HTML + CSS + JS)
├── README.md
├── LICENSE                     # MIT License
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
├── SECURITY.md
├── .nojekyll
└── .gitignore
```

## 🛠️ Tech Stack

- **HTML5 / CSS3** — layout, animations, glassmorphism UI
- **Vanilla JavaScript** — game state, battle logic, DOM rendering
- **Google Fonts** — Orbitron, Space Grotesk, Inter, JetBrains Mono
- **Anthropic Claude API** — AI-generated battle narration

## 🤝 Contributing

Contributions are welcome! Feel free to fork this repo, make changes, and open a pull request. See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## 📄 License

Licensed under the [MIT License](LICENSE).

---

**⭐ If you like this project, consider starring the repo!**
