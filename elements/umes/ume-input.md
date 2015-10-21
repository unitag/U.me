#ume-input

##Definition
Polymer's iron-input binding :
+ [Polymer Github documentation](https://github.com/PolymerElements/iron-input)
+ [Polymer iron-input docs and demo](https://elements.polymer-project.org/elements/iron-input)

###Properties
+ `label` - The label for the input
  + _Type_: String
+ `inputType` - The type of input that will be validate. 'email', 'alpha', 'alphanumerical', 'numbers', or 'none' will add a preset regexp as pattern. Otherwise the inputType will bind to the pattern
  + _Type_: String
  + __Default__: `none`
+ `name` - See Polymer description
+ `value` - See Polymer description
+ `errorMessage` - See Polymer description
+ `charCounter` - See Polymer description
+ `required` - See Polymer description
+ `type` - See Polymer description
+ `validator` - See Polymer description
+ `autoValidate` - See Polymer description
+ `inputmode` - See Polymer description
+ `pattern` - See Polymer description

###Blocks
`/!\` Nested blocks unavailable `/!\`


###Example
```json
{
    type: "ume-input",
    properties: {
        label: "Name",
        name : "name",
        required : true,
        auto-validate: true,
        errorMessage : "Name required"
    }
}
```
Will return something approximately something like :
```html
<ume-input id="umestatic-pagei0bind-formi1ume-input" label="Name" name="name" error-message="Name required." required="" input-type="alpha" auto-validate="" aria-disabled="false">
  <label class="style-scope ume-input" id="paper-input-label-401">
    <span class="style-scope ume-input">Name</span>
    <input is="iron-input" class="style-scope ume-input" required="" autocomplete="off" placeholder="" autocapitalize="none" autocorrect="off" aria-describedby="" name="name" pattern="[a-zA-Z]*" aria-labelledby="paper-input-label-401">
    <span>
      </span><span class="invalid style-scope ume-input" hidden="">Name required.</span><span>
    </span><template is="dom-if" class="style-scope ume-input"></template>
  </label>
</ume-input>
```