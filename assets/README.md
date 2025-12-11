# Assets Directory

This directory is reserved for local assets such as images, icons, fonts, or other static files.

## Current Status

Currently, the SunSpot application uses CDN-hosted resources:

- **CSS Framework**: Tailwind CSS (via CDN)
- **Icons**: Font Awesome 6.4.0 (via CDN)
- **Fonts**: Google Fonts - Inter (via CDN)
- **Maps**: Mapbox GL JS (via CDN)

## Local Asset Options

If you want to host assets locally for offline use or better performance:

1. Download Tailwind CSS and include locally
2. Download Font Awesome icons and fonts
3. Download Google Fonts (Inter) and host locally
4. Add custom images, logos, or other media files

## Structure

```
assets/
├── css/          # Local CSS files (if not using CDN)
├── js/           # Local JavaScript libraries
├── images/       # Images, logos, screenshots
├── fonts/        # Local font files
└── icons/        # Icon files (if not using Font Awesome)
```

