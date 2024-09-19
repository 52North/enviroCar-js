## ARCHIVED

This project is no longer maintained and will not receive any further updates. If you plan to continue using it, please be aware that future security issues will not be addressed.

## enviroCar-js

JavaScript components for enviroCar maps -  based on the ESRI ArcGIS JavaScript API 3.5.

### example

view [the example](http://52north.github.io/enviroCar-js/)

### usage
Usage is as simple as including some JavaScripts and defining `<div>` elements as placeholders:

```html
<!doctype html>
<html>
    <head>
        <link rel="stylesheet"
            href="http://serverapi.arcgisonline.com/jsapi/arcgis/3.5/js/dojo/dijit/themes/tundra/tundra.css">
        <link rel="stylesheet"
            href="http://serverapi.arcgisonline.com/jsapi/arcgis/3.5/js/esri/css/esri.css">
        <link rel="stylesheet" href="http://raw.github.com/52North/enviroCar-js/master/css/enviroCarMap.css" />

        <script>var dojoConfig = {parseOnLoad : true};</script>
        <script src="http://serverapi.arcgisonline.com/jsapi/arcgis/3.5/"></script>
        <script src="http://raw.github.com/52North/enviroCar-js/master/js/enviroCarMap.js"></script>
    </head>

    <body class="tundra">
        <div data-dojo-type="dijit.layout.BorderContainer"
            data-dojo-props="design:'headline',gutters:true"
            style="width: 100%; height: 400px; margin: 10px 0 10px 0;">
            <div id="enviroCarMap" data-dojo-type="dijit.layout.ContentPane"
                data-dojo-props="region:'center'">
                <div id="feedback" class="shadow">
                    <div style="position: absolute; right: 5px; top: 5px">
                        <img id="loading" src="images/ajax.gif" width="18" />
                    </div>
                    <h3>enviroCar Tracks</h3>
                    <div id="info">
                        <!-- filtering select -->
                        <label for="fieldNames">Select Phenomenon: </label>
                        <select id="fieldNames" name="baseSym"
                            data-dojo-type="dijit.form.FilteringSelect"
                            data-dojo-props="style:'width:200px;'">
                        </select>
                    </div>
                </div>
            </div>
        </div>
    </body>
</html>
```
