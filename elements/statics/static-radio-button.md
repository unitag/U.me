#static-radio-button

##Definition

###Properties

+ `name` - Name of the radio-button group
  + _Type_: String
  + __Default__: `""`
+ `value` - Value of the radio-button
  + _Type_: String
  + __Default__: `""`
+ `checked` - Equals true when the radio-button is checked
  + _Type_: Boolean
  + __Default__: `false`
+ `label` - Label displayed with the radio-button
  + _Type_: String
  + __Default__: `""`

###Example
This JSON :
```json
{
    "type": "static-radio-button",
    "properties": {
        "name": "sex",
        "value" : "male",
        "label" : "Male"
    }
}
```
Will return something approximately something like :
```html
<input type="radio" class="static" name="sex" value="male" checked="true">"Male"
```

