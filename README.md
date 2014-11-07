# atom-js-transpiler
I have a number of Atom packages, all with the same transpilation step.
Rather than copy-paste this across packages, it seems easier to centralize it here.

## Requirements

* Pre-transpiled source code must live in the package's `src` directory.
* Generated source code will be written in the package's `lib` directory.
* Source code may use the following features:
  * async/await
  * JSX
  * es6
  * type annotations

## Usage

```js
"scripts": {
  "prepublish": "node_modules/.bin/atom-js-transpile"
}
```
