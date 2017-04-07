# api documentation for  [xss-filters (v1.2.7)](https://github.com/yahoo/xss-filters)  [![npm package](https://img.shields.io/npm/v/npmdoc-xss-filters.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-xss-filters) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-xss-filters.svg)](https://travis-ci.org/npmdoc/node-npmdoc-xss-filters)
#### Secure XSS Filters - Just sufficient output filtering to prevent XSS!

[![NPM](https://nodei.co/npm/xss-filters.png?downloads=true)](https://www.npmjs.com/package/xss-filters)

[![apidoc](https://npmdoc.github.io/node-npmdoc-xss-filters/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-xss-filters_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-xss-filters/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-xss-filters/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-xss-filters/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Adonis Fung",
        "email": "adon@yahoo-inc.com"
    },
    "bugs": {
        "url": "https://github.com/yahoo/xss-filters/issues"
    },
    "contributors": [
        {
            "name": "Adonis Fung",
            "email": "adon@yahoo-inc.com"
        },
        {
            "name": "Nera Liu",
            "email": "neraliu@gmail.com"
        },
        {
            "name": "Albert Yu",
            "email": "yukinying@gmail.com"
        }
    ],
    "dependencies": {},
    "description": "Secure XSS Filters - Just sufficient output filtering to prevent XSS!",
    "devDependencies": {
        "expect.js": "^0.3.1",
        "grunt": "^1.0.1",
        "grunt-browserify": "^5.0.0",
        "grunt-cli": "^1.2.0",
        "grunt-contrib-clean": "^1.0.0",
        "grunt-contrib-copy": "^1.0.0",
        "grunt-contrib-jshint": "^1.0.0",
        "grunt-contrib-uglify": "^2.0.0",
        "grunt-jsdoc": "^2.1.0",
        "grunt-karma": "^2.0.0",
        "grunt-mocha-istanbul": "^5.0.2",
        "ink-docstrap": "^1.3.0",
        "istanbul": "^0.4.5",
        "karma": "^1.3.0",
        "karma-chrome-launcher": "^2.0.0",
        "karma-firefox-launcher": "^1.0.0",
        "karma-ie-launcher": "^1.0.0",
        "karma-mocha": "^1.1.1",
        "karma-sauce-launcher": "^1.0.0",
        "mocha": "^3.0.2"
    },
    "directories": {},
    "dist": {
        "shasum": "59fa1de201f36f2f3470dcac5f58ccc2830b0a9a",
        "tarball": "https://registry.npmjs.org/xss-filters/-/xss-filters-1.2.7.tgz"
    },
    "gitHead": "5174da0a282f5fbd9289be1d0dd217f874a9f05c",
    "homepage": "https://github.com/yahoo/xss-filters",
    "keywords": [
        "xss",
        "output filter",
        "sanitize",
        "sanitise",
        "escape",
        "encode",
        "filter",
        "context-aware",
        "context-sensitive",
        "security",
        "yahoo"
    ],
    "licenses": [
        {
            "type": "BSD",
            "url": "https://github.com/yahoo/xss-filters/blob/master/LICENSE"
        }
    ],
    "main": "src/xss-filters.js",
    "maintainers": [
        {
            "name": "adon",
            "email": "adon@yahoo-inc.com"
        },
        {
            "name": "neraliu",
            "email": "neraliu@gmail.com"
        },
        {
            "name": "yukinying",
            "email": "yukinying@gmail.com"
        },
        {
            "name": "davglass",
            "email": "davglass@gmail.com"
        }
    ],
    "name": "xss-filters",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/yahoo/xss-filters.git"
    },
    "scripts": {
        "build": "grunt",
        "clean": "grunt clean",
        "docs": "grunt docs",
        "hint": "grunt jshint",
        "test": "grunt test"
    },
    "version": "1.2.7"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module xss-filters](#apidoc.module.xss-filters)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>_getPrivFilters ()](#apidoc.element.xss-filters._getPrivFilters)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>inDoubleQuotedAttr (s)](#apidoc.element.xss-filters.inDoubleQuotedAttr)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>inHTMLComment (s)](#apidoc.element.xss-filters.inHTMLComment)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>inHTMLData (s)](#apidoc.element.xss-filters.inHTMLData)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>inSingleQuotedAttr (s)](#apidoc.element.xss-filters.inSingleQuotedAttr)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>inUnQuotedAttr (s)](#apidoc.element.xss-filters.inUnQuotedAttr)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriComponentInDoubleQuotedAttr (s)](#apidoc.element.xss-filters.uriComponentInDoubleQuotedAttr)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriComponentInHTMLComment (s)](#apidoc.element.xss-filters.uriComponentInHTMLComment)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriComponentInHTMLData ()](#apidoc.element.xss-filters.uriComponentInHTMLData)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriComponentInSingleQuotedAttr (s)](#apidoc.element.xss-filters.uriComponentInSingleQuotedAttr)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriComponentInUnQuotedAttr (s)](#apidoc.element.xss-filters.uriComponentInUnQuotedAttr)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriFragmentInDoubleQuotedAttr (s)](#apidoc.element.xss-filters.uriFragmentInDoubleQuotedAttr)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriFragmentInHTMLComment (s)](#apidoc.element.xss-filters.uriFragmentInHTMLComment)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriFragmentInHTMLData ()](#apidoc.element.xss-filters.uriFragmentInHTMLData)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriFragmentInSingleQuotedAttr (s)](#apidoc.element.xss-filters.uriFragmentInSingleQuotedAttr)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriFragmentInUnQuotedAttr (s)](#apidoc.element.xss-filters.uriFragmentInUnQuotedAttr)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriInDoubleQuotedAttr (s)](#apidoc.element.xss-filters.uriInDoubleQuotedAttr)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriInHTMLComment (s)](#apidoc.element.xss-filters.uriInHTMLComment)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriInHTMLData (s)](#apidoc.element.xss-filters.uriInHTMLData)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriInSingleQuotedAttr (s)](#apidoc.element.xss-filters.uriInSingleQuotedAttr)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriInUnQuotedAttr (s)](#apidoc.element.xss-filters.uriInUnQuotedAttr)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriPathInDoubleQuotedAttr (s)](#apidoc.element.xss-filters.uriPathInDoubleQuotedAttr)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriPathInHTMLComment (s)](#apidoc.element.xss-filters.uriPathInHTMLComment)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriPathInHTMLData ()](#apidoc.element.xss-filters.uriPathInHTMLData)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriPathInSingleQuotedAttr (s)](#apidoc.element.xss-filters.uriPathInSingleQuotedAttr)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriPathInUnQuotedAttr (s)](#apidoc.element.xss-filters.uriPathInUnQuotedAttr)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriQueryInDoubleQuotedAttr (s)](#apidoc.element.xss-filters.uriQueryInDoubleQuotedAttr)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriQueryInHTMLComment (s)](#apidoc.element.xss-filters.uriQueryInHTMLComment)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriQueryInHTMLData ()](#apidoc.element.xss-filters.uriQueryInHTMLData)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriQueryInSingleQuotedAttr (s)](#apidoc.element.xss-filters.uriQueryInSingleQuotedAttr)
1.  [function <span class="apidocSignatureSpan">xss-filters.</span>uriQueryInUnQuotedAttr (s)](#apidoc.element.xss-filters.uriQueryInUnQuotedAttr)
1.  object <span class="apidocSignatureSpan">xss-filters.</span>_privFilters

#### [module xss-filters._privFilters](#apidoc.module.xss-filters._privFilters)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>d (s, namedRefMap, reNamedRef, skipReplacement)](#apidoc.element.xss-filters._privFilters.d)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>frCoPt (num)](#apidoc.element.xss-filters._privFilters.frCoPt)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>y (s)](#apidoc.element.xss-filters._privFilters.y)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>ya (s)](#apidoc.element.xss-filters._privFilters.ya)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yavd (s)](#apidoc.element.xss-filters._privFilters.yavd)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yavs (s)](#apidoc.element.xss-filters._privFilters.yavs)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yavu (s)](#apidoc.element.xss-filters._privFilters.yavu)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yc (s)](#apidoc.element.xss-filters._privFilters.yc)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yced (s)](#apidoc.element.xss-filters._privFilters.yced)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yces (s)](#apidoc.element.xss-filters._privFilters.yces)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yceu (s)](#apidoc.element.xss-filters._privFilters.yceu)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yceud (s)](#apidoc.element.xss-filters._privFilters.yceud)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yceus (s)](#apidoc.element.xss-filters._privFilters.yceus)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yceuu (s)](#apidoc.element.xss-filters._privFilters.yceuu)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yd (s)](#apidoc.element.xss-filters._privFilters.yd)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yu ()](#apidoc.element.xss-filters._privFilters.yu)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yubl (s)](#apidoc.element.xss-filters._privFilters.yubl)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yublf (s)](#apidoc.element.xss-filters._privFilters.yublf)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yuc ()](#apidoc.element.xss-filters._privFilters.yuc)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yufull (s)](#apidoc.element.xss-filters._privFilters.yufull)
1.  [function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yup (s)](#apidoc.element.xss-filters._privFilters.yup)



# <a name="apidoc.module.xss-filters"></a>[module xss-filters](#apidoc.module.xss-filters)

#### <a name="apidoc.element.xss-filters._getPrivFilters"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>_getPrivFilters ()](#apidoc.element.xss-filters._getPrivFilters)
- description and source-code
```javascript
_getPrivFilters = function () {

    var LT     = /</g,
        QUOT   = /"/g,
        SQUOT  = /'/g,
        AMP    = /&/g,
        NULL   = /\x00/g,
        SPECIAL_ATTR_VALUE_UNQUOTED_CHARS = /(?:^$|[\x00\x09-\x0D "''=<>])/g,
        SPECIAL_HTML_CHARS = /[&<>"'']/g,
        SPECIAL_COMMENT_CHARS = /(?:\x00|^-*!?>|--!?>|--?!?$|\]>|\]$)/g;

    // CSS sensitive chars: ()"'/,!*@{}:;
    // By CSS: (Tab|NewLine|colon|semi|lpar|rpar|apos|sol|comma|excl|ast|midast);|(quot|QUOT)
    // By URI_PROTOCOL: (Tab|NewLine);
    var SENSITIVE_HTML_ENTITIES = /&(?:#([xX][0-9A-Fa-f]+|\d+);?|(Tab|NewLine|colon|semi|lpar|rpar|apos|sol|comma|excl|ast|midast
|ensp|emsp|thinsp);|(nbsp|amp|AMP|lt|LT|gt|GT|quot|QUOT);?)/g,
        SENSITIVE_NAMED_REF_MAP = {Tab: '\t', NewLine: '\n', colon: ':', semi: ';', lpar: '(', rpar: ')', apos: '\'', sol: '/',
comma: ',', excl: '!', ast: '*', midast: '*', ensp: '\u2002', emsp: '\u2003', thinsp: '\u2009', nbsp: '\xA0', amp: '&', lt: '<', gt: '>', quot: '"', QUOT: '"'};

    // var CSS_VALID_VALUE =
    //     /^(?:
    //     (?!-*expression)#?[-\w]+
    //     |[+-]?(?:\d+|\d*\.\d+)(?:em|ex|ch|rem|px|mm|cm|in|pt|pc|%|vh|vw|vmin|vmax)?
    //     |!important
    //     | //empty
    //     )$/i;
    var CSS_VALID_VALUE = /^(?:(?!-*expression)#?[-\w]+|[+-]?(?:\d+|\d*\.\d+)(?:r?em|ex|ch|cm|mm|in|px|pt|pc|%|vh|vw|vmin|vmax)?|!
important|)$/i,
        // TODO: prevent double css escaping by not encoding \ again, but this may require CSS decoding
        // \x7F and \x01-\x1F less \x09 are for Safari 5.0, added []{}/* for unbalanced quote
        CSS_DOUBLE_QUOTED_CHARS = /[\x00-\x1F\x7F\[\]{}\\"]/g,
        CSS_SINGLE_QUOTED_CHARS = /[\x00-\x1F\x7F\[\]{}\\']/g,
        // (, \u207D and \u208D can be used in background: 'url(...)' in IE, assumed all \ chars are encoded by QUOTED_CHARS, and
 null is already replaced with\uFFFD
        // otherwise, use this CSS_BLACKLIST instead (enhance it with url matching): /(?:\\?\(|[\u207D\u208D]|\\0{0,4}28 ?|\\0{0
,2}20[78][Dd] ?)+/g
        CSS_BLACKLIST = /url[\(\u207D\u208D]+/g,
        // this assumes encodeURI() and encodeURIComponent() has escaped 1-32, 127 for IE8
        CSS_UNQUOTED_URL = /['\(\)]/g; // " \ treated by encodeURI()

    // Given a full URI, need to support "[" ( IPv6address ) "]" in URI as per RFC3986
    // Reference: https://tools.ietf.org/html/rfc3986
    var URL_IPV6 = /\/\/%5[Bb]([A-Fa-f0-9:]+)%5[Dd]/;


    // Reference: http://shazzer.co.uk/database/All/characters-allowd-in-html-entities
    // Reference: http://shazzer.co.uk/vector/Characters-allowed-after-ampersand-in-named-character-references
    // Reference: http://shazzer.co.uk/database/All/Characters-before-javascript-uri
    // Reference: http://shazzer.co.uk/database/All/Characters-after-javascript-uri
    // Reference: https://html.spec.whatwg.org/multipage/syntax.html#consume-a-character-reference
    // Reference for named characters: https://html.spec.whatwg.org/multipage/entities.json
    var URI_BLACKLIST_PROTOCOLS = {'javascript':1, 'data':1, 'vbscript':1, 'mhtml':1, 'x-schema':1},
        URI_PROTOCOL_COLON = /(?::|&#[xX]0*3[aA];?|&#0*58;?|&colon;)/,
        URI_PROTOCOL_WHITESPACES = /(?:^[\x00-\x20]+|[\t\n\r\x00]+)/g,
        URI_PROTOCOL_NAMED_REF_MAP = {Tab: '\t', NewLine: '\n'};

    var x,
        strReplace = function (s, regexp, callback) {
            return s === undefined ? 'undefined'
                    : s === null            ? 'null'
                    : s.toString().replace(regexp, callback);
        },
        fromCodePoint = String.fromCodePoint || function(codePoint) {
            if (arguments.length === 0) {
                return '';
            }
            if (codePoint <= 0xFFFF) { // BMP code point
                return String.fromCharCode(codePoint);
            }

            // Astral code point; split in surrogate halves
            // http://mathiasbynens.be/notes/javascript-encoding#surrogate-formulae
            codePoint -= 0x10000;
            return String.fromCharCode((codePoint >> 10) + 0xD800, (codePoint % 0x400) + 0xDC00);
        };


    fun ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.inDoubleQuotedAttr"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>inDoubleQuotedAttr (s)](#apidoc.element.xss-filters.inDoubleQuotedAttr)
- description and source-code
```javascript
inDoubleQuotedAttr = function (s) {
    return strReplace(s, QUOT, '&quot;');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.inHTMLComment"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>inHTMLComment (s)](#apidoc.element.xss-filters.inHTMLComment)
- description and source-code
```javascript
inHTMLComment = function (s) {
    return strReplace(s, SPECIAL_COMMENT_CHARS, function(m){
        return m === '\x00' ? '\uFFFD'
            : m === '--!' || m === '--' || m === '-' || m === ']' ? m + ' '
            :/*
            :  m === ']>'   ? '] >'
            :  m === '-->'  ? '-- >'
            :  m === '--!>' ? '--! >'
            : /-*!?>/.test(m) ? */ m.slice(0, -1) + ' >';
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.inHTMLData"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>inHTMLData (s)](#apidoc.element.xss-filters.inHTMLData)
- description and source-code
```javascript
inHTMLData = function (s) {
    return strReplace(s, LT, '&lt;');
}
```
- example usage
```shell
...
'''javascript
var express = require('express');
var app = express();
var xssFilters = require('xss-filters');

app.get('/', function(req, res){
  var firstname = req.query.firstname; //an untrusted input collected from user
  res.send('<h1> Hello, ' + xssFilters.inHTMLData(firstname) + '!</h1>');
});

app.listen(3000);
'''

### Client-side (browser)
...
```

#### <a name="apidoc.element.xss-filters.inSingleQuotedAttr"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>inSingleQuotedAttr (s)](#apidoc.element.xss-filters.inSingleQuotedAttr)
- description and source-code
```javascript
inSingleQuotedAttr = function (s) {
    return strReplace(s, SQUOT, '&#39;');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.inUnQuotedAttr"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>inUnQuotedAttr (s)](#apidoc.element.xss-filters.inUnQuotedAttr)
- description and source-code
```javascript
inUnQuotedAttr = function (s) {
    return strReplace(s, SPECIAL_ATTR_VALUE_UNQUOTED_CHARS, function (m) {
        return m === '\t'   ? '&#9;'  // in hex: 09
            :  m === '\n'   ? '&#10;' // in hex: 0A
            :  m === '\x0B' ? '&#11;' // in hex: 0B  for IE. IE<9 \v equals v, so use \x0B instead
            :  m === '\f'   ? '&#12;' // in hex: 0C
            :  m === '\r'   ? '&#13;' // in hex: 0D
            :  m === ' '    ? '&#32;' // in hex: 20
            :  m === '='    ? '&#61;' // in hex: 3D
            :  m === '<'    ? '&lt;'
            :  m === '>'    ? '&gt;'
            :  m === '"'    ? '&quot;'
            :  m === "'"    ? '&#39;'
            :  m === '''    ? '&#96;'
            : /*empty or null*/ '\uFFFD';
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriComponentInDoubleQuotedAttr"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriComponentInDoubleQuotedAttr (s)](#apidoc.element.xss-filters.uriComponentInDoubleQuotedAttr)
- description and source-code
```javascript
uriComponentInDoubleQuotedAttr = function (s) {
    return privFilters.yavd(privFilters.yuc(s));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriComponentInHTMLComment"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriComponentInHTMLComment (s)](#apidoc.element.xss-filters.uriComponentInHTMLComment)
- description and source-code
```javascript
uriComponentInHTMLComment = function (s) {
    return privFilters.yc(privFilters.yuc(s));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriComponentInHTMLData"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriComponentInHTMLData ()](#apidoc.element.xss-filters.uriComponentInHTMLData)
- description and source-code
```javascript
function encodeURIComponent() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriComponentInSingleQuotedAttr"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriComponentInSingleQuotedAttr (s)](#apidoc.element.xss-filters.uriComponentInSingleQuotedAttr)
- description and source-code
```javascript
uriComponentInSingleQuotedAttr = function (s) {
    return privFilters.yavs(privFilters.yuc(s));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriComponentInUnQuotedAttr"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriComponentInUnQuotedAttr (s)](#apidoc.element.xss-filters.uriComponentInUnQuotedAttr)
- description and source-code
```javascript
uriComponentInUnQuotedAttr = function (s) {
    return privFilters.yavu(privFilters.yuc(s));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriFragmentInDoubleQuotedAttr"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriFragmentInDoubleQuotedAttr (s)](#apidoc.element.xss-filters.uriFragmentInDoubleQuotedAttr)
- description and source-code
```javascript
uriFragmentInDoubleQuotedAttr = function (s) {
    return privFilters.yubl(privFilters.yavd(privFilters.yuc(s)));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriFragmentInHTMLComment"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriFragmentInHTMLComment (s)](#apidoc.element.xss-filters.uriFragmentInHTMLComment)
- description and source-code
```javascript
uriFragmentInHTMLComment = function (s) {
    return privFilters.yc(privFilters.yuc(s));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriFragmentInHTMLData"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriFragmentInHTMLData ()](#apidoc.element.xss-filters.uriFragmentInHTMLData)
- description and source-code
```javascript
function encodeURIComponent() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriFragmentInSingleQuotedAttr"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriFragmentInSingleQuotedAttr (s)](#apidoc.element.xss-filters.uriFragmentInSingleQuotedAttr)
- description and source-code
```javascript
uriFragmentInSingleQuotedAttr = function (s) {
    return privFilters.yubl(privFilters.yavs(privFilters.yuc(s)));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriFragmentInUnQuotedAttr"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriFragmentInUnQuotedAttr (s)](#apidoc.element.xss-filters.uriFragmentInUnQuotedAttr)
- description and source-code
```javascript
uriFragmentInUnQuotedAttr = function (s) {
    return privFilters.yubl(privFilters.yavu(privFilters.yuc(s)));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriInDoubleQuotedAttr"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriInDoubleQuotedAttr (s)](#apidoc.element.xss-filters.uriInDoubleQuotedAttr)
- description and source-code
```javascript
uriInDoubleQuotedAttr = function (s) {
    return uriInAttr(s, privFilters.yavd);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriInHTMLComment"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriInHTMLComment (s)](#apidoc.element.xss-filters.uriInHTMLComment)
- description and source-code
```javascript
uriInHTMLComment = function (s) {
    return privFilters.yc(privFilters.yufull(s));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriInHTMLData"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriInHTMLData (s)](#apidoc.element.xss-filters.uriInHTMLData)
- description and source-code
```javascript
uriInHTMLData = function (s) {
    return x.yu(s).replace(URL_IPV6, function(m, p) {
        return '//[' + p + ']';
    });
}
```
- example usage
```shell
...
[dep-status]: https://david-dm.org/yahoo/xss-filters
[dep-badge]: https://img.shields.io/david/yahoo/xss-filters.svg?style=flat-square

## Goals

- **More Secure.** Context-dependent output filters that are developer-friendly. It is safe to apply these filters like so:

'document.write("<a href=" + xssFilters.uriInUnQuotedAttr(url) + ">" + xssFilters.uriInHTMLData(url) + "</a>");'

In this example, the traditional wisdom of blindly escaping some special html entity characters ('&' '<' '>' ''' '"' '' ' '') would
 not stop XSS (e.g., when 'url' is equal to 'javascript:alert(1)' or ' onclick=alert(1)').

- **Faster with Just Sufficient Encoding.** Encode the *minimal* set of characters to thwart JavaScript executions, thus preventing
 XSS attacks while keeping most characters intact. Compared to the traditional blindly escape filter, our filters are [up to two
 times faster](http://jsperf.com/context-sensitive-vs-blindly-escape), and there is no more double-encoding problems such as '&amp
;amp;lt;'!!

![alt Visualizing the concept of just sufficient encoding](https://ierg4210.github.io/web/images/xss-filters/xss-filters.png)
Figure 1. "Just sufficient" encoding based on the HTML5 spec.
...
```

#### <a name="apidoc.element.xss-filters.uriInSingleQuotedAttr"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriInSingleQuotedAttr (s)](#apidoc.element.xss-filters.uriInSingleQuotedAttr)
- description and source-code
```javascript
uriInSingleQuotedAttr = function (s) {
    return uriInAttr(s, privFilters.yavs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriInUnQuotedAttr"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriInUnQuotedAttr (s)](#apidoc.element.xss-filters.uriInUnQuotedAttr)
- description and source-code
```javascript
uriInUnQuotedAttr = function (s) {
    return uriInAttr(s, privFilters.yavu);
}
```
- example usage
```shell
...
[dep-status]: https://david-dm.org/yahoo/xss-filters
[dep-badge]: https://img.shields.io/david/yahoo/xss-filters.svg?style=flat-square

## Goals

- **More Secure.** Context-dependent output filters that are developer-friendly. It is safe to apply these filters like so:

'document.write("<a href=" + xssFilters.uriInUnQuotedAttr(url) + ">" + xssFilters.uriInHTMLData(url) + "</a>");'

In this example, the traditional wisdom of blindly escaping some special html entity characters ('&' '<' '>' ''' '"' '' ' '') would
 not stop XSS (e.g., when 'url' is equal to 'javascript:alert(1)' or ' onclick=alert(1)').

- **Faster with Just Sufficient Encoding.** Encode the *minimal* set of characters to thwart JavaScript executions, thus preventing
 XSS attacks while keeping most characters intact. Compared to the traditional blindly escape filter, our filters are [up to two
 times faster](http://jsperf.com/context-sensitive-vs-blindly-escape), and there is no more double-encoding problems such as '&amp
;amp;lt;'!!

![alt Visualizing the concept of just sufficient encoding](https://ierg4210.github.io/web/images/xss-filters/xss-filters.png)
Figure 1. "Just sufficient" encoding based on the HTML5 spec.
...
```

#### <a name="apidoc.element.xss-filters.uriPathInDoubleQuotedAttr"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriPathInDoubleQuotedAttr (s)](#apidoc.element.xss-filters.uriPathInDoubleQuotedAttr)
- description and source-code
```javascript
uriPathInDoubleQuotedAttr = function (s) {
    return uriInAttr(s, privFilters.yavd, privFilters.yu);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriPathInHTMLComment"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriPathInHTMLComment (s)](#apidoc.element.xss-filters.uriPathInHTMLComment)
- description and source-code
```javascript
uriPathInHTMLComment = function (s) {
    return privFilters.yc(privFilters.yu(s));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriPathInHTMLData"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriPathInHTMLData ()](#apidoc.element.xss-filters.uriPathInHTMLData)
- description and source-code
```javascript
function encodeURI() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriPathInSingleQuotedAttr"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriPathInSingleQuotedAttr (s)](#apidoc.element.xss-filters.uriPathInSingleQuotedAttr)
- description and source-code
```javascript
uriPathInSingleQuotedAttr = function (s) {
    return uriInAttr(s, privFilters.yavs, privFilters.yu);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriPathInUnQuotedAttr"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriPathInUnQuotedAttr (s)](#apidoc.element.xss-filters.uriPathInUnQuotedAttr)
- description and source-code
```javascript
uriPathInUnQuotedAttr = function (s) {
    return uriInAttr(s, privFilters.yavu, privFilters.yu);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriQueryInDoubleQuotedAttr"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriQueryInDoubleQuotedAttr (s)](#apidoc.element.xss-filters.uriQueryInDoubleQuotedAttr)
- description and source-code
```javascript
uriQueryInDoubleQuotedAttr = function (s) {
    return uriInAttr(s, privFilters.yavd, privFilters.yu);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriQueryInHTMLComment"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriQueryInHTMLComment (s)](#apidoc.element.xss-filters.uriQueryInHTMLComment)
- description and source-code
```javascript
uriQueryInHTMLComment = function (s) {
    return privFilters.yc(privFilters.yu(s));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriQueryInHTMLData"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriQueryInHTMLData ()](#apidoc.element.xss-filters.uriQueryInHTMLData)
- description and source-code
```javascript
function encodeURI() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriQueryInSingleQuotedAttr"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriQueryInSingleQuotedAttr (s)](#apidoc.element.xss-filters.uriQueryInSingleQuotedAttr)
- description and source-code
```javascript
uriQueryInSingleQuotedAttr = function (s) {
    return uriInAttr(s, privFilters.yavs, privFilters.yu);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters.uriQueryInUnQuotedAttr"></a>[function <span class="apidocSignatureSpan">xss-filters.</span>uriQueryInUnQuotedAttr (s)](#apidoc.element.xss-filters.uriQueryInUnQuotedAttr)
- description and source-code
```javascript
uriQueryInUnQuotedAttr = function (s) {
    return uriInAttr(s, privFilters.yavu, privFilters.yu);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xss-filters._privFilters"></a>[module xss-filters._privFilters](#apidoc.module.xss-filters._privFilters)

#### <a name="apidoc.element.xss-filters._privFilters.d"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>d (s, namedRefMap, reNamedRef, skipReplacement)](#apidoc.element.xss-filters._privFilters.d)
- description and source-code
```javascript
function htmlDecode(s, namedRefMap, reNamedRef, skipReplacement) {

    namedRefMap = namedRefMap || SENSITIVE_NAMED_REF_MAP;
    reNamedRef = reNamedRef || SENSITIVE_HTML_ENTITIES;

    function regExpFunction(m, num, named, named1) {
        if (num) {
            num = Number(num[0] <= '9' ? num : '0' + num);
            // switch(num) {
            //     case 0x80: return '\u20AC';  // EURO SIGN (€)
            //     case 0x82: return '\u201A';  // SINGLE LOW-9 QUOTATION MARK (‚)
            //     case 0x83: return '\u0192';  // LATIN SMALL LETTER F WITH HOOK (ƒ)
            //     case 0x84: return '\u201E';  // DOUBLE LOW-9 QUOTATION MARK („)
            //     case 0x85: return '\u2026';  // HORIZONTAL ELLIPSIS (…)
            //     case 0x86: return '\u2020';  // DAGGER (†)
            //     case 0x87: return '\u2021';  // DOUBLE DAGGER (‡)
            //     case 0x88: return '\u02C6';  // MODIFIER LETTER CIRCUMFLEX ACCENT (ˆ)
            //     case 0x89: return '\u2030';  // PER MILLE SIGN (‰)
            //     case 0x8A: return '\u0160';  // LATIN CAPITAL LETTER S WITH CARON (Š)
            //     case 0x8B: return '\u2039';  // SINGLE LEFT-POINTING ANGLE QUOTATION MARK (‹)
            //     case 0x8C: return '\u0152';  // LATIN CAPITAL LIGATURE OE (Œ)
            //     case 0x8E: return '\u017D';  // LATIN CAPITAL LETTER Z WITH CARON (Ž)
            //     case 0x91: return '\u2018';  // LEFT SINGLE QUOTATION MARK (‘)
            //     case 0x92: return '\u2019';  // RIGHT SINGLE QUOTATION MARK (’)
            //     case 0x93: return '\u201C';  // LEFT DOUBLE QUOTATION MARK (“)
            //     case 0x94: return '\u201D';  // RIGHT DOUBLE QUOTATION MARK (”)
            //     case 0x95: return '\u2022';  // BULLET (•)
            //     case 0x96: return '\u2013';  // EN DASH (–)
            //     case 0x97: return '\u2014';  // EM DASH (—)
            //     case 0x98: return '\u02DC';  // SMALL TILDE (˜)
            //     case 0x99: return '\u2122';  // TRADE MARK SIGN (™)
            //     case 0x9A: return '\u0161';  // LATIN SMALL LETTER S WITH CARON (š)
            //     case 0x9B: return '\u203A';  // SINGLE RIGHT-POINTING ANGLE QUOTATION MARK (›)
            //     case 0x9C: return '\u0153';  // LATIN SMALL LIGATURE OE (œ)
            //     case 0x9E: return '\u017E';  // LATIN SMALL LETTER Z WITH CARON (ž)
            //     case 0x9F: return '\u0178';  // LATIN CAPITAL LETTER Y WITH DIAERESIS (Ÿ)
            // }
            // // num >= 0xD800 && num <= 0xDFFF, and 0x0D is separately handled, as it doesn't fall into the range of x.pec()
            // return (num >= 0xD800 && num <= 0xDFFF) || num === 0x0D ? '\uFFFD' : x.frCoPt(num);

            return skipReplacement ? fromCodePoint(num)
                    : num === 0x80 ? '\u20AC'  // EURO SIGN (€)
                    : num === 0x82 ? '\u201A'  // SINGLE LOW-9 QUOTATION MARK (‚)
                    : num === 0x83 ? '\u0192'  // LATIN SMALL LETTER F WITH HOOK (ƒ)
                    : num === 0x84 ? '\u201E'  // DOUBLE LOW-9 QUOTATION MARK („)
                    : num === 0x85 ? '\u2026'  // HORIZONTAL ELLIPSIS (…)
                    : num === 0x86 ? '\u2020'  // DAGGER (†)
                    : num === 0x87 ? '\u2021'  // DOUBLE DAGGER (‡)
                    : num === 0x88 ? '\u02C6'  // MODIFIER LETTER CIRCUMFLEX ACCENT (ˆ)
                    : num === 0x89 ? '\u2030'  // PER MILLE SIGN (‰)
                    : num === 0x8A ? '\u0160'  // LATIN CAPITAL LETTER S WITH CARON (Š)
                    : num === 0x8B ? '\u2039'  // SINGLE LEFT-POINTING ANGLE QUOTATION MARK (‹)
                    : num === 0x8C ? '\u0152'  // LATIN CAPITAL LIGATURE OE (Œ)
                    : num === 0x8E ? '\u017D'  // LATIN CAPITAL LETTER Z WITH CARON (Ž)
                    : num === 0x91 ? '\u2018'  // LEFT SINGLE QUOTATION MARK (‘)
                    : num === 0x92 ? '\u2019'  // RIGHT SINGLE QUOTATION MARK (’)
                    : num === 0x93 ? '\u201C'  // LEFT DOUBLE QUOTATION MARK (“)
                    : num === 0x94 ? '\u20 ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.frCoPt"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>frCoPt (num)](#apidoc.element.xss-filters._privFilters.frCoPt)
- description and source-code
```javascript
frCoPt = function (num) {
    return num === undefined || num === null ? '' :
        !isFinite(num = Number(num)) || // 'NaN', '+Infinity', or '-Infinity'
        num <= 0 ||                     // not a valid Unicode code point
        num > 0x10FFFF ||               // not a valid Unicode code point
        // Math.floor(num) != num ||

        (num >= 0x01 && num <= 0x08) ||
        (num >= 0x0E && num <= 0x1F) ||
        (num >= 0x7F && num <= 0x9F) ||
        (num >= 0xFDD0 && num <= 0xFDEF) ||

         num === 0x0B ||
        (num & 0xFFFF) === 0xFFFF ||
        (num & 0xFFFF) === 0xFFFE ? '\uFFFD' : fromCodePoint(num);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.y"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>y (s)](#apidoc.element.xss-filters._privFilters.y)
- description and source-code
```javascript
y = function (s) {
    return strReplace(s, SPECIAL_HTML_CHARS, function (m) {
        return m === '&' ? '&amp;'
            :  m === '<' ? '&lt;'
            :  m === '>' ? '&gt;'
            :  m === '"' ? '&quot;'
            :  m === "'" ? '&#39;'
            :  /*m === '''*/ '&#96;';       // in hex: 60
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.ya"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>ya (s)](#apidoc.element.xss-filters._privFilters.ya)
- description and source-code
```javascript
ya = function (s) {
    return strReplace(s, AMP, '&amp;');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.yavd"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yavd (s)](#apidoc.element.xss-filters._privFilters.yavd)
- description and source-code
```javascript
yavd = function (s) {
    return strReplace(s, QUOT, '&quot;');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.yavs"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yavs (s)](#apidoc.element.xss-filters._privFilters.yavs)
- description and source-code
```javascript
yavs = function (s) {
    return strReplace(s, SQUOT, '&#39;');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.yavu"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yavu (s)](#apidoc.element.xss-filters._privFilters.yavu)
- description and source-code
```javascript
yavu = function (s) {
    return strReplace(s, SPECIAL_ATTR_VALUE_UNQUOTED_CHARS, function (m) {
        return m === '\t'   ? '&#9;'  // in hex: 09
            :  m === '\n'   ? '&#10;' // in hex: 0A
            :  m === '\x0B' ? '&#11;' // in hex: 0B  for IE. IE<9 \v equals v, so use \x0B instead
            :  m === '\f'   ? '&#12;' // in hex: 0C
            :  m === '\r'   ? '&#13;' // in hex: 0D
            :  m === ' '    ? '&#32;' // in hex: 20
            :  m === '='    ? '&#61;' // in hex: 3D
            :  m === '<'    ? '&lt;'
            :  m === '>'    ? '&gt;'
            :  m === '"'    ? '&quot;'
            :  m === "'"    ? '&#39;'
            :  m === '''    ? '&#96;'
            : /*empty or null*/ '\uFFFD';
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.yc"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yc (s)](#apidoc.element.xss-filters._privFilters.yc)
- description and source-code
```javascript
yc = function (s) {
    return strReplace(s, SPECIAL_COMMENT_CHARS, function(m){
        return m === '\x00' ? '\uFFFD'
            : m === '--!' || m === '--' || m === '-' || m === ']' ? m + ' '
            :/*
            :  m === ']>'   ? '] >'
            :  m === '-->'  ? '-- >'
            :  m === '--!>' ? '--! >'
            : /-*!?>/.test(m) ? */ m.slice(0, -1) + ' >';
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.yced"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yced (s)](#apidoc.element.xss-filters._privFilters.yced)
- description and source-code
```javascript
yced = function (s) {
    return cssBlacklist(htmlDecode(s).replace(CSS_DOUBLE_QUOTED_CHARS, cssEncode));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.yces"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yces (s)](#apidoc.element.xss-filters._privFilters.yces)
- description and source-code
```javascript
yces = function (s) {
    return cssBlacklist(htmlDecode(s).replace(CSS_SINGLE_QUOTED_CHARS, cssEncode));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.yceu"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yceu (s)](#apidoc.element.xss-filters._privFilters.yceu)
- description and source-code
```javascript
yceu = function (s) {
    s = htmlDecode(s);
    return CSS_VALID_VALUE.test(s) ? s : ";-x:'" + cssBlacklist(s.replace(CSS_SINGLE_QUOTED_CHARS, cssEncode)) + "';-v:";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.yceud"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yceud (s)](#apidoc.element.xss-filters._privFilters.yceud)
- description and source-code
```javascript
yceud = function (s) {
    return cssUrl(s);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.yceus"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yceus (s)](#apidoc.element.xss-filters._privFilters.yceus)
- description and source-code
```javascript
yceus = function (s) {
    return cssUrl(s).replace(SQUOT, '\\27 ');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.yceuu"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yceuu (s)](#apidoc.element.xss-filters._privFilters.yceuu)
- description and source-code
```javascript
yceuu = function (s) {
    return cssUrl(s).replace(CSS_UNQUOTED_URL, function (chr) {
        return  chr === '\''        ? '\\27 ' :
                chr === '('         ? '%28' :
                /* chr === ')' ? */   '%29';
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.yd"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yd (s)](#apidoc.element.xss-filters._privFilters.yd)
- description and source-code
```javascript
yd = function (s) {
    return strReplace(s, LT, '&lt;');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.yu"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yu ()](#apidoc.element.xss-filters._privFilters.yu)
- description and source-code
```javascript
function encodeURI() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.yubl"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yubl (s)](#apidoc.element.xss-filters._privFilters.yubl)
- description and source-code
```javascript
yubl = function (s) {
    return URI_BLACKLIST_PROTOCOLS[x.yup(s)] ? 'x-' + s : s;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.yublf"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yublf (s)](#apidoc.element.xss-filters._privFilters.yublf)
- description and source-code
```javascript
yublf = function (s) {
    return x.yubl(x.yufull(s));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.yuc"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yuc ()](#apidoc.element.xss-filters._privFilters.yuc)
- description and source-code
```javascript
function encodeURIComponent() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.yufull"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yufull (s)](#apidoc.element.xss-filters._privFilters.yufull)
- description and source-code
```javascript
yufull = function (s) {
    return x.yu(s).replace(URL_IPV6, function(m, p) {
        return '//[' + p + ']';
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xss-filters._privFilters.yup"></a>[function <span class="apidocSignatureSpan">xss-filters._privFilters.</span>yup (s)](#apidoc.element.xss-filters._privFilters.yup)
- description and source-code
```javascript
yup = function (s) {
    s = getProtocol(s.replace(NULL, ''));
    // URI_PROTOCOL_WHITESPACES is required for left trim and remove interim whitespaces
    return s ? htmlDecode(s, URI_PROTOCOL_NAMED_REF_MAP, null, true).replace(URI_PROTOCOL_WHITESPACES, '').toLowerCase() : null;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
