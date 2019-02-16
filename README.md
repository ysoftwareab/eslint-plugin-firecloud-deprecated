# eslint-config-firecloud [![Build Status][2]][1]

The ESLint config used within Tobii Cloud Services.

In your project's `.eslintrc.js`

```js
module.exports = {
  extends: [
    'firecloud/node.js'
  ],
  rules: {
    'override-some-rule': error
  }
}
```

Optionally, you can run `node_modules/eslint-config-firecloud/npm-install-peer-dependencies`
in order to install the required peer dependencies.


## Bundles

Common bundles are provided as following:

- Node.js: `firecloud/node.js`
- Browser: `firecloud/browser.js`

- Node.js test with Jest: `firecloud/test-jest.js`
- Node.js test with Mocha&Chai: `firecloud/test-mocha-chai.js`


## Guiding Principles

"I (don't) like/want ..." is no argument in this codebase.
Instead, we follow a few guiding principles
that have concrete consequences on daily work.

1. Keep It Short
  * lines
  * functions
  * modules
2. Reduce merge conflicts
  * do less on the same line
  * break array/object expressions/patterns
  * break import specifiers
  * break conditions
3. Reduce cognitive load via explicit code
  * even if code becomes more verbose
4. Reduce dependency on specific ecma versions
  * use a transpiler like babel (for syntax)
  * use a utility library like lodash-firecloud (for functionality)
5. Increase consistency
  * Don't use arrow functions when you don't need them
  * Don't use template literals when you don't need them


## License

[UNLICENSE](UNLICENSE)


  [1]: https://travis-ci.com/tobiipro/eslint-config-firecloud
  [2]: https://travis-ci.com/tobiipro/eslint-config-firecloud.svg?branch=master
