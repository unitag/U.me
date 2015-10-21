#Bind-email-input

##Definition
Polymer's gold-email-input binding :
+ [Polymer Github documentation](https://github.com/PolymerElements/gold-email-input)
+ [Polymer gold-email-input docs and demo](https://elements.polymer-project.org/elements/gold-email-input)


###Properties
+ `label` - See Polymer description
+ `regex` - See Polymer description

###Blocks
`/!\` Nested blocks unavailable `/!\`

###Example
```json
{
    type: "bind-email-input",
    properties: {
        label: "E-mail"
    }
}
```
Will return something approximately something like :
```html
<gold-email-input id="umestatic-pagei0bind-formi3bind-email-input" label="E-mail" aria-disabled="false">
</gold-email-input>
```