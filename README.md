berlin-geodata
==============

Collection of geographical data as TopoJSON of Berlin. 


### berlin.orsteile.topojson

Unsimplified topojson file, converted from [http://daten.berlin.de/datensaetze/ortsteil-geometrien-berlin](http://daten.berlin.de/datensaetze/ortsteil-geometrien-berlin).
File contains the id and name of every district (96).

Converted with the following command line:

    topojson -o berlin.ortsteile.topojson -p Name --id-property data_id --shapefile-encoding utf8 -- shapes.shp 
