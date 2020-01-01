# Self-hosted map tile server with OpenStreetMap data

## Tile server data

- http://download.geofabrik.de
- https://downloadlayer--onlinechart-ol3.netlify.com

## Tile servers

### docker-osm

https://github.com/kartoza/docker-osm

A docker compose project to setup an OSM PostGIS database with automatic updates from OSM periodically

License : GPL

### openstreetmap-tile-server

https://github.com/Overv/openstreetmap-tile-server

Docker file for a minimal effort OpenStreetMap tile server

https://switch2osm.org/using-tiles/getting-started-with-leaflet

License : Apache License, Version 2.0

### openmaptiles

OpenMapTiles, a self-hosted map tile server with OpenStreetMap data

- https://openmaptiles.org
- https://openmaptiles.com
- https://golb.hplar.ch/2018/07/self-hosted-tile-server.html

#### openmaptiles/openmaptiles

https://github.com/openmaptiles/openmaptiles

OpenMapTiles Vector Tile Schema Implementation https://openmaptiles.org/schema/

License : BSD 3-Clause License

Create mbtiles data :

    git clone https://github.com/openmaptiles/openmaptiles
    cd openmaptiles
    ./quickstart.sh europe                       # Europe
    ./quickstart.sh france                       # France, Europe

#### klokantech/openmaptiles-server

- https://github.com/openmaptiles
- docker pull klokantech/openmaptiles-server
- https://fr.slideshare.net/Docker/take-control-of-your-maps-with-docker

    docker run --rm -it -v $(pwd):/data -p 8080:80 klokantech/openmaptiles-server

License:

#### klokantech/tileserver-gl

https://github.com/maptiler/tileserver-gl

Requires a mbtiles file

    docker run -it -v $(pwd):/data -p 8080:80 klokantech/tileserver-gl

License: Mix BSD/MIT/Apache/Boost

#### openmaptiles/klokantech-3d-gl-style

https://github.com/openmaptiles/klokantech-3d-gl-style

License: BSD 3
