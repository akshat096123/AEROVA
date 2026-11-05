# VayuVision

VayuVision is a front-end prototype for a Delhi NCR air-quality and climate-awareness dashboard. It brings together an AQI display, pollutant composition chart, pollution-zone map, GRAP information, and an EV-map view.

> **Prototype note:** The current dashboard uses sample AQI, pollutant, and location values in the JavaScript. It is not connected to a verified live sensor or EV-station API. Treat displayed values as demo data, not real-time public-health or travel guidance.

## Features

- AQI overview with a visual status indicator
- Pollutant composition chart powered by Chart.js
- Delhi NCR map with sample location markers powered by Leaflet
- Expandable information panels for GRAP measures
- EV map view
- Responsive single-page layout and animated background particles

## Project structure

```text
.
├── index.html
├── assets/
│   ├── css/
│   │   └── styles.css
│   └── js/
│       └── script.js
├── .gitignore
└── README.md
```

## Run locally

No build step or package installation is required.

1. Clone or download this repository.
2. Open `index.html` in a browser, or serve the folder with a local static server.
3. Allow location access if prompted. The dashboard falls back to its Delhi default view if location access is unavailable.

For example, with Python installed:

```bash
python3 -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000).

## External libraries

- [Leaflet](https://leafletjs.com/) — interactive maps
- [Chart.js](https://www.chartjs.org/) — pollutant chart
- [Font Awesome](https://fontawesome.com/) — icons
- [Google Fonts](https://fonts.google.com/) — Space Grotesk and Outfit

These dependencies are loaded from CDNs, so an internet connection is required for the complete interface.

## Next steps

- Connect a trusted AQI data provider and display source + last-updated time.
- Replace hard-coded pollution markers with verified monitoring-station data.
- Connect a maintained EV charging-station dataset or API.
- Verify GRAP stage and restrictions against current official CAQM notices before displaying them as active rules.
- Add automated checks for broken asset paths and JavaScript errors.

## License

No license has been specified yet. All rights remain with the respective owners unless a license is added.
