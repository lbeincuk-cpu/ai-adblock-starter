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
# Privacy Policy — AI Ad Block (Starter)

**Last updated:** August 20, 2025  

AI Ad Block (Starter) is a browser extension that blocks advertisements and trackers.  
It is designed to operate entirely on your device and minimize data access.

---

## Data Collection

- The extension **does not collect, store, or transmit** personally identifiable information (PII), browsing history, page content, or usage analytics to any external server.  
- All processing happens locally within your browser.

---

## Permissions and Justification

- **declarativeNetRequest** (Chromium only):  
  Needed to apply static blocking rules to network requests (ad/tracker blocking).  
- **scripting**:  
  Used to inject content scripts that hide or remove ad elements in the DOM.  
- **storage**:  
  Stores extension settings and preferences locally on the user’s device.  
- **host_permissions: `<all_urls>`**:  
  Required to allow the extension to function on any website the user chooses.  
- **tabs** (if used):  
  Only to apply blocking rules to the correct tab. No tab content is collected.  
- **webRequest / webRequestBlocking** (Firefox or legacy use):  
  Only to block/redirect ad and tracker requests. Requests are never logged or transmitted.  

---

## AI / Heuristic Features

If AI/heuristic features are enabled, analysis of page structure is performed **entirely in the browser**.  
No content is uploaded to remote servers.

---

## Third-Party Sharing

- No data is shared, sold, or transferred to third parties.  

---

## Children’s Privacy

This extension does not target children and does not knowingly collect any data from children.

---

## Changes

We may update this policy from time to time. The latest version will always be available in this repository and at:  
[https://<your-username>.github.io/ai-adblock-starter/privacy.html](https://<your-username>.github.io/ai-adblock-starter/privacy.html)

---

## Contact

Questions? Contact: **service@eye3.uk**  
Or open an issue: [GitHub Issues](https://github.com/lbeincuk/ai-adblock-starter/issues)

---


## License
MIT License. See [LICENSE](./LICENSE).
