# npmdoc-budo

#### api documentation for  [budo (v9.4.7)](https://github.com/mattdesl/budo)  [![npm package](https://img.shields.io/npm/v/npmdoc-budo.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-budo) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-budo.svg)](https://travis-ci.org/npmdoc/node-npmdoc-budo)

#### a browserify server for rapid prototyping

[![NPM](https://nodei.co/npm/budo.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/budo)

- [https://npmdoc.github.io/node-npmdoc-budo/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-budo/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-budo/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-budo/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-budo/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-budo/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Matt DesLauriers",
        "url": "https://github.com/mattdesl"
    },
    "bin": {
        "budo": "./bin/cmd.js"
    },
    "bugs": {
        "url": "https://github.com/mattdesl/budo/issues"
    },
    "dependencies": {
        "bole": "^2.0.0",
        "browserify": "^13.0.1",
        "chokidar": "^1.0.1",
        "connect-pushstate": "^1.0.0",
        "escape-html": "^1.0.3",
        "events": "^1.0.2",
        "garnish": "^5.0.0",
        "get-ports": "^1.0.2",
        "http-proxy": "^1.14.0",
        "inject-lr-script": "^2.0.0",
        "internal-ip": "^1.0.1",
        "micromatch": "^2.2.0",
        "minimist": "^1.1.0",
        "on-finished": "^2.3.0",
        "on-headers": "^1.0.1",
        "once": "^1.3.2",
        "opn": "^3.0.2",
        "pem": "^1.8.3",
        "resolve": "^1.1.6",
        "resp-modifier": "^6.0.0",
        "serve-static": "^1.10.0",
        "simple-html-index": "^1.4.0",
        "stacked": "^1.1.1",
        "stdout-stream": "^1.4.0",
        "strip-ansi": "^3.0.0",
        "term-color": "^1.0.1",
        "tiny-lr": "^0.2.0",
        "url-trim": "^1.0.0",
        "watchify-middleware": "^1.6.0",
        "xtend": "^4.0.0"
    },
    "description": "a browserify server for rapid prototyping",
    "devDependencies": {
        "2d-context": "^1.2.0",
        "babel-preset-es2015": "^6.18.0",
        "babelify": "^7.3.0",
        "brfs": "^1.4.0",
        "canvas-loop": "^1.0.4",
        "getuservideo": "^0.1.3",
        "ndjson": "^1.4.1",
        "request": "^2.53.0",
        "standard": "^8.6.0",
        "tap-spec": "^4.1.0",
        "tape": "^4.0.0",
        "through2": "^2.0.0",
        "tree-kill": "^1.0.0",
        "win-spawn": "^2.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "a6cdcf2572c22ed1331ae91f34a07f265b3dd20b",
        "tarball": "https://registry.npmjs.org/budo/-/budo-9.4.7.tgz"
    },
    "gitHead": "fdf5d0e6dba28a73d9e95b6d71361bf44f24aa27",
    "homepage": "https://github.com/mattdesl/budo",
    "keywords": [
        "browserify",
        "watchify",
        "browser",
        "dev",
        "development",
        "server",
        "beefy",
        "wzrd",
        "local",
        "locally",
        "localhost",
        "watch",
        "live",
        "reload",
        "livereload",
        "lr"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "mattdesl"
        },
        {
            "name": "yoshuawuyts"
        }
    ],
    "name": "budo",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/mattdesl/budo.git"
    },
    "scripts": {
        "pushstate": "node bin/cmd.js example/app.js:bundle.js -v --dir example --live --pushstate -- -t [ babelify --presets [ es2015 ] ]",
        "start": "node bin/cmd.js example/app.js:bundle.js --live -v --dir example -- -t [ babelify --presets [ es2015 ] ]",
        "test": "standard && tape test/test*.js | tap-spec"
    },
    "version": "9.4.7"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
