<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->

# isCollection

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Test if a value is a collection.

<section class="intro">

A collection is defined as either an [`Array`][mdn-array], [`Typed Array`][mdn-typed-array], or an array-like [`Object`][mdn-object] (excluding `strings` and `functions`).

</section>

<!-- ./intro -->



<section class="usage">

## Usage

```javascript
import isCollection from 'https://cdn.jsdelivr.net/gh/stdlib-js/assert-is-collection@esm/index.mjs';
```

#### isCollection( value )

Tests if a value is a collection.

```javascript
var bool = isCollection( [] );
// returns true
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint-disable object-curly-newline -->

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="module">

import Int8Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-int8@esm/index.mjs';
import Uint8Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-uint8@esm/index.mjs';
import Uint8ClampedArray from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-uint8c@esm/index.mjs';
import Int16Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-int16@esm/index.mjs';
import Uint16Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-uint16@esm/index.mjs';
import Int32Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-int32@esm/index.mjs';
import Uint32Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-uint32@esm/index.mjs';
import Float32Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-float32@esm/index.mjs';
import Float64Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-float64@esm/index.mjs';
import isCollection from 'https://cdn.jsdelivr.net/gh/stdlib-js/assert-is-collection@esm/index.mjs';

var bool = isCollection( [] );
// returns true

bool = isCollection( new Float64Array( 10 ) );
// returns true

bool = isCollection( new Float32Array( 10 ) );
// returns true

bool = isCollection( new Int32Array( 10 ) );
// returns true

bool = isCollection( new Uint32Array( 10 ) );
// returns true

bool = isCollection( new Int16Array( 10 ) );
// returns true

bool = isCollection( new Uint16Array( 10 ) );
// returns true

bool = isCollection( new Int8Array( 10 ) );
// returns true

bool = isCollection( new Uint8Array( 10 ) );
// returns true

bool = isCollection( new Uint8ClampedArray( 10 ) );
// returns true

bool = isCollection( { 'length': 0 } );
// returns true

bool = isCollection( {} );
// returns false

bool = isCollection( 'beep' );
// returns false

bool = isCollection( isCollection );
// returns false

bool = isCollection( null );
// returns false

bool = isCollection( void 0 );
// returns false

bool = isCollection( 3.14 );
// returns false

</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/assert/is-array-like`][@stdlib/assert/is-array-like]</span><span class="delimiter">: </span><span class="description">test if a value is array-like.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2023. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/assert-is-collection.svg
[npm-url]: https://npmjs.org/package/@stdlib/assert-is-collection

[test-image]: https://github.com/stdlib-js/assert-is-collection/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/assert-is-collection/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/assert-is-collection/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/assert-is-collection?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/assert-is-collection.svg
[dependencies-url]: https://david-dm.org/stdlib-js/assert-is-collection/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/assert-is-collection/tree/deno
[umd-url]: https://github.com/stdlib-js/assert-is-collection/tree/umd
[esm-url]: https://github.com/stdlib-js/assert-is-collection/tree/esm
[branches-url]: https://github.com/stdlib-js/assert-is-collection/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/assert-is-collection/main/LICENSE

[mdn-array]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array

[mdn-typed-array]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/TypedArray

[mdn-object]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object

<!-- <related-links> -->

[@stdlib/assert/is-array-like]: https://github.com/stdlib-js/assert-is-array-like/tree/esm

<!-- </related-links> -->

</section>

<!-- /.links -->
