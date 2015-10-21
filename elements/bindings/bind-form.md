#Bind-form

##Definition
Polymer's iron-form binding :
+ [Polymer Github documentation](https://github.com/PolymerElements/iron-form)
+ [Polymer iron-form docs and demo](https://elements.polymer-project.org/elements/iron-form)


###Properties
+ `label` - See Polymer description
+ `action` - See Polymer description
+ `method` - See Polymer description
+ `withCredentials` - See Polymer description
+ `disableNativeValidation` - See Polymer description
+ `contentType` - See Polymer description

###Blocks

###Example
```json
{
    type: "bind-form",
    properties: {
        label: "Basic form"
    },
    blocks: [
        {
            type: "bind-input",
            properties: {
                label: "Name"
            }
        },
        {
            type: "bind-email-input",
            properties: {
                label: "E-mail"
            }
        },
        {
            type: "bind-button",
            blocks: [
                {
                    type: "static-text",
                    data: {
                        text: "Submit"
                    }
                }
            ]
        }
    ]
}
```
Will return something approximately something like :
```html
<form is="iron-form" id="umestatic-pagei0bind-form" label="Basic Form">
...</form>
```