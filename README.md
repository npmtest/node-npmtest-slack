# npmtest-slack

#### basic test coverage for  [slack (v8.3.0)](https://github.com/smallwins/slack#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-slack.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-slack) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-slack.svg)](https://travis-ci.org/npmtest/node-npmtest-slack)

#### Slack API client written in JS

[![NPM](https://nodei.co/npm/slack.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/slack)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-slack/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-slack/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-slack/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-slack/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-slack/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-slack/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-slack/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-slack/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-slack/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-slack/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-slack/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-slack/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-slack/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-slack/build/test-report.html](https://npmtest.github.io/node-npmtest-slack/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-slack/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-slack/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-slack/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-slack/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-slack/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-slack/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-slack/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-slack/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Brian LeRoux"
    },
    "browser": {
        "./methods/rtm.client.js": "./methods/rtm.client-browser.js",
        "./test/_env.js": "./test/_env-browser.js"
    },
    "bugs": {
        "url": "https://github.com/smallwins/slack/issues"
    },
    "dependencies": {
        "tiny-json-http": "^5.1.0",
        "ws": "^1.1.4"
    },
    "description": "Slack API client written in JS",
    "devDependencies": {
        "async": "^2.1.2",
        "babel-cli": "^6.3.15",
        "babel-plugin-add-module-exports": "^0.1.1",
        "babel-preset-es2015": "^6.3.13",
        "babelify": "^7.2.0",
        "browser-run": "^4.0.1",
        "browserify": "^14.1.0",
        "chalk": "^1.1.1",
        "cheerio": "^0.22.0",
        "cpr": "^1.1.2",
        "envify": "^3.4.0",
        "glob": "^7.0.5",
        "lodash": "^4.5.0",
        "mustache": "^2.2.1",
        "node-env-file": "^0.1.8",
        "request": "^2.78.0",
        "rimraf": "^2.5.3",
        "tap": "^5.8.0",
        "tap-spec": "^4.1.1",
        "tape": "^4.6.0"
    },
    "directories": {},
    "dist": {
        "shasum": "35614c849d6336686a721b92ffa1b646faed0770",
        "tarball": "https://registry.npmjs.org/slack/-/slack-8.3.0.tgz"
    },
    "gitHead": "d3e8b34aba7af319948e3958dfa78c7e0be7a5d3",
    "homepage": "https://github.com/smallwins/slack#readme",
    "keywords": [
        "slack",
        "api",
        "client"
    ],
    "license": "Apache-2.0",
    "main": "methods/index",
    "maintainers": [
        {
            "name": "brianleroux"
        },
        {
            "name": "dam"
        },
        {
            "name": "matthewmueller"
        },
        {
            "name": "mbrevoort"
        }
    ],
    "name": "slack",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/smallwins/slack.git"
    },
    "scripts": {
        "btest": "npm run build && ./scripts/test-browser | browser-run | tap-spec",
        "build": "rimraf methods && babel src --out-dir methods && cpr src/api.json methods/api.json",
        "generate": "./scripts/generate-all",
        "prepublish": "npm run build",
        "start": "npm run build && ./scripts/repl",
        "t": "npm run build && ./scripts/t",
        "test": "npm run build && ./scripts/test"
    },
    "version": "8.3.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
