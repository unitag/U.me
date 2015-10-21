#ume-scratch

##Definition


###Properties
+ `bgColor` - Background color behind the scratchcard.
  + _Type_: String
  + __Default__: `#a0a0a0`
+ `threshold` - Threshold value that defines the minimum percentage of surface that need to be scratched in order to complete the scratchcard.
  + _Type_: Number
  + __Default__: `70`
+ `realtime` - Define if the progress of the scratch appears dynamically or when the user realease the scratchcard.
  + _Type_: Boolean
  + __Default__: `false`
+ `font` - The font of the text displayed on the scratchcard.
  + _Type_: String
  + __Default__: `2rem Courier`
+ `displayMode` - The type of content displayed on the scratchable area. Only `color`, `image` and `pattern` value are accepted.
  + _Type_: String
  + __Default__: `color`
+ `textColor` - The color of the text displayed on the scratchcard.
  + _Type_: String
  + __Default__: `#ffffff`
+ `text` - The text that will be displayed on the scratchcard.
  + _Type_: String
  + __Default__: `Scratch here`
+ `src` - Source of the image that will be displayed on the scratchable area. `/!\` Only URL who support the CORS specification will work `/!\`
  + _Type_: String
  + __Default__: ``
+ `textAlign` - The alignement of the text displayed on the scratchcard.
  + _Type_: String
  + __Default__: `center`
+ `minHeight` - The minimum heigth in pixels of the scratchcard.
  + _Type_: Number
  + __Default__: `1`
+ `shape` - Shape of the scratchcard. Only 'square', 'fit', 'circle' and 'diamond' are accepted. The 'fit' value will fit the scratchard size with its content size. `/!\` Some Browsers like Internet Explorer does not support clipping. Otherwise works perfectly for Chrome, Firefox, Safari and Opera `/!\`
  + _Type_: String
  + __Default__: `fit`
+ `scratchColor` - The color inside the scratchcard
  + _Type_: String
  + __Default__: `#a0a0a0`
+ `strokeWidth` - The width of the white stroke around the scratchard
  + _Type_: Number
  + __Default__: `3`


###Example
```json
{
    "type": "ume-scratch",
    "properties": {
        "displayMode": "color",
        "text" : "Scratch here!"
    },
    "blocks": []
}
```


##Tricks
###1. Define various shapes for the scratchcard
You can modify the shape of the scratchard into a circle, a square or a diamond. There will always be a white stroke around the scratchard and you can also select the background color.This JSON :
```json
{
    "type": "ume-scratch",
    "properties": {
        "bgColor": "#ff0000",
        "textColor": "#0000ff",
        "displayMode": "color",
        "shape" : "circle"
    }
}
```

With an image behind the scratchard, this will return something approximately something like :
```html
<div class="scratchcard" style="position: relative;">
    <canvas width="363" height="255" style="position: absolute; z-index: 4; -webkit-tap-highlight-color: rgba(0, 0, 0, 0); clip-path: url(#circleClip); -webkit-clip-path: url(#circleClip);"></canvas>
</div>
<div class="scratch-content style-scope ume-scratch" style="min-height: 1px; visibility: visible; clip-path: url(#circleClip); -webkit-clip-path: url(#circleClip);">
    <img id="img" role="none" class="style-scope iron-image" src="http://www.lorempixel.com/600/400"/>
</div>
<div id="stroke" class="style-scope ume-scratch" style="clip-path: url(#circleStroke); -webkit-clip-path: url(#circleStroke);"></div>
<div id="bg" class="style-scope ume-scratch" style="background-color: rgb(255, 0, 0);"></div>
```

###2. Filling the scratchard

You can also fill the scratchcard with a selected color, image or pattern (Only if the image URL is supported by CORS).This JSON :
```json
{
    "type": "ume-scratch",
    "properties": {
        "displayMode": "image",
        "src" : "http://www.lorempixel.com/600/400"
    }
}
```

With an image behind the scratchard, this will return something approximately something like :
```html
<ume-scratch id="umestatic-pagei0ume-scratch" src="http://www.lorempixel.com/600/400" display-mode="image">
  <div class="scratchcard" style="position: relative;">
      <canvas width="363" height="255" style="position: absolute; z-index: 4; -webkit-tap-highlight-color: rgba(0, 0, 0, 0);"></canvas>
  </div>
  <div class="scratch-content style-scope ume-scratch" style="min-height: 1px; visibility: visible;">
      <img id="img" role="none" class="style-scope iron-image" src="http://www.robertswebdesign.co.uk/thedailyskid.com/wordpress/wp-content/uploads/2014/04/vampire-bat.jpg">
  </div>
</ume-scratch>
