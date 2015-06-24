

# Viewer.js demo with analytics plugin activated

### Description

This is  a temporary demo app that is intended to be run locally. After cloning this repository, install the dependencies below and use Grunt to bundle and serve the app.

### Dev Dependencies

To install the development dependencies, you'll need [node](http://nodejs.org/) and [npm](https://npmjs.org/). Most node installs come with npm pre-packaged.

Once you have npm, you'll need to install grunt-cli:
```
npm install -g grunt-cli
```

Then go to the viewer.js directory and run:
```
npm install
```

That's it! You should be setup with development dependencies and ready to go.


### Grunt

* `grunt test` - runs `jshint` and `qunit` tests against the code
* `grunt doc` - runs `test` and `jsdoc` to generate documentation in `doc/`
* `grunt` (alias for `grunt default`) - runs `test` and `concat` to build the following files:
    - `dist/crocodoc.viewer.js`
    - `dist/crocodoc.viewer.css`
* `grunt build` - runs `default` as well as `cssmin` and `uglify` to build the following compressed files (in addition to the files built in `grunt default`):
    - `dist/crocodoc.viewer.min.js`
    - `dist/crocodoc.viewer.min.css`
* `grunt serve` - runs a static webserver for viewing examples and qunit tests
    - defaults to port 9000
    - examples: `http://localhost:9000/examples`
    - tests: `http://localhost:9000/test`


### Demoing

1. Click "examples"
2. Click the "presentations" demo
3. Right Click, "Inspect Element", access the browser Console
4. Toggle between pages of the document to restart the timer 
