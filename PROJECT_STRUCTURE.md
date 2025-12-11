# Project Structure

This document describes the organization of the SunSpot website ZIP file.

## Directory Structure

```
ugod5104-sunspot/
├── index.html              # Main application file (single-page app)
├── README.md               # Project documentation
├── LICENSE                 # MIT License
├── PROJECT_STRUCTURE.md    # This file
├── assets/                 # Static assets directory
│   └── README.md          # Assets documentation
├── data/                   # Data sources documentation
│   └── README.md          # Data sources and links
└── src/                    # Source code documentation
    └── README.md          # Code structure information
```

## File Descriptions

### Core Files

- **index.html**: Complete single-page application containing HTML, CSS, and JavaScript
- **README.md**: Comprehensive project documentation for public audience
- **LICENSE**: MIT License file

### Documentation Directories

- **assets/**: Documentation for static assets (currently using CDN resources)
- **data/**: Documentation of external data sources and API links
- **src/**: Documentation of source code structure and organization

## External Dependencies

All external resources are loaded via CDN:
- Mapbox GL JS (maps and 3D rendering)
- Tailwind CSS (styling)
- Font Awesome (icons)
- Google Fonts (typography)

## Running the Application

1. Extract the ZIP file
2. Open `index.html` in a modern web browser
3. Ensure internet connection for CDN resources
4. Mapbox access token is included in `index.html` (line 533)

## Notes

- This is a single-page application with all code in `index.html`
- No build process required
- No local server required (can open directly in browser)
- Mapbox token is embedded; replace for production use

