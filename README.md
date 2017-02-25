## Roboto Condensed Font v13

This package contains regular *Roboto Condensed* font [style](https://github.com/ox2/css-font-roboto-condensed#bundled-font-styles) that is converted to base64-encoded data URI strings and embedded into a css file.

### Installation
Install using [npm](http://npmjs.com):
```
npm install @ox2/css-font-roboto-condensed --save
```
Install using [yarn](http://yarnpkg.com):
```
yarn add @ox2/css-font-roboto-condensed
```
### Why
This is useful for prototyping as you can start using the font quickly by importing single css file to your project/playground and it does not require internet connection to use it once the package has been installed. Depending on your setup and use case this could be used in a production app as well, for example you could merge it with your current style sheet and included in Cordova app bundle for a more consistent font loading experience.

### Usage
You can use it in a webpack project by importing it `import '@ox2/css-font-roboto-condensed'` in your top level js file like `index.js` or in a `.storybook/config.js` if your using [React Storybook](https://github.com/storybooks/react-storybook).

### Bundled font styles
- Regular 300
- Regular 400

### Bundled font language subsets
- Latin

### Font update instructions
Note: There may only be a need to update it when there is a new **font** version released by Google Fonts.

Current font version: **v13**

1. Download remote css file from Google fonts, output: `downloads/index.css`:
```
npm run download
```

2. Convert font data into base64-encoded data URI strings, output: `src/index.css`:
```
npm run convert
```

3. Build and publish the package, output: `build/`
```
npm run build
cd build && npm publish
```
**TIP**: You can check if theres a new font version by running the `download` script and inspecting font urls `...gstatic.com/s/robotocondensed/v13/Zd2E9a...` in the output file or just opening the google font link in your browser and inspecting urls there.


### Build your own package
You can easily build your own package with other font family/styles variations by changing `FONT_URL` variable in `scripts/download.sh` to your custom one from https://fonts.google.com/ and then following the steps in **Update Instructions** section.

### Font License
Apache License, version 2.0

More info: https://www.google.com/fonts/specimen/Roboto

Repository: https://github.com/google/roboto

### Package License
MIT
