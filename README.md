# ai-adblock-starter
 AI-powered blocker (your path) Hybrid rules + on-page heuristic for Firefox MV3. Uses a machine learning model (running in the browser with ONNX Runtime) to see or analyze the DOM.

AI-powered ad blocker demo extension for Chromium and Firefox.

## Features
- 🚫 Blocks ads using hybrid methods:
  - Declarative Net Request (Chromium MV3)
  - On-page AI heuristic detection (both Chromium + Firefox)
- ⚡ Lightweight starter project
- 🌍 Open-source and privacy-friendly (no data leaves your browser)

## Installation
### Chromium / Chrome
1. Clone or download this repo.
2. Open **chrome://extensions** → enable **Developer Mode**.
3. Click **Load unpacked** and select the `dist/chromium` folder.

### Firefox
1. Clone or download this repo.
2. Open **about:debugging → This Firefox → Load Temporary Add-on**.
3. Select `dist/firefox/manifest.json`.

## Development
- Chromium build uses **Manifest V3** with Declarative Net Request.
- Firefox build uses **Manifest V2**.
- Models and vendor scripts load locally — no remote code.

## Privacy
See our [Privacy Policy](./docs/privacy.html).

## License
MIT License. See [LICENSE](./LICENSE).
