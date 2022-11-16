Based on https://openlayers.org/en/latest/examples/webgl-points-layer.html

https://gitter.im/openlayers/openlayers?utm_source=notification&utm_medium=email&utm_campaign=unread-notifications#

Tim Schaub @tschaub Nov 14 22:16

I think a custom renderer for vector fields would make a great addition. 

I can imagine a WebGL solution that took advantage of the existing data tile source (https://openlayers.org/en/latest/apidoc/module-ol_source_DataTile-DataTileSource.html)and some of the existing WebGL tile renderer for loading the data and uploading textures representing velocity vectors.

The remaining work would be to calculate and render particle positions.

WebGL issue conversation: https://github.com/openlayers/openlayers/pull/12008
----------------------------
To-Do:
    [X] Load example map with WebGL
    [X] Render *any* animation (red circles on load)
    [X] Render any *data-driven* animation (red lines on load)
    [ ] Render *any* animation with WebGL/GLSL
    [ ] Render any *data-driven* animation with WebGL/GLSL
    