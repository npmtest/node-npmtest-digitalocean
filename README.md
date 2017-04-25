# npmtest-digitalocean

#### basic test coverage for  [digitalocean (v0.9.1)](https://github.com/phillbaker/digitalocean-node#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-digitalocean.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-digitalocean) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-digitalocean.svg)](https://travis-ci.org/npmtest/node-npmtest-digitalocean)

#### nodejs wrapper for digitalocean v2 api

[![NPM](https://nodei.co/npm/digitalocean.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/digitalocean)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-digitalocean/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-digitalocean/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-digitalocean/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-digitalocean/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-digitalocean/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-digitalocean/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-digitalocean/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-digitalocean/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-digitalocean/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-digitalocean/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-digitalocean/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-digitalocean/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-digitalocean/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-digitalocean/build/test-report.html](https://npmtest.github.io/node-npmtest-digitalocean/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-digitalocean/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-digitalocean/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-digitalocean/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-digitalocean/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-digitalocean/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-digitalocean/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-digitalocean/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-digitalocean/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Phillip Baker"
    },
    "bugs": {
        "url": "https://github.com/phillbaker/digitalocean-node/issues"
    },
    "dependencies": {
        "bluebird": "^3.0",
        "deep-extend": "0.x.x",
        "request": "^2.50"
    },
    "description": "nodejs wrapper for digitalocean v2 api",
    "devDependencies": {
        "bower": ">= 0.0.0",
        "browserify": "^13.0.0",
        "chai": "~1.10.0",
        "chai-shallow-deep-equal": "^1.4.0",
        "jsdoc": "3.4.0",
        "mocha": "~2.1.0",
        "mocha-jshint": "^2.3.1",
        "nock": "0.57.x"
    },
    "directories": {},
    "dist": {
        "shasum": "aec145c104fa91f76ad8fab115f609fd4340b2b6",
        "tarball": "https://registry.npmjs.org/digitalocean/-/digitalocean-0.9.1.tgz"
    },
    "engines": {
        "node": ">0.4.11",
        "npm": ">= 2.13.1"
    },
    "gitHead": "b34f83df3ff54b664fc7cad62ff2a871c8969306",
    "homepage": "https://github.com/phillbaker/digitalocean-node#readme",
    "keywords": [
        "wrapper",
        "api",
        "v2",
        "digital ocean",
        "digitalocean",
        "droplet"
    ],
    "license": "MIT",
    "main": "./lib/digitalocean",
    "maintainers": [
        {
            "name": "phillbaker"
        }
    ],
    "name": "digitalocean",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/phillbaker/digitalocean-node.git"
    },
    "scripts": {
        "build": "mkdir -p dist && npm run build:js && npm run doc",
        "build:js": "browserify lib/digitalocean.js -o dist/digitalocean.js --standalone 'digitalocean'",
        "clean": "rm -r dist/*",
        "doc": "jsdoc lib/ --configure jsdoc.conf.json",
        "preversion": "npm test",
        "release": "git push --follow-tags && npm publish",
        "release:major": "npm version major -m 'Bump version to %s'",
        "release:minor": "npm version minor -m 'Bump version to %s'",
        "release:patch": "npm version patch -m 'Bump version to %s'",
        "test": "mocha --bail --recursive --reporter dot",
        "version": "npm run build && git add -A dist"
    },
    "tonicExampleFilename": "examples/make_droplet.js",
    "version": "0.9.1",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
