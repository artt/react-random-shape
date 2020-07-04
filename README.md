# react-random-shapes

Create a random, wavy `svg` image. A few different shapes are planned:

* [`RandomHLine`](#randomhline)
* [`RandomVLine`](#randomvline)
* [`RandomBlob`](#randomblob)

This package was inspired by [blobmaker.app](https://www.blobmaker.app/).

[![NPM](https://img.shields.io/npm/v/react-random-shape.svg)](https://www.npmjs.com/package/react-random-shape) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

## Install

```bash
npm install --save react-random-shape
```

## Usage

```jsx
import React from 'react'

import RandomHLine from 'react-random-shape'

export default function Example() {
  return <RandomHLine width="600" height="300" />
}
```

For all shapes, `width` and `height` attributes are required. Additionally, various options could be specified.

### List of Shapes

#### `RandomHLine`

Generates a horizontal line (going roughly from left to right). Options available are:

* `leftPos` (default `0.5*height`) Vertical position of the left handle.
* `leftRoom` (default `0.3*height`) Size of the [1-D] window in which `leftPos` could wiggle around.
* `rightPos` (default `0.5*height`) Similar to `leftPos`.
* `rightRoom` (default `0.3*height`) Similar to `leftRoom`.
* `sections` (default `1`) Number of section the curve will be divided into.
* `midRoom` (default `0.2*height`) Size of the [2-D] window in which the middle control points could wiggle around.
* `angleRoom` (default `Math.PI / 3`) Size of the window in which the angle of the control point, as measured from the control point, could wiggle around.
* `fillTop` (default `"transparent"`) Fill of the top part.
* `fillBottom` (default `"transparent"`) Fill of the bottom part.
* `strokeMid` (default `"black"`) Stroke style of the dividing line.
* `showHandles` (default `false`) Show the handles and control points (for debug purpose).

#### `RandomVLine`

[Not yet available.]

#### `RandomBlob`

[Not yet available.]

## License

MIT © [artt](https://github.com/artt)
