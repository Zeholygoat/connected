# CONNECTED

Connected is a Netlify-ready animated global mobility observatory.

## Current build
- Dark world visual with route network
- Air / Sea / Rail / Road / All filters
- Unique neon colour for each mode
- Animated vehicle particles
- Curved routes and trails
- Clickable moving nodes with detail cards
- Pause / resume
- Reset
- Live UTC clock
- Animated activity/frequency panels
- Responsive mobile layout
- Zero build step: `index.html` is enough for Netlify

## Data integrity
The browser build currently uses a **clearly labelled simulation layer**. It does not claim that its counters, routes, or vehicle identities are live telemetry.

A true live production version needs a backend/edge data layer and licensed or public feeds. GTFS Realtime supports vehicle positions, trip updates, service alerts and trip modifications for participating public-transport agencies. Vehicle positions can include latitude, longitude, bearing, speed and vehicle/trip identifiers. See https://gtfs.org/documentation/realtime/feed-entities/vehicle-positions/ and https://gtfs.org/documentation/realtime/.

OpenSky provides live aircraft state data and API access, with authentication/rate limits and usage policies that must be respected. See https://opensky-network.org/data/api and https://opensky-network.org/about/faq.

## Deploy
1. Unzip.
2. Put `index.html` in a GitHub repository.
3. In Netlify, import that repository.
4. Build command: none.
5. Publish directory: repository root.

For a real-data deployment, keep API credentials server-side rather than putting secrets in `index.html`.
