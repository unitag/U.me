#Grid demo

Demo of a grid using various example of display for the same content

```json
{
    "label": "Demo grid",
    "ume": {
        "type": "ume",
        "blocks": {
            "type": "static-page",
            "blocks": [
                {
                    "type": "static-text",
                    "data": {
                        "text": "Classic grid using the default value of the grid-class"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "ume-grid",
                    "blocks": [
                        {
                            "type": "static-text",
                            "data": {
                                "text": "TEST1"
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
                                "text": "TEST TEST TEST TEST TEST"
                            }
                        },
                        {
                            "type": "bind-image",
                            "data": {
                                "src": "http://lorempixel.com/500/300"
                            }
                        },
                        {
                            "type": "static-text",
                            "data": {
                                "text": "TEST TEST TEST"
                            }
                        }
                    ]
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Small-6 columns"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "ume-grid",
                    "properties": {
                        "gridClass": [
                            "small-6 panel"
                        ]
                    },
                    "blocks": [
                        {
                            "type": "static-text",
                            "data": {
                                "text": "TEST1"
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
                                "text": "TEST3 TEST TEST TEST TEST"
                            }
                        },
                        {
                            "type": "bind-image",
                            "data": {
                                "src": "http://lorempixel.com/500/300"
                            }
                        },
                        {
                            "type": "static-text",
                            "data": {
                                "text": "TEST TEST TEST"
                            }
                        }
                    ]
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Small-6 columns equalized"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "ume-grid",
                    "properties": {
                        "equalizer": true,
                        "notEqualizedOnStack": false,
                        "gridClass": [
                            "small-6 panel"
                        ]
                    },
                    "blocks": [
                        {
                            "type": "static-text",
                            "data": {
                                "text": "TEST1"
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
                                "text": "TEST3 TEST TEST TEST TEST"
                            }
                        },
                        {
                            "type": "bind-image",
                            "data": {
                                "src": "http://lorempixel.com/500/300"
                            }
                        },
                        {
                            "type": "static-text",
                            "data": {
                                "text": "TEST TEST TEST"
                            }
                        }
                    ]
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Small-6 Small-2 Small-4 columns equalized"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "ume-grid",
                    "properties": {
                        "equalizer": true,
                        "notEqualizedOnStack": false,
                        "gridClass": [
                            "small-6 panel",
                            "small-2 panel",
                            "small-4 panel"
                        ]
                    },
                    "blocks": [
                        {
                            "type": "static-text",
                            "data": {
                                "text": "TEST1"
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
                                "text": "TEST3 TEST TEST TEST TEST"
                            }
                        },
                        {
                            "type": "bind-image",
                            "data": {
                                "src": "http://lorempixel.com/500/300"
                            }
                        },
                        {
                            "type": "static-text",
                            "data": {
                                "text": "TEST TEST TEST"
                            }
                        }
                    ]
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Small-7 Small-5 Small-8 Small-4 columns equalized"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "ume-grid",
                    "properties": {
                        "equalizer": true,
                        "notEqualizedOnStack": false,
                        "gridClass": [
                            "small-7 panel",
                            "small-5 panel",
                            "small-8 panel",
                            "small-4 panel"
                        ]
                    },
                    "blocks": [
                        {
                            "type": "static-text",
                            "data": {
                                "text": "TEST1"
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
                                "text": "TEST3 TEST TEST TEST TEST"
                            }
                        },
                        {
                            "type": "bind-image",
                            "data": {
                                "src": "http://lorempixel.com/500/300"
                            }
                        },
                        {
                            "type": "static-text",
                            "data": {
                                "text": "TEST TEST TEST"
                            }
                        }
                    ]
                }
            ]
        }
    }
}
```
