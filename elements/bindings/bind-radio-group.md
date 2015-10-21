#Bind-radio-group

##Definition
Polymer's paper-radio-group binding :
+ [Polymer Github documentation](https://github.com/PolymerElements/paper-radio-group)
+ [Polymer paper-radio-group docs and demo](https://elements.polymer-project.org/elements/paper-radio-group)


###Properties
+ `label` - See Polymer description
+ `checked` - See Polymer description
+ `toggles` - See Polymer description
+ `name` - See Polymer description
    +`/!\` Required if part of a radio-group `/!\`

###Blocks
`/!\` Nested blocks unavailable `/!\`

###Example
```json
{
    type: "bind-radio-button",
    properties: {
        label: "Item 1"
    }
}
```
Will return something approximately something like :
```html
<paper-radio-button id="umestatic-pagei0bind-formi2bind-radio-button" role="radio" tabindex="0" toggles="" aria-pressed="false" aria-disabled="false" aria-checked="false" class="x-scope paper-radio-button-0" aria-label="Item 1">
</paper-radio-button>
```