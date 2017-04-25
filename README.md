# npmdoc-phantom

#### basic api documentation for  [phantom (v4.0.2)](https://github.com/amir20/phantomjs-node)  [![npm package](https://img.shields.io/npm/v/npmdoc-phantom.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-phantom) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-phantom.svg)](https://travis-ci.org/npmdoc/node-npmdoc-phantom)

#### PhantomJS integration module for NodeJS

[![NPM](https://nodei.co/npm/phantom.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/phantom)

- [https://npmdoc.github.io/node-npmdoc-phantom/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-phantom/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-phantom/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-phantom/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-phantom/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-phantom/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Amir Raminfar"
    },
    "bugs": {
        "url": "https://github.com/amir20/phantomjs-node/issues"
    },
    "contributors": [
        {
            "name": "Amir Raminfar",
            "url": "http://amirraminfar.com/"
        }
    ],
    "dependencies": {
        "phantomjs-prebuilt": "^2.1.4",
        "split": "^1.0.0",
        "winston": "^2.2.0"
    },
    "description": "PhantomJS integration module for NodeJS",
    "devDependencies": {
        "babel-core": "^6.7.7",
        "babel-eslint": "^7.0.0",
        "babel-plugin-transform-flow-strip-types": "^6.14.0",
        "babel-polyfill": "^6.5.0",
        "babel-preset-env": "^1.0.2",
        "babel-preset-es2015": "^6.18.0",
        "del": "^2.2.0",
        "eslint": "^3.8.1",
        "eslint-config-fb-strict": "^19.0.0",
        "eslint-config-fbjs": "^1.1.1",
        "eslint-plugin-flowtype": "^2.20.0",
        "eslint-plugin-react": "^6.4.1",
        "flow-bin": "^0.43.0",
        "gulp": "^3.9.1",
        "gulp-babel": "^6.1.2",
        "gulp-copy": "^1.0.0",
        "gulp-eslint": "^3.0.0",
        "gulp-newer": "^1.3.0",
        "gulp-watch": "^4.3.5",
        "jest": "^19.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "40a82dbbabe7d1b16306ec8420b66b3ca428a56e",
        "tarball": "https://registry.npmjs.org/phantom/-/phantom-4.0.2.tgz"
    },
    "engines": {
        "node": ">=6.9.0"
    },
    "gitHead": "c832a105f4fdaf798c10fa2a9bb86a41237d3b62",
    "homepage": "https://github.com/amir20/phantomjs-node",
    "jest": {
        "roots": [
            "<rootDir>/lib"
        ],
        "collectCoverage": true,
        "coveragePathIgnorePatterns": [
            "node_modules/",
            "jest-modules/"
        ],
        "testEnvironment": "node"
    },
    "keywords": [
        "phantom",
        "phantomjs",
        "driver"
    ],
    "license": "ISC",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "amir20"
        }
    ],
    "name": "phantom",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/amir20/phantomjs-node.git"
    },
    "scripts": {
        "lint": "eslint . && flow check",
        "prepublish": "gulp build",
        "pretest": "gulp build:test",
        "test": "npm run lint && jest"
    },
    "version": "4.0.2",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
