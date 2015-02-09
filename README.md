# postcss-host

> [PostCSS](https://github.com/postcss/postcss) plugin to make :host selectors work properly with pseudo-classes

## Installation

```console
$ npm install postcss-host
```

## Usage

```js
// dependencies
var fs = require("fs")
var postcss = require("postcss")
var postcssHost = require("postcss-host")

// css to be processed
var css = fs.readFileSync("input.css", "utf8")

// process css
var output = postcss()
  .use(postcssHost())
  .process(css, {
    from: "src/index.css"
    to: "dist/index.css"
  })
  .css
```

Checkout [tests](test) for examples.

## Contributing

Work on a branch

```console
$ git clone https://github.com/postcss/postcss-url.git
$ git checkout -b patch-1
$ npm install
$ npm test
```