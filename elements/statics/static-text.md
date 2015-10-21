#static-text

##Definition

###Data
+ `text` - Text appended into HTML element.
  + _Type_: String
  + __Default__: `""`

###Properties
+ `element` - HTML element. [See HTML elements list](https://developer.mozilla.org/fr/docs/Web/HTML/Element)
  + _Type_: String
  + __Default__: `p`

###Example
```json
{
    "type": "static-text",
    "data": {
        "text": "Hello World!"
    },
    "properties": {
        "element": "h1"
    }
}
```


##Tricks
###1. Multi-text
This JSON :
```json
{
    "type": "static-text",
    "properties": {"element": "div"},
    "data": {"text": ["Hello ", "World", "!"]}
}
```
Will return something approximately something like :
```html
<div>Hello World!</div>
```

###2. Bold in title
This JSON :
```json
{
    "type": "static-text",
    "properties": {"element": "h1"},
    "data": {"text": "Hello "},
    "blocks": [
        {
            "type": "static-text",
            "properties": {"element": "strong"},
            "data": {"text": "World!"}
        }
    ]
}
```
Will return something approximately something like :
```html
<h1>Hello <strong>World!</strong></h1>
```
