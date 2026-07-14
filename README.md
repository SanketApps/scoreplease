# 🏏 ScorePlease

**Free cricket scoring app — no login, no backend, no cost, ever.**

🔗 Live app: **https://sanketapps.github.io/scoreplease/**

ScorePlease is a lightweight, offline-friendly cricket scorer that runs entirely in your browser. Built for weekend turf/box cricket games where nobody wants to be the designated "scorer" arguing over how many balls are left in the over or who's actually on strike.

---

## Why this exists

Anyone who's played turf or gully cricket knows the real MVP of the match isn't the top scorer — it's whoever can keep the score straight. Without a scorer, every close game ends the same way: a group huddle arguing about the run count, whose over it is, or whether that last ball was a wide. ScorePlease exists to end that argument before it starts — open it on one phone, tap through the overs, and everyone can see the same number.

## Features

- 🏏 Full ball-by-ball scoring — runs, wides, no-balls, byes, leg-byes, wickets
- 🔄 Automatic strike rotation and over completion
- 🎯 Two-innings match support with target/required-run-rate tracking
- 🪙 Built-in coin toss animation
- 📊 Live scoreboard, batting cards, and ball-by-ball over history
- ↩️ Full undo support (button, keyboard shortcut, or swipe gesture)
- 🔊 Sound effects and on-screen celebrations (both toggleable)
- 🌗 Light/dark theme
- 📋 Copy score / share / export as image / export as PDF
- 💾 Match history saved locally — resume an in-progress match anytime
- 🔒 No login, no ads, no tracking, no backend — everything runs client-side

## Tech stack

Plain HTML, CSS, and vanilla JavaScript — no build step, no framework, no npm install. Two small CDN libraries (`html2canvas`, `jsPDF`) power the image/PDF export, loaded with [Subresource Integrity](https://developer.mozilla.org/en-US/docs/Web/Security/Subresource_Integrity) checks so the browser verifies they haven't been tampered with. All match data is stored locally in your browser via `localStorage` — nothing is sent to a server, because there is no server.

## Running it locally

No installation needed. Either:
- Open `index.html` directly in a browser, or
- Serve it locally for a closer-to-production feel:
  ```bash
  python3 -m http.server 8000
  # then visit http://localhost:8000
  ```

## Deployment

Hosted for free on **GitHub Pages**, served over HTTPS automatically. See [`SECURITY-SEO-GUIDE.md`](./SECURITY-SEO-GUIDE.md) in this repo for the security hardening and SEO setup applied to this project.

## Contributing

Issues and pull requests are welcome. If you spot a scoring edge case (e.g. an unusual extras rule for your local league), open an issue describing it.

## License

© ScorePlease. All rights reserved. This source is provided for use of the ScorePlease app; copying, redistributing, or repackaging it (in whole or substantial part) without permission isn't allowed. Want to use it for something specific? Reach out below — happy to talk.

## Contact

📧 sanketdeveloperr@gmail.com
