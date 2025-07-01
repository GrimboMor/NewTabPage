# Grimbo's Links - Customizable Start Page

A responsive, and customisable browser start page for your home, office, or personal use. 

Designed for quick access to your favourite sites, tools, and folders, with live clock and weather tiles, and a modern, touch-friendly UI.

## Features

- **Tile-based Home Screen:** Add links, folders (with nested tiles), a live clock, and a weather forecast tile.
- **Folder Overlays:** Click a folder to open a dynamic overlay with a grid of tiles, automatically sized for your screen and content.
- **Responsive Design:** Looks great on desktops, tablets, and phones. Tiles and folder overlays resize and reflow automatically.
- **Custom Icons:** Use your own PNG/JPG/WebP icons for each tile, or use the provided sample icons.
- **Live Clock Tile:** Shows the current time, day, and date.
- **Weather Tile:** Shows a 3-day forecast for your city (uses OpenWeatherMap, just set your lat/lon and API key in the code).
- **No Build Tools Needed:** Just open `index.html` in your browser. No frameworks, no dependencies, no server required.

## Screenshots

### Sample Start Page
![Start Page](https://github.com/GrimboMor/NewTabPage/blob/main/Screenshots/01.png?raw=true)

### Folder Overlay Opened
![Folder Open](https://github.com/GrimboMor/NewTabPage/blob/main/Screenshots/02.png?raw=true)

### Portrait Mode Example
![Portrait Resize](https://github.com/GrimboMor/NewTabPage/blob/main/Screenshots/03.png?raw=true)


## Getting Started

1. **Clone or Download:**
   ```
   git clone https://github.com/YOUR_USERNAME/your-repo-name.git
   ```
   Or download and unzip the project.

2. **Open in Browser:**
   Open `index.html` directly in your browser. All features work offline (except weather, which needs internet).

3. **Customize Tiles:**
   - Edit the `tileData` array in `index.html` to add, remove, or change tiles and folders.
   - Place your icon images in the `Images/` folder and reference them in your tile objects.
   - To change the weather city, update the `lat`, `lon`, and `city` fields in the weather tile object and API call.

4. **Deploy:**
   - Host on GitHub Pages, Netlify, Vercel, or any static web server.

## Folder Overlay Logic
- Folder overlays are set to 20% of the viewport width (min 220px, max 90vw), and their height is based on the number of rows of tiles, with dynamic padding and gap that shrink on small screens.
- Tiles inside folders are always square and automatically sized to fit the overlay.
- All overlay sizing and layout is handled in JavaScript for maximum flexibility.

## Customization
- **Add/Remove Tiles:** Edit the `tileData` array.
- **Change Icons:** Place new images in `Images/` and update the `icon` field.
- **Change Colors/Styles:** Edit the CSS in the `<style>` block in `index.html`.
- **Add More Tile Types:** Extend the `renderTiles` function to support new tile types.

## Credits
- Icons and images are property of their respective owners or from open icon sets.
- Weather data from [OpenWeatherMap](https://openweathermap.org/).

## License
See LICENSE file.

---

**Enjoy your new tab/start page!**
