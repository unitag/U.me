#Bind-input

##Definition
Polymer's paper-input binding :
+ [Polymer Github documentation](https://github.com/PolymerElements/paper-input)
+ [Polymer paper-input docs and demo](https://elements.polymer-project.org/elements/paper-input)


###Properties
+ `label` - See Polymer description
+ `errorMessage` - See Polymer description
+ `charCounter` - See Polymer description
+ `prefix` - See Polymer description
+ `suffix` - See Polymer description


###Blocks
`/!\` Nested blocks unavailable `/!\`

###Example
```json
{
    type: "bind-input",
    properties: {
        label: "Name"
    }
}
```
Will return something approximately something like :
```html
<paper-input id="umestatic-pagei0bind-formi0bind-input" label="Name" >
</paper-input>
```