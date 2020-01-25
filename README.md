# sacss-netlify-forms-nuxt

> My praiseworthy Nuxt.js project

## Build Setup

``` bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev

# build for production and launch server
$ yarn build
$ yarn start

# generate static project
$ yarn generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).

### インストール編

Nuxt.jsの公式ドキュメントに従い、Nuxt.jsの環境を構築します。  
npm もしくは yarn がインストールされていることが前提になります。  
※npx は NPM 5.2.0 からデフォルトでバンドルされています。Node8.2以降であればデフォルトで npxが利用できます。  
npxはローカルにインストールしたnpmパッケージバイナリを直接実行できるコマンドになります。  
`run-script` の設定せずにローカルインストールしたコマンドを実行することができます。  
`create-nuxt-app` というコマンドでNuxtの基本的な環境を用意してくれるコマンドのため、`create-nuxt-app`を使いインストールを進めます。

```sh
npx create-nuxt-app  sacss-netlify-forms-nuxt
or
yarn create nuxt-app sacss-netlify-forms-nuxt
```

```sh
✨ Generating Nuxt.js project in sacss-netlify-forms-nuxt
? Project name sacss-netlify-forms-nuxt
? Project description My praiseworthy Nuxt.js project
? Author name redamoon
? Choose the package manager Yarn
? Choose UI framework Element
? Choose custom server framework None (Recommended)
? Choose Nuxt.js modules Axios, DotEnv
? Choose linting tools ESLint, Prettier, StyleLint
? Choose test framework None
? Choose rendering mode Universal (SSR)
? Choose development tools (Press <space> to select, <a> to toggle all, <i> to invert selection)
```

```sh
cd sacss-netlify-forms-nuxt
yarn dev
```

#### stylelintのエラー解消

stylelintでエラーがでるので、rulesのkeyを入れておきます。

```js
module.exports = {
  // add your custom config here
  // https://stylelint.io/user-guide/configuration
}
↓
module.exports = {
  "rules": {}
}
```

### Sass install

```sh
yarn add -D node-sass sass-loader
```

