#ume-check-group

##Definition

###Properties

+ `name` - Name of the check-group
  + _Type_: String
  + __Default__: `""`
+ `value` - Value of the checked elements during initialisation
  + _Type_: String
  + __Default__: `""`
+ `gridClass` - The class of the grid that will display the elements
  + _Type_: Array
  + __Default__: `['small-12]`
+ `label` - Label displayed with the check-group
  + _Type_: String
  + __Default__: `""`

###Blocks
Only checkbox and radio-button will be update the value of the checkbox

###Example
This JSON :
```json
{
    "type": "ume-check-group",
    "properties": {
        "name": "sex",
        "value" : "male",
        "label" : "Sex",
        "gridClass" : ["small-4"]
    },
    "blocks" : [
      {
        "type": "static-radio-button",
        "properties": {
            "name": "sex",
            "value" : "male",
            "label" : "Male"
        }
      },
      {
        "type": "static-radio-button",
        "properties": {
            "name": "sex",
            "value" : "female",
            "label" : "Female"
        }
      },
      {
        "type": "static-radio-button",
        "properties": {
            "name": "sex",
            "value" : "undetermined",
            "label" : "Undetermined"
        }
      }
    ]
}
```
Will return something approximately something like :
```html
<ume-check-group id="umestatic-pagei0bind-formi5ume-check-group" label="Sex" name="sex" value="[&quot;male&quot;]" grid-class="[&quot;small-4&quot;]">
  <label class="style-scope ume-check-group">Sex</label>
  <ume-grid grid-class="[&quot;small-4&quot;]" equalizer="">
    <div class="row style-scope ume-grid" data-equalizer="">
      <div class="columns small-4" data-equalizer-watch="" style="height: 29px;">
        <input type="radio" class="static" name="sex" value="male" checked="true">Male
      </div>
      <div class="columns small-4" data-equalizer-watch="" style="height: 29px;">
        <input type="radio" class="static" name="sex" value="female">Female
      </div>
      <div class="columns end small-4" data-equalizer-watch="" style="height: 29px;">
        <input type="radio" class="static" name="sex" value="undetermined">Undetermined
      </div>
    </div>
  </ume-grid>
</ume-check-group>"Male"
```

