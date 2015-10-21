#ume-grid

##Definition


###Properties
+ `gridClass` - Array of classes for grid behaviours.[See Foundation grid documentation](http://foundation.zurb.com/docs/components/grid.html) for more details.
  + _Type_: Array
  + __Default__: [`small-12`]
+ `equalizer` - Enable Equalizer module to equalize grid columns height.
  + _Type_: Boolean
  + __Default__: `false`
+ `notEqualizedOnStack` - Specify if Equalizer should **NOT** make elements equal height once they become stacked.height.
  + _Type_: Boolean
  + __Default__: `false`


###Example
```json
{
    "type": "ume-grid",
    "properties": {
        "equalizer": true,
        "notEqualizedOnStack" : false,
        "gridClass": ["small-6"]
    },
    "blocks": []
}
```


##Tricks
###1. Define various grid classes
You can specify an array of classes for responsive purpose. This JSON :
```json
{
    "type": "ume-grid",
    "properties": {"gridClass": ["small-6", "medium-8 medium-offset-2", "large-12"]}
}
```

With 3 blocks, this will return something approximately something like :
```html
<div class="row">
    <div class="column small-6"></div>
    <div class="column medium-8 medium-offset-2"></div>
    <div class="column large-12"></div>
</div>
```

