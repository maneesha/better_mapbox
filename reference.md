## Change Map Style (basemap)
https://docs.mapbox.com/mapbox-gl-js/example/setstyle/ 

## Question: Add layers based on Custom property filter
https://github.com/mapbox/mapbox-gl-js/issues/7996
Answer 
https://docs.mapbox.com/mapbox-gl-js/style-spec/sources/#geojson-clusterProperties

https://stackoverflow.com/questions/51481471/adding-custom-icons-for-each-feature-in-feature-collection-with-mapbox-gl-js


## THINGS TO DO TO GET WORKING SELECTORS AND CLICK EFFECTS

* Set up my own mapbox accessToken

* Move data to its own file

* Add fields to geojson:
  * condition
  * description
  * image

* Inside `places.features.forEach`:
  * Add new vars:
    * `var symbol = feature.properties['condition'];`
    * `var txtlab = feature.properties['condition'];`
    * `var ic = feature.properties['icon'];`
    * `var layerID = 'poi-' + symbol;`

* To start with, make all symbols be rockets
  * inside `layout`:
    * `'icon-image': 'rocket' + '-15'

* Make the text labels be the condition
  
