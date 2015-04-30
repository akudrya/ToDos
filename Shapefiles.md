2 basic types of shapefiles:

1. kml - google format (XML - style)
 - coordinates of areas
 - holes, mutual-crossings
 Keyhole Markup Language (KML) is an XML notation for expressing geographic annotation and visualization within Internet-based, two-dimensional maps and three-dimensional Earth browsers. KML was developed for use with Google Earth,
KML 
<placemark>
<point>
<coordinates></coordinates>
</point>
</placemark>
KMZ - archive based on 1 KML file + all meta and media data. If KML>10 kb - it is stored as kmz
2. shp - Esri format shape file: objects and attributes like rivers (binary)
  * .shp — shape format; the feature geometry itself
  * .shx — shape index format; a positional index of the feature geometry to allow seeking forwards and backwards quickly
  * .dbf — attribute format; columnar attributes for each shape, in dBase IV format
  
  
 
