# cardinal-spline

A cardinal spline is a sequence of individual curves joined to form a larger curve. The spline is specified by an array of points and a tension parameter. A cardinal spline passes smoothly through each point in the array; there are no sharp corners and no abrupt changes in the tightness of the curve. The following illustration shows a set of points and a cardinal spline that passes through each point in the set.


![figure!](cardinal-spline-ex.png)


## Install
[![NPM](https://nodei.co/npm/cardinal-spline.png?downloads=true)](https://nodei.co/npm/cardinal-spline/)

`npm install cardinal-spline`

or with bower:

`bower install cardinal-spline`


## Use


```js
var cSpline = require('cardinal-spline');

var splinePoints = cSpline(points[, tension, numOfSeg, close]);
//-> splinePoints is a flat Float32Array, [x1, y1, x2, y2, ..., xn, yn]

```

### Options

```js
/**
* @param {Array} points - (flat) point array: [x1, y1, x2, y2, ..., xn, yn]
* @param {Number} [tension=0.5] - tension. Typically between [0.0, 1.0] but can be exceeded
* @param {Number} [numOfSeg=25] - number of segments between two points (line resolution)
* @param {Boolean} [close=false] - Close the ends making the line continuous
* @returns {Float32Array} - the spline points.
*/
```

## License

MIT
