# Three.js and R

Three.js widgets for R and shiny. The package includes

* globejs:  a widget that plots data and images on a 3-d globe
* scatterplot3js:  a 3-d scatterplot widget.

Both widgets are easy to use and render directly in RStudio or in web browsers.
The widgets can be invoked directly or from Shiny applications. They produce
high-quality interactive visualizations with just a few lines of R code.

See http://threejs.org for details on three.js.

See http://bwlewis.github.io/rthreejs  for an example.

This project is based on the new htmlwidgets package. See
https://github.com/ramnathv/htmlwidgets for details and links to several
amazingly cool visualization widgets for R.

## NOTE!

These examples generally run best in WebGL-enabled viewers, including at least
Chrome, Firefox, and recent versions of Internet Explorer web browsers.  We do
try to maintain basic support for non-WebGL equipped browsers, but the
performance and rendering quality will generally be inferior to WebGL
visualizations.

## Examples

The following example illustrates the 3D scatterplot widget.
```r
library("shiny")
runApp(system.file("examples/scatterplot",package="threejs"))
```

The next example illustrates the globe widget by plotting the relative
population of some cities using data from the R maps package on a globe. It's
based on the JavaScript WebGL Globe Toolkit (https://github.com/dataarts) by
the Google Creative Lab Data Arts Team.
```r
runApp(system.file("examples/globe",package="threejs"))
```

For detailed help on the widgets and additional examples, see
```r
?scatterplot3js
?globejs
```

# Licenses

## Three.js

The MIT License

Copyright (c) 2010-2014 three.js authors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

## Globe example

Includes ideas and images from the dat.globe JavaScript WebGL Globe Toolkit
https://github.com/dataarts/webgl-globe

Copyright 2011 Data Arts Team, Google Creative Lab
Licensed under the Apache License, Version 2.0
http://www.apache.org/licenses/LICENSE-2.0.
