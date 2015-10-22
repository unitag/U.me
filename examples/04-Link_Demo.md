#Link Demo

Live demo [here](http://opn.to/r/ume/link-demo)

```json
{
    "label": "Demo link",
    "ume": {
        "type": "ume",
        "blocks": {
            "type": "static-page",
            "blocks": [
                {
                    "type": "static-text",
                    "data": {
                        "text": "Default link without properties"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "static-link",
                    "data": {
                        "text": "Click"
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Button with redirection"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "static-link",
                    "data": {
                        "text": "Click"
                    },
                    "properties": {
                        "href": "http://www.unitag.io",
                        "type": "button"
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Button with redirection in another tab"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "static-link",
                    "data": {
                        "text": "Click"
                    },
                    "properties": {
                        "href": "http://www.unitag.io",
                        "type": "button",
                        "target": "blank"
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Offset Button"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "static-link",
                    "data": {
                        "text": "Click"
                    },
                    "properties": {
                        "type": "buttonOffset"
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Inline link with redirection"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "static-link",
                    "data": {
                        "text": "Click"
                    },
                    "properties": {
                        "href": "http://www.unitag.io",
                        "type": "inline"
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Buttons with color properties"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "static-link",
                    "data": {
                        "text": "Click"
                    },
                    "properties": {
                        "baseColor": "#abc456"
                    }
                },
                {
                    "type": "static-link",
                    "data": {
                        "text": "Click"
                    },
                    "properties": {
                        "baseColor": "#ff0011"
                    }
                },
                {
                    "type": "static-link",
                    "data": {
                        "text": "Click"
                    },
                    "properties": {
                        "baseColor": "#0055ff"
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Text and image inside a button"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "static-link",
                    "data": {
                        "text": "Click"
                    },
                    "blocks": [
                        {
                            "type": "static-text",
                            "data": {
                                "text": " Strong Text Inside"
                            },
                            "properties": {
                                "element": "strong"
                            }
                        },
                        {
                            "type": "bind-image",
                            "data": {
                                "src": "http://lorempixel.com/100/100"
                            }
                        }
                    ]
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Inline link inside a text"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "If you want to use this link just click "
                    },
                    "blocks": [
                        {
                            "type": "static-link",
                            "data": {
                                "text": "here"
                            },
                            "properties": {
                                "type": "inline"
                            }
                        }
                    ]
                }
            ]
        }
    }
}
```
