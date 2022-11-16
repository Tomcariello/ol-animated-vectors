What's the plan??
    My goal for this project is to develop the ability to render WIND AND OCEAN CURRENTS from an MVT file on an OpenLayers map. This needs to work well across browsers & on mobile & interact nicely with OpenLayers existing functionality.
        
    I believe this feature would be welcome by OpenLayers users looking to achieve similar goals. I will keep a dialogue open on the OpenLayers gitter (https://gitter.im/openlayers/openlayers) for feedback and/or guidance.

    Tim Schaub, an OL contributor/developer, suggested (top of head, just ideas!):
        A WebGL solution utilizing the existing DATA TILE SOURCE (https://openlayers.org/en/latest/apidoc/module-ol_source_DataTile-DataTileSource.html) and the existing WEBGL TILE RENDERER (https://openlayers.org/en/latest/apidoc/module-ol_renderer_webgl_TileLayer-WebGLTileLayerRenderer.html) for loading the data and uploading textures representing velocity vectors. 

Some brief notes about the data in this repo:
    /data/geoJSON/world-cities.geoJSON: taken from the webgl-points-layer demo mentioned above
    
    /data/geoJSON/weather.json: taken from a wind-arrows example (https://openlayers.org/en/latest/examples/wind-arrows.html) which sourced from https://openweathermap.org/current. This data covers a small area around Baton Rouge (this file is NOT in geoJSON format!!)
    
    /data/geoJSON/spread-weather.json: this is derivative of weather.json, but the lats/lons have been randomized to spread them across the globe. This has also been converted to geoJSON format.
    
    /data/mvt/ascat.mvt: This data is sourced from NOAA (https://manati.star.nesdis.noaa.gov/datasets/ASCATData.php). I ultimately need this project to work with MVT data.

This project started as a clone of https://openlayers.org/en/latest/examples/webgl-points-layer.html

If you find this repo & want to contribute/chat/criticize, feel free to reach out.
----------------------------
Intended Roadmap:
    [X] Clone webgl-points-layer example & reduce to the basics
    [X] Replace data source "world-cities.geojson" with "spread_weather.json"
    [ ] Render *any* animation with WebGL/GLSL; for instance, random streaking lines
    [ ] Calculate and render weather particle positions (direction & strength)
    [ ] Render /data/mvt/ascat.mvt on map
    [ ] Calculate and render ASCAT particle positions (direction & strength)
    