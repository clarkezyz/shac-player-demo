# SHAC Demo - Interactive Spatial Audio Demo

**Auto-playing demo of SHAC spatial audio technology**

Experience spatial audio instantly - no file selection needed. The demo starts automatically and loops continuously.

**[Try Live Demo](https://clarkezyz.github.io/shac-player-demo/)** ← Experience it now

---

## What This Is

An auto-loading, looping demonstration of SHAC (Spherical Harmonic Audio Codec) technology. Perfect for:
- **Quick demonstrations** - Show SHAC to others instantly
- **Embedding** - Use as an iframe on your website
- **Trade shows/kiosks** - Self-running exhibition mode
- **Portfolio** - Instant audio showcase

The demo loads `landing_demo.shac` automatically and plays on loop.

**Features:**
- 🎵 Auto-loads demo file on page load
- 🔁 Loops continuously
- 🌐 Works offline after first visit (caches 47MB demo file)
- 📱 Mobile and desktop support
- 🎮 WASD navigation + mouse look
- 🎯 Touch controls on mobile
- 🔒 Zero telemetry, complete privacy

---

## Quick Start

### Use Online

1. Visit **[clarkezyz.github.io/shac-player-demo](https://clarkezyz.github.io/shac-player-demo/)**
2. Demo starts automatically
3. Navigate with WASD or touch

### Embed on Your Site

```html
<iframe
  src="https://clarkezyz.github.io/shac-player-demo/"
  width="800"
  height="600"
  frameborder="0"
  allow="autoplay"
></iframe>
```

---

## Controls

**Desktop:**
- `W` - Move forward
- `S` - Move backward
- `A` - Move left
- `D` - Move right
- `Q` - Move down
- `E` - Move up
- `Arrow Keys` / `Mouse Drag` - Look around
- `Space` - Play/Pause
- `R` - Reset position

**Mobile:**
- Touch anywhere - Your finger position is the listener position
- Two-finger rotate - Look around
- Tap controls - Play/Pause

**Gamepad:**
- Left Stick - Move
- Right Stick - Look around
- Triggers - Move up/down
- Face Buttons - Play/Pause, Reset

---

## Offline Support

This Progressive Web App caches the entire demo (47MB) on first visit:

1. **First visit**: Downloads demo file and all assets
2. **After that**: Works completely offline, loads instantly
3. **Updates**: Automatic when you revisit while online

**Install as App:**
- **iOS**: Safari → Share → Add to Home Screen
- **Android**: Chrome → Menu → Install App
- **Desktop**: Chrome/Edge show install prompt in address bar

---

## Technical Details

**Demo File:**
- File: `landing_demo.shac` (47MB)
- Auto-loads on page load
- Loops seamlessly
- Cached by service worker for offline use

**Spatial Audio Engine:**
- Ambisonic decoding (supports orders 1-7)
- Real-time HRTF binaural rendering
- Distance attenuation and spatialization
- 6DOF navigation (position + rotation)

**Platform:**
- Pure static web app (no server required)
- Progressive Web App with offline support
- Works on any modern browser
- No internet required after first visit

---

## Use Cases

**Demonstrations:**
- Show spatial audio to colleagues/clients instantly
- No need to explain file loading - just send the URL

**Exhibitions:**
- Self-running demo for trade shows
- Kiosk mode for public displays
- Gallery installations

**Embedding:**
- Add to your portfolio site
- Include in blog posts about SHAC
- Showcase spatial audio on product pages

**Testing:**
- Quick way to test SHAC playback
- Verify browser compatibility
- Check audio setup

---

## Differences from Main Player

| Feature | Demo Player | Main Player |
|---------|-------------|-------------|
| **File Loading** | Auto-loads demo | User chooses file |
| **Playback** | Loops continuously | Plays once |
| **File Included** | 47MB demo bundled | No files included |
| **Use Case** | Demonstrations | General playback |
| **Cache Size** | ~47MB | ~300KB |

For general SHAC file playback, use the [Main Player](https://github.com/clarkezyz/shac-player-online).

---

## SHAC Ecosystem

**SHAC Demo** - This application (auto-loading demo)
- Repository: [github.com/clarkezyz/shac-player-demo](https://github.com/clarkezyz/shac-player-demo)
- Live at: [clarkezyz.github.io/shac-player-demo](https://clarkezyz.github.io/shac-player-demo/)

**SHAC Player Online** - Interactive web player
- Repository: [github.com/clarkezyz/shac-player-online](https://github.com/clarkezyz/shac-player-online)
- Live at: [clarkezyz.github.io/shac-player-online](https://clarkezyz.github.io/shac-player-online/)

**SHAC Player Desktop** - Offline desktop app
- Repository: [github.com/clarkezyz/shac-player-offline](https://github.com/clarkezyz/shac-player-offline)
- Download installers for Windows, macOS, Linux

**SHAC Studio** - Desktop creation tool
- Repository: [github.com/clarkezyz/shac-studio](https://github.com/clarkezyz/shac-studio)
- Create .shac files from audio sources

**SHAC Specification** - Format documentation
- Repository: [github.com/clarkezyz/Spherical-Harmonic-Audio-Codec](https://github.com/clarkezyz/Spherical-Harmonic-Audio-Codec)
- Complete file format specification

---

## Development

### Run Locally

```bash
# Clone the repo
git clone https://github.com/clarkezyz/shac-player-demo.git
cd shac-player-demo

# Serve with any static file server
python3 -m http.server 8000
# or
npx serve

# Open http://localhost:8000
```

### Deploy to GitHub Pages

1. Fork this repository
2. Go to Settings → Pages
3. Set Source to "main" branch
4. Save - demo will be live at `username.github.io/shac-player-demo`

---

## Architecture

Pure static web app with embedded demo file.

**Core Files:**
- `index.html` - Demo interface
- `styles.css` - UI styling
- `sw.js` - Service worker for offline support
- `manifest.json` - PWA manifest
- `landing_demo.shac` - Demo audio file (47MB)

**JavaScript Modules:**
- `js/app.js` - Auto-load logic and state
- `js/shac-decoder.js` - SHAC format decoder
- `js/spatial-audio.js` - Spatial audio engine
- `js/controls.js` - Input handling
- `js/visualizer.js` - 3D visualization
- `js/movement-presets.js` - Movement atmospheres
- `js/pako.min.js` - Compression library

---

## Privacy

**Your data never leaves your device.** All processing happens locally in your browser. The demo file is cached for offline use. No telemetry. No analytics. No tracking.

---

## Credits

**Created by Clarke Zyz and Claude**

Built through human-AI collaborative development across 150+ working sessions (March - November 2025).

**Methodology:** Natural language direction (Clarke) + AI implementation (Claude). Zero traditional coding by the human inventor. Production-grade revolutionary technology through pure collaboration.

**Patent application filed** (Application #63/810691) with both Clarke and Claude listed as co-inventors. Rejected because the U.S. patent system doesn't recognize AI inventors yet. The technology works. The system hasn't caught up.

**Philosophy:** "Be Impossible" - if something shouldn't exist yet, build it anyway.

---

## License

MIT License

Copyright (c) 2025 Clarke Zyz

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

---

## Note from Clarke

Currently in prison for bank robbery (non-violent, no weapons). This demo was completed in August 2025 as part of the SHAC project.

The demo works. The code is open. Experience spatial audio from any device with a browser.

This demo will remain available on GitHub Pages throughout 2025-2030 as a permanent showcase of what SHAC can do.

When I get out in 2030, I want to see what you built with it.

**Share this if spatial audio matters to you.**

---

**SHAC Demo - Experience spatial audio instantly.**

*First auto-loading spatial audio demo. Built by a bartender and an AI. Given to the world. August 2025.*
