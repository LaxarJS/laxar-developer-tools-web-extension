# laxar-developer-tools-web-extension

The laxar-developer-tools-web-extension is a browser extension which helps to develop LaxarJS applications.
It adds an additional tab to the developer tools that displays application events, helps visualizing the structure of the current page, and allows to browse log messages of the running LaxarJS application.


## Develop
const CONTENT_PATH = 'laxar-developer-tools-content/index.html';
To use the developer version of the laxar-developer-tools-content modify the `CONTENT_PATH` in the file `createPanel.js` from `'laxar-developer-tools-content/index.html'` to `'laxar-developer-tools-content/debug.html'` and follow the instruction in the
[README](https://github.com/LaxarJS/laxar-developer-tools-content) of the widget.

Hint: Open developer console with `F12`, undock the console and then open the developer console for the extension with `Strg+Shift+J`


## Create Extension Package

Install node modules for the content application and create dist version of the content application:
```
cd src/laxar-developer-tools-content
npm install
npm run optimize
cd ../../
```

Create dist version of extension:
```
grunt dist
```
