# npmdoc-engine.io

#### api documentation for  [engine.io (v3.0.0)](https://github.com/socketio/engine.io)  [![npm package](https://img.shields.io/npm/v/npmdoc-engine.io.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-engine.io) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-engine.io.svg)](https://travis-ci.org/npmdoc/node-npmdoc-engine.io)

#### The realtime engine behind Socket.IO. Provides the foundation of a bidirectional connection between client and server

[![NPM](https://nodei.co/npm/engine.io.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/engine.io)

- [https://npmdoc.github.io/node-npmdoc-engine.io/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-engine.io/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-engine.io/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-engine.io/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-engine.io/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-engine.io/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Guillermo Rauch"
    },
    "bugs": {
        "url": "https://github.com/socketio/engine.io/issues"
    },
    "contributors": [
        {
            "name": "Eugen Dueck",
            "url": "https://github.com/EugenDueck"
        },
        {
            "name": "Afshin Mehrabani",
            "url": "https://github.com/afshinm"
        },
        {
            "name": "Christoph Dorn",
            "url": "https://github.com/cadorn"
        },
        {
            "name": "Mark Mokryn"
        }
    ],
    "dependencies": {
        "accepts": "1.3.3",
        "base64id": "1.0.0",
        "cookie": "0.3.1",
        "debug": "2.3.3",
        "engine.io-parser": "2.0.3",
        "uws": "0.14.1",
        "ws": "2.2.3"
    },
    "description": "The realtime engine behind Socket.IO. Provides the foundation of a bidirectional connection between client and server",
    "devDependencies": {
        "babel-eslint": "5.0.0",
        "babel-preset-es2015": "^6.24.0",
        "engine.io-client": "3.0.0",
        "eslint-config-standard": "4.4.0",
        "eslint-plugin-standard": "1.3.2",
        "expect.js": "^0.3.1",
        "gulp": "^3.9.1",
        "gulp-babel": "^6.1.2",
        "gulp-eslint": "1.1.1",
        "gulp-mocha": "^4.3.0",
        "gulp-nsp": "^2.4.1",
        "mocha": "^3.2.0",
        "s": "0.1.1",
        "superagent": "0.15.4"
    },
    "directories": {},
    "dist": {
        "shasum": "fde0f460686f09e295bc55933663c1cf37759933",
        "tarball": "https://registry.npmjs.org/engine.io/-/engine.io-3.0.0.tgz"
    },
    "files": [
        "index.js",
        "lib/"
    ],
    "gitHead": "07d57d553f1da9c04a4c903d971346b339df2404",
    "homepage": "https://github.com/socketio/engine.io",
    "license": "MIT",
    "main": "./lib/engine.io",
    "maintainers": [
        {
            "name": "darrachequesne"
        },
        {
            "name": "rauchg"
        }
    ],
    "name": "engine.io",
    "optionalDependencies": {
        "uws": "0.14.1"
    },
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/socketio/engine.io.git"
    },
    "scripts": {
        "test": "gulp test; EIO_WS_ENGINE=ws gulp test;"
    },
    "version": "3.0.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
