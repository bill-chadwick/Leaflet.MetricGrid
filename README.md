# Leaflet.MetricGrid
A general purpose Metric Grid overlay for Leaflet with ready defined British, Irish Grids and WGS84 UTM grids.

British and Irish Example http://www.bdcc.co.uk/leaflet/example.html

Swiss Example http://www.bdcc.co.uk/leaflet/swiss_example.html

UTM Example http://www.bdcc.co.uk/leaflet/utm_example.html including northern and southern hemisphere grids.

This is a grid for map projections with constant scale such as UTM, British Grid, Irish Grid etc. On the ground, grid squares are square with sides of 100m, 1km, 10km or 100km (other intervals would be possible but are unusual). 

The grid can have its left/west axis and south/bottom axis labeled with values corresponding to the grid line position within a 100km square. Most grids repeat their numbering every 100km. These labels can optionally included subscripted hundreds of km.

The grid can also label every square in its bottom left corner. This label may be preceeded with a 100km square identifier defined for the grid - 2 letters for the British Grid. For the predefined UTM grid on the WGS84 datum, MGRS 100km letter pairs can be used.

Such a grid normally has a rectangular bound but this code allows a grid to be 'clipped' so that a grid may hidden where it would overlap another grid. The example uses clipped Irish (EPSG code 29903) and British (EPSG code 27700) grids - zoom the example out between Ireland and the British mainland to see the clipping in action. The grid may also be clipped with a rectangular Lat/Lon bounds - useful for adjacent UTM grids.

Grid lines gnerally project as curves on Web Mercator at low zooms, but will tend to straight as the map is zoomed in. At all zooms, the minimum number of straight line segments are used to the draw grid lines so perfomance is good.

This code depends on proj4.js 2.5.0 or later

Development sponsored by Geograph Britain and Ireland - http://www.geograph.org.uk/mapper/photomap.php

Bill Chadwick


