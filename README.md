# defining-hardware
defining physical hardware as structured data using JSON and JSON schema

"hardware-family.json"
>Document used to define high level categories or "families" for hardware e.g. fixings.

"hardware-type.json"
>Document used to define types of hardware that fall within hardware families e.g. screw which fall under the hardware family fixings. "hardware-type.json references "hardware-familty.json".

"hardware-product.json"
>Contains all variations available on a type of hardware such as a screw. "hardware-product.json" references many documents including units, dimensions, materials and standards. Documents referenced as options.

"hardware-object.json"
>Document refers to specific piece of hardware available to buy through a supplier. A hardware-object will match certain options within "hardware-product.json" enabling specs to be described seperatly to solutions. The exact solution or "hardware-object" can be chosen by a maker based on the spec described through selections made in "hardware-product.json". Quantified config doc. needed to list selections made in "hardware-product.json" enabling match to "hardware-object.json" docs. Many matches expected in most cases.
