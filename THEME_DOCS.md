# Project Theme Registry: "Dark Glass" UI
**Version:** 2.1 (India & US Variants)
**Date:** Nov 21, 2025

## 1. Core Tech Stack
* **Engine:** [Leaflet.js](https://leafletjs.com/) (v1.9.4) - Chosen for lightweight performance and mobile touch support.
* **Data Format:** GeoJSON (Standardized geographic data).
* **Basemap:** CartoDB Dark Matter.
    * *URL:* `https://{s}.basemaps.cartocdn.com/dark_all/{z}/{x}/{y}{r}.png`
    * *Reason:* Provides the deep grey/black texture of roads and cities without adding visual noise.

## 2. Design System
The "Dark Glass" theme relies on three CSS properties working together:

### A. The Glassmorphism (Sidebar & Header)
Instead of solid colors, we use a semi-transparent background with a blur filter.
```css
background: rgba(20, 20, 20, 0.6);       /* 60% opacity black */
backdrop-filter: blur(12px);             /* The "Frost" effect */
border: 1px solid rgba(255,255,255,0.1); /* Subtle white border */
