#Bind-button

##Definition
Polymer's paper-button binding :
+ [Polymer Github documentation](https://github.com/PolymerElements/paper-button)
+ [Polymer paper-button docs and demo](https://elements.polymer-project.org/elements/paper-button)


###Properties
+ `raised` - See Polymer description
+ `toggles` - See Polymer description
+ `noink` - See Polymer description


###Blocks

###Example
```json
{
    type: "bind-button",
    blocks: [
        {
            type: "static-text",
            data: {
                text: "Submit"
            }
        }
    ],
    properties: {
        raised: true
    }
}
```
Will return something approximately something like :
```html
<paper-button id="umestatic-pagei0bind-formi4bind-button" role="button" tabindex="0" aria-disabled="false" class="x-scope paper-button-0">
...</paper-button>
```