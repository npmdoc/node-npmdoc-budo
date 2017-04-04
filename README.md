# api documentation for  [budo (v9.4.7)](https://github.com/mattdesl/budo)  [![npm package](https://img.shields.io/npm/v/npmdoc-budo.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-budo) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-budo.svg)](https://travis-ci.org/npmdoc/node-npmdoc-budo)
#### a browserify server for rapid prototyping

[![NPM](https://nodei.co/npm/budo.png?downloads=true)](https://www.npmjs.com/package/budo)

[![apidoc](https://npmdoc.github.io/node-npmdoc-budo/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-budo_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-budo/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-budo/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-budo/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Matt DesLauriers",
        "email": "dave.des@gmail.com",
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
            "name": "mattdesl",
            "email": "dave.des@gmail.com"
        },
        {
            "name": "yoshuawuyts",
            "email": "i@yoshuawuyts.com"
        }
    ],
    "name": "budo",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module budo](#apidoc.module.budo)
1.  [function <span class="apidocSignatureSpan">budo.</span>cli (args, opts)](#apidoc.element.budo.cli)
1.  [function <span class="apidocSignatureSpan">budo.</span>error_handler (err, cwd, rootDirName)](#apidoc.element.budo.error_handler)

#### [module budo.error_handler](#apidoc.module.budo.error_handler)
1.  [function <span class="apidocSignatureSpan">budo.</span>error_handler (err, cwd, rootDirName)](#apidoc.element.budo.error_handler.error_handler)
1.  [function <span class="apidocSignatureSpan">budo.error_handler.</span>render (message, cwd, rootDirName)](#apidoc.element.budo.error_handler.render)



# <a name="apidoc.module.budo"></a>[module budo](#apidoc.module.budo)

#### <a name="apidoc.element.budo.cli"></a>[function <span class="apidocSignatureSpan">budo.</span>cli (args, opts)](#apidoc.element.budo.cli)
- description and source-code
```javascript
function budoCLI(args, opts) {
  var argv = parseArgs(args, opts)

  // if no stream is specified, default to stdout
  if (argv.stream !== false) {
    argv.stream = /^win/.test(process.platform) ? process.stdout : stdoutStream
  }

  var entries = argv._
  delete argv._

  argv.browserifyArgs = argv['--']
  delete argv['--']

  if (argv.version) {
    console.log('budo v' + require('./package.json').version)
    console.log('browserify v' + require('browserify/package.json').version)
    console.log('watchify v' + require('watchify-middleware').getWatchifyVersion())
    return null
  }

  if (argv.help) {
    var help = require('path').join(__dirname, 'bin', 'help.txt')
    require('fs').createReadStream(help)
      .pipe(process.stdout)
    return null
  }

  if (argv.outfile) {
    console.error(color.yellow('WARNING'), '--outfile has been removed in budo@3.0')
  }

  if (typeof argv.port === 'string') {
    argv.port = parseInt(argv.port, 10)
  }
  if (typeof argv.livePort === 'string') {
    argv.livePort = parseInt(argv.livePort, 10)
  }

  // opts.live can be a glob or a boolean
  if (typeof argv.live === 'string' && /(true|false)/.test(argv.live)) {
    argv.live = argv.live === 'true'
  }

  // CLI only option for executing a child process
  var instance = budo(entries, argv).on('error', exit)
  var onUpdates = [].concat(argv.onupdate).filter(Boolean)
  onUpdates.forEach(function (cmd) {
    instance.on('update', execFunc(cmd))
  })

  return instance
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.budo.error_handler"></a>[function <span class="apidocSignatureSpan">budo.</span>error_handler (err, cwd, rootDirName)](#apidoc.element.budo.error_handler)
- description and source-code
```javascript
function errorHandler(err, cwd, rootDirName) {
  console.error('%s', err)
  var msgStr = stripAnsi(err.message)
  var params = [
    JSON.stringify(msgStr),
    JSON.stringify(cwd),
    JSON.stringify(rootDirName)
  ].join(',')
  return ';(' + bundleError + ')(' + params + ');'
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.budo.error_handler"></a>[module budo.error_handler](#apidoc.module.budo.error_handler)

#### <a name="apidoc.element.budo.error_handler.error_handler"></a>[function <span class="apidocSignatureSpan">budo.</span>error_handler (err, cwd, rootDirName)](#apidoc.element.budo.error_handler.error_handler)
- description and source-code
```javascript
function errorHandler(err, cwd, rootDirName) {
  console.error('%s', err)
  var msgStr = stripAnsi(err.message)
  var params = [
    JSON.stringify(msgStr),
    JSON.stringify(cwd),
    JSON.stringify(rootDirName)
  ].join(',')
  return ';(' + bundleError + ')(' + params + ');'
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.budo.error_handler.render"></a>[function <span class="apidocSignatureSpan">budo.error_handler.</span>render (message, cwd, rootDirName)](#apidoc.element.budo.error_handler.render)
- description and source-code
```javascript
function bundleError(message, cwd, rootDirName) {
  // Everything has to be contained inside this function
  // for it to get stringified correctly. i.e. no require()!
  console.error(message)

  if (typeof document === 'undefined') {
    return
  } else if (!document.body) {
    document.addEventListener('DOMContentLoaded', createErrorBox)
  } else {
    createErrorBox()
  }

  function createErrorBox () {
    var parsed = parseError(message)

    var overlayBox = document.createElement('div')
    css(overlayBox, {
      position: 'fixed',
      width: '100%',
      height: '100%',
      zIndex: '100000000',
      top: '0',
      left: '0',
      padding: '20px',
      margin: '0px',
      'box-sizing': 'border-box',
      background: '#fff',
      display: 'block',
      'font-size': '14px',
      'font-weight': 'normal',
      'font-family': 'monospace'
    })

    if (!parsed.format) {
      var pre = document.createElement('pre')
      pre.textContent = message
      css(pre, {
        'word-wrap': 'break-word',
        'white-space': 'pre-wrap',
        'box-sizing': 'border-box',
        margin: '0',
        color: '#ff0000'
      })
      overlayBox.appendChild(pre)
    } else {
      var commonElements = []

      var messageDiv = document.createElement('div')
      commonElements.push(messageDiv)
      messageDiv.textContent = parsed.message
      overlayBox.appendChild(messageDiv)
      css(messageDiv, {
        color: '#ff2e2e',
        'font-size': '16px'
      })

      var pathLocContainer = document.createElement('div')
      css(pathLocContainer, { 'padding-top': '10px' })

      if (isFinite(parsed.line)) {
        var location = document.createElement('div')
        commonElements.push(location)
        var colStr = isFinite(parsed.column) ? (', column ' + parsed.column) : ''
        location.textContent = ('line ' + parsed.line + colStr).trim()
        css(location, {
          color: 'hsl(0, 0%, 50%)',
          'padding-bottom': '0px',
          'font-size': '12px',
          'font-weight': 'bold'
        })
        pathLocContainer.appendChild(location)
      }

      var path = document.createElement('div')
      path.textContent = trimPath(parsed.path)
      commonElements.push(path)
      css(path, { 'font-style': 'italic' })
      pathLocContainer.appendChild(path)
      overlayBox.appendChild(pathLocContainer)

      if (parsed.code) {
        var sourceContainer = document.createElement('div')
        var source = document.createElement('div')
        var hr = document.createElement('div')
        css(hr, {
          background: 'hsl(0, 0%, 90%)',
          width: '100%',
          height: '2px',
          padding: '0',
          'margin-bottom': '10px',
          'margin-top': '10px'
        })
        commonElements.push(source)
        source.textContent = parsed.code
        css(source, {
          color: 'black',
          'font-weight': 'bold',
          'font-size': '14px',
          'padding-left': '0px'
        })

        sourceContainer.appendChild(hr)
        sourceContainer.appendChild(source)
        overlayBox.appendChild(sourceContainer)
      }

      // apply common styles
      commonElements.forEach(function (e) {
        css(e, {
          'word-wrap': 'break-word',
          'white-space': 'pre-wrap',
          'box-sizing': 'border-box',
          display: 'block',
          margin: '0',
          'vertical-align': 'bottom'
        })
      })
    }
    document.body.appendChild(overlayBox)
  }

  function trimPath (filePath) {
    if (filePath.indexOf(cwd) === 0) {
      filePath = rootDirName + filePath.substring(cwd.length + 1)
    }
    return filePath
  }

  function css (element, style) {
    Object.keys(style).forEach(function (k) {
      element.style[k] = style[k]
    })
  }

  // parse an error message into pieces
  function parseError (err) {
    var filePath, lineNum, splitLines
    var result = {}

    // For root files that syntax-error doesn't pick up:
    var parseFilePrefix = 'Parsing file '
    if (err.indexOf(parseFilePrefix) === 0) {
      var pathWi ...
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
