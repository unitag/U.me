# static-form

## Definition

### Data

### Properties
* `method` - Method for submitting the form
  * _Type_: String
  * __Default__: `"POST"`

* `action` - Target URI
  * _Type_: String
  * __Default__: `""`

### Blocks

### Example
```json
{
    "type": "static-form",
    "data": {},
    "properties": {},
    "blocks": [],
    "css": ""
}
```

### Legacy example (from the `subscription` template)

#### Raw version
```json
{
    "inputs": {
        "<union>": [
            {
                "<loop@field>": "<((io.formFields))>",
                "format": "<((loop.field.type))>",
                "label": "<(((loop.field.type in ['radio', 'checkbox']) ? loop.field.label : null))>",
                "placeholder": "<(((loop.field.type in ['radio', 'checkbox']) ? null : loop.field.label))>",
                "name": "<((loop.field.name))>",
                "value": "<((loop.field.value))>",
                "required": "<((loop.field.required))>",
                "multiline": true,
                "choices": {
                    "<disabled>": "<((!(loop.field.type in ['select', 'radio', 'checkbox'])))>",
                    "<loop@choice>": "<((loop.field.choices))>",
                    "label": "<((loop.choice))>",
                    "value": "<((loop.choice))>"
                }
            },
            {
                "<disabled>": "<((!meta.form.dataUsage.ask))>",
                "format": "checkbox",
                "name": "dataUsage",
                "choices": [
                    {
                        "label": "<((meta.form.dataUsage.text))>",
                        "value": "checked"
                    }
                ],
                "value": "<((meta.form.dataUsage.preChecked ? 'checked' : ''))>"
            }
        ]
    },
    "btnText": "<((meta.form.submitLabel))>"
}
```

#### Sample meta
```json
{
    "title": "Inscrivez-vous dès maintenant !",
    "text": "Remplissez le formulaire pour participer à notre évènement.",
    "fields": [
        {
            "label": "Nom",
            "type": "text",
            "choices": [],
            "required": false
        },
        {
            "label": "Email",
            "type": "email",
            "choices": [],
            "required": true
        },
        {
            "label": "Genre",
            "type": "radio",
            "choices": [
                {
                    "label": "Femme"
                },
                {
                    "label": "Homme"
                }
            ],
            "required": true
        },
        {
            "label": "OS préféré",
            "type": "select",
            "choices": [
                {
                    "label": "Android"
                },
                {
                    "label": "iOS"
                }
            ],
            "require": false
        }
    ],
    "dataUsage": {
        "text": "J’accepte de recevoir des informations commerciales de Société organisatrice.",
        "preChecked": true,
        "ask": true
    },
    "submitLabel": "Je m’inscris"
}
```

#### Compiled version
```json
{
    "inputs": [
        {
            "format": "text",
            "label": null,
            "placeholder": "Nom",
            "name": "field0",
            "value": null,
            "required": false,
            "multiline": true
        },
        {
            "format": "email",
            "label": null,
            "placeholder": "Email",
            "name": "field1",
            "value": null,
            "required": true,
            "multiline": true
        },
        {
            "format": "radio",
            "label": "Genre",
            "placeholder": null,
            "name": "field2",
            "value": null,
            "required": true,
            "multiline": true,
            "choices": [
                {
                    "label": "Femme",
                    "value": "Femme"
                },
                {
                    "label": "Homme",
                    "value": "Homme"
                }
            ]
        },
        {
            "format": "select",
            "label": null,
            "placeholder": "OS préféré",
            "name": "field3",
            "value": null,
            "required": false,
            "multiline": true,
            "choices": [
                {
                    "label": "Android",
                    "value": "Android"
                },
                {
                    "label": "iOS",
                    "value": "iOS"
                }
            ]
        },
        {
            "format": "checkbox",
            "name": "dataUsage",
            "choices": [
                {
                    "label": "J’accepte de recevoir des informations commerciales de Société organisatrice.",
                    "value": "checked"
                }
            ],
            "value": "checked"
        }
    ],
    "btnText": "Je m’inscris"
}
```

#### Important notes

 - We must be able to initialize any input with a given value (including checkbox and radio groups).
 - Generating the form was relatively easy because all the inputs supported similar keys.
 - Handling closed-ended questions was tricky because of their specificities:
     + `radio` and `checkbox` do not support a placeholder like other inputs: they need to use a label instead (inconsistent rendering)
     + `select` artificially supports a placeholder, if one is given:
         * The placeholder is inserted at the top of the options list, with a grayed style which indicates that it does not count as an actual choice. However, there are chances that this is not well understood, especially on mobile browsers (options are displayed using a native dropdown menu, without any grayed effect on the placeholder).
         * If the initial value is empty, the placeholder is initially selected.
         * If the input is required, the placeholder cannot be selected again once another option has been chosen (disabled state).
 - The `multiline` key is only used by `radio` and `checkbox`, but is left for the others for convenience.
 - The (unique) input names are automatically generated from their position in meta.

### Possible improvements
 - New inputs may be defined as distinct blocks, or as a single `static-input` block with multiple available formats.
 - Using some JavaScript form validation could improve the UX.
 - Some useful input types are missing, such as date or datetime (native implementations are not widely available).
 - To handle the distinction between `label` and `placeholder`, we could:
     1. Use `label` for all inputs
     2. Add a boolean property that indicate that we prefer the label to be displayed as a placeholder (only honored by compatible inputs)
