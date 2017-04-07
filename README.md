# api documentation for  [postcss-font-magician (v1.6.1)](https://github.com/jonathantneal/postcss-font-magician)  [![npm package](https://img.shields.io/npm/v/npmdoc-postcss-font-magician.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-postcss-font-magician) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-postcss-font-magician.svg)](https://travis-ci.org/npmdoc/node-npmdoc-postcss-font-magician)
#### PostCSS plugin that magically generates all the @font-face rules

[![NPM](https://nodei.co/npm/postcss-font-magician.png?downloads=true)](https://www.npmjs.com/package/postcss-font-magician)

[![apidoc](https://npmdoc.github.io/node-npmdoc-postcss-font-magician/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-postcss-font-magician_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-postcss-font-magician/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-postcss-font-magician/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-postcss-font-magician/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jonathan Neal",
        "email": "jonathantneal@hotmail.com"
    },
    "bugs": {
        "url": "https://github.com/jonathantneal/postcss-font-magician/issues"
    },
    "contributors": [
        {
            "name": "Jonathan Neal",
            "email": "jonathantneal@hotmail.com"
        },
        {
            "name": "Ruslan Abdullaev",
            "email": "skarlatin@mail.ru"
        }
    ],
    "dependencies": {
        "bootstrap-fonts-complete": "^1.0.0",
        "directory-fonts-complete": "^1.1.0",
        "google-fonts-complete": "^1.1.0",
        "postcss": "^5.0.12"
    },
    "description": "PostCSS plugin that magically generates all the @font-face rules",
    "devDependencies": {
        "chai": "^3.4.1",
        "google-fonts-complete": "^1.1.1",
        "gulp": "^3.9.0",
        "gulp-eslint": "^1.1.1",
        "gulp-mocha": "^2.2.0"
    },
    "directories": {},
    "dist": {
        "shasum": "0245382f8e81672d0af806651aed656fc660ebe5",
        "tarball": "https://registry.npmjs.org/postcss-font-magician/-/postcss-font-magician-1.6.1.tgz"
    },
    "gitHead": "1bfb714eebd40f31b2bfd468d917d503038a6047",
    "homepage": "https://github.com/jonathantneal/postcss-font-magician",
    "keywords": [
        "postcss",
        "css",
        "postcss-plugin",
        "fonts",
        "faces",
        "generate",
        "generation",
        "weights",
        "styles",
        "variants",
        "google",
        "web"
    ],
    "license": "CC0-1.0",
    "maintainers": [
        {
            "name": "jonathantneal",
            "email": "jonathantneal@hotmail.com"
        },
        {
            "name": "rajdee",
            "email": "abdullaev.rt@gmail.com"
        }
    ],
    "name": "postcss-font-magician",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/jonathantneal/postcss-font-magician.git"
    },
    "scripts": {
        "test": "gulp"
    },
    "version": "1.6.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module postcss-font-magician](#apidoc.module.postcss-font-magician)
1.  [function <span class="apidocSignatureSpan">postcss-font-magician.</span>process (css, options)](#apidoc.element.postcss-font-magician.process)



# <a name="apidoc.module.postcss-font-magician"></a>[module postcss-font-magician](#apidoc.module.postcss-font-magician)

#### <a name="apidoc.element.postcss-font-magician.process"></a>[function <span class="apidocSignatureSpan">postcss-font-magician.</span>process (css, options)](#apidoc.element.postcss-font-magician.process)
- description and source-code
```javascript
process = function (css, options) {
    var processed = postcss([module.exports(options)]).process(css, options);

    return options && options.map && !options.map.inline ? processed : processed.css;
}
```
- example usage
```shell
...
npm install postcss --save-dev
'''

2. Use [Font Magician] in your script:
'''js
postcss([
   require('postcss-font-magician')({ /* options */ })
]).process(
   fs.readFileSync('./css/src/style.css', 'utf8')
).then(function (result) {
   fs.writeFileSync('./css/style.css', result.css);
});
'''
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
