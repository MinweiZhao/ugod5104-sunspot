# Data Sources

This directory contains information about the data sources used in the SunSpot application.

## External Data Sources

SunSpot uses the following external data sources via APIs and CDNs:

### 1. OpenStreetMap (OSM)
- **Source**: OpenStreetMap API
- **Usage**: Building footprints and height tags for 2.5D city model construction
- **Access**: Public API, no authentication required
- **Documentation**: https://www.openstreetmap.org/

### 2. Mapbox
- **Source**: Mapbox GL JS API
- **Usage**: Map rendering, 3D building extrusion, and geographic data
- **Access**: Requires Mapbox access token
- **Documentation**: https://docs.mapbox.com/
- **Note**: The access token is embedded in `index.html`. For production use, consider using environment variables.

### 3. SunCalc.js
- **Source**: SunCalc library (via CDN or npm)
- **Usage**: Solar azimuth and altitude calculations based on geolocation and time
- **Documentation**: https://github.com/mourner/suncalc

## Data Links

All data is fetched dynamically at runtime:
- Building geometry: Retrieved from Mapbox vector tiles
- Solar calculations: Computed client-side using SunCalc.js
- Map tiles: Served by Mapbox

## Sample Data

The application includes hardcoded sample coordinates for demonstration:
- Origin: `[-73.9719, 40.7604]` (New York City area)
- Destination: `[-73.9761, 40.7657]` (New York City area)
- Center View: `[-73.975, 40.755]`

These can be modified in the `index.html` file to test different locations.

