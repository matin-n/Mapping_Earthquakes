# Mapping_Earthquakes

## Project Overview

An interactive map is created to visualize live earthquake data in relation to tectonic plate locations.

### Earthquake Data

The script fetches live geoJSON data from the Earthquake Hazards Program from [USGS.gov](https://earthquake.usgs.gov/earthquakes/feed/v1.0/geojson.php). The earthquake data is updated every minute and includes earthquakes within the past week.

Each earthquake is drawn as a `circleMarker` with the circle color and size to indicate the earthquake's magnitude. Additionally, each `circleMarker` features a clickable popup to display the magnitude and location of the earthquake.

### Tectonic Plates

The tectonic plate `LineString` data is overlayed on top of the map. The tectonic data is made available by [Hugo Ahlenius](https://github.com/fraxen), Nordpil and Peter Bird. Additionally, [csterling](https://github.com/csterling) made the data available in geoJSON format.

## Resources

- Data Source: [`4.5_week.geojson`](https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/4.5_week.geojson), [`all_week.geojson`](https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_week.geojson), [`PB2002_boundaries.json`](https://raw.githubusercontent.com/matin-n/tectonicplates/master/GeoJSON/PB2002_boundaries.json)
- Libraries: [`Leaflet.js`](https://leafletjs.com/), [`D3.js`](https://d3js.org/)
- Additional: [OpenStreetMap](https://www.openstreetmap.org/), [Mapbox](https://www.mapbox.com/)
- Source Code: [challenge_logic.js](Earthquake_Challenge/static/js/challenge_logic.js), [index.html](Earthquake_Challenge/index.html), [style.css](Earthquake_Challenge/static/css/style.css)
