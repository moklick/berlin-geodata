berlin-geodata
==============

Collection of geographical data as TopoJSON of Berlin. 


## berlin.orsteile.topojson
Unsimplified topojson file, converted from [http://daten.berlin.de/datensaetze/ortsteil-geometrien-berlin](http://daten.berlin.de/datensaetze/ortsteil-geometrien-berlin).
File contains the id and name of every district (96).

Converted with the following command lines:

    ogr2ogr -f 'ESRI Shapefile' berlin-ortsteile.shp berlin-ortsteile.kml
    topojson -o berlin.ortsteile.topojson -p Name --id-property data_id --shapefile-encoding utf8 -- berlin-ortsteile.shp 
