#Bind-radio-button

##Definition
Polymer's paper-radio-button binding :
+ [Polymer Github documentation](https://github.com/PolymerElements/paper-radio-button)
+ [Polymer paper-radio-button docs and demo](https://elements.polymer-project.org/elements/paper-radio-button)


###Properties
+ `selected` - See Polymer description
+ `attrForSelected` - See Polymer description
+ `selectable` - See Polymer description
+ `selectedAttributes` - See Polymer description
+ `keyBindings` - See Polymer description


###Blocks


###Example
```json
{
    type: "bind-radio-group",
    properties: {
        selected: "Female"
    },
    blocks: [
        {
            type: "bind-radio-button",
            properties: {
                label: "Female",
                name: "Female"
            }
        },
        {
            type: "bind-radio-button",
            properties: {
                label: "Male",
                name: "Male"
            }
        }
    ]
}
```
Will return something approximately something like :
```html
<paper-radio-group id="umestatic-pagei0bind-formi5bind-radio-group" selected="Female" role="radiogroup" tabindex="0">
    <paper-radio-button id="umestatic-pagei0bind-formi5bind-radio-groupi0bind-radio-button" name="Female" class="iron-selected x-scope paper-radio-button-0" checked="" role="radio" tabindex="0" toggles="" aria-pressed="true" aria-disabled="false" aria-checked="true" active="" aria-label="Female">
    </paper-radio-button>
    <paper-radio-button id="umestatic-pagei0bind-formi5bind-radio-groupi1bind-radio-button" name="Male" role="radio" tabindex="0" toggles="" aria-pressed="false" aria-disabled="false" aria-checked="false" class="x-scope paper-radio-button-0" aria-label="Male">
    </paper-radio-button>
</paper-radio-group>
```