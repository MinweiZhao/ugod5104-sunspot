# 🌞 SunSpot: The Ephemeral City

> **Redefining Navigation through Human Light Preferences**

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Available-blue)](https://minweizhao.github.io/ugod5104-sunspot/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

SunSpot is an innovative web application that revolutionizes urban navigation by incorporating solar exposure and shadow patterns into route planning. Unlike traditional navigation apps that optimize solely for distance or time, SunSpot considers the dynamic thermal comfort of urban environments, helping users find paths that maximize or minimize sunlight exposure based on their preferences and needs.

---

## 🎯 The Problem

### The Urban Canyon Effect

In dense metropolises, skyscrapers create a complex, ever-changing shadow environment. As the sun moves across the sky, these "urban canyons" cast shadows that dramatically affect thermal comfort—a factor that current navigation systems completely ignore.

> *"Shadows are not just absence of light; they define thermal comfort of the city."*

### The Disconnect

- **Static Efficiency**: Current apps optimize strictly for distance or time, treating the city as a flat, static surface
- **Dynamic Comfort**: Humans need thermal comfort—we seek sun in winter and shade in summer, but maps don't show this

---

## 👥 Who is this for?

### 🧑‍💼 Office Workers
Craving Vitamin D and warm spots during winter lunch breaks

### 📸 Photographers
Hunting for the "Golden Hour" lighting in specific urban alleys

### 👶 Vulnerable Groups
Elderly and parents needing cool, shaded routes during summer heat

---

## ✨ Features

- **🌡️ Dual-Mode Routing Algorithm**
  - **Sun-Seeker Mode**: Maximizes solar exposure (ideal for winter)
  - **Vampire Mode**: Prioritizes building shadows to minimize UV exposure (essential for summer)

- **🗺️ Interactive 3D Map**
  - Real-time shadow visualization using building geometry
  - Time-based scenarios (Morning, Noon, Evening, Night)
  - Dynamic sun simulation throughout the day

- **🎨 Modern UI Design**
  - Beautiful glass-morphism interface inspired by VisionOS
  - Smooth scroll-snap navigation
  - Intuitive route comparison interface

- **📊 Route Comparison**
  - Compare Shadow Path, Direct Path, and Sunny Path
  - Real-time shade percentage calculations
  - Estimated walking time and distance

---

## 🛠️ Technology Stack

### Data Sources
- **OpenStreetMap (OSM)**: Building footprints & height tags for 2.5D city model construction
- **SunCalc.js**: Solar azimuth and altitude calculations based on geolocation and time
- **Mapbox GL JS**: Rendering engine for 3D extrusion and real-time shadow casting

### Frontend Technologies
- **Mapbox GL JS v3.4.0**: Interactive 3D mapping
- **Tailwind CSS**: Utility-first CSS framework
- **Font Awesome 6.4.0**: Icon library
- **Google Fonts (Inter)**: Typography

---

## 🚀 Getting Started

### Live Demo
Visit the live application: [https://minweizhao.github.io/ugod5104-sunspot/](https://minweizhao.github.io/ugod5104-sunspot/)

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/MinweiZhao/ugod5104-sunspot.git
   cd ugod5104-sunspot
   ```

2. **Open in browser**
   Simply open `index.html` in a modern web browser, or use a local server:

   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js (http-server)
   npx http-server
   ```

3. **Access the application**
   Navigate to `http://localhost:8000` in your browser

### Requirements
- Modern web browser with JavaScript enabled
- Internet connection (for CDN resources and Mapbox API)
- Mapbox access token (for production use)

---

## 📖 How to Use

1. **Select Your Preference**
   - **Cool** (❄️): Minimize sun exposure, maximize shade
   - **Fast** (⚡): Traditional shortest path
   - **Hot** (☀️): Maximize sun exposure

2. **Choose Origin & Destination**
   - Click on the map to set your starting point
   - Click again to set your destination

3. **View Route Options**
   - Compare three route alternatives with different shade percentages
   - Switch between routes to see the optimal path for your preference

4. **Explore Time Scenarios**
   - Use the time selector to see how shadows change throughout the day
   - Watch the sun simulation to understand dynamic shadow patterns

---

## 🔬 Methodology

### Dual-Mode Routing Algorithm

The core innovation of SunSpot is its **Dual-Mode Routing Algorithm** that calculates path weights based on solar exposure:

1. **Building Geometry Analysis**: Extract 3D building data from OpenStreetMap
2. **Solar Position Calculation**: Use SunCalc.js to determine sun position at any given time
3. **Shadow Ray-Casting**: Calculate which parts of the route are in shadow
4. **Path Weight Optimization**: Adjust route weights to maximize or minimize solar exposure based on user preference

---

## ⚠️ Limitations & Future Work

### Current Limitations

- **Data Gaps**: Building heights in OSM are often estimated or missing, leading to potential "light leaks" in the shadow model
- **Missing Canopy**: Current model only accounts for concrete structures. Street trees, a vital source of shade, are not yet included

### Future Enhancements

- Integration of street tree canopy data
- Real-time weather integration
- Machine learning for improved shadow prediction
- Mobile app development
- Multi-modal transportation support

---

## 📁 Project Structure

```
ugod5104-sunspot/
├── index.html          # Main application file
└── README.md           # Project documentation
```

---

## 👨‍💻 Team

**UGOD5104 Group 4**

This project was developed as part of the UGOD5104 course.

---

## 📄 License

© 2024 UGOD5104 Group 4. All rights reserved.

---

## 🙏 Acknowledgments

- **OpenStreetMap** contributors for building data
- **Mapbox** for mapping infrastructure
- **SunCalc.js** for solar calculations
- The open-source community for inspiration and tools

---

## 📧 Contact

For questions, suggestions, or collaborations, please open an issue on the [GitHub repository](https://github.com/MinweiZhao/ugod5104-sunspot).

---

<div align="center">

**Made with ❤️ by UGOD5104 Group 4**

[⬆ Back to Top](#-sunspot-the-ephemeral-city)

</div>
