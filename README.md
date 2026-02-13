# K-Means Clustering Visualiser

**See it in action at [quantumphysicist.github.io/k-means-visualisation](https://quantumphysicist.github.io/k-means-visualisation/).**

An interactive, single-file HTML demo that visualises the **k-means clustering algorithm** step by step on a 2D canvas.

![HTML5](https://img.shields.io/badge/HTML5-Canvas-orange) ![No Dependencies](https://img.shields.io/badge/dependencies-none-brightgreen) ![License](https://img.shields.io/badge/license-MIT-blue)

## What is K-Means?

K-means partitions *n* data points into *k* clusters by repeating two steps until convergence:

1. **Assignment** — assign each point to the cluster whose centroid is nearest.
2. **Update** — move each centroid to the mean position of its assigned points.

Centroids are initialised using the **k-means++** strategy (D²-weighted random selection) for faster, more reliable convergence.

## Demo

1. **Download or clone** this repository.
2. **Open `index.html`** in any modern browser (double-click the file — no server needed).
3. **Click** inside the canvas to add data points (or press **+50 Random** for instant sample data).
4. Press **Step** to advance one iteration, or **Run** to animate the algorithm.

No build step, no dependencies, no Node.js — just one HTML file.

## Features

| Feature | Description |
|---|---|
| **Click to add points** | Place data points anywhere on the canvas |
| **Random point generation** | Add 50 Gaussian-clustered points in one click |
| **Adjustable k** | Choose 2–8 clusters with +/− controls |
| **Step-by-step mode** | Advance one iteration at a time to study convergence |
| **Animated run** | Auto-step with adjustable speed (50 ms – 950 ms per step) |
| **K-means++ init** | Smart centroid seeding for better initial placement |
| **Voronoi regions** | Soft colour-coded background showing cluster boundaries |
| **Connecting lines** | Faint lines link each point to its centroid (≤ 150 points) |
| **Dynamic status** | Live stats (point count, iteration, convergence badge) and contextual hints |
| **Reset / Clear** | Reset centroids (keep points) or clear everything |
| **HiDPI support** | Crisp rendering on Retina / high-DPI displays via `devicePixelRatio` scaling |

## Project Structure

```
.
└── index.html   ← entire app (HTML + CSS + JS, ~350 lines)
```

## Browser Support

Works in all modern browsers that support the HTML5 Canvas API:

- Chrome / Edge
- Firefox
- Safari

## License

MIT — use it however you like.
