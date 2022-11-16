Based on https://openlayers.org/en/latest/examples/webgl-points-layer.html

https://gitter.im/openlayers/openlayers?utm_source=notification&utm_medium=email&utm_campaign=unread-notifications#

Tim Schaub @tschaub: 

I think a custom renderer for vector fields would make a great addition. I can imagine a WebGL solution that took advantage of the existing DATA TILE SOURCE (https://openlayers.org/en/latest/apidoc/module-ol_source_DataTile-DataTileSource.html) 

...and some of the existing WEBGL TILE RENDERER (https://openlayers.org/en/latest/apidoc/module-ol_renderer_webgl_TileLayer-WebGLTileLayerRenderer.html)

...for loading the data and uploading textures representing velocity vectors. The remaining work would be to calculate and render particle positions.

----------------------------
To-Do:
    [X] Load example map with WebGL
    [X] Render *any* animation (red circles on load)
    [X] Render any *data-driven* animation (red lines on load)
    [ ] Render *any* animation with WebGL/GLSL
    [ ] Render any *data-driven* animation with WebGL/GLSL
    