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

Presented at [NACIS Annual Meeting 2017](https://nacis2017.sched.com/)

***

<img src="https://github.com/ztephm/responsive-cluster/blob/master/images/slides/responsive_cartography_slide1.png" alt="Slide 1: Tips for Making Web Maps Responsive Title Card" />
<img src="https://github.com/ztephm/responsive-cluster/blob/master/images/slides/responsive_cartography_slide2.png" alt="Slide 2: Data Optimization Tips Title Card" />
<img src="https://github.com/ztephm/responsive-cluster/blob/master/images/slides/responsive_cartography_slide3.png" alt="Slide 3: Optimization Tips" />
<img src="https://github.com/ztephm/responsive-cluster/blob/master/images/slides/responsive_cartography_slide4.png" alt="Slide 4" Interface Design Issues Title Card/>
<img src="https://github.com/ztephm/responsive-cluster/blob/master/images/slides/responsive_cartography_slide5.png" alt="Slide 5: Scroll Problem" />
<img src="https://github.com/ztephm/responsive-cluster/blob/master/images/slides/responsive_cartography_slide6.png" alt="Slide 6: Pan/Zoom Problem" />
<img src="https://github.com/ztephm/responsive-cluster/blob/master/images/slides/responsive_cartography_slide7.png" alt="Slide 7: Overlay Problem" />
<img src="https://github.com/ztephm/responsive-cluster/blob/master/images/slides/responsive_cartography_slide8.png" alt="Slide 8: Interactivity Problem" />
<img src="https://github.com/ztephm/responsive-cluster/blob/master/images/slides/responsive_cartography_slide9.png" alt="Slide 9: Cartography Tips Title Card" />
<img src="https://github.com/ztephm/responsive-cluster/blob/master/images/slides/responsive_cartography_slide10.png" alt="Slide 10: Projection, Marker and Font Tips" />
<img src="https://github.com/ztephm/responsive-cluster/blob/master/images/slides/responsive_cartography_slide10.png" alt="Slide 11: Responsive Thematic Map Coding Tips Title Card" />
<img src="https://github.com/ztephm/responsive-cluster/blob/master/images/slides/responsive_cartography_slide12.png" alt="Slide 12: Responsive Cartography Example" />
<img src="https://github.com/ztephm/responsive-cluster/blob/master/images/slides/responsive_cartography_slide13.png" alt="Slide 13: Window Function" />
<img src="https://github.com/ztephm/responsive-cluster/blob/master/images/slides/responsive_cartography_slide14.png" alt="Slide 14: Queries for Clusters or Points" />
<img src="https://github.com/ztephm/responsive-cluster/blob/master/images/slides/responsive_cartography_slide15.png" alt="Slide 15: Resource Links" />
