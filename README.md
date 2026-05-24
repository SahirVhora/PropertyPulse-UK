# 🏠 UK Property Toolkit - PropertyPulse-UK

**The flagship dashboard: postcode intelligence with scoring, mapping, and multi-dimensional analytics.**

[![License: MIT](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![PropertyPulse](https://img.shields.io/badge/toolkit-flagship-blue)](https://sahirvhora.github.io/PropertyPulse-UK)

Part of the **[UK Property Toolkit](https://github.com/SahirVhora?tab=repositories&q=uk-property+OR+PropertyPulse+OR+HomeFinder+OR+postcode-checker)** - three free tools for UK home buyers.

| Tool | Purpose | Best For |
|---|---|---|
| **PropertyPulse-UK** ← you are here | Postcode intelligence + scoring + map | Deep area research |
| [UK-HomeFinder](https://github.com/SahirVhora/UK-HomeFinder) | Property tracking + SDLT + checklist | Active buyers comparing properties |
| [uk-postcode-checker](https://github.com/SahirVhora/uk-postcode-checker) | Quick demographic lookup | Fast postcode overview |
| [uk-mortgage-rate-monitor](https://github.com/SahirVhora/uk-mortgage-rate-monitor) | Daily 2-year fixed mortgage monitoring | Rate timing and lock/watch decisions |

👉 **[Launch PropertyPulse-UK](https://sahirvhora.github.io/PropertyPulse-UK)**

---

## 🌟 Key Features

### 📊 Multi-Dimensional Intelligence
- **Crime Analytics:** Street-level crime statistics and trends via Police Data API
- **Education Insights:** Nearby schools with ratings, proximity, and Ofsted links
- **Demographic Data:** Census 2021 ethnicity and tenure data via ONS Beta API
- **Environmental Risk:** Real-time flood risk monitoring via Environment Agency API
- **Geospatial Mapping:** Interactive Leaflet maps powered by OpenStreetMap
- **Air Quality:** Local air quality index data
- **Composite Scoring:** Weighted scores across crime, schools, transport, and flood

### ⚡ Zero-Infrastructure Architecture
- **Serverless:** Pure HTML/JS/CSS - no backend, no database, no install
- **Direct API Integration:** Fetches from government/public APIs in-browser
- **Dark-mode UI:** Modern intelligence dashboard aesthetic, responsive layout

## 🛠️ Technical Stack

- **Frontend:** Vanilla JavaScript (ES6+), HTML5, CSS3
- **Mapping:** [Leaflet.js](https://leafletjs.com/)

## 🚀 Getting Started

```bash
git clone https://github.com/SahirVhora/PropertyPulse-UK.git
cd PropertyPulse-UK
open index.html
```

No server, no build step. Just open the file.

### Google Places API (Optional)
To enable star ratings for schools:
1. Get an API key from [Google Cloud Console](https://console.cloud.google.com)
2. Enable the **Places API**
3. Open `index.html` and paste your key in `const GOOGLE_PLACES_KEY = ""`

## 🔌 APIs Integrated

| API | Purpose | License |
|---|---|---|
| **Postcodes.io** | Lat/Lng, Ward, District, LSOA | Open |
| **Police Data API** | Street-level crime statistics | Open Government Licence |
| **ONS Beta API** | Census 2021 ethnicity & tenure | Open Government Licence |
| **DfE Education API** | Schools search and details | Public |
| **Environment Agency** | Flood risk monitoring | Open Government Licence |
| **OpenStreetMap** | Map tiles and geospatial data | ODbL |

## 📂 Project Structure
```
PropertyPulse-UK/
├── index.html    ← Core Application
└── README.md     ← Documentation
```

## 🔗 Also in the UK Property Toolkit

- **[UK-HomeFinder](https://github.com/SahirVhora/UK-HomeFinder)** - Property comparison tracker, SDLT calculator, readiness checklist, Rightmove/Zoopla URL parser
- **[uk-postcode-checker](https://github.com/SahirVhora/uk-postcode-checker)** - Fast demographics: crime charts, ethnicity/religion/tenure breakdowns, schools, transport

## 📝 Notes
- All data sourced from official public APIs. School catchment boundaries are indicative.
- No user data is stored or transmitted - all API calls are client-side.
- Privacy-first: no tracking, no ads, no analytics.

## License

MIT - see [LICENSE](LICENSE)
