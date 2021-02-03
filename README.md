This repo documents a behavior difference between Browserify and Webpack in the handling of the `browser` field in `package.json`. I consider it to be a bug in Browserify. This bug was first reported here: https://github.com/defunctzombie/package-browser-field-spec/issues/13.

## Demo

```sh
$ npm ci
$ npm run test-browserify
foo_bar.js
$ npm run test-webpack
node_modules/foo/bar.js
```
