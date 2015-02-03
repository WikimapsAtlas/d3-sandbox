>**Click States to test me !**>**Click States to test me !**

Alternative of: [Map zoom + static frame](http://bl.ocks.org/hugolpz/9643738d5f79c7b594d0), with more details.

Exploration around automatic centering, zooming, and responsive framing. This gist have **RESPONSIVE** frames.

Here, only the width is provided, the minimal height is calculated from the svg hook's width and the projected shape ratio. This tied frame is the relevant approach when waste of the webpage's space is not acceptable.

Inputs are the topojson file, a target feature (shape), and the svg canevas `width=300px`. Height, if missing (as in this demo), is recalculated elegantly. There is always a 5% margin on each side of the shape.

 1. Create a projection and d3.geo.path
 2. Profile the current projection : bounds, relevant dimensions, and shape's width/height ratio
 3. Compute scale and translation. Must fit within the width AND height. Without height, it caculate it from the canevas width and shape's ratio.
 4. Recreate the projection

The innovative part compared to Mike Bostock's [Centering a map given a GeoJSON object](http://stackoverflow.com/questions/14492284) is the responsive frame.

It is also projection proof. Which is not the case of the more common frame adjustment using the lat / lon dimensions' ratio, which works only with the common but hightly deforming rectangular projections.