# npmtest-json-mask

#### basic test coverage for  [json-mask (v0.3.8)](https://github.com/nemtsov/json-mask#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-json-mask.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-json-mask) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-json-mask.svg)](https://travis-ci.org/npmtest/node-npmtest-json-mask)

#### Tiny language and engine for selecting specific parts of a JS object, hiding the rest.

[![NPM](https://nodei.co/npm/json-mask.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/json-mask)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-json-mask/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-json-mask/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-json-mask/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-json-mask/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-json-mask/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-json-mask/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-json-mask/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-json-mask/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-json-mask/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-json-mask/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-json-mask/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-json-mask/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-json-mask/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-json-mask/build/test-report.html](https://npmtest.github.io/node-npmtest-json-mask/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-json-mask/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-json-mask/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-json-mask/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-json-mask/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-json-mask/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-json-mask/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-json-mask/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-json-mask/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "nemtsov@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/nemtsov/json-mask/issues"
    },
    "dependencies": {},
    "description": "Tiny language and engine for selecting specific parts of a JS object, hiding the rest.",
    "devDependencies": {
        "browserify": "^10.2.6",
        "istanbul": "^0.3.17",
        "mocha": "~1.12.0",
        "standard": "^7.1.0",
        "uglifyjs": "^2.4.10"
    },
    "directories": {},
    "dist": {
        "shasum": "2d66415de14b0e8bc6c1514554a90bfca8356941",
        "tarball": "https://registry.npmjs.org/json-mask/-/json-mask-0.3.8.tgz"
    },
    "gitHead": "cf8457ba617d9ecf749e0a65f38b33f2ce76457a",
    "homepage": "https://github.com/nemtsov/json-mask#readme",
    "keywords": [
        "mask",
        "filter",
        "select",
        "fields",
        "projection",
        "query",
        "json"
    ],
    "license": "MIT",
    "main": "lib/index",
    "maintainers": [
        {
            "name": "nemtsov"
        }
    ],
    "name": "json-mask",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/nemtsov/json-mask.git"
    },
    "scripts": {
        "_build-browser-full": "browserify -s jsonMask -e lib/index.js | sed -e \"s/\\[ *'.*' *\\]/;/\" > build/jsonMask.js",
        "_build-browser-license": "cat build/copyright  | cat - build/jsonMask.js  | tee build/jsonMask.js",
        "_build-browser-min": "cat build/jsonMask.js | uglifyjs --comments > build/jsonMask.min.js",
        "build-browser": "npm run-script _build-browser-full; npm run-script _build-browser-license; npm run-script _build-browser-min",
        "lint": "standard 'lib/**/*.js' 'test/**/*.js'",
        "test": "npm run lint && mocha",
        "test-cov": "istanbul cover _mocha",
        "test-watch": "mocha -w -G -R min"
    },
    "testling": {
        "browsers": [
            "ie/8..latest",
            "firefox/16..latest",
            "firefox/nightly",
            "chrome/22..latest",
            "chrome/canary",
            "opera/12..latest",
            "opera/next",
            "safari/5.1..latest",
            "ipad/6.0..latest",
            "iphone/6.0..latest",
            "android-browser/4.2..latest"
        ],
        "harness": "mocha",
        "files": "test/*.js"
    },
    "version": "0.3.8",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
