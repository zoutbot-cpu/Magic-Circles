# 🔮 Magic Circle & Sigil Tools

A suite of interactive, browser-based occult geometry tools. No installation, no dependencies, no internet required — open any file and start creating.

**[▶ Magic Circle Generator](https://zoutbot-cpu.github.io/Magic-Circles/)**  
**[📱 Mobile Version](https://zoutbot-cpu.github.io/Magic-Circles/magic_circle_mobile.html)**  
**[✦ Sigil Creator](https://zoutbot-cpu.github.io/Magic-Circles/sigil_creator.html)**

---

## Tools

### 🔮 Magic Circle Generator — `index.html`

Design and animate intricate magic circles with full control over geometry, colour, symbols, and text.

**17 geometry styles**

| Style | Description |
|---|---|
| Star polygon | Classic n-pointed star with nested rings |
| Orbital | Concentric orbital rings with satellite nodes |
| Alchemic | Triangle, hexagram and square overlays |
| Pentagram | Five-pointed star with nested pentagrams |
| Mandala | Spoke-divided radial mandala |
| Celtic knot | Interlocking curved arc weave |
| Sigil | Angular web connecting n vertices |
| Rose window | Overlapping petal circles, cathedral style |
| Enochian | Four-tablet ceremonial grid |
| Sacred geometry | Flower of Life — hexagonal circle packing |
| Compass rose | Navigation wheel with cardinal arrowheads |
| Labyrinth | Alternating circles and rounded squares |
| Zodiac wheel | 12-house astrological segment wheel |
| Fractal rings | Recursive satellite circle expansion |
| Gothic arch | Pointed arches and trefoil tracery |
| Norse web | Vegvisir-style 8-stave rune compass |
| Chaos star | 8-arrow chaos star with inner web |

**Features**
- Points / symmetry (3–16), rings (1–8), detail levels (1–5)
- Scale, line width, glow, opacity, rotation, animation speed
- 12 colour palettes + custom colour picker, 7 dark backgrounds
- Second colour for dual-layer mode
- 5 center detail patterns per style (0–4)
- Unicode symbol rings — 8 sets: Alchemical (64 glyphs), Astrological, Elder Futhark, Greek, Geometric, Occult, Latin, Arabic
- 3 independent text rings with per-ring radius, size, spacing, offset, flip
- Center inscription
- Layer toggles: outer rings, inner rings, geometry, nodes, spokes, ticks, center core, symbols, text rings, particles
- Inner geometry detail: cross lines, double ring, dashed ring, node rings, node size, tick multiplier, spoke skip
- Modes: Dual layer, Mirror, Pulse, Sparks
- 7 built-in presets + save/load your own
- **Export:** PNG / SVG / GIF (looping) / MP4 — quality 240–720px, 30–120 frames

---

### 📱 Mobile Version — `magic_circle_mobile.html`

Full-featured mobile interface optimised for phones and tablets.

- Canvas fills the screen edge-to-edge
- Slide-up bottom sheet with 7 tabs: Adjust, Color, Symbols, Text, Layers, Presets, Export
- iOS-style toggle switches
- 3 floating action buttons: Pulse, Dual layer, Sparks
- Add to home screen for full-screen app mode (iOS & Android)

---

### ✦ Sigil Creator — `sigil_creator.html`

Turn words and intentions into unique magical sigils using classical occult methods.

**How it works**
1. Type a word or intention (e.g. `PROTECTION`, `I AM CREATIVE`)
2. Choose a letter reduction method — remove duplicates, remove duplicates and vowels (traditional), or keep all
3. The remaining letters are mapped onto a geometric grid
4. Lines connect each letter in sequence — the path is your sigil

**5 grid types**

| Grid | Description |
|---|---|
| Rose Cross | Classic 3-column occult letter grid |
| Number wheel | 9 numerological positions (A=1, B=2… J=1, S=1…) |
| Letter circle | All 26 letters equally spaced around a ring |
| 5×5 square | Polybius-style grid (I/J share a cell) |
| Chaos scatter | Seeded pseudo-random placement |

**Features**
- 3 line styles: Angular, Bezier curves, Arc curves
- Smoothness slider for curve intensity
- 5 terminal styles: None, Dot, Circle, Diamond, Cross
- Circle overlay — place any magic circle style behind the sigil at adjustable opacity
- Trace animation — the sigil draws itself letter by letter
- History panel — last 10 intentions, click to restore
- Letter interpretation panel
- **Export:** PNG (240–1080px) or animated GIF (sigil traces itself)

---

## Export formats

| Format | Details |
|---|---|
| PNG | Static image at selected quality |
| SVG | PNG embedded in SVG wrapper, opens in Inkscape / Illustrator |
| GIF | Looping animation, 20fps, 30–120 frames, no CDN required |
| MP4 / WebM | 30fps video loop, WhatsApp-compatible (Magic Circle only) |

GIF encoding is fully self-contained — no external libraries, works offline and from `file://`.

---

## How to use

### Online
Just open the links above — no installation needed.

### Locally
```bash
# Option 1: double-click any .html file

# Option 2: serve with Python for a local URL
python -m http.server 8080
# then open http://localhost:8080
```

### Add to your phone (iOS / Android)
Open [`magic_circle_mobile.html`](https://zoutbot-cpu.github.io/Magic-Circles/magic_circle_mobile.html) in Safari or Chrome, tap Share → **Add to Home Screen**. It opens as a full-screen app with no browser chrome.

---

## Technical notes

- Pure vanilla HTML / CSS / JavaScript — zero frameworks, zero dependencies
- Fully self-contained — GIF encoder (LZW + NeuQuant palette quantiser) is written inline
- Works offline after first load, and directly from disk (`file://`)
- GIF palette sampled from 4 frames spread across the loop for accurate colour
- Canvas auto-resizes to fill the browser window
- All Unicode symbol sets are built into modern browsers — no font files needed

---

## Files

| File | Description |
|---|---|
| `index.html` | Magic Circle Generator (desktop) |
| `magic_circle_mobile.html` | Magic Circle Generator (mobile) |
| `sigil_creator.html` | Sigil Creator |
| `README.md` | This file |

---

## License

MIT — free to use, modify, and share.
