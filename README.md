<p align="center">
  <a href="#">
    <img width="150" src="logo.png">
  </a>
</p>

# @extensionengine/eslint-config
[![npm package version](https://badgen.net/npm/v/@extensionengine/eslint-config)](https://npm.im/@extensionengine/eslint-config) [![github license](https://badgen.net/github/license/extensionengine/eslint-config)](https://github.com/extensionengine/eslint-config/blob/master/LICENSE)

This package provides Extension Engine's extensible ESLint config.

## Usage

Package contains two shared ESLint configs:

### @extensionengine/eslint-config

This is default configuration supporting both server & Vue powered client codebases.

### @extensionengine/eslint-config/base

This is base configuration without Vue specific rules.

### Install

Use `install-peerdeps`

```
npx install-peerdeps --dev @extensionengine/eslint-config
```
or the classic way:
```
npm install --save-dev eslint @extensionengine/eslint-config eslint-plugin-import eslint-plugin-node eslint-plugin-promise eslint-plugin-standard eslint-plugin-vue eslint-config-standard eslint-config-semistandard
```

### Using `@extensionengine/eslint-config` in your project
In your local `.eslintrc.*` extend this configuration

```js
'use strict';

module.exports = {
  root: true,
  extends: '@extensionengine'
};
```

If you don't need Vue you can use base configuration:

```js
'use strict';

module.exports = {
  root: true,
  extends: '@extensionengine/base'
};
```

Check [ESlint documentation](https://eslint.org/docs/rules/) for rules explanation. 
