## name

## version

## main
The main field is a module ID that is the primary entry point to your program. That is, if your package is named `var`, and a user installs it, and then does `require("var")`, then your main module's exports object will be returned.
This should be a module relative to the root of your package folder.
For most modules, it makes the most sense to have a mainn script and often not much else.
If `main` is not set it defaults to `index.js` in the package's root folder.

## engines

## type
The package.json "type" field defines how Node.js should interpret `.js` files. If a package.json file does not have a "type" field, .js files are treated as CommonJS.
A package.json "type" value of "module" tells Node.js to interpret .js files within that package as using ES module syntax.
The "type" field applies not only to initial entry points but also to files referenced by import statements and import() expressions.

```js
// my-app.js, treated as an ES module because there is a package.json
// file in the same folder with "type": "module".

import './startup/init.js';
// Loaded as ES module since ./startup contains no package.json file,
// and therefore inherits the "type" value from one level up.

import 'commonjs-package';
// Loaded as CommonJS since ./node_modules/commonjs-package/package.json
// lacks a "type" field or contains "type": "commonjs".

import './node_modules/commonjs-package/index.js';
// Loaded as CommonJS since ./node_modules/commonjs-package/package.json
// lacks a "type" field or contains "type": "commonjs".
```
## pregerGlobal

## description

## author

## license

## repository

## keywords

## main

## bin

## scripts

## devDependencies

## dependencies

