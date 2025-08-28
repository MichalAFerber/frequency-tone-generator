# Frequency Tone Generator

A tiny, no-build, browser-based frequency tone generator powered by the Web Audio API. Type a frequency in Hz, hit **Play**, and you’ll hear a pure tone. Comes with a reference chart of commonly discussed frequencies and a ZIP of pre-generated WAV files.

**Live demo:** [https://michalferber.me/frequency-tone-generator/](https://michalferber.me/frequency-tone-generator/) ([Michal Ferber][1])

---

## Features

* **Instant tones** — Enter any frequency (Hz) and play/stop directly in the browser. ([Michal Ferber][1])
* **Reference chart** — A curated list of frequently mentioned ranges (anecdotal/alt-medicine sources). ([Michal Ferber][1])
* **Bulk download** — Pre-rendered `.wav` files packaged as a ZIP for offline use. ([Michal Ferber][1])
* **No build tools** — Plain HTML/CSS/JS. Host it anywhere (GitHub Pages, static hosts). The repo includes `index.html`, `style.css`, and a ZIP asset. ([GitHub][2])

---

## Quick Start (Local)

1. **Clone** this repo:

   ```bash
   git clone https://github.com/MichalAFerber/frequency-tone-generator.git
   cd frequency-tone-generator
   ```

2. **Open** `index.html` in your browser (double-click or serve with any static server).
3. **Interact** with the page (e.g., click) if your browser requires a user gesture before audio can start.

---

## Usage

* Enter a **frequency** (e.g., `440` for A4) and press **Play**.
* Use **headphones** for the cleanest result. The page includes a **“Works best with headphones”** note. ([Michal Ferber][1])
* Download the **ZIP** of tones from the page if you prefer offline playback. ([Michal Ferber][1])

> ⚠️ **Disclaimer**
> The frequency chart and associated use cases are **anecdotal** and **not medical advice**. This tool is **not** a substitute for professional care. Always consult a qualified healthcare provider. The page carries this disclaimer as well. ([Michal Ferber][1])

---

## Deploying

### GitHub Pages

1. Push the repository to GitHub.
2. In **Settings → Pages**, set the source to the `main` branch (root).
3. Your site will publish to a URL like: `https://<username>.github.io/frequency-tone-generator/`.

   * This project is published at: **michalferber.me/frequency-tone-generator**. ([GitHub][2])

### Any Static Host

Upload `index.html`, `style.css`, and the assets (including the ZIP) to your static hosting provider.

---

## How it Works (High Level)

* Uses the **Web Audio API** to create an oscillator node at the requested frequency and route it to the destination (your speakers/headphones).
* Most browsers require a **user gesture** (click/tap) before audio playback begins.

For a deeper dive into Web Audio tone generation, see MDN’s advanced Web Audio guide. ([MDN Web Docs][3])

---

## Project Structure

```bash
.
├── index.html          # App UI (input + controls + chart + download link)
├── style.css           # Minimal styles
├── frequency_tones.zip # Pre-generated WAVs referenced on the site
└── LICENSE             # MIT
```

(See repository file list on GitHub.) ([GitHub][2])

---

## Roadmap / Ideas

* Waveform selection (sine, square, triangle, sawtooth)
* Volume & fade-in/out controls
* Sweep/step modes (e.g., hearing tests, equipment checks)
* PWA support for offline use
* Keyboard shortcuts

---

## Contributing

PRs and issues are welcome! If you’re proposing features, please include a brief rationale and UI sketch (text or screenshot is fine).

---

## License

[MIT](./LICENSE). Reuse, remix, and build on it.

---

## Acknowledgments

* Thanks to the browser **Web Audio API** for making real-time synthesis trivial to experiment with.
* Published via **GitHub Pages**. ([GitHub][2])

---

[1]: https://michalferber.me/frequency-tone-generator/ "Frequency Tone Generator"
[2]: https://github.com/MichalAFerber/frequency-tone-generator "GitHub - MichalAFerber/frequency-tone-generator"
[3]: https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API/Advanced_techniques?utm_source=chatgpt.com "Advanced techniques: Creating and sequencing audio - MDN"
