# My Reference Notes

## Links for reference

### Change Map Style (basemap)

<https://docs.mapbox.com/mapbox-gl-js/example/setstyle/>

### Question: Add layers based on Custom property filter

<https://github.com/mapbox/mapbox-gl-js/issues/7996>
Answer
<https://docs.mapbox.com/mapbox-gl-js/style-spec/sources/#geojson-clusterProperties>

<https://stackoverflow.com/questions/51481471/adding-custom-icons-for-each-feature-in-feature-collection-with-mapbox-gl-js>

### Load external geojson file

<https://stackoverflow.com/questions/45536403/mapbox-gl-js-and-geojson-as-an-external-file>

### Using filter expresion

A filter expression that singles out all features where "icon" is equal to symbol (a variable that is set to the selected feature's icon property):
<https://docs.mapbox.com/help/glossary/filter/>
this is what makes the icon the symbol. Otherwise all symbols go on top of each other.

<https://stackoverflow.com/questions/53672066/data-driven-styling-using-multiple-filters-in-mapbox-gl-js>
<https://docs.mapbox.com/mapbox-gl-js/style-spec/other/#other-filter>





## THINGS TO DO TO GET WORKING SELECTORS AND CLICK EFFECTS

&#9733; indicates things that are done.

* Set up my own mapbox accessToken

* Move data to its own file  &#9733; 

* Add fields to geojson:
  * condition
  * description
  * image *NOTE: image is not necessary with if statement dependent on condition*

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
  
