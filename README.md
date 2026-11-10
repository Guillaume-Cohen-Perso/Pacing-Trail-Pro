# 🏔️ Pacing Trail Pro

> **Advanced Trail Running Simulator, Topographic Pacing Planner & Physiological Endurance Modeler**

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38Bdf8?style=flat&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Leaflet](https://img.shields.io/badge/Leaflet-199900?style=flat&logo=leaflet&logoColor=white)](https://leafletjs.com/)

---

## 🚀 Overview

**Pacing Trail Pro** is a comprehensive, client-side web application designed for trail runners, ultra-endurance athletes, and coaches. It takes raw GPX track data (or generates synthetic race profiles) and computes an adaptive, scientifically-grounded pacing strategy across micro-segments based on topography, runner physiology, and fatigue models.

---

## ✨ Key Features

- **🗺️ Interactive OpenTopoMap Integration:** Visualizes your GPX track directly on topographic maps with color-coded effort zones (steep climbs, rolling hills, technical descents).
- **📈 Advanced Endurance Models:** Supports multiple physiological degradation models to project realistic target speeds based on total course load:
  - **Riegel Model** (Exponential power degradation)
  - **MIT / CNRS Model** (Logarithmic degradation via Endurance Index $IE$)
  - **Daniels / VDOT Model** (Oxygen uptake-based performance curves)
  - **Critical Power (CP & W')** & **Fixed Ultra Coefficients** (>60km format)
- **⚙️ Synthetic Course Generator:** Build custom training simulations by configuring total distance, elevation gain ($D^+$), climbing ratios, and relief profiles (single pass, rolling hills, or break-legs).
- **⚡ Grade-Adjusted Pace (GAP):** Computes precise segment speeds using Minetti's energy cost equations and custom vertical ascent speed (VAM) limits for hiking steep climbs.
- **❤️ Target Heart Rate & Mechanical Power:** Estimates heart rate targets via Karvonen's formula and mechanical power (Watts) accounting for total runner/pack mass and slope inclinations.
- **🔄 Synchronous Multi-View Inspection:** Hovering over the canvas elevation profile instantly syncs with a map marker and a detailed kilometer split roadbook.

---

## 🛠️ Tech Stack

- **Core:** Pure Vanilla JavaScript (ES6+), HTML5 Canvas
- **Styling:** Tailwind CSS (via CDN)
- **Mapping:** Leaflet.js with OpenTopoMap tiles
- **Icons:** Lucide Icons
- **Math Rendering:** MathJax for formal equations

---

## 📂 Project Structure

```text
├── trail_pacing_calculator_map_8_eng.html # Complete self-contained application (HTML, CSS, JS)
└── README.md                               # Project documentation
