
# 🥁 Beat Machine

A browser-based drum machine / beat maker built with vanilla HTML, CSS, and JavaScript. No installs, no frameworks — just open it and make beats.

**Live demo:** [haulstreet.github.io/beatmachine](https://haulstreet.github.io/beatmachine/)

---

## What it does

- 6 drum tracks: Kick, Snare, Hi-hat, Clap, Tom, Open Hi-hat
- 16-step sequencer grid
- Adjustable BPM (60–180)
- Real-time audio using the Web Audio API (no samples needed)
- Shuffle button to generate a random beat
- Visual beat indicator that follows the playhead

---

## How to use

1. **Click any pad** to toggle it on/off
2. Hit **Play** to start the sequence
3. Adjust the **BPM slider** to change the tempo
4. Click **Shuffle** for a randomly generated beat
5. Click **Clear** to reset the grid

---

## How it works

Everything runs in a single `index.html` file using the browser's built-in **Web Audio API** — no libraries or dependencies required. Each drum sound is synthesized on the fly:

| Track | Sound synthesis |
|-------|----------------|
| Kick | Sine wave with frequency drop |
| Snare | White noise + triangle oscillator |
| Hi-hat | Short burst of white noise |
| Clap | Exponentially decaying white noise |
| Tom | Sine wave with slow frequency drop |
| Open HH | Longer burst of white noise |

---

## Running locally

No server needed. Just open the file in your browser:

```bash
# Clone the repo
git clone https://github.com/haulstreet/beatmachine.git

# Open in browser
open index.html
```

---

## Built with

- HTML / CSS / JavaScript (zero dependencies)
- Web Audio API
- GitHub Pages (free hosting)

---

## License

Feel free to use, remix, and build on this.
