# dotmysvg

**[Try it live](https://haavelund.no/dotmysvg/)**

A browser-based tool for importing any SVG icon and adding a customizable dot indicator to it — useful for creating "unread" badges, notification markers, or status indicators on existing icons.

## Features

- **Import any SVG** — drag and drop or browse for a file
- **Position the dot** — control angle (0–360°) and distance from center
- **Customize the dot** — adjust radius, gap width, and color
- **Live preview** — see changes in real time on a checkerboard background
- **Export** — download the modified SVG or copy the code to clipboard

## Usage

Open `index.html` in a browser. No build step or dependencies required (Tailwind CSS is loaded from CDN).

1. Drop an SVG file into the import zone
2. Adjust the dot position, size, gap, and color using the sliders
3. Download the result or copy the SVG code

## How It Works

The imported SVG content is wrapped in a `<g>` element with an SVG mask that cuts out space for the dot. A colored circle is then placed on top at the specified position, creating a clean overlay effect without modifying the original icon paths.
