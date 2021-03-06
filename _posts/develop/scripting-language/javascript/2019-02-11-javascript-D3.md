---
title: javascript / API / D3
categories:
-   javascript
tags:
-   javascript
-   api
header:  
    actions:
    -   label: GitHub
        url: https://github.com/d3/d3
---

# D3
D3(**D**ata-**D**riven **D**ocuments).js는 은 웹 표준을 사용하여 데이터를 시각화하는 JavaScript 라이브러리입니다. SVG, Canvas 및 HTML을 사용하여 데이터를 실제로 사용할 수 있도록 도와줍니다. 강력한 시각화 및 상호 작용 기술과 DOM 조작에 대한 데이터 중심 접근 방식을 결합하여 최신 브라우저의 모든 기능을 제공하고 데이터에 적합한 시각적 인터페이스를 자유롭게 설계 할 수 있습니다.

## API Reference
아래의 기준에따라 시각화를 분류할 수 있습니다.

-   [Arrays](https://github.com/d3/d3/blob/master/API.md#arrays-d3-array)  ([Statistics](https://github.com/d3/d3/blob/master/API.md#statistics),  [Search](https://github.com/d3/d3/blob/master/API.md#search),  [Transformations](https://github.com/d3/d3/blob/master/API.md#transformations),  [Histograms](https://github.com/d3/d3/blob/master/API.md#histograms))
-   [Axes](https://github.com/d3/d3/blob/master/API.md#axes-d3-axis)
-   [Brushes](https://github.com/d3/d3/blob/master/API.md#brushes-d3-brush)
-   [Chords](https://github.com/d3/d3/blob/master/API.md#chords-d3-chord)
-   [Collections](https://github.com/d3/d3/blob/master/API.md#collections-d3-collection)  ([Objects](https://github.com/d3/d3/blob/master/API.md#objects),  [Maps](https://github.com/d3/d3/blob/master/API.md#maps),  [Sets](https://github.com/d3/d3/blob/master/API.md#sets),  [Nests](https://github.com/d3/d3/blob/master/API.md#nests))
-   [Colors](https://github.com/d3/d3/blob/master/API.md#colors-d3-color)
-   [Color Schemes](https://github.com/d3/d3/blob/master/API.md#color-schemes-d3-scale-chromatic)
-   [Contours](https://github.com/d3/d3/blob/master/API.md#contours-d3-contour)
-   [Dispatches](https://github.com/d3/d3/blob/master/API.md#dispatches-d3-dispatch)
-   [Dragging](https://github.com/d3/d3/blob/master/API.md#dragging-d3-drag)
-   [Delimiter-Separated Values](https://github.com/d3/d3/blob/master/API.md#delimiter-separated-values-d3-dsv)
-   [Easings](https://github.com/d3/d3/blob/master/API.md#easings-d3-ease)
-   [Fetches](https://github.com/d3/d3/blob/master/API.md#fetches-d3-fetch)
-   [Forces](https://github.com/d3/d3/blob/master/API.md#forces-d3-force)
-   [Number Formats](https://github.com/d3/d3/blob/master/API.md#number-formats-d3-format)
-   [Geographies](https://github.com/d3/d3/blob/master/API.md#geographies-d3-geo)  ([Paths](https://github.com/d3/d3/blob/master/API.md#paths),  [Projections](https://github.com/d3/d3/blob/master/API.md#projections),  [Spherical Math](https://github.com/d3/d3/blob/master/API.md#spherical-math),  [Spherical Shapes](https://github.com/d3/d3/blob/master/API.md#spherical-shapes),  [Streams](https://github.com/d3/d3/blob/master/API.md#streams),  [Transforms](https://github.com/d3/d3/blob/master/API.md#transforms))
-   [Hierarchies](https://github.com/d3/d3/blob/master/API.md#hierarchies-d3-hierarchy)
-   [Interpolators](https://github.com/d3/d3/blob/master/API.md#interpolators-d3-interpolate)
-   [Paths](https://github.com/d3/d3/blob/master/API.md#paths-d3-path)
-   [Polygons](https://github.com/d3/d3/blob/master/API.md#polygons-d3-polygon)
-   [Quadtrees](https://github.com/d3/d3/blob/master/API.md#quadtrees-d3-quadtree)
-   [Random Numbers](https://github.com/d3/d3/blob/master/API.md#random-numbers-d3-random)
-   [Scales](https://github.com/d3/d3/blob/master/API.md#scales-d3-scale)  ([Continuous](https://github.com/d3/d3/blob/master/API.md#continuous-scales),  [Sequential](https://github.com/d3/d3/blob/master/API.md#sequential-scales),  [Diverging](https://github.com/d3/d3/blob/master/API.md#diverging-scales),  [Quantize](https://github.com/d3/d3/blob/master/API.md#quantize-scales),  [Ordinal](https://github.com/d3/d3/blob/master/API.md#ordinal-scales))
-   [Selections](https://github.com/d3/d3/blob/master/API.md#selections-d3-selection)  ([Selecting](https://github.com/d3/d3/blob/master/API.md#selecting-elements),  [Modifying](https://github.com/d3/d3/blob/master/API.md#modifying-elements),  [Data](https://github.com/d3/d3/blob/master/API.md#joining-data),  [Events](https://github.com/d3/d3/blob/master/API.md#handling-events),  [Control](https://github.com/d3/d3/blob/master/API.md#control-flow),  [Local Variables](https://github.com/d3/d3/blob/master/API.md#local-variables),  [Namespaces](https://github.com/d3/d3/blob/master/API.md#namespaces))
-   [Shapes](https://github.com/d3/d3/blob/master/API.md#shapes-d3-shape)  ([Arcs](https://github.com/d3/d3/blob/master/API.md#arcs),  [Pies](https://github.com/d3/d3/blob/master/API.md#pies),  [Lines](https://github.com/d3/d3/blob/master/API.md#lines),  [Areas](https://github.com/d3/d3/blob/master/API.md#areas),  [Curves](https://github.com/d3/d3/blob/master/API.md#curves),  [Links](https://github.com/d3/d3/blob/master/API.md#links),  [Symbols](https://github.com/d3/d3/blob/master/API.md#symbols),  [Stacks](https://github.com/d3/d3/blob/master/API.md#stacks))
-   [Time Formats](https://github.com/d3/d3/blob/master/API.md#time-formats-d3-time-format)
-   [Time Intervals](https://github.com/d3/d3/blob/master/API.md#time-intervals-d3-time)
-   [Timers](https://github.com/d3/d3/blob/master/API.md#timers-d3-timer)
-   [Transitions](https://github.com/d3/d3/blob/master/API.md#transitions-d3-transition)
-   [Voronoi Diagrams](https://github.com/d3/d3/blob/master/API.md#voronoi-diagrams-d3-voronoi)
-   [Zooming](https://github.com/d3/d3/blob/master/API.md#zooming-d3-zoom)

## Gallery
[Gallery](https://github.com/d3/d3/wiki/Gallery) 에서 데이터들을 정렬한 방식들을 확인할 수 있습니다.
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTg3MDg1NTQwN119
-->