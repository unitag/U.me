#static-link

##Definition

###Data
+ `text` - Text appended into link element.
  + _Type_: String
  + __Default__: `""`

###Properties
+ `href` - href attribute.
  + _Type_: String
  + __Default__: `"#"`
+ `target` - target attribute.
  + _Type_: String
  + __Default__: `null`
+ `type` - Link type
  + _Type_: String Enum
    + `inline`
    + `button`
    + `buttonOffset`
  + __Default__: `button`
+ `baseColor` - Button CSS class main color.
  + _Type_: String
  + __Default__: **TODO**
+ `disabled`
    + _Type_: Boolean
    + __Default__: `False`


###Example
```json
{
    "type": "static-link",
    "data": {
        "text": "Click here!"
    },
    "properties": {
      "href": "http://unitag.io",
      "target": "_blank"
    },
    "blocks": []
}
```


##Tricks
###1. Formated text in disabled link
This JSON :
```json
{
    "type": "static-link",
    "data": {
        "text": "Click "
    },
    "properties": {
       "href": "http://unitag.io",
       "disabled": true
    },
    "blocks": [{
        "type": "static-text",
        "properties": {"element": "strong"},
        "data": {"text": "here! "}
    }]
}
```
Will return something approximately something like :
```html
<a class="button" href="http://unitag.io" disabled>Click <strong>here!</strong></a>
```

