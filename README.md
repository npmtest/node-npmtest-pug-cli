# npmtest-pug-cli

#### basic test coverage for  pug-cli (v1.0.0-alpha6)  [![npm package](https://img.shields.io/npm/v/npmtest-pug-cli.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-pug-cli) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-pug-cli.svg)](https://travis-ci.org/npmtest/node-npmtest-pug-cli)

#### Pug's CLI interface

[![NPM](https://nodei.co/npm/pug-cli.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/pug-cli)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-pug-cli/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-pug-cli/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-pug-cli/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-pug-cli/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-pug-cli/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-pug-cli/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-pug-cli/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-pug-cli/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-pug-cli/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-pug-cli/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-pug-cli/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-pug-cli/build/test-report.html](https://npmtest.github.io/node-npmtest-pug-cli/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-pug-cli/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-pug-cli/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-pug-cli/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-pug-cli/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-pug-cli/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-pug-cli/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-pug-cli/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-pug-cli/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "pug-cli",
    "version": "1.0.0-alpha6",
    "description": "Pug's CLI interface",
    "bin": {
        "pug": "./index.js"
    },
    "preferGlobal": true,
    "keywords": [],
    "dependencies": {
        "chalk": "^1.0.0",
        "commander": "^2.8.1",
        "pug": "^2.0.0-alpha7",
        "mkdirp": "^0.5.1"
    },
    "devDependencies": {
        "istanbul": "*",
        "mocha": "*",
        "rimraf": "^2.3.4"
    },
    "scripts": {
        "test": "mocha -R spec --bail",
        "precoverage": "rimraf coverage && rimraf cov-pt*",
        "coverage": "istanbul cover --report none --dir cov-pt0 node_modules/mocha/bin/_mocha -- -R dot",
        "postcoverage": "istanbul report --include cov-pt\\*/coverage.json && rimraf cov-pt*"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/pugjs/pug-cli.git"
    },
    "author": "TJ Holowaychuk <tj@vision-media.ca>",
    "maintainers": [
        "Timothy Gu <timothygu99@gmail.com>",
        "Forbes Lindesay <forbes@lindesay.co.uk>"
    ],
    "license": "MIT"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
