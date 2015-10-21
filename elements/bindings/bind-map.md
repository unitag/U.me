#Bind-map

##Definition
Polymer's google-map, google-map-markers and google-map-directions binding :
+ [Polymer Github documentation](https://github.com/PolymerElements/google-map)
+ [Polymer iron-image docs and demo](https://elements.polymer-project.org/elements/google-map)


###Properties
+ `additionalMapOption` - See Polymer description
+ `apiKey` - See Polymer description
+ `clickEvents` - See Polymer description
+ `clientId` - See Polymer description
+ `disableDefaultUI` - See Polymer description
+ `disableZoom` - See Polymer description
+ `dragEvents` - See Polymer description
+ `fitToMarkers` - See Polymer description
+ `latitude` - See Polymer description
+ `longitude` - See Polymer description
+ `libraires` - See Polymer description
+ `mapType` - See Polymer description
+ `maxZoom` - See Polymer description
+ `minZoom` - See Polymer description
+ `mouseEvents` - See Polymer description
+ `noAutoTilt` - See Polymer description
+ `signedIn` - See Polymer description
+ `styles` - See Polymer description
+ `version` - See Polymer description
+ `zoom` - See Polymer description
+ `markers` - Array of markers set on the map. See Polymer description of google-map-marker
  + _Type_: Array
  + __Default__: `[]`
+ `directions` - Directions set on the map. See Polymer description of google-map-directions
  + _Type_: Object
  + __Default__: `{}`

`/!\` The language property of the google-map and google-map-directions elements is not customizable and forced to english by default`/!\`


###Example
```json
{
    "type": "bind-map",
    "css": "{height:550px;}",
    "properties": {
        "fittomarkers" : true,
        "markers": [
            {
                "latitude" : "47.5833",
                "longitude" : "1.3333",
                "title" : "Blois"
            },
            {
                "latitude" : "43.6043",
                "longitude" : "1.4437",
                "title" : "Toulouse"
            }
        ],
        "directions": {
            "startAddress" : "Nantes, France",
            "endAddress" : "Strasbourg, France"
        }
    }
}
```

Will return something approximately something like :
```html
<google-map language="en" fit-to-markers>
    <google-map-marker latitude="47.5833" longitude="1.3333" title="Blois"></google-map-marker>
    <google-map-marker latitude="43.6043" longitude="1.4437" title="Toulouse"></google-map-marker>
</google-map>
<google-map-directions start-address="Nantes, France" end-address="Strasbourg, France"></google-map-directions>
```

