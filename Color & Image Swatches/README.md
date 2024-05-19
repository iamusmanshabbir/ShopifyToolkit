# Step 1: Add Code in `settings_schema.json`

Add the Following Code in `settings_schema.json` just open this file in shopify and jUst put this below the first info tag where you see the shopify version etc just put under that


```json

    "//": "Developed by Usman Shabbir. Code Purpose: Image Color Swatches",

{
    "name": "Color Swatches ",
    "settings": [
        {
            "type": "paragraph",
            "content": "Developed by Usman Shabbir, For any shopify related service please email at usmanshabbir1004@gmail.com"
        },
        {
            "type": "text",
            "id": "optionName",
            "label": "Swatch option name",
            "default": "Color",
            "info": "Make sure capitalization is same as variant for e.g Color not color "
        },
        {
            "type": "paragraph",
            "content": "If your store is in different languages, type in all the different words and separate them with commas. For example: Color, Colour, Couleur"
        },
        {
            "type": "select",
            "id": "swatchType",
            "label": "Swatch type",
            "options": [
                {
                    "value": "color",
                    "label": "Color"
                },
                {
                    "value": "variantImage",
                    "label": "Variant image"
                }
            ],
            "default": "color"
        },
        {
            "type": "textarea",
            "id": "swatchColors",
            "label": "Colors",
            "placeholder": "Red:#ff0000\nGreen:#00ff00\nBlue:#0000ff",
            "default": "Black:#000000\nWhite:#f5f5f5\nBlue:#005eff\nRed:#c9002c\nPink:#ffd5e6\nBrown:#a2896b\nOlive:#808000\nGreenRed:#008000#c9002c\nGreenRedBlue:#008000#c9002c#005eff",
            "info": "One rule per line. Example: Blue:#005eff\n2 Color Swatch Example: GreenRed:#008000#c9002c\n3 Color Swatch Example: GreenRedBlue:#008000#c9002c#005eff"
        },
        {
            "type": "paragraph",
            "content": "You can also add [image files](\/admin\/content\/files?selectedView=all&media_type=Image) instead of using colors, in lowercase with spaces replaced by hyphens. Example: Green kaki: green-kaki.png"
        },
        {
            "type": "select",
            "id": "swatchStyle",
            "label": "Swatch style",
            "options": [
                {
                    "value": "round",
                    "label": "Round"
                },
                {
                    "value": "square",
                    "label": "Square"
                },
                {
                    "value":"square-round-corners",
                    "label":"Square round corners"
                },
                {
                    "value": "portrait",
                    "label": "Portrait"
                }
            ],
            "default": "round",
            "info":"Portrait mode is only available for the variant image type."
        },
        {
            "type": "range",
            "id": "swatchSize",
            "min": 20,
            "max": 120,
            "step": 2,
            "unit": "px",
            "label": "Swatch size",
            "default": 40
        }
    ]
}
