# 🏠 PropertyPulse UK - Intelligence Dashboard

A high-performance, single-file property research tool that aggregates real-time public data to provide deep insights into any UK postcode. Designed for home buyers, renters, and real estate researchers to make data-driven decisions.

## 🌟 Key Features

### 📊 Multi-Dimensional Intelligence
The dashboard transforms a simple postcode into a comprehensive intelligence report:
- **Crime Analytics:** Street-level crime statistics and trends using the Police Data API.
- **Education Insights:** Nearby schools discovery including ratings and proximity.
- **Demographic Data:** Census 2021 ethnicity and tenure data from the ONS Beta API.
- **Environmental Risk:** Real-time flood risk monitoring via the Environment Agency Flood API.
- **Geospatial Mapping:** Integrated interactive maps powered by Leaflet and OpenStreetMap.

### ⚡ Zero-Infrastructure Architecture
- **Serverless:** Pure HTML/JS/CSS. No backend, no database, and no installation required.
- **Direct API Integration:** Fetches data directly from government and public APIs in the browser.
- **High Performance:** Optimized for speed with a modern dark-mode UI and responsive layout.

## 🛠️ Technical Stack

- **Frontend:** Vanilla JavaScript (ES6+), HTML5, CSS3
- **Mapping:** [Leaflet.js](https://leafletjs.com/)
- **Data Visualization:** [Chart.js](https://www.chartjs.org/)
- **Styling:** Custom CSS Variables for a modern "Intelligence Dashboard" aesthetic.

## 🚀 Getting Started

### How to Run
Since this is a self-contained application, there is no build step:
1. Clone the repository.
2. Double-click `index.html` to open it in any modern web browser.

### Google Places API (Optional)
To enable star ratings for schools:
1. Get an API key from the [Google Cloud Console](https://console.cloud.google.com).
2. Enable the **Places API**.
3. Open `index.html` and find the `GOOGLE_PLACES_KEY` constant.
4. Paste your key between the quotes:
   ```javascript
   const GOOGLE_PLACES_KEY = "YOUR_KEY_HERE";
   ```

## 🔌 APIs Integrated

| API | Purpose | License |
|-----|----------|-------|
| **Postcodes.io** | Lat/Lng, Ward, District, LSOA codes | Open |
| **Police Data API** | Street-level crime statistics | Open Government Licence |
| **ONS Beta API** | Census 2021 ethnicity & tenure data | Open Government Licence |
| **DfE Education API**| Schools search and details | Public |
| **Environment Agency**| Flood risk monitoring | Open Government Licence |
| **OpenStreetMap** | Map tiles and geospatial data | ODbL |

## 📂 Project Structure
```
PropertyPulse-UK/
├── index.html    ← Core Application (UI, Logic, and Styles)
└── README.md     ← Documentation
```

## 📝 Notes
- **Data Accuracy:** All data is sourced from official public APIs. School catchment boundaries and crime dates are indicative of the latest available public releases.
- **Privacy:** No user data is stored or transmitted to a private server; all API calls are made directly from the client's browser to the respective public endpoints.
