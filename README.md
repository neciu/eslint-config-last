# Your last ESLint config
`eslint-config-last` is an opinionated [ESLint](http://eslint.org) config which incorporates [Prettier](https://github.com/prettier/prettier) for even better code formatting and unification.

## Usage 
[Yarn](https://yarnpkg.com) version:
1. Add `eslint-config-last` to your project: `yarn add eslint-config-last -D -E`.
2. Add peer dependencies: `yarn add eslint babel-eslint prettier  eslint-config-prettier eslint-plugin-prettier -D -E`.
3. Create `.eslintrc.js` configuration file: 
```js
module.exports = {
  extends: ['last'],
};
```
4. Add lint scripts to `package.json`:
```json
"scripts": {
  "lint": "yarn eslint .",
  "lint:fix": "yarn lint --fix"
}
```
5. Run `yarn lint` to lint your code.
6. Run `yarn lint:fix` to lint, format and fix your code.
