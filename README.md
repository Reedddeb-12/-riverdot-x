# 🌊 RiverDOT-X - LiDAR River Intelligence Dashboard

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

A modern, interactive web-based dashboard for LiDAR-driven river intelligence and erosion monitoring. Built for hackathons and rapid prototyping with zero backend dependencies.

![RiverDOT-X Dashboard](https://via.placeholder.com/800x400/0ea5e9/ffffff?text=RiverDOT-X+Dashboard)

## ✨ Features

### 🗺️ Interactive Mapping
- **Multi-layer visualization** - Satellite imagery, LiDAR hillshade, elevation/slope analysis
- **Real-time hotspot tracking** - Erosion and sedimentation zones with risk severity indicators
- **5 pre-configured rivers** - Yamuna, Ganga, Brahmaputra, Godavari, Narmada
- **Custom river support** - Add your own river locations

### 📊 Advanced Analytics
- **Clickable hotspots** - Detailed risk analysis with time-to-failure estimates
- **Interactive charts** - Monthly erosion trends powered by Plotly.js
- **Risk summary dashboard** - Real-time statistics for critical, high, and moderate zones

### 🎮 Scenario Simulation
- **Discharge simulator** - Visualize impact of +10%, +30%, +50% river discharge
- **Digital twin timeline** - View riverbank evolution from 2020-2024
- **Dynamic hotspot updates** - See real-time changes based on scenarios

### 📤 Data Management
- **LiDAR data upload** - Support for GeoJSON, TIF, LAS, LAZ formats
- **Automatic processing** - Instant visualization of uploaded datasets
- **Sample datasets included** - Ready-to-use Yamuna and Ganga river data

### 👥 Community Engagement
- **Issue reporting** - Citizens can report erosion, flooding, pollution
- **Community reports** - View and upvote community-submitted issues
- **Alert subscriptions** - Email/SMS notifications for critical events
- **Severity filtering** - Sort reports by risk level

## 🚀 Quick Start

### Option 1: Direct Browser
```bash
# Clone the repository
git clone https://github.com/yourusername/riverdot-x.git

# Navigate to directory
cd riverdot-x

# Open in browser
open index.html  # macOS
start index.html # Windows
xdg-open index.html # Linux
```

### Option 2: Local Server
```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx http-server

# Then visit http://localhost:8000
```

## 📁 Project Structure

```
riverdot-x/
├── index.html                      # Main application
├── styles.css                      # Light blue theme styling
├── app.js                          # Core functionality
├── sample-lidar-yamuna.geojson    # Sample dataset 1
├── sample-lidar-ganga.geojson     # Sample dataset 2
└── README.md                       # Documentation
```

## 🎯 Usage Guide

### 1. Exploring the Dashboard
1. Click **"Explore River Dashboard"** on the landing page
2. Use the **river selector** in the header to switch between rivers
3. Toggle **map layers** in the left sidebar
4. Click on **colored hotspots** to view detailed analysis

### 2. Running Scenarios
1. Adjust the **"River Discharge"** slider to simulate flood conditions
2. Move the **"Digital Twin Timeline"** slider to view historical data
3. Watch hotspots dynamically update based on your selections

### 3. Uploading LiDAR Data
1. Select a river from the dropdown
2. Click **"Choose LiDAR File"** in the left sidebar
3. Select a GeoJSON file (samples provided)
4. Click **"Process & Display"**
5. New hotspots will appear with purple borders

### 4. Community Features
1. Click the **floating community button** (bottom-right)
2. **Report issues** - Submit erosion or flooding reports
3. **View reports** - Browse community submissions
4. **Subscribe** - Get alerts for your area

## 🌍 Pre-configured Rivers

| River | Location | Hotspots | Risk Level |
|-------|----------|----------|------------|
| Yamuna | Delhi-Agra Corridor | 8 | High |
| Ganga | Varanasi-Patna | 5 | Medium |
| Brahmaputra | Assam Valley | 6 | Critical |
| Godavari | Telangana Region | 4 | Medium |
| Narmada | Madhya Pradesh | 4 | Medium |

## 🛠️ Technologies

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Mapping**: [Leaflet.js](https://leafletjs.com/) v1.9.4
- **Charts**: [Plotly.js](https://plotly.com/javascript/) v2.27.0
- **Styling**: Custom CSS with gradient themes
- **No Backend**: 100% client-side application

## 🎨 Design Features

- **Modern light blue theme** - Clean, professional aesthetic
- **Gradient animations** - Smooth transitions and hover effects
- **Responsive layout** - Adapts to different screen sizes
- **Glass-morphism effects** - Modern UI design patterns
- **Interactive elements** - Engaging user experience

## 📊 Sample Data Format

### GeoJSON Structure
```json
{
  "type": "FeatureCollection",
  "features": [{
    "type": "Feature",
    "properties": {
      "name": "Riverbank Section A",
      "elevation_min": 185.2,
      "elevation_max": 198.5,
      "erosion_risk": "High",
      "scan_date": "2024-11-15"
    },
    "geometry": {
      "type": "Polygon",
      "coordinates": [[[lng, lat], ...]]
    }
  }]
}
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🎯 Use Cases

- **Government Agencies** - River monitoring and flood management
- **Research Institutions** - Erosion pattern analysis
- **NGOs** - Community-driven environmental monitoring
- **Hackathons** - Rapid prototyping and demos
- **Education** - Teaching GIS and environmental science

## 🚧 Roadmap

- [ ] Real-time data integration via APIs
- [ ] Machine learning for erosion prediction
- [ ] Mobile app version
- [ ] Multi-language support
- [ ] Export reports as PDF
- [ ] Integration with weather data

## 📧 Contact

For questions or feedback, please open an issue on GitHub.

## 🙏 Acknowledgments

- Leaflet.js for excellent mapping library
- Plotly.js for interactive charts
- OpenStreetMap contributors
- Esri for satellite imagery tiles

---

**Built with ❤️ for better river management**
