
# JSVerify [![Build Status](https://secure.travis-ci.org/phadej/jsverify.png?branch=master)](http://travis-ci.org/phadej/jsverify)

Property based checking.

## Getting Started
Install the module with: `npm install jsverify`

## Synopsis

```js
var jsc = require("jsverify");
```

Example output of `node example.js`:

```
Propery doesn't hold, counterexample with undefined
inc failing: false
inc fixed: true
Propery doesn't hold, counterexample with [ 0 ]
add failing: { counterexample: [ 0 ] }
add fixed: true
Propery doesn't hold, counterexample with [ 0, -1 ]
add3 failing: { counterexample: [ 0, -1 ] }
intersects([1, 2], [1, 3]) true
intersects([1, 2], [3, 4]) false
Propery doesn't hold, counterexample with [ [] ]
intersects try 1: { counterexample: [ [] ] }
Propery doesn't hold, counterexample with [ [] ]
intersects try 2: { counterexample: [ [] ] }
intersects try 3: true
intersects try 4: true
```

## Documentation

## Contributing

In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).

- You can use `grunt jasmine-build` to generate `_SpecRunner.html` to run tests in your browser of choice.

### Preparing for release

- run `grunt readme` to regenerate `README.md`

## Release History

- 0.0.0 Initial preview

## License

Copyright (c) 2013 Oleg Grenrus. Licensed under the BSD3 license.

## Related work

- [JSCheck](http://www.jscheck.org/)
- [claire](https://npmjs.org/package/claire)
- [gent](https://npmjs.org/package/gent)
- [fatcheck](https://npmjs.org/package/fatcheck)
- [quickcheck](https://npmjs.org/package/quickcheck)