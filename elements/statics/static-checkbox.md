#static-checkbox

##Definition

###Properties

+ `name` - Name of the checkbox group
  + _Type_: String
  + __Default__: `""`
+ `value` - Value of the checkbox
  + _Type_: String
  + __Default__: `""`
+ `checked` - Equals true when the checkbox is checked
  + _Type_: Boolean
  + __Default__: `false`
+ `label` - Label displayed with the checkbox
  + _Type_: String
  + __Default__: `""`

###Example
This JSON :
```json
{
    "type": "static-checkbox",
    "properties": {
        "name": "language",
        "value" : "french",
        "label" : "French"
    }
}
```
Will return something approximately something like :
```html
<input type="checkbox" class="static" name="language" value="french">"French"
```

