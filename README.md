# is-symbol <sup>[![Version Badge][2]][1]</sup>

[![dependency status][5]][6]
[![dev dependency status][7]][8]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][11]][1]

Is this an ES6 Symbol value?

## Example

```js
var isSymbol = require('is-symbol');
assert(!isSymbol(function () {}));
assert(!isSymbol(null));
assert(!isSymbol(function* () { yield 42; return Infinity; });

assert(isSymbol(Symbol.iterator));
assert(isSymbol(Symbol('foo')));
assert(isSymbol(Symbol.for('foo')));
assert(isSymbol(Object(Symbol('foo'))));
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[1]: https://npmjs.org/package/is-symbol
[2]: https://versionbadg.es/inspect-js/is-symbol.svg
[5]: https://david-dm.org/inspect-js/is-symbol.svg
[6]: https://david-dm.org/inspect-js/is-symbol
[7]: https://david-dm.org/inspect-js/is-symbol/dev-status.svg
[8]: https://david-dm.org/inspect-js/is-symbol#info=devDependencies
[11]: https://nodei.co/npm/is-symbol.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/is-symbol.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/is-symbol.svg
[downloads-url]: https://npm-stat.com/charts.html?package=is-symbol
