#Bind-checkbox

##Definition
Polymer's paper-checkbox binding :
+ [Polymer Github documentation](https://github.com/PolymerElements/paper-checkbox)
+ [Polymer paper-checkbox docs and demo](https://elements.polymer-project.org/elements/paper-checkbox)


###Properties
+ `label` - See Polymer description
+ `checked` - See Polymer description
+ `toggles` - See Polymer description

###Blocks
`/!\` Nested blocks unavailable `/!\`

###Example
```json
{
    type: "bind-checkbox",
    properties: {
        label: "Item 1"
    }
}
```
Will return something approximately something like :
```html
<paper-checkbox id="umestatic-pagei0bind-formi1bind-checkbox" role="checkbox" tabindex="0" toggles="" aria-pressed="false" aria-disabled="false" aria-checked="false" class="x-scope paper-checkbox-0" aria-label="Item 1">
  </paper-checkbox>
```