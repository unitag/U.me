#Map demo

Demo of the google map, Google map markers and Google map directions components

```json
{
    "label": "Demo Google Map",
    "ume": {
        "type": "ume",
        "blocks": {
            "type": "static-page",
            "blocks": [
                {
                    "type": "static-text",
                    "data": {
                        "text": "Default map without properties"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "bind-map",
                    "css": "{height:500px; margin:15px}"
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Map with a specific latitude and longitude"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "bind-map",
                    "css": "{height:500px; margin:15px}",
                    "properties": {
                        "latitude" : "47.5833",
                        "longitude" : "1.3333"
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Map with zoom properties"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "bind-map",
                    "css": "{height:500px; margin:15px}",
                    "properties": {
                        "latitude" : "47.5833",
                        "longitude" : "1.3333",
                        "zoom": 4,
                        "minZoom": 2,
                        "maxZoom": 7
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Map with markers"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "bind-map",
                    "css": "{height:500px; margin:15px}",
                    "properties": {
                        "fitToMarkers": true,
                        "markers": [
                            {
                                "latitude": "47.5833",
                                "longitude": "1.3333",
                                "title": "Blois"
                            },
                            {
                                "latitude": "43.6043",
                                "longitude": "1.4437",
                                "title": "Toulouse"
                            }
                        ]
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Same map with an hybrid display"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "bind-map",
                    "css": "{height:500px; margin:15px}",
                    "properties": {
                        "fitToMarkers": true,
                        "mapType": "hybrid",
                        "markers": [
                            {
                                "latitude": "47.5833",
                                "longitude": "1.3333",
                                "title": "Blois"
                            },
                            {
                                "latitude": "43.6043",
                                "longitude": "1.4437",
                                "title": "Toulouse"
                            }
                        ]
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "Now with directions"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "bind-map",
                    "css": "{height:500px; margin:15px}",
                    "properties": {
                        "fitToMarkers": true,
                        "markers": [
                            {
                                "latitude": "47.5833",
                                "longitude": "1.3333",
                                "title": "Blois"
                            },
                            {
                                "latitude": "43.6043",
                                "longitude": "1.4437",
                                "title": "Toulouse"
                            }
                        ],
                        "directions": {
                            "startAddress": "Paris, France",
                            "endAddress": "Toulouse, France"
                        }
                    }
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "You can also select the travel mode"
                    },
                    "properties": {
                        "element": "h1"
                    }
                },
                {
                    "type": "bind-map",
                    "css": "{height:500px; margin:15px}",
                    "properties": {
                        "language": "es",
                        "fitToMarkers": true,
                        "markers": [
                            {
                                "latitude": "44.5833",
                                "longitude": "1.3333"
                            },
                            {
                                "latitude": "45.6043",
                                "longitude": "1.4437"
                            },
                            {
                                "latitude": "45.6043",
                                "longitude": "2.4437"
                            }
                        ],
                        "directions": {
                            "startAddress": "Paris, France",
                            "endAddress": "Toulouse, France",
                            "travelMode": "TRANSIT"
                        }
                    }
                }
            ]
        }
    }
}
```