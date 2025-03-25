# Simple Leaflet Bounds Checker

Simple bounds checker for a Leaflet map. Checks if the map is panned or zoomed too far, and the map edge or 'World Bounds' is visible within the map's container. 

Useful for validating whether the returned bounds of a Leaflet map have been cropped to account for values outside of the Mercator projection, ie. greater than +90/-90 degrees latitude.

Since the spatial extent of the Mercator projection covers +90/-90 degrees latitude, Leaflet's getBounds() works as expected, however for displaying overlays or calculating the map view these clipped values might give unexpected results.

## Usage

Open the HTML page in a browser and adjust the zoom & pan until the map bounds are visible within the map container. 
