# OpenLayers map marker (ver. 6)
OpenLayers map marker with popup. Create marker with geolocation or double click. Delivery area with polygon. Multiple markers with html popups. Animated markers.

#### Working examples 
https://moovspace.github.io/ol-map

### Map file contains
  - Add image marker to map
  - Show map popup on click
  - Create marker on double click
  - Clear all layer markers on double click
  - Create map polygon from points array  
  - Create delivery area, export polygon
  - Test delivery area with polygon
  - Search location from address (geolocation)
  - Animate marker, marker highlight (ontop)
  - Animate marker popup
  - Multiple markers with popups from array or database
  
### Map marker, geolocation or on click
https://github.com/moovspace/map-marker-openlayers/blob/master/map-marker-click.html
<img src="https://github.com/moovspace/map-marker-openlayers/blob/master/img/map-marker-polygon-click.png" style="width: 100%;">

### Delivery area with polygon
Create, load or edit polygon sample. Load polygon in json format. Download polygon file. https://github.com/moovspace/map-marker-openlayers/blob/master/map-polygon.html
<img src="https://github.com/moovspace/map-marker-openlayers/blob/master/img/map-polygon.png" style="width: 100%;">

### Map multipe markers
Multiple markers with popups from array or database. https://github.com/moovspace/map-marker-openlayers/blob/master/map-multiple-markers.html
<img src="https://raw.githubusercontent.com/moovspace/map-marker-openlayers/master/img/map-marker-multi.png" style="width: 100%;">

# Important!
Map style height 
```css
map{
float: left; 
width: 100%;
height: 400px;
}
```

### Check if point(coordinates) is inside a polygon
```js
/*
    Test delivery area coordinates
    var coordinate = [21.002902, 52.22885]
    var polygon_points = [[20.57, 53.30], [21.24, 53.30], [22.152810, 52.648142], [21.24, 52], [20.50, 52], [19.785212, 52.783446]];
*/
function PointInPolygon(coordinate, polygon_points_array)
{
    var polygon = new ol.geom.Polygon([polygon_points_array]);
    var out = polygon.intersectsCoordinate(coordinate);
    return out;
}
```

### Small version
Create marker, polygon
https://github.com/MoovFun/awesome-map-marker
