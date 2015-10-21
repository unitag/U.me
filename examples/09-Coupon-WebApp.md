#Web App example for a coupon

```json
{
    "label": "Coupon Demo",
    "ume": {
        "type": "ume",
        "blocks": {
            "type": "static-page",
            "css": "{line-height: 0px; background-color: purple; padding-bottom: 10px;}",
            "blocks": [
                {
                    "type": "bind-image",
                    "data": {
                        "src": "https://static-unitag.com/file/filepicker/a21dd59e564b196b12eec267e0056702.png"
                    },
                    "css": "{background-color: white;} img{position: relative; margin-left: auto; margin-right: auto; display: block; max-height: 200px;}"
                },
                {
                    "type": "bind-image",
                    "data": {
                        "src": "https://static-unitag.com/file/filepicker/9210e9dc33d1fb2e6cebab71a5015c28.jpeg"
                    },
                    "properties": {
                        "sizing": "cover",
                        "height": "200px"
                    },
                    "css": "img{position: relative; display: block;}"
                },
                {
                    "type": "static-text",
                    "css": "{line-height: normal; font-family: Arial; border-top: 5px dashed white; color: white; font-weight: bold; text-align: center; margin-top: 10px; font-size: 80px; padding-top: 20px; margin-bottom: 0px;}",
                    "blocks": [
                        {
                            "type": "static-text",
                            "data": {
                                "text": "20%"
                            },
                            "properties": {
                                "element": "span"
                            },
                            "css": "{font-size : 80px;}"
                        },
                        {
                            "type": "static-text",
                            "data": {
                                "text": "0ff"
                            },
                            "properties": {
                                "element": "span"
                            },
                            "css": "{font-size : 40px; vertical-align: super;}"
                        }
                    ]
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "on the summer collection when you purchase two items."
                    },
                    "css": "{color: white; text-align: center;}"
                },
                {
                    "type": "static-text",
                    "css": "{border-bottom: 5px dashed white; margin-bottom: 10px; margin-top: 0px;}",
                    "blocks": [
                        {
                            "type": "static-link",
                            "css": "{width: auto; position: relative; margin-left: 20%; margin-right: 20%; text-align: center; padding-bottom: 20px; border-width: 0px; display: block; padding-bottom: 20px; color: purple; padding: 10px;}",
                            "data": {
                                "text": "DOWNLOAD MY COUPON"
                            },
                            "properties": {
                                "baseColor": "#fff"
                            }
                        }
                    ]
                },
                {
                    "type": "static-text",
                    "properties": {
                        "element": "div"
                    }
                }
            ]
        }
    }
}

```
