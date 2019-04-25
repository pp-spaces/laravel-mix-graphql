# Laravel Mix GraphQL Extension

[![Downloads](https://img.shields.io/npm/dm/@pp-spaces/laravel-mix-graphql.svg)](https://www.npmjs.com/package/@pp-spaces/laravel-mix-graphql)
[![Release](https://img.shields.io/npm/v/@pp-spaces/laravel-mix-graphql/latest.svg)](https://www.npmjs.com/package/@pp-spaces/laravel-mix-graphql)
[![License](https://img.shields.io/github/license/pp-spaces/laravel-mix-graphql.svg)](LICENSE)

A Laravel Mix extension for GraphQL support for Webpack.

# Installation

```sh
yarn add -D @pp-spaces/laravel-mix-graphql
```

or

```sh
npm install @pp-spaces/laravel-mix-graphql --save-dev
```

# Laravel Mix Configuration

In your `webpack.mix.js`, import `@pp-spaces/laravel-mix-graphql`:

```js
// webpack.mix.js

const mix = require("laravel-mix");

/**
 * Import laravel-mix-graphql
 */
require("@pp-spaces/laravel-mix-graphql");

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
