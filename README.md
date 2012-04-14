This is a very simple tool to build a visibility graph. There are many caveats.

* The algorithm is very simple but shows the concept of building visibility graphs. It has a complexity in the neighborhood if [[$O(N^3)$]]; other algorithms are more efficient.

* It requires a single polygon as input, in WKT format, on stdin. It writes multiple WKT lines on stdout.

* JTS must be on your classpath.

* Lines which are coincident with edges of the polygon are not reproduced. JTS considers them not to be contained in the polygon.

Frankly, for any serious work I'd recommend a different library; I wrote this solely as a proof of concept.