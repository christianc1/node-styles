# Lift Styles for npm
## Base Styles and Variables for a NPM Managed Project

### What is this?
A placeholder where styles are supposed to go.  This repo will not accept pull requests, it's normalized variables to probably be extended in a _fork_ of this repo.  Based on [bitters](https://github.com/thoughtbot/bitters), requires [bourbon](https://github.com/thoughtbot/bourbon).  Made available by [Lift](http://liftux.com) for us to use with our internal and client projects, YMMV.

### Getting Started
**Install using npm**
`npm install https://github.com/{USER_or_ORG}/{YOUR-FORK}`

### Using in a project
**Webpack:**  If you're using `sass-loader`, in the component scss...
```
@import '~bourbon/app/assets/stylesheets/bourbon';
@import '~lift-styles/base/base';
```
... and make sure you are not excluding `node_modules` in your webpack config for the scss loader.  As long as you aren't, webpack should resolve `~lift-styles/` to `{PATH}/node_modules/lift-styles/`

**Other:** Generally speaking, if you define your scss to be loaded by path...
```
var baseStylePath = require('lift-styles').includePath;
```
... then include `baseStylePath` in your scss file paths array.


	