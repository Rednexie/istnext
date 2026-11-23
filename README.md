# istnext (formerly iettnext)

> Real-time Istanbul public transport vehicle tracking and city data platform.
> **"Bringing data to 16 million people."**

 [istnext.com.tr](https://istnext.com.tr)
**v2:** [istnext.com.tr/app](https://istnext.com.tr/app)
**v1:** [iett.rednexie.workers.dev](https://iett.rednexie.workers.dev)

🇹🇷 [Türkçe README](./README.tr.md)

---

## About

istnext is an independent, open-source project that brings Istanbul's public transport and city data together in a single, fast interface. It lets you track buses live, query stops and lines, look up vehicle details, and explore city statistics.

> **Disclaimer:** istnext is **not** an official service of the Istanbul Metropolitan Municipality (İBB) or İETT. It is built by independent developers.

> **Data availability notice:** Some features and information that were previously available are no longer shared, because of the administrative pressure and data access restrictions imposed by the Istanbul Metropolitan Municipality (İBB). As a result, some features may be limited, unavailable, or removed over time.

---

## Features

### 🚍 Vehicle Query (`/app/arac`)
- Look up live İETT, ÖHO and Otobüs A.Ş. vehicles by **door code** or **plate number**
- Live GPS position, speed, model and technical/fleet details
- View the vehicle's location on a map and open it in Google Maps
- Favorite vehicles
- Share a vehicle card: native share, WhatsApp, copy as Markdown, copy as text, or share link
- "View on İETT" shortcut

### 🚏 Journey: Stop & Line Query (`/app/yolculuk`)
- **Stop search:** stop details and live arrival times of approaching buses
- **Line search:** route, timetable (departure times), vehicles currently on the line, and line info
- Direction switching and line filtering at a stop
- Stop and line announcements, with the option to share them
- Line-type indicators: ÖHO (red) and İETT (normal)
- Favorites for stops and lines
- Offline mode: previously saved data is shown when you're offline

### 🏠 Home (`/app`)
- Quick access to Stop, Line, Vehicle and Explore
- **Traffic status:** traffic index, plus Europe and Anatolia side percentages
- **City announcements:** filter by All / Route & Road / Trip Cancellations
- **My Shortcuts:** saved favorite stops, lines and vehicles
- **Sync key:** move your favorites between devices with a personal key (format `IST-XXXX-XXXX-XXXX`), with no account needed

### 🧭 Explore & Data Hub (`/app/kesfet`)
- Open-data statistics, metro line routes, fuel consumption, archived trips and live announcements
- Old lines and archive: past years' line data, removed routes and archived trip records
- City information: Istanbul dam occupancy rates, live traffic density and other city data
- Links to the official source pages

### 📱 PWA
- Installable as an app on your device, for a faster, full-screen experience
- Optional launch notifications
- Dark and light themes

---

## Privacy (summary)

- **Location:** your device location is processed only temporarily in your browser's memory for nearby-stop features and is not saved to servers.
- **Local Storage:** used only for your theme and favorite stops/lines. There are no advertising cookies and no profiling.
- **Security data:** your IP address and basic device data may be processed for security, bot prevention and anonymous statistics.
- **Infrastructure:** Cloudflare is used for network security and fast delivery.

Full text: see the *Privacy Policy* and *Terms of Use* on the website.

---

## Data Sources & Accuracy

Vehicle positions, trip info, stop data and other statistics are compiled from various open-data sources, including the [İBB Open Data Portal](https://data.ibb.gov.tr/). Some data that was previously shared is no longer provided by İBB, so the related features and information are no longer available. istnext cannot be held responsible for delayed, incorrect or missing data. The service is provided "as is", with no uptime guarantee.

---

## Tech Stack

- **Runtime / Hosting:** Bun.js
- **Database:** PostgreSQL
- **Language:** TypeScript
- **Frontend:** HTML, JavaScript, CSS

---

## Contributing

Issues and pull requests are welcome. Please open an issue first to discuss major changes.

---

## License

The source code of this project is licensed under the **MIT License**. See the [LICENSE](./LICENSE) file for details.

Data obtained from the İBB Open Data Portal is subject to its own terms: [data.ibb.gov.tr/license](https://data.ibb.gov.tr/license).

---

## Changelog

### v2.0.1
- Added support for dam information
- Old lines data is back
- Fixed an issue with the vehicle information page

### v2.0.0
- Added Progressive Web App (PWA) support
- Expanded the available metrics section on the Explore page
- Added formatted sharing for query results
- Added light theme

### v1 — iettnext
- Initial release, still available at [iett.rednexie.workers.dev](https://iett.rednexie.workers.dev)
