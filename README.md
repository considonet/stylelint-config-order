# @considonet/stylelint-config-order

> Default [`stylelint`](https://github.com/stylelint/stylelint) profile to handle properties ordering in CSS stylesheets for ConsidoNet projects.

## Rules

* Inspired by [Idiomatic CSS declaration order](https://github.com/necolas/idiomatic-css#declaration-order).
* Requires `content` property to go first (if set).


## Installation

Using npm:

```sh
npm install --save-dev @considonet/stylelint-config-order
```

or using yarn:

```sh
yarn add @considonet/stylelint-config-order --dev
```

## Usage

In your .stylelintrc.js file extend your config:

```json
{ 
  "extends": "@considonet/stylelint-config-order"
}
```

### Usage with other configs

**This config contains only rules for properties ordering and probably you don't want to use it standalone.**
We recommend to use `@considonet/stylelint-config-order` with at least [`@considonet/stylelint-config-scss`](https://github.com/considonet/stylelint-config-scss) or any other general ruleset.

See [popular `stylelint` configs](https://www.npmjs.com/search?q=stylelint-config&ranking=popularity) for more inspirations.

Example usage with other our packages:

```json
{
  "extends": [
    "@considonet/stylelint-config-bem",
    "@considonet/stylelint-config-scss",
    "@considonet/stylelint-config-order"
  ]
}
```

You can also use our default preset which includes this configuration - [`@considonet/stylelint-config-default`](https://github.com/considonet/stylelint-config-default).
