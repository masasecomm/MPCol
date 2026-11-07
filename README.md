# Collage Studio

A lightweight photo-collage maker that runs entirely in the browser. It uses no build tools, external libraries, tracking scripts, or server-side image uploads.

## Run locally

Open `index.html` in a modern browser, or serve this folder with any static web server.

## Publish on GitHub Pages

1. Push this repository to GitHub.
2. In the repository, open **Settings → Pages** and set **Build and deployment → Source** to **GitHub Actions**.
3. Push to the `main` branch. The included workflow publishes the site; subsequent pushes to `main` deploy automatically.

## Features

- Upload or drag in up to 100 JPG, PNG, GIF, or WebP photos. The Photos panel shows the uploaded count and lets you filter photos on the canvas versus unused photos; choosing an on-canvas photo selects its cell, while choosing an unused photo selects it for placement. Click **Add selected photo to canvas** to place it in an empty holder.
- Choose from the 12 named photo-grid layouts, including feature mosaics and 1–4-column galleries.
- Pick square, portrait, HD 16:9, HD 9:16 portrait, 30 × 30 cm, or 20 × 20 cm presets, or enter a custom size in pixels or centimeters.
- Swap photos into cells and drag within a cell to reposition the crop.
- Remove a selected photo from its cell while keeping the holder, or delete the holder and reflow the remaining collage cells. Deleted-holder photos remain available in the photo library.
- Use **Auto Fix** in Grids to arrange every uploaded photo into a balanced collage, reset crops, and fit the canvas preview to the workspace.
- Adjust photo zoom, grid spacing, and rounded photo corners (square corners are the default). Select a photo to show its selection outline and editing controls; click outside it to deselect. Set a side margin to zero to reach the cell edge, with a warning when the photo touches or may touch a neighbor.
- Add text and emoji stickers, choose a background, and add a frame.
- Undo and redo edits, zoom the preview, and export a full-size PNG.
- Photos are processed locally in the browser and are not uploaded.

The editor is a static GitHub Pages site: it does not include user accounts, cloud storage, shared projects, or a backend.

The provided “Featured Left Split Stack” defines four slots, so it is available as a 4-photo layout; there is no 3-photo preset in this set. “Central Feature Wall” uses a 4×4 matrix to fit all 11 photos without overlapping cells.

Custom centimeter dimensions are converted to export pixels at 300 DPI. Canvas dimensions are limited to 8,192 px per edge and 40 megapixels total.
