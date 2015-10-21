#Bind-image

##Definition
Polymer's iron-image binding :
+ [Polymer Github documentation](https://github.com/PolymerElements/iron-image)
+ [Polymer iron-image docs and demo](https://elements.polymer-project.org/elements/iron-image)

###Data
+ `src` - See Polymer description

###Properties
+ `canLoad` - See Polymer description
+ `fade` - See Polymer description
+ `height` - See Polymer description
    + __Default__: `100%`
+ `loaded` - See Polymer description
+ `loading` - See Polymer description
+ `placeholder` - See Polymer description
+ `position` - See Polymer description
+ `preload` - See Polymer description
+ `preventLoad` - See Polymer description
+ `requiresPreload` - See Polymer description
+ `sizing` - See Polymer description
+ `width` - See Polymer description
    + __Default__: `100%`

###Blocks
`/!\` Nested blocks unavailable `/!\`

###Example
```json
{
    "type" : "bind-image",
     "data" : {
        "src" : "http://lorempixel.com/600/400"
    },
     "properties" : {
        "sizing" : "cover"
    },
    "css" : "{height: 300px; width: 100%}"
}
```
Will return something approximately something like :
```html
<iron-image style="height: 210px; width: 100%; background-image: url(http://lorempixel.com/600/400); background-size: cover; background-position: 50% 50%; background-repeat: no-repeat;"></iron-image>
```

