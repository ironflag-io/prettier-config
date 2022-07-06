# @ironflag/prettier-config

![CI status](https://github.com/ironflag-io/prettier-config/actions/workflows/node-ci.yml/badge.svg)
[![npm version](https://badge.fury.io/js/@ironflag%2Fprettier-config.svg)](https://badge.fury.io/js/@ironflag%2Fprettier-config)

[IRONFLAG]'s extensible shared Prettier config.

[ironflag]: https://ironflag.io/

## Usage

### 1. Install prettier and this package

```sh
npm i -D @ironflag/prettier-config prettier
```

### 2. Add `@ironflag/prettier-config` to your `.prettierrc`

## What is overriden

```js
{
    semi: false, // boost code readability.
    singleQuote: true, // no Shift key.
    tabWidth: 4, // delete code duplicates.
    trailingComma: 'all', // easier code insert/delete.
    overrides: [
        // shorter tab for non-source code.
        {
            files: '*.{md,json,yml,yaml}',
            options: {
                tabWidth: 2,
            },
        },
    ],
}
```
