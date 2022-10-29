# What is webpack

Webpack is a open-source module bundler for JavaScript.

When webpack processes your application, it internally builds a dependency graph from one or more entry points and then combines every module your project needs into one or more bundles.

Webpack's configuration file is `webpack.config.js`.
In `webpack.config.js`, you can define below properties.

- entry
  - `entry` indicates which module webpack should use to begin building out its internal dependency graph.

- output
  - `output` indicates where to emit the bundles it creates and how to name these files.

- loaders
  - By default, webpack only understands JavaScript and JSON. Loaders allow webpack to process other types of files and convert them into valid modules that can be consumed by your application and added to the dependency graph.

- plugins
  - While loaders are used to transform certain types of modules, plugins can be leveraged to perform a wider range of tasks like bundle optimization, asset management and injection of environment variables.
