# select2-theme-bootstrap5

![select2-theme-bootstrap5 version](https://img.shields.io/badge/select2--theme--bootstrap5-v0.1.1-brightgreen.svg)
[![License](http://img.shields.io/badge/License-MIT-blue.svg)](http://opensource.org/licenses/MIT)

A [Select2](https://select2.github.io/) v4 [Theme](https://select2.github.io/examples.html#themes) for Bootstrap 5

Demonstrations [available](https://angel-vladov.github.io/select2-theme-bootstrap5/).

### Compatibility

Built and tested with Bootstrap v5 and Select2 v4.0.13 in the latest Chrome, Firefox and Safari (Mac).

### Installation

You can [download select2-theme-bootstrap5 from this GitHub repo](https://github.com/angel-vladov/select2-theme-bootstrap5/releases), or install it using `npm` and `yarn` – required if you want to integrate the Sass.

#### Install using npm/yarn

You may install select2-theme-bootstrap5-theme with [npm](https://www.npmjs.com/) or [Yarn](https://yarnpkg.com/):

```shell

// npm
npm install select2-theme-bootstrap5

// yarn
yarn add select2-theme-bootstrap5
```

### Usage

`select2-theme-bootstrap5` only works with Select2 v4.x. Applying the theme requires `select2-bootstrap.css` referenced after the default `select2.css` that comes with Select2:

```html
<link rel="stylesheet" href="select2.css">
<link rel="stylesheet" href="select2-bootstrap.css">
```

To apply the theme, tell Select2 to do so by passing `bootstrap` to the [`theme`](https://select2.github.io/examples.html#themes) option when initializing Select2:

```js
$('#dropdown').select2({
    theme: 'bootstrap'
});
```

You may also set it as the default theme for all Select2 widgets like so:

```js
$.fn.select2.defaults.set('theme', 'bootstrap');
```

### Changelog

##### 0.1.1
* `libsass` friendly division by 2
* Added additional select2 examples
* Documentation updates

##### 0.1.0 
 * Initial integration with Bootstrap 5
 * Forked from [select2-theme-bootstrap4](https://github.com/angel-vladov/select2-theme-bootstrap4)

### Contributing

The project offers [Sass](http://sass-lang.com/) sources for building `select2-bootstrap.css`; The code makes use of SCSS variables from [Bootstrap](https://getbootstrap.com/docs/5.1/customize/sass/#variable-defaults). The demo pages are built using [Jekyll](http://jekyllrb.com/) and there are a bunch of [Grunt](http://gruntjs.com/) tasks to ease development.

With [Jekyll](http://jekyllrb.com/), [node.js](http://nodejs.org/) and [Less](http://lesscss.org/) installed, run

```sh
npm install
```

to install all necessary development dependencies (Sass is compiled v[LibSass](https://github.com/sass/libsass/)/[node-sass](https://github.com/sass/node-sass)).

 * `grunt build` builds `docs`
 * `grunt serve` builds `docs` and serves them via Jekyll's `--watch` flag on http://localhost:3000

Develop in `src/select2-bootstrap.scss` and test your changes using `grunt serve`. Make sure tests are passing and verify that Sass compiles down to the target CSS via `npm test`.

### Copyright and license

Forked and modified from [select2 Bootstrap 3 theme](https://github.com/select2/select2-bootstrap-theme). All credits go to the original authors.
   
The license is available within the repository in the [LICENSE](LICENSE) file.
