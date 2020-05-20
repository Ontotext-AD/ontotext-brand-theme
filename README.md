# ontotext-brand-theme

A package containing UI theme css and resources.

## Installation

`npm install`

## Build

`npm run build` will process resources and output result in `build` directory.

`npm run watch` will watch source files for changes and rebuild automatically.

## Develope and test

All styles and resources can be tested in the `index.html`. Import everything which is needed and check it in a browser.

`npm run test` This is special command which runs the watch mode and opens the index.html file with a live-server that
will reload the page whenever styles or resources are changed.

## Usage

`npm install ontotext-visual-theme` installs the package in local node_modules. After that there are two basic scenarios available.

### Link to resources directly in the html header

```html
<link href="/node_modules/ontotext-visual-theme/build/css/theme.css" rel="stylesheet">
```

This requires the package from the node modules to be accessible/exposed by the web server or better have a script which moves the 
sources in the public directory of your server and link from there.

### Import styles in components

In some `homepage.js` component:

```javascript
import 'ontotext-visual-theme/build/css/theme.css';
```

If the web application is bundled by e.g. webpack, the sources could be imported directly in javascript components.
