# npmdoc-superagent

#### api documentation for  [superagent (v3.5.2)](https://github.com/visionmedia/superagent#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-superagent.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-superagent) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-superagent.svg)](https://travis-ci.org/npmdoc/node-npmdoc-superagent)

#### elegant & feature rich browser / node HTTP with a fluent API

[![NPM](https://nodei.co/npm/superagent.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/superagent)

- [https://npmdoc.github.io/node-npmdoc-superagent/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-superagent/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-superagent/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-superagent/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-superagent/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-superagent/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "TJ Holowaychuk"
    },
    "browser": {
        "./lib/node/index.js": "./lib/client.js",
        "./test/support/server.js": "./test/support/blank.js"
    },
    "bugs": {
        "url": "https://github.com/visionmedia/superagent/issues"
    },
    "component": {
        "scripts": {
            "superagent": "lib/client.js"
        }
    },
    "contributors": [
        {
            "name": "Kornel Lesiński"
        },
        {
            "name": "Peter Lyons"
        },
        {
            "name": "Hunter Loftis"
        }
    ],
    "dependencies": {
        "component-emitter": "^1.2.0",
        "cookiejar": "^2.0.6",
        "debug": "^2.2.0",
        "extend": "^3.0.0",
        "form-data": "^2.1.1",
        "formidable": "^1.1.1",
        "methods": "^1.1.1",
        "mime": "^1.3.4",
        "qs": "^6.1.0",
        "readable-stream": "^2.0.5"
    },
    "description": "elegant & feature rich browser / node HTTP with a fluent API",
    "devDependencies": {
        "Base64": "^1.0.0",
        "basic-auth-connect": "^1.0.0",
        "body-parser": "^1.15.0",
        "browserify": "^14.0.0",
        "cookie-parser": "^1.4.1",
        "express": "^4.13.4",
        "express-session": "^1.13.0",
        "marked": "^0.3.5",
        "mocha": "^3.1.2",
        "multer": "^1.2.0",
        "should": "^11.1.1",
        "should-http": "^0.0.4",
        "zuul": "^3.11.1"
    },
    "directories": {},
    "dist": {
        "shasum": "3361a3971567504c351063abeaae0faa23dbf3f8",
        "tarball": "https://registry.npmjs.org/superagent/-/superagent-3.5.2.tgz"
    },
    "engines": {
        "node": ">= 0.12"
    },
    "gitHead": "ef9af6c85b2b1a0cf5f350bece2f7e33d89b888a",
    "homepage": "https://github.com/visionmedia/superagent#readme",
    "keywords": [
        "http",
        "ajax",
        "request",
        "agent"
    ],
    "license": "MIT",
    "main": "./lib/node/index.js",
    "maintainers": [
        {
            "name": "defunctzombie"
        },
        {
            "name": "kof"
        },
        {
            "name": "kornel"
        },
        {
            "name": "naman34"
        },
        {
            "name": "nw"
        },
        {
            "name": "rauchg"
        },
        {
            "name": "superjoe"
        },
        {
            "name": "tjholowaychuk"
        },
        {
            "name": "travisjeffery"
        },
        {
            "name": "yields"
        }
    ],
    "name": "superagent",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/visionmedia/superagent.git"
    },
    "scripts": {
        "prepublish": "make all",
        "test": "make test"
    },
    "version": "3.5.2"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
