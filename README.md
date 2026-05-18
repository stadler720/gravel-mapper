# 🪨 GravelMapper

> Find it. Ride it. Report it.

GravelMapper is a community-powered mobile app for gravel cyclists to discover, map, and rate gravel roads. Built with React Native, Expo, and Mapbox — seeded with OpenStreetMap data and kept accurate by riders like you.

---

## The Problem

Gravel cyclists currently stitch together Google Maps, Strava, local Facebook groups, and paper maps just to find rideable gravel. There's no purpose-built tool for it. GravelMapper fixes that.

---

## Features (v1)

- 🗺️ **Map view** — gravel roads highlighted automatically using OpenStreetMap data
- 👆 **Tap any road** — see surface type, condition, and community notes
- ✏️ **Trace roads** — draw new gravel segments directly on the map
- 📍 **Drop pins** — mark a road with a quick condition report
- 📁 **GPX upload** — import a route file and tag its surface
- 🟢🟡🔴 **Condition tags** — Rideable / Rough / Avoid

---

## Tech Stack

| Layer | Tool |
|---|---|
| Mobile framework | React Native + Expo |
| Maps | Mapbox SDK |
| Backend / Database | Supabase |
| Road surface data | OpenStreetMap (Overpass API) |
| Language | TypeScript |
| Version control | GitHub |

---

## Project Structure

```
gravel-mapper/
├── app/
│   ├── index.tsx          # Main map screen
│   ├── report.tsx         # Add / edit a road report
│   └── route-detail.tsx   # View a saved route
├── components/
│   ├── MapView.tsx        # Mapbox map wrapper
│   ├── RoadPin.tsx        # Pin marker on map
│   ├── ConditionTag.tsx   # Rideable / Rough / Avoid badge
│   └── GPXUploader.tsx    # GPX file import component
├── services/
│   ├── osm.ts             # OpenStreetMap Overpass API queries
│   ├── supabase.ts        # Supabase database client
│   └── gpx.ts             # GPX file parser
├── assets/                # Icons, images, fonts
├── docs/
│   ├── SETUP.md           # Dev environment setup guide
│   └── CONTRIBUTING.md    # How to contribute
└── app.json               # Expo configuration
```

---

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher)
- [Expo CLI](https://docs.expo.dev/get-started/installation/)
- [Mapbox account](https://account.mapbox.com/auth/signup/) (free)
- [Supabase account](https://supabase.com/) (free)

### Installation

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/gravel-mapper.git
cd gravel-mapper

# Install dependencies
npm install

# Copy environment variables
cp .env.example .env

# Add your keys to .env
# MAPBOX_ACCESS_TOKEN=your_token_here
# SUPABASE_URL=your_url_here
# SUPABASE_ANON_KEY=your_key_here

# Start the app
npx expo start
```

Then scan the QR code with the **Expo Go** app on your phone.

---

## Roadmap

### v1 — Core (current)
- [x] Project setup
- [ ] Mapbox map displaying on device
- [ ] OSM gravel roads highlighted on map
- [ ] Tap road → view condition
- [ ] Add condition report (pin / trace / GPX)
- [ ] Save reports to Supabase

### v2 — Community
- [ ] User accounts
- [ ] Route saving and sharing
- [ ] Search by distance / elevation / % gravel
- [ ] Photos on road reports

### v3 — Discovery
- [ ] Route recommendations
- [ ] Offline map downloads
- [ ] Integration with Garmin / Wahoo devices

---

## Contributing

Gravel riders welcome! See [CONTRIBUTING.md](docs/CONTRIBUTING.md) to get started.

---

## License

MIT — free to use, fork, and ride.

---

*Built by a gravel cyclist, for gravel cyclists.*
