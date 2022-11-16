The goal of this project is to develop the ability to render WIND AND OCEAN CURRENTS on an OpenLayers map. 

The starting point for this project is https://openlayers.org/en/latest/examples/webgl-points-layer.html

What's the plan??
    I would prefer to develop this to a standard for acceptance as a contribution to OpenLayers. To that end, I have had a brief interation with OL developer/contributor Tim Schaub @tschaub on the OpenLayers gitter (https://gitter.im/openlayers/openlayers?utm_source=notification&utm_medium=email&utm_campaign=unread-notifications#) & he expressed interest in this project. 

    "...a custom renderer for vector fields would make a great addition. I can imagine a WebGL solution that took advantage of the existing DATA TILE SOURCE (https://openlayers.org/en/latest/apidoc/module-ol_source_DataTile-DataTileSource.html) 

    ...and some of the existing WEBGL TILE RENDERER (https://openlayers.org/en/latest/apidoc/module-ol_renderer_webgl_TileLayer-WebGLTileLayerRenderer.html)

    ...for loading the data and uploading textures representing velocity vectors. The remaining work would be to calculate and render particle positions."

I am pursuing my solution & once I have something functional I will reach out to Mr Schaub again for feedback.

The data:
    world-cities.geoJSON: taken from the webgl-points-layer demo mentioned above
    weather.json: taken from a wind-arrows example (https://openlayers.org/en/latest/examples/wind-arrows.html) which sourced from https://openweathermap.org/current. This data covers a small area around Baton Rouge
    spread-weather.json: this is derivative of weather.json, but the lats/lons have been randomized to spread them across the globe. This has also been hand-tuned into geoJSON format.

----------------------------
Roadmap:
    [X] Render /data/geojson/spread_weather.json on map
    [ ] Render *any* animation with WebGL/GLSL; for instance, random streaking lines
    [ ] Render weather data with WebGL/GLSL accurately
    [ ] Render /data/mvt/ascat.mvt on map
    [ ] Render ascat data with WebGL/GLSL accurately
    