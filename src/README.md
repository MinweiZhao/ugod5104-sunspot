# Source Code Directory

This directory contains the source code structure information for the SunSpot application.

## Current Structure

The SunSpot application is currently a single-page application with all code in `index.html`:

- **HTML**: Structure and content
- **CSS**: Embedded styles (glass-morphism UI, animations, responsive design)
- **JavaScript**: Map initialization, routing logic, UI interactions

## Code Organization

### Main Components (in index.html):

1. **HTML Structure**
   - Navigation (top nav and side dots)
   - 8 main sections (Home, Phenomenon, Gap, Users, Data, Methods, Demo, Discussion)
   - Map container and UI panels

2. **CSS Styles**
   - Core layout (scroll snap)
   - Glass-morphism UI components
   - Animations and transitions
   - Map-specific styling

3. **JavaScript Logic**
   - Scroll navigation
   - Mapbox initialization
   - Route calculation and display
   - User interaction handlers
   - Time scenario management

## Future Refactoring

For better code organization, consider splitting into:

```
src/
├── js/
│   ├── main.js          # Main application logic
│   ├── map.js           # Mapbox initialization and map logic
│   ├── routing.js       # Route calculation algorithms
│   └── ui.js            # UI interactions and animations
├── css/
│   ├── main.css         # Core styles
│   ├── components.css   # UI components
│   └── animations.css   # Animation definitions
└── html/
    └── index.html       # Main HTML structure
```

## External Dependencies

- Mapbox GL JS v3.4.0
- Tailwind CSS (CDN)
- Font Awesome 6.4.0
- Google Fonts (Inter)

