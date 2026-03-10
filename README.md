# Yamhill County Aerial Survey Archive — 1948

An interactive web application for browsing a simulated historical aerial photography archive of Yamhill County, Oregon.

## Features

- **Interactive Map** — Pan and zoom a PLSS (Public Land Survey System) grid covering Townships 1S–7S × Ranges 2W–6W. Click any section to open a detail modal with a procedurally-rendered aerial photograph.
- **Photo Gallery** — Browse, filter, and download all generated survey photographs. Toggle between grid and list views. Filter by Township, Range, or Section number.
- **Film-Style UI** — Authentic period-appropriate aesthetic with Playfair Display / Courier Prime typography, parchment/ink color palette, and filmstrip overlays.
- **Procedural Aerial Rendering** — All photographs are generated at runtime via HTML5 Canvas using a seeded random algorithm — no external images required.
- **Fully Offline** — No server needed. Only loads Google Fonts and jsPDF from CDNs.

## Project Structure

| File | Description |
|---|---|
| `index.html` | Main HTML with embedded JavaScript |
| `styles.css` | All CSS styles |
| `yamhill-seal.svg` | Yamhill County seal graphic |
| `headerlogo.png` | Header logo image |

## Usage

Open `index.html` in any modern browser. No build step, no backend.

```bash
open index.html
# or
python3 -m http.server 8080   # then visit http://localhost:8080
```

## Technical Notes

| Property | Value |
|---|---|
| Coverage | T1S–T7S × R2W–R6W, Willamette Meridian |
| Survey Year | Summer 1948 |
| Scale | 1:20,000 |
| Film | Panchromatic |
| Sections per Township/Range | ~4–10 (seeded random) |
| Photo resolution (simulated) | 600, 800, or 1200 DPI |

## Browser Support

All modern browsers (Chrome, Firefox, Safari, Edge). Designed for both desktop and mobile.

## License

See `LICENSE` file.
