# cardinal-spline

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
