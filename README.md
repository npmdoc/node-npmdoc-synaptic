# npmdoc-synaptic

#### basic api documentation for  [synaptic (v1.0.10)](http://synaptic.juancazala.com)  [![npm package](https://img.shields.io/npm/v/npmdoc-synaptic.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-synaptic) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-synaptic.svg)](https://travis-ci.org/npmdoc/node-npmdoc-synaptic)

#### architecture-free neural network library

[![NPM](https://nodei.co/npm/synaptic.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/synaptic)

- [https://npmdoc.github.io/node-npmdoc-synaptic/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-synaptic/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-synaptic/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-synaptic/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-synaptic/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-synaptic/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Juan Cazala",
        "url": "http://juancazala.com/"
    },
    "bugs": {
        "url": "https://github.com/cazala/synaptic/issues"
    },
    "dependencies": {},
    "description": "architecture-free neural network library",
    "devDependencies": {
        "chai": "^3.5.0",
        "chai-stats": "^0.3.0",
        "karma": "^1.1.2",
        "karma-chrome-launcher": "^1.0.1",
        "karma-firefox-launcher": "^1.0.0",
        "karma-mocha": "^1.1.1",
        "karma-phantomjs-launcher": "^1.0.1",
        "karma-safari-launcher": "^1.0.0",
        "karma-webpack": "^1.7.0",
        "mocha": "^2.2.4",
        "pre-push": "^0.1.1",
        "webpack": "^1.13.1"
    },
    "directories": {},
    "dist": {
        "shasum": "40282b4b4e12554f55b756d37cd28017ad7d49ed",
        "tarball": "https://registry.npmjs.org/synaptic/-/synaptic-1.0.10.tgz"
    },
    "engines": {
        "node": ">=4"
    },
    "gitHead": "76f322f0b748d9e2236d388e13f98b2308e6a875",
    "homepage": "http://synaptic.juancazala.com",
    "keywords": [
        "neural network",
        "machine learning",
        "long short term memory",
        "perceptron",
        "architecture free"
    ],
    "license": {
        "type": "MIT",
        "url": "https://github.com/cazala/synaptic/blob/master/LICENSE"
    },
    "main": "./src/synaptic",
    "maintainers": [
        {
            "name": "cazala"
        }
    ],
    "name": "synaptic",
    "optionalDependencies": {},
    "prepush": [
        "test",
        "build"
    ],
    "repository": {
        "type": "git",
        "url": "git+https://github.com/cazala/synaptic.git"
    },
    "scripts": {
        "build": "webpack --config webpack.config.js",
        "test": "npm run test:src",
        "test:dist": "npm run build && npm run test:mocha:dist && npm run test:karma:browsers",
        "test:karma:browsers": "karma start --single-run --browsers Chrome,Firefox,SafariPrivate",
        "test:karma:phantomjs": "karma start --single-run --browsers PhantomJS",
        "test:mocha:dist": "mocha test --require dist/synaptic.js ./test",
        "test:mocha:src": "mocha test --require src/synaptic.js ./test",
        "test:src": "mocha test --require src/synaptic.js ./test",
        "test:travis": "npm run test:mocha:src && npm run build && npm run test:mocha:dist"
    },
    "version": "1.0.10",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
