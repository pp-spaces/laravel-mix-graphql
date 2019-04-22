# Laravel Mix GraphQL Extension

A Laravel Mix extension for GraphQL support for Webpack.

# Installation

```sh
yarn add -D laravel-mix-graphql
```

or

```sh
npm install laravel-mix-graphql --save-dev
```

# Laravel Mix Configuration

In your `webpack.mix.js`, import `laravel-mix-graphql`:

```js
// webpack.mix.js

const mix = require("laravel-mix");

/**
 * Import laravel-mix-graphql
 */
require("laravel-mix-graphql");

/**
 * Register loader
 */
mix
  .js("resources/js/app.js", "public/js")
  .sass("resources/sass/app.scss", "public/css")
  .graphql();
```

Done!, re-run your compile command.

# Usage

Within your project, e.g. `app.js`, you can import `.graphql` or `.gql` schema directly.

```js
// app.js

import UserQuery from "./graphql/UserQuery.graphql";
```

# Author

Socheat, Web Developer

![Twitter Follow](https://img.shields.io/twitter/follow/socheatsok78.svg?style=social)
