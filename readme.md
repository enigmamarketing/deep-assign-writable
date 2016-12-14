# This fork of [deep-assign](https://github.com/sindresorhus/deep-assign) is exactly the same, except:

Non-writable properties will not be merged, and the original value will be kept.

## Install

```
$ npm install --save deep-assign-writable
```


## Usage

```js
var deepAssign = require('deep-assign-writable');

deepAssign({a: {b: 0}}, {a: {b: 1, c: 2}}, {a: {c: 3}});
//=> {a: {b: 1, c: 3}}
```


### deepAssign(target, source, [source, ...])

Recursively assigns own enumerable properties of `source` objects to the `target` object and returns the `target` object. Additional `source` objects will overwrite previous ones, if it is writable.


## License

MIT © [Enigma Marketing Services](http://www.enigma-marketing.co.uk/)
