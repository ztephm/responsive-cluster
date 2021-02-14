## Responsive Map

This is a demonstration of how thematic map types can be changed responsively.

### Why should a map theme change when screen size changes?
Interface design guidelines like [this](https://msdn.microsoft.com/en-us/library/windows/apps/hh202889) and [this](https://developer.apple.com/ios/human-interface-guidelines/visual-design/adaptivity-and-layout/) recommend minimum touchscreen target sizes.
An interactive map marker's minimum clickable area can extend across other markers.

This is a prototype of one solution: *aggregate map points into interactive clusters on small screens.*

* This prototype is made with [CARTO.js v3/3.15](https://github.com/CartoDB/cartodb.js/tree/3.15.9), which incorporates [these other libraries](https://github.com/CartoDB/cartodb.js/tree/3.15.9/vendor).
* Clusters are created via a [PostgreSQL](https://www.postgresql.org/) query based on a modified [CARTO algorithm](https://github.com/CartoDB/cartodb/blob/63318c443c81932c6a7faf3d8cdbb627eb8b9f13/lib/assets/javascripts/cartodb/models/carto.js#L207), and styled with [CartoCSS](https://carto.com/docs/carto-engine/cartocss/).
* [Window functions](https://developer.mozilla.org/en-US/docs/Web/API/Window) are used to make clusters for small screens only.
* Different functionality can become enabled in smaller-width screens. Click on the four-arrow button to enable zoom, home (return original center and zoom), and legend toggle buttons.
