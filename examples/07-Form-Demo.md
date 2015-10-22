#Form Demo

Live demo [here](http://opn.to/r/ume/form-demo)

```json
{
    "label": "Demo form 1",
    "ume": {
        "type": "ume",
        "blocks": {
            "type": "static-page",
            "blocks": [
                {
                    "type": "bind-form",
                    "properties": {
                        "label": "FORM inscription",
                        "method": "POST"
                    },
                    "blocks": [
                        {
                            "type": "static-text",
                            "data": {
                                "text": "Inscription au jeu"
                            },
                            "properties": {
                                "element": "h2"
                            }
                        },
                        {
                            "type": "bind-input",
                            "properties": {
                                "label": "Nom"
                            }
                        },
                        {
                            "type": "bind-input",
                            "properties": {
                                "label": "Prénom"
                            }
                        },
                        {
                            "type": "bind-email-input",
                            "properties": {
                                "label": "E-mail"
                            }
                        },
                        {
                            "type": "static-text",
                            "data": {
                                "text": "Sexe: "
                            }
                        },
                        {
                            "type": "bind-radio-group",
                            "blocks": [
                                {
                                    "type": "bind-radio-button",
                                    "properties": {
                                        "label": "Femme",
                                        "name": "Femme"
                                    }
                                },
                                {
                                    "type": "bind-radio-button",
                                    "properties": {
                                        "label": "Homme",
                                        "name": "Homme"
                                    }
                                }
                            ]
                        },
                        {
                            "type": "bind-checkbox",
                            "properties": {
                                "label": "Je souhaite recevoir la newsletter"
                            }
                        },
                        {
                            "type": "bind-button",
                            "blocks": [
                                {
                                    "type": "static-text",
                                    "data": {
                                        "text": "S'inscrire"
                                    }
                                }
                            ],
                            "properties": {
                                "raised": true
                            }
                        }
                    ]
                }
            ]
        }
    }
}
```
