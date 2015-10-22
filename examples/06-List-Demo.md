#List Demo

Live demo [here](http://opn.to/r/ume/list-demo)

```json
{
    "label": "Demo List",
    "ume": {
        "type": "ume",
        "blocks": {
            "type": "static-page",
            "blocks": [
                {
                    "type": "static-list",
                    "properties": {
                        "lines": [
                            {
                                "data": {
                                    "text": "Basic item with just a text"
                                }
                            },
                            {
                                "data": {
                                    "text": "Basic item with a text and a subtext",
                                    "subtext ": "Subtext that add more informations about the content"
                                }
                            },
                            {
                                "data": {
                                    "text": "Item with a image",
                                    "subtext": "This one has an image",
                                    "src": "http://lorempixel.com/75/75",
                                    "srcset": "http://lorempixel.com/150/150"
                                }
                            },
                            {
                                "data": {
                                    "text": "Complete item with a link",
                                    "subtext": "Click here to go to another selected page",
                                    "link ":  "http://www.google.com",
                                    "src": "http://lorempixel.com/75/75",
                                    "srcset": "http://lorempixel.com/150/150"
                                }
                            }
                        ]
                    }
                }
            ]
        }
    }
}
```
