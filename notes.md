The goal of this project is to develop the ability to render WIND AND OCEAN CURRENTS on an OpenLayers map.

The starting point for this project is https://openlayers.org/en/latest/examples/webgl-points-layer.html

What's the plan??
    I would prefer to develop this to a standard for acceptance as a contribution to OpenLayers. To that end, I have had a brief interation with OL developer/contributor Tim Schaub @tschaub on the OpenLayers gitter (https://gitter.im/openlayers/openlayers?utm_source=notification&utm_medium=email&utm_campaign=unread-notifications#) & he expressed some interest in the project. I plan to keep in touch as progress is made.

    He suggested (top of head, just ideas!):
        A WebGL solution utilizing the existing DATA TILE SOURCE (https://openlayers.org/en/latest/apidoc/module-ol_source_DataTile-DataTileSource.html) and the existing WEBGL TILE RENDERER (https://openlayers.org/en/latest/apidoc/module-ol_renderer_webgl_TileLayer-WebGLTileLayerRenderer.html) for loading the data and uploading textures representing velocity vectors. 

Some brief notes about the data in this repo:
    /data/geoJSON/world-cities.geoJSON: taken from the webgl-points-layer demo mentioned above
    /data/geoJSON/weather.json: taken from a wind-arrows example (https://openlayers.org/en/latest/examples/wind-arrows.html) which sourced from https://openweathermap.org/current. This data covers a small area around Baton Rouge (this file is NOT in geoJSON format!!)
    /data/geoJSON/spread-weather.json: this is derivative of weather.json, but the lats/lons have been randomized to spread them across the globe. This has also been converted to geoJSON format.
    /data/mvt/ascat.mvt: This data is sourced from NOAA (https://manati.star.nesdis.noaa.gov/datasets/ASCATData.php). I ultimately need this project to work with MVT data.

----------------------------
Roadmap:
    [X] Render /data/geojson/spread_weather.json on map (any fashion)
    [ ] Render *any* animation with WebGL/GLSL; for instance, random streaking lines
    [ ] Calculate and render weather particle positions (direction & strength)
    [ ] Render /data/mvt/ascat.mvt on map
    [ ] Calculate and render ASCAT particle positions (direction & strength)
    