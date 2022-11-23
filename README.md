# What's the plan??

My goal for this project is to develop the ability to render **WIND AND OCEAN CURRENTS** from an MVT file on an OpenLayers 7.1.0 map. This needs to work well across browsers & on mobile & behave nicely with OpenLayers existing functionality.

# How to run
- git clone https://github.com/Tomcariello/ol-animated-vectors.git
- npm install
- npm start

# Data in this repo
- /data//weather.json: This is randomly generated data which covers covers the globe. Each entry includes lat/lon coordinates as well as wind speed & wind degree (direction).
    
{

    "coord": { "lat": -58, "lon": 87 },

    "wind": { "speed": 29.47, "deg": 214 }
    
}

# Intended Roadmap
[X] Clone webgl-points-layer example & reduce to the basics

[X] Update data source with sufficient worldwide points to cover the map

[X] Calculate and render weather particle positions (direction & velocity)

[-] Render *any* animation with WebGL/GLSL; for instance, random streaking lines

[-] Render particle positions (direction & velocity)

# Other Stuff
This project was helped along by multiple Openlayers examples https://openlayers.org/en/latest/examples/

If you find this repo & want to contribute/chat/criticize, feel free to reach out. I monitor the OpenLayers gitter (https://gitter.im/openlayers/openlayers) as well as github; you can find me there.
