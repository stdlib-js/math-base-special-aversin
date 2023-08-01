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

# Arcversine

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Compute the [inverse versed sine][inverse-versed-sine].

<section class="intro">

The [inverse versed sine][inverse-versed-sine] is defined as

<!-- <equation class="equation" label="eq:arcversine" align="center" raw="\operatorname{aversin}(\theta) = \arccos(1-\theta)" alt="Inverse versed sine."> -->

```math
\mathop{\mathrm{aversin}}(\theta) = \arccos(1-\theta)
```

<!-- <div class="equation" align="center" data-raw-text="\operatorname{aversin}(\theta) = \arccos(1-\theta)" data-equation="eq:arcversine">
    <img src="https://cdn.jsdelivr.net/gh/stdlib-js/stdlib@bb29798906e119fcb2af99e94b60407a270c9b32/lib/node_modules/@stdlib/math/base/special/aversin/docs/img/equation_arcversine.svg" alt="Inverse versed sine.">
    <br>
</div> -->

<!-- </equation> -->

</section>

<!-- /.intro -->



<section class="usage">

## Usage

```javascript
import aversin from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-aversin@deno/mod.js';
```

#### aversin( x )

Computes the [inverse versed sine][inverse-versed-sine].

```javascript
var v = aversin( 0.0 );
// returns 0.0

v = aversin( 3.141592653589793/2.0 );
// returns ~2.1783

v = aversin( 3.141592653589793/6.0 );
// returns ~1.0742
```

If `x < 0`, `x > 2`, or `x` is `NaN`, the function returns `NaN`.

```javascript
var v = aversin( -1.0 );
// returns NaN

v = aversin( 3.14 );
// returns NaN

v = aversin( NaN );
// returns NaN
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
import linspace from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-base-linspace@deno/mod.js';
import aversin from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-aversin@deno/mod.js';

var x = linspace( 0.0, 2.0, 100 );

var i;
for ( i = 0; i < x.length; i++ ) {
    console.log( aversin( x[ i ] ) );
}
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/math-base/special/avercos`][@stdlib/math/base/special/avercos]</span><span class="delimiter">: </span><span class="description">compute the inverse versed cosine.</span>
-   <span class="package-name">[`@stdlib/math-base/special/vercos`][@stdlib/math/base/special/vercos]</span><span class="delimiter">: </span><span class="description">compute the versed cosine.</span>

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

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-special-aversin.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-special-aversin

[test-image]: https://github.com/stdlib-js/math-base-special-aversin/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/math-base-special-aversin/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-special-aversin/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-special-aversin?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-special-aversin.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-special-aversin/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/math-base-special-aversin/tree/deno
[umd-url]: https://github.com/stdlib-js/math-base-special-aversin/tree/umd
[esm-url]: https://github.com/stdlib-js/math-base-special-aversin/tree/esm
[branches-url]: https://github.com/stdlib-js/math-base-special-aversin/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-special-aversin/main/LICENSE

[inverse-versed-sine]: https://en.wikipedia.org/wiki/Versine

<!-- <related-links> -->

[@stdlib/math/base/special/avercos]: https://github.com/stdlib-js/math-base-special-avercos/tree/deno

[@stdlib/math/base/special/vercos]: https://github.com/stdlib-js/math-base-special-vercos/tree/deno

<!-- </related-links> -->

</section>

<!-- /.links -->
