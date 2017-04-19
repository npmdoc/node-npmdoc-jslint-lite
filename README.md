# npmdoc-jslint-lite

#### api documentation for  [jslint-lite (v2017.4.6)](https://github.com/kaizhu256/node-jslint-lite)  [![npm package](https://img.shields.io/npm/v/npmdoc-jslint-lite.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-jslint-lite) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-jslint-lite.svg)](https://travis-ci.org/npmdoc/node-npmdoc-jslint-lite)

#### this zero-dependency package will provide browser-compatible, classic-versions of jslint and csslint

[![NPM](https://nodei.co/npm/jslint-lite.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/jslint-lite)

- [https://npmdoc.github.io/node-npmdoc-jslint-lite/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-jslint-lite/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-jslint-lite/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-jslint-lite/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-jslint-lite/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-jslint-lite/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "kai zhu"
    },
    "bin": {
        "jslint-lite": "lib.jslint.js"
    },
    "bugs": {
        "url": "https://github.com/kaizhu256/node-jslint-lite/issues"
    },
    "dependencies": {},
    "description": "this zero-dependency package will provide browser-compatible, classic-versions of jslint and csslint",
    "devDependencies": {
        "electron-lite": "github:kaizhu256/node-electron-lite#alpha",
        "utility2": "github:kaizhu256/node-utility2#alpha"
    },
    "directories": {},
    "dist": {
        "shasum": "4e8e60b7aae80083310d73efa1ae23e70f3d9a61",
        "tarball": "https://registry.npmjs.org/jslint-lite/-/jslint-lite-2017.4.6.tgz"
    },
    "engines": {
        "node": ">=4.0"
    },
    "homepage": "https://github.com/kaizhu256/node-jslint-lite",
    "keywords": [
        "browser",
        "csslint",
        "eshint",
        "eslint",
        "jshint",
        "jslint",
        "lint"
    ],
    "license": "MIT",
    "main": "lib.jslint.js",
    "maintainers": [
        {
            "name": "kaizhu"
        }
    ],
    "name": "jslint-lite",
    "nameAlias": "jslint",
    "nameAliasPublish": "es5lint jslint-classic",
    "nameOriginal": "jslint-lite",
    "optionalDependencies": {},
    "os": [
        "darwin",
        "linux"
    ],
    "readmeParse": "1",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/kaizhu256/node-jslint-lite.git"
    },
    "scripts": {
        "build-ci": "utility2 shReadmeTest build_ci.sh",
        "env": "env",
        "heroku-postbuild": "(set -e; npm install \"kaizhu256/node-utility2#alpha\"; utility2 shDeployHeroku)",
        "postinstall": "if [ -f npm_scripts.sh ]; then ./npm_scripts.sh postinstall; fi",
        "start": "(set -e; export PORT=${PORT:-8080}; utility2 start test.js)",
        "test": "(set -e; export PORT=$(utility2 shServerPortRandom); utility2 test test.js)"
    },
    "version": "2017.4.6"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
