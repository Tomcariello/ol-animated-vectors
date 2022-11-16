# What's the plan??

My goal for this project is to develop the ability to render **WIND AND OCEAN CURRENTS** from an MVT file on an OpenLayers 7.1.0 map. This needs to work well across browsers & on mobile & interact nicely with OpenLayers existing functionality.

I will try to remain active on the OpenLayers gitter (https://gitter.im/openlayers/openlayers) for feedback and/or guidance for the duration of this project. 

# How to run
- git clone https://github.com/Tomcariello/ol-animated-vectors.git
- npm install
- npm start

# Data in this repo
- /data/geoJSON/world-cities.geoJSON: taken from the webgl-points-layer demo mentioned above

- /data/geoJSON/spread-weather.json: this is derivative of weather.json, but the lats/lons have been randomized to spread them across the globe. This has also been converted to geoJSON format.

- /data/geoJSON/weather.json: taken from a wind-arrows example (https://openlayers.org/en/latest/examples/wind-arrows.html) which is sourced from https://openweathermap.org/current. This data covers a small area around Baton Rouge (this file is NOT in geoJSON format!!)

- /data/mvt/ascat.mvt: This data is sourced from NOAA (https://manati.star.nesdis.noaa.gov/datasets/ASCATData.php). I ultimately need this project to work with MVT data but am starting with GeoJSON for simplicity.

# Intended Roadmap
[X] Clone webgl-points-layer example & reduce to the basics

[X] Replace data source "world-cities.geojson" with "spread_weather.json"

[-] Render *any* animation with WebGL/GLSL; for instance, random streaking lines

[-] Calculate and render weather particle positions (direction & velocity)

[-] Render /data/mvt/ascat.mvt on map

[-] Calculate and render ASCAT particle positions (direction & velocity)

# Other Stuff
This project started as a clone of https://openlayers.org/en/latest/examples/webgl-points-layer.html

If you find this repo & want to contribute/chat/criticize, feel free to reach out.