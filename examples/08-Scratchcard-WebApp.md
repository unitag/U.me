#Web App example for a scratchcard

```json
{
    "label": "SratchCard Demo",
    "ume": {
        "type": "ume",
        "blocks": {
            "type": "static-page",
            "css": "{background-color: #537732; }",
            "blocks": [
                {
                    "type": "bind-image",
                    "data": {
                        "src": "https://static-unitag.com/file/filepicker/a21dd59e564b196b12eec267e0056702.png"
                    },
                    "class": [
                        "logo"
                    ]
                },
                {
                    "type": "static-text",
                    "css": "{font-family: Arial; color: white; text-align: center; margin-top: 10px; font-size: 30px; padding-top:20px; margin-bottom: 0px;}",
                    "data": {
                        "text": "Your turn to play!"
                    }
                },
                {
                    "type": "ume-scratch",
                    "css": "{margin-bottom: 100px; margin-top:40px;}",
                    "properties": {
                        "bgColor": "#537732",
                        "realtime": true,
                        "shape": "circle",
                        "text": " "
                    },
                    "blocks": [
                        {
                            "type": "static-text",
                            "data": {
                                "text": "Won"
                            },
                            "css": "{line-height: 350px; font-style: italic; text-align: center; color: white; background-color: #ff6600; height: 350px; width: 100%; vertical-align: text-middle; font-weight: bold; font-size: 80px; font-family: Monotye Corsiva;}"
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
