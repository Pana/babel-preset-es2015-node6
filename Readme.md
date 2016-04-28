# babel-preset-es6-node6

> Babel preset to make node@6 fully ES2015 compatible.

[![](https://img.shields.io/npm/v/babel-preset-es6-node6.svg)](https://npmjs.org/package/babel-preset-es6-node6)
[![](http://img.shields.io/npm/dm/babel-preset-es6-node6.svg)](https://npmjs.org/package/babel-preset-es6-node6)

Node@6 has great [ES2015 support](https://nodejs.org/en/docs/es6/),
this module just adds missing features:
- modules ([transform-es2015-modules-commonjs](http://babeljs.io/docs/plugins/transform-es2015-modules-commonjs/))
- unicode & sticky regular expressions ([transform-es2015-sticky-regex](http://babeljs.io/docs/plugins/transform-es2015-sticky-regex/) & [transform-es2015-unicode-regex](http://babeljs.io/docs/plugins/transform-es2015-unicode-regex/))

## Install

    npm install --save-dev babel-preset-es6-node6

## Usage

Read ["Configuring Babel 6" article](http://www.2ality.com/2015/11/configuring-babel6.html)
for more information about babel@6 configuration.

### Via `.babelrc` (recommended)

**.babelrc**

```json
{
  "presets": ["es6-node6"]
}
```

### Via CLI

    babel script.js --presets es6-node6

### Via Node API

```js
require('babel-core').transform('code', {
  presets: ['es6-node6'],
})
```

## License

[MIT](./LICENSE)
