# 🎒 Musette

**Enrich your ride.** Drop a GPX file, pick what you need along the route, and download an enriched file with waypoints for cafes, water, camping, pubs, and more.

[**Try it →**](https://surlykm.github.io/Musette)

## What it does

Musette takes a GPX route file and enriches it with points of interest along the way:

- ⛺ Camping & lodging
- 💧 Water & restrooms
- ☕ Cafes, restaurants & pubs
- 🛒 Supermarkets & convenience stores
- 🚲 Bike shops
- 🏥 Hospitals & pharmacies
- 💳 ATMs

Plus a live preview with:

- Route map with toggleable POI layers
- Elevation profile with hover tracking
- 7-day weather forecast at points along the route
- Route stats (distance, climbing, elevation range)

Download the enriched GPX and upload it to Ride with GPS, Garmin Connect, or your GPS device. POIs appear as waypoints with proper icons.

## How to use

1. Go to [surlykm.github.io/musette](https://surlykm.github.io/musette)
2. Upload your `.gpx` file
3. Enter your [Geoapify API key](https://myprojects.geoapify.com) (free, 3,000 requests/day)
4. Pick which POI types you want and set the search radius
5. Hit **Enrich route**
6. Preview on the map, then **Download enriched GPX**

## Tech

Fully client-side. No backend, no data leaves your browser except API calls to:

- [Geoapify Places API](https://www.geoapify.com) for POI data
- [Open-Meteo](https://open-meteo.com) for weather forecasts
- [OpenStreetMap](https://www.openstreetmap.org) for map tiles

Hosted on GitHub Pages.

## Output format

Currently exports GPX with waypoints formatted for **RidewithGPS** (using their POI type values) and Garmin, Wahoo, and Komoot formats.

## Local development

It's a single `index.html`. Open it in a browser or serve it locally:

```
python3 -m http.server 8000
```

## Licence

MIT
