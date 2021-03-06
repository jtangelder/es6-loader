# es6-loader
Transpiles ES6 modules for [webpack](https://github.com/webpack/webpack).

## Usage

```js
import bamboo from 'es6!./bamboo.js';

function Panda() {
  this.eat = bamboo;
}

export default Panda;
```

```js
var Panda = require('es6!./panda.js');
```

Or within the webpack config:

```js
module: {
  loaders: [
    { test: /\.js$/, loader: 'es6-loader' }
  ]
}
```

and then import normally:

```js
import bamboo from './bamboo.js';
```

## Install

`npm install es6-loader --save-dev`

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style.

## Release History
* 0.1.0 - Initial release

## License
Copyright (c) 2014 Kyle Robinson Young  
Licensed under the MIT license.
