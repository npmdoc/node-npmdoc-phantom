# api documentation for  [phantom (v4.0.1)](https://github.com/amir20/phantomjs-node)  [![npm package](https://img.shields.io/npm/v/npmdoc-phantom.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-phantom) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-phantom.svg)](https://travis-ci.org/npmdoc/node-npmdoc-phantom)
#### PhantomJS integration module for NodeJS

[![NPM](https://nodei.co/npm/phantom.png?downloads=true)](https://www.npmjs.com/package/phantom)

[![apidoc](https://npmdoc.github.io/node-npmdoc-phantom/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-phantom_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-phantom/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-phantom/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-phantom/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Amir Raminfar",
        "email": "findamir@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/amir20/phantomjs-node/issues"
    },
    "contributors": [
        {
            "name": "Amir Raminfar",
            "email": "findamir@gmail.com",
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
        "flow-bin": "^0.39.0",
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
        "shasum": "2c7bb95e32e4a774250d95d711a33396ad9b1d90",
        "tarball": "https://registry.npmjs.org/phantom/-/phantom-4.0.1.tgz"
    },
    "engines": {
        "node": ">=6.9.0"
    },
    "gitHead": "20cc92dc83a40ed39548de62f71a3fb68df87175",
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
            "name": "amir20",
            "email": "findamir@gmail.com"
        }
    ],
    "name": "phantom",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
    "version": "4.0.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module phantom](#apidoc.module.phantom)
1.  [function <span class="apidocSignatureSpan">phantom.</span>create (args, config)](#apidoc.element.phantom.create)
1.  object <span class="apidocSignatureSpan"></span>phantom
1.  object <span class="apidocSignatureSpan">phantom.</span>command
1.  object <span class="apidocSignatureSpan">phantom.</span>default
1.  object <span class="apidocSignatureSpan">phantom.</span>out_object
1.  object <span class="apidocSignatureSpan">phantom.</span>page

#### [module phantom.command](#apidoc.module.phantom.command)
1.  [function <span class="apidocSignatureSpan">phantom.command.</span>default (target, name, params = [])](#apidoc.element.phantom.command.default)

#### [module phantom.default](#apidoc.module.phantom.default)
1.  [function <span class="apidocSignatureSpan">phantom.default.</span>create (args, config)](#apidoc.element.phantom.default.create)

#### [module phantom.out_object](#apidoc.module.phantom.out_object)
1.  [function <span class="apidocSignatureSpan">phantom.out_object.</span>default (phantom)](#apidoc.element.phantom.out_object.default)

#### [module phantom.page](#apidoc.module.phantom.page)
1.  [function <span class="apidocSignatureSpan">phantom.page.</span>default (phantom, pageId)](#apidoc.element.phantom.page.default)

#### [module phantom.phantom](#apidoc.module.phantom.phantom)
1.  [function <span class="apidocSignatureSpan">phantom.phantom.</span>default (if unset or default)](#apidoc.element.phantom.phantom.default)



# <a name="apidoc.module.phantom"></a>[module phantom](#apidoc.module.phantom)

#### <a name="apidoc.element.phantom.create"></a>[function <span class="apidocSignatureSpan">phantom.</span>create (args, config)](#apidoc.element.phantom.create)
- description and source-code
```javascript
function create(args, config) {
  return new Promise(resolve => resolve(new _phantom2.default(args, config)));
}
```
- example usage
```shell
...


## Super easy to use
'''js
const phantom = require('phantom');

(async function() {
const instance = await phantom.create();
const page = await instance.createPage();
await page.on("onResourceRequested", function(requestData) {
    console.info('Requesting', requestData.url)
});

const status = await page.open('https://stackoverflow.com/');
console.log(status);
...
```



# <a name="apidoc.module.phantom.command"></a>[module phantom.command](#apidoc.module.phantom.command)

#### <a name="apidoc.element.phantom.command.default"></a>[function <span class="apidocSignatureSpan">phantom.command.</span>default (target, name, params = [])](#apidoc.element.phantom.command.default)
- description and source-code
```javascript
class Command {

    constructor(target, name, params = []) {
        this.id = NEXT_ID++;
        this.target = target;
        this.name = name;
        this.params = params;
        this.deferred = null;
    }
}
```
- example usage
```shell
...
/**
 * Returns a new instance of Promise which resolves to a {@link Page}.
 * @returns {Promise.<Page>}
 */
createPage() {
    const logger = this.logger;
    return this.execute('phantom', 'createPage').then(response => {
        let page = new _page2.default(this, response.pageId);
        if (typeof Proxy === 'function') {
            page = new Proxy(page, {
                set: function (target, prop) {
                    logger.warn('Using page.${prop} = ...; is not supported. Use page.property('${prop}', ...) ' + 'instead. See
 the README file for more examples of page#property.');
                    return false;
                }
            });
...
```



# <a name="apidoc.module.phantom.default"></a>[module phantom.default](#apidoc.module.phantom.default)

#### <a name="apidoc.element.phantom.default.create"></a>[function <span class="apidocSignatureSpan">phantom.default.</span>create (args, config)](#apidoc.element.phantom.default.create)
- description and source-code
```javascript
function create(args, config) {
  return new Promise(resolve => resolve(new _phantom2.default(args, config)));
}
```
- example usage
```shell
...


## Super easy to use
'''js
const phantom = require('phantom');

(async function() {
const instance = await phantom.create();
const page = await instance.createPage();
await page.on("onResourceRequested", function(requestData) {
    console.info('Requesting', requestData.url)
});

const status = await page.open('https://stackoverflow.com/');
console.log(status);
...
```



# <a name="apidoc.module.phantom.out_object"></a>[module phantom.out_object](#apidoc.module.phantom.out_object)

#### <a name="apidoc.element.phantom.out_object.default"></a>[function <span class="apidocSignatureSpan">phantom.out_object.</span>default (phantom)](#apidoc.element.phantom.out_object.default)
- description and source-code
```javascript
class OutObject {

    constructor(phantom) {
        this._phantom = phantom;
        this.target = 'OutObject$' + _crypto2.default.randomBytes(16).toString('hex');
    }

    property(name) {
        return this._phantom.execute(this.target, 'property', [name]);
    }
}
```
- example usage
```shell
...
/**
 * Returns a new instance of Promise which resolves to a {@link Page}.
 * @returns {Promise.<Page>}
 */
createPage() {
    const logger = this.logger;
    return this.execute('phantom', 'createPage').then(response => {
        let page = new _page2.default(this, response.pageId);
        if (typeof Proxy === 'function') {
            page = new Proxy(page, {
                set: function (target, prop) {
                    logger.warn('Using page.${prop} = ...; is not supported. Use page.property('${prop}', ...) ' + 'instead. See
 the README file for more examples of page#property.');
                    return false;
                }
            });
...
```



# <a name="apidoc.module.phantom.page"></a>[module phantom.page](#apidoc.module.phantom.page)

#### <a name="apidoc.element.phantom.page.default"></a>[function <span class="apidocSignatureSpan">phantom.page.</span>default (phantom, pageId)](#apidoc.element.phantom.page.default)
- description and source-code
```javascript
class Page {

    constructor(phantom, pageId) {
        this.target = 'page$' + pageId;
        this.phantom = phantom;
    }

<span class="apidocCodeCommentSpan">    /**
     * Add an event listener to the page on phantom
     *
     * @param event The name of the event (Ej. onResourceLoaded)
     * @param [runOnPhantom=false] Indicate if the event must run on the phantom runtime or not
     * @param listener The event listener. When runOnPhantom=true, this listener code would be run on phantom, and thus,
     * all the closure info wont work
     * @returns {*}
     */
</span>    on(event, runOnPhantom, listener) {
        let mustRunOnPhantom;
        let callback;
        let args;

        if (typeof runOnPhantom === 'function') {
            args = [].slice.call(arguments, 2);
            mustRunOnPhantom = false;
            callback = runOnPhantom.bind(this);
        } else {
            args = [].slice.call(arguments, 3);
            mustRunOnPhantom = runOnPhantom;
            callback = mustRunOnPhantom ? listener : listener.bind(this);
        }

        return this.phantom.on(event, this.target, mustRunOnPhantom, callback, args);
    }

    /**
     * Removes an event listener
     *
     * @param event the event name
     * @returns {*}
     */
    off(event) {
        return this.phantom.off(event, this.target);
    }

    /**
     * Invokes an asynchronous method
     */
    invokeAsyncMethod() {
        return this.phantom.execute(this.target, 'invokeAsyncMethod', [].slice.call(arguments));
    }

    /**
     * Invokes a method
     */
    invokeMethod() {
        return this.phantom.execute(this.target, 'invokeMethod', [].slice.call(arguments));
    }

    /**
     * Defines a method
     */
    defineMethod(name, definition) {
        return this.phantom.execute(this.target, 'defineMethod', [name, definition]);
    }

    /**
     * Gets or sets a property
     */
    property() {
        return this.phantom.execute(this.target, 'property', [].slice.call(arguments));
    }

    /**
     * Gets or sets a setting
     */
    setting() {
        return this.phantom.execute(this.target, 'setting', [].slice.call(arguments));
    }
}
```
- example usage
```shell
...
/**
 * Returns a new instance of Promise which resolves to a {@link Page}.
 * @returns {Promise.<Page>}
 */
createPage() {
    const logger = this.logger;
    return this.execute('phantom', 'createPage').then(response => {
        let page = new _page2.default(this, response.pageId);
        if (typeof Proxy === 'function') {
            page = new Proxy(page, {
                set: function (target, prop) {
                    logger.warn('Using page.${prop} = ...; is not supported. Use page.property('${prop}', ...) ' + 'instead. See
 the README file for more examples of page#property.');
                    return false;
                }
            });
...
```



# <a name="apidoc.module.phantom.phantom"></a>[module phantom.phantom](#apidoc.module.phantom.phantom)

#### <a name="apidoc.element.phantom.phantom.default"></a>[function <span class="apidocSignatureSpan">phantom.phantom.</span>default (if unset or default)](#apidoc.element.phantom.phantom.default)
- description and source-code
```javascript
class Phantom {

<span class="apidocCodeCommentSpan">    /**
     * Creates a new instance of Phantom
     *
     * @param args command args to pass to phantom process
     * @param [phantomPath] path to phantomjs executable
     * @param [logger] object containing functions used for logging
     * @param [logLevel] log level to apply on the logger (if unset or default)
     */
</span>    constructor(args = [], { phantomPath = _phantomjsPrebuilt2.default.path, logger = defaultLogger, logLevel = defaultLogLevel } = {
        phantomPath: _phantomjsPrebuilt2.default.path,
        logger: defaultLogger,
        logLevel: defaultLogLevel
    }) {
        if (!Array.isArray(args)) {
            throw new Error('Unexpected type of parameters. Expecting args to be array.');
        }

        if (typeof phantomPath !== 'string') {
            throw new Error('PhantomJS binary was not found. ' + 'This generally means something went wrong when installing phantomjs
-prebuilt. Exiting.');
        }

        if (typeof logger !== 'object') {
            throw new Error('logger must be ba valid object.');
        }

        logger.debug = logger.debug || (() => undefined);
        logger.info = logger.info || (() => undefined);
        logger.warn = logger.warn || (() => undefined);
        logger.error = logger.error || (() => undefined);

        this.logger = logger;

        if (logLevel !== defaultLogLevel) {
            this.logger = createLogger();
            this.logger.transports.console.level = logLevel;
        }

        const pathToShim = _path2.default.normalize(__dirname + '/shim/index.js');
        this.logger.debug('Starting ${phantomPath} ${args.concat([pathToShim]).join(' ')}');

        this.process = (0, _child_process.spawn)(phantomPath, args.concat([pathToShim]), { env: process.env });
        this.process.stdin.setDefaultEncoding('utf-8');

        this.commands = new Map();
        this.events = new Map();

        this.process.stdout.pipe((0, _split2.default)()).on('data', data => {
            const message = data.toString('utf8');
            if (message[0] === '>') {
                // Server end has finished NOOP, lets allow NOOP again..
                if (message === '>' + NOOP) {
                    this.logger.debug('Received NOOP command.');
                    this.isNoOpInProgress = false;
                    return;
                }
                const json = message.substr(1);
                this.logger.debug('Parsing: %s', json);

                const parsedJson = JSON.parse(json);
                const command = this.commands.get(parsedJson.id);

                if (command != null) {
                    const deferred = command.deferred;

                    if (deferred != null) {
                        if (parsedJson.error === undefined) {
                            deferred.resolve(parsedJson.response);
                        } else {
                            deferred.reject(new Error(parsedJson.error));
                        }
                    } else {
                        this.logger.error('deferred object not found for command.id: ' + parsedJson.id);
                    }

                    this.commands.delete(command.id);
                } else {
                    this.logger.error('command not found for command.id: ' + parsedJson.id);
                }
            } else if (message.indexOf('<event>') === 0) {
                const json = message.substr(7);
                this.logger.debug('Parsing: %s', json);
                const event = JSON.parse(json);

                const emitter = this.events.get(event.target);
                if (emitter) {
                    emitter.emit.apply(emitter, [event.type].concat(event.args));
                }
            } else if (message && message.length > 0) {
                this.logger.info(message);
            }
        });

        this.process.stderr.on('data', data => this.logger.error(data.toString('utf8')));
        this.process.on('exit', code => {
            this.logger.debug('Child exited with code {${code}}');
            this._rejectAllComman ...
```
- example usage
```shell
...
/**
 * Returns a new instance of Promise which resolves to a {@link Page}.
 * @returns {Promise.<Page>}
 */
createPage() {
    const logger = this.logger;
    return this.execute('phantom', 'createPage').then(response => {
        let page = new _page2.default(this, response.pageId);
        if (typeof Proxy === 'function') {
            page = new Proxy(page, {
                set: function (target, prop) {
                    logger.warn('Using page.${prop} = ...; is not supported. Use page.property('${prop}', ...) ' + 'instead. See
 the README file for more examples of page#property.');
                    return false;
                }
            });
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
