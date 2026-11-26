# istnext (formerly iettnext)


> **"Making Istanbul's data owned to its 16 million people."**

**v2:** [istnext.com.tr/app](https://istnext.com.tr/app)



**v1:** [iett.rednexie.workers.dev](https://iett.rednexie.workers.dev)

🇹🇷 [Türkçe README](./README.tr.md)

---

## About

istnext is a platform to access istanbul's public transport data sources from a single, modern, open source and fast gui.

> [!Caution]
>  istnext is **not** an official service of the Istanbul Metropolitan Municipality or İETT.

> [!Caution]
> Some features and information that were previously available are no longer shared, because of the administrative pressure and data access restrictions imposed by the Istanbul Metropolitan Municipality. As a result, some features may be limited, unavailable, or removed over time.

---

## Features

### Vehicle Query (`/app/arac`)
- Look up live İETT, ÖHO and Otobüs A.Ş. vehicles by **door code** or **plate number**
- Live GPS position, speed, model and technical/fleet details
- View the vehicle's location on a map and open it in Google Maps
- Favorite vehicles to easily track them later
- Share a vehicle card: native share, WhatsApp, copy as Markdown, copy as text, or share link

### Journey: Stop & Line Query (`/app/yolculuk`)
- **Stop search:** stop details and live arrival times of approaching buses
- **Line search:** route, timetable (departure times), vehicles currently on the line, and line info
- Direction switching and line filtering at a stop
- Stop and line announcements, with the option to share them
- Favorites for stops and lines
- Offline mode: previously saved data is shown when you're offline

### Home (`/app`)
- **Traffic status:** traffic index, plus Europe and Anatolia side percentages
- **City announcements:** filter by All / Route & Road / Trip Cancellations
- **Dam Information**: Access the water levels of Istanbul's dams.

### Explore & Data Hub (`/app/kesfet`)
- Open-data statistics, metro line routes, fuel consumption, archived trips and live announcements
- Old lines and archive: past years' line data, removed routes and archived trip records

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

- **Server Runtime:** Cloudflare Workers
- **Database:** PostgreSQL
- **Language:** TypeScript
- **Frontend:** HTML, JavaScript, CSS

---

## Contributing

- Problems & bugs? -> issues
- Code Changes? -> pull requests 
- Suggestions, discussions, chat? -> discussions

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
