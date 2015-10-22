#Simple demo

Live demo [here](http://opn.to/r/ume/simple-demo)

```json
{
    "label": "Simple Demo",
    "ume": {
        "type": "ume",
        "blocks": {
            "type": "static-page",
            "blocks": [
                {
                    "type": "static-text",
                    "data": {
                        "text": "Classic text paragraph without properties"
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Now it's a h1!"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Then it's a h2!"
                    },
                    "properties": {
                        "element": "h2"
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "And h3!"
                    },
                    "properties": {
                        "element": "h3"
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "h4 here we are!"
                    },
                    "properties": {
                        "element": "h4"
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "h5 this is it!"
                    },
                    "properties": {
                        "element": "h5"
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Finally h6!"
                    },
                    "properties": {
                        "element": "h6"
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Now back to a longer paragrpah, but this one is actually set with the paragraph element as properties. No more no less."
                    },
                    "properties": {
                        "element": "p"
                    }
                },
                {
                    "type": "static-text",
                    "properties": {
                        "element": "h1"
                    },
                    "data": {
                        "text": "Now we have a text,"
                    },
                    "blocks": [
                        {
                            "type": "static-text",
                            "properties": {
                                "element": "strong"
                            },
                            "data": {
                                "text": " and a strong text inside this text!"
                            }
                        }
                    ]
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Classic image without any properties"
                    }
                },
                {
                    "type": "bind-image",
                    "data": {
                        "src": "http://lorempixel.com/600/400"
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Sizing: cover"
                    }
                },
                {
                    "type": "bind-image",
                    "data": {
                        "src": "http://lorempixel.com/600/400"
                    },
                    "properties": {
                        "sizing": "cover",
                        "height": "150",
                        "width": "400"
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Sizing: contain"
                    }
                },
                {
                    "type": "bind-image",
                    "data": {
                        "src": "http://lorempixel.com/600/400"
                    },
                    "properties": {
                        "sizing": "contain",
                        "height": "500",
                        "width": "500"
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "With preload"
                    }
                },
                {
                    "type": "bind-image",
                    "data": {
                        "src": "http://lorempixel.com/600/400"
                    },
                    "properties": {
                        "preload": true
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "With preload and fade"
                    }
                },
                {
                    "type": "bind-image",
                    "data": {
                        "src": "http://lorempixel.com/600/400"
                    },
                    "properties": {
                        "preload": true,
                        "fade": true
                    }
                }
            ]
        }
    }
}
```
