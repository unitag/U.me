#static-text

##Definition



###Properties
+ `lines` - Array of the lines object that are included in the list
  + _Type_: Array
  + __Default__: `[]`

###Lines Object

####Data
+ `text` - Text to be displayed as an h3 element.
  + _Type_: String
  + __Default__: `""`
+ `subtext` - Subtext to be displayed as a paragraph.
  + _Type_: String
  + __Default__: `""`
+ `link` - Url if the user click on this item. Without a link, the object will appear as a  list item.
  + _Type_: String
  + __Default__: `""`
+ `src` - Url of the left image.
  + _Type_: String
  + __Default__: `""`
+ `srcset` - Retina Url of the left image.
  + _Type_: String
  + __Default__: `""`


###Example
```json
{
    "type:" "static-list",
        "properties": {
            "lines": [
                {
                    data: {
                        "text": "Title of the element",
                        "subtext": "Subtext to describe the element",
                        "link": "http://www.google.com",
                        "src": "http://lorempixel.com/150/150",
                        "srcset": "http://lorempixel.com/300/300"
                    }
                },
                {
                    data: {
                        "text": "Second element ",
                        "subtext": "Subtext to describe the second element",
                        "link": "http://www.unitag.io"
                        "src": "http://lorempixel.com/150/150",
                        "srcset": "http://lorempixel.com/300/300"
                    }
                },
                {
                    data: {
                        "text": "Title of the element",
                        "subtext": "Subtext to describe the element",
                    }
                }
            ]
        }
}
```


