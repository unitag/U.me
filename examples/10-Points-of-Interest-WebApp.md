#Web App example for a coupon

Adapted from the file single-coupon.png

```json
{
    "ume": {
        "type": "ume",
        "blocks": {
            "type": "static-page",
            "css": "{line-height:0px;}",
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
                    "type": "bind-image",
                    "data": {
                        "src": "https://static-unitag.com/file/filepicker/9210e9dc33d1fb2e6cebab71a5015c28.jpeg"
                    },
                    "properties": {
                        "sizing": "cover",
                        "height": "200px"
                    },
                    "class": [
                        "cover"
                    ]
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "N°4 - The Eiffel Tower"
                    },
                    "properties": {
                        "element": "h2"
                    },
                    "css": "{text-align: center; background-color: teal; color: white; margin: 0px; padding: 10px; padding-bottom: 5px; padding-top: 20px;}"
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "This monument as tall as 312 meters has become the symbol of the French capital"
                    },
                    "properties": {
                        "element": "h4"
                    },
                    "css": "{font-family: Arial; text-align: center; font-size: 14px; background-color: teal; color: white; margin: 0px; padding-bottom: 20px; padding-left: 40px; padding-right: 40px; border-width: 0px;}"
                },
                {
                    "type": "static-text",
                    "data": {
                        "text": "The Eiffel Tower was built by Gustave Eiffel for the universal exhibition taking place in Paris in 1889. The work lasted tow years, two months and five days. It has been recognised as a historical monument since 1964 and as a worldwide heritage by Unesco since 1991"
                    },
                    "css": "{font-family: Arial; text-align: justify; font-size: 13px; color: #777; margin: 0px; padding: 10px; padding-left: 15px; padding-right: 15px; border-width: 0px;}"
                }
            ]
        }
    }
}


```
