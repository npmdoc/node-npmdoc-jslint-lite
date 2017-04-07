# api documentation for  [jslint-lite (v2017.4.6)](https://github.com/kaizhu256/node-jslint-lite)  [![npm package](https://img.shields.io/npm/v/npmdoc-jslint-lite.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-jslint-lite) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-jslint-lite.svg)](https://travis-ci.org/npmdoc/node-npmdoc-jslint-lite)
#### this zero-dependency package will provide browser-compatible, classic-versions of jslint and csslint

[![NPM](https://nodei.co/npm/jslint-lite.png?downloads=true)](https://www.npmjs.com/package/jslint-lite)

[![apidoc](https://npmdoc.github.io/node-npmdoc-jslint-lite/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-jslint-lite%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-jslint-lite/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-jslint-lite/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-jslint-lite/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "kai zhu",
        "email": "kaizhu256@gmail.com"
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
            "name": "kaizhu",
            "email": "kaizhu256@gmail.com"
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
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module jslint-lite](#apidoc.module.jslint-lite)
1.  [function <span class="apidocSignatureSpan">jslint-lite.</span>CSSLint._Reporter (e, t)](#apidoc.element.jslint-lite.CSSLint._Reporter)
1.  [function <span class="apidocSignatureSpan">jslint-lite.</span>JSLINT (t, n)](#apidoc.element.jslint-lite.JSLINT)
1.  [function <span class="apidocSignatureSpan">jslint-lite.</span>jslintAndPrint (script, file)](#apidoc.element.jslint-lite.jslintAndPrint)
1.  [function <span class="apidocSignatureSpan">jslint-lite.</span>jslintEs6 (e, i, s)](#apidoc.element.jslint-lite.jslintEs6)
1.  object <span class="apidocSignatureSpan">jslint-lite.</span>CSSLint
1.  object <span class="apidocSignatureSpan">jslint-lite.</span>CSSLint.Util
1.  object <span class="apidocSignatureSpan">jslint-lite.</span>CSSLint._Reporter.prototype
1.  object <span class="apidocSignatureSpan">jslint-lite.</span>jslint
1.  object <span class="apidocSignatureSpan">jslint-lite.</span>local
1.  object <span class="apidocSignatureSpan">jslint-lite.</span>module
1.  string <span class="apidocSignatureSpan">jslint-lite.</span>__dirname
1.  string <span class="apidocSignatureSpan">jslint-lite.</span>modeJs

#### [module jslint-lite.CSSLint](#apidoc.module.jslint-lite.CSSLint)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>_Reporter (e, t)](#apidoc.element.jslint-lite.CSSLint._Reporter)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>addFormatter (e)](#apidoc.element.jslint-lite.CSSLint.addFormatter)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>addRule (t )](#apidoc.element.jslint-lite.CSSLint.addRule)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>clearRules ()](#apidoc.element.jslint-lite.CSSLint.clearRules)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>format (e, t, n, r)](#apidoc.element.jslint-lite.CSSLint.format)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>getFormatter (e)](#apidoc.element.jslint-lite.CSSLint.getFormatter)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>getRules ()](#apidoc.element.jslint-lite.CSSLint.getRules)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>getRuleset ()](#apidoc.element.jslint-lite.CSSLint.getRuleset)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>hasFormat (e)](#apidoc.element.jslint-lite.CSSLint.hasFormat)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>verify (t, r)](#apidoc.element.jslint-lite.CSSLint.verify)
1.  object <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>Util
1.  object <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>_listeners
1.  string <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>version

#### [module jslint-lite.CSSLint.Util](#apidoc.module.jslint-lite.CSSLint.Util)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint.Util.</span>forEach (e, t)](#apidoc.element.jslint-lite.CSSLint.Util.forEach)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint.Util.</span>indexOf (e, t)](#apidoc.element.jslint-lite.CSSLint.Util.indexOf)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint.Util.</span>mix (e, t)](#apidoc.element.jslint-lite.CSSLint.Util.mix)

#### [module jslint-lite.CSSLint._Reporter](#apidoc.module.jslint-lite.CSSLint._Reporter)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>_Reporter (e, t)](#apidoc.element.jslint-lite.CSSLint._Reporter._Reporter)

#### [module jslint-lite.CSSLint._Reporter.prototype](#apidoc.module.jslint-lite.CSSLint._Reporter.prototype)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint._Reporter.prototype.</span>constructor (e, t)](#apidoc.element.jslint-lite.CSSLint._Reporter.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint._Reporter.prototype.</span>error (e, t, n, r )](#apidoc.element.jslint-lite.CSSLint._Reporter.prototype.error)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint._Reporter.prototype.</span>info (e, t, n, r)](#apidoc.element.jslint-lite.CSSLint._Reporter.prototype.info)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint._Reporter.prototype.</span>report (e, t , n, r)](#apidoc.element.jslint-lite.CSSLint._Reporter.prototype.report)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint._Reporter.prototype.</span>rollupError (e, t)](#apidoc.element.jslint-lite.CSSLint._Reporter.prototype.rollupError)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint._Reporter.prototype.</span>rollupWarn (e, t)](#apidoc.element.jslint-lite.CSSLint._Reporter.prototype.rollupWarn)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint._Reporter.prototype.</span>stat (e, t)](#apidoc.element.jslint-lite.CSSLint._Reporter.prototype.stat)
1.  [function <span class="apidocSignatureSpan">jslint-lite.CSSLint._Reporter.prototype.</span>warn (e, t, n, r)](#apidoc.element.jslint-lite.CSSLint._Reporter.prototype.warn)

#### [module jslint-lite.JSLINT](#apidoc.module.jslint-lite.JSLINT)
1.  [function <span class="apidocSignatureSpan">jslint-lite.</span>JSLINT (t, n)](#apidoc.element.jslint-lite.JSLINT.JSLINT)
1.  [function <span class="apidocSignatureSpan">jslint-lite.JSLINT.</span>color (e)](#apidoc.element.jslint-lite.JSLINT.color)
1.  [function <span class="apidocSignatureSpan">jslint-lite.JSLINT.</span>data ( )](#apidoc.element.jslint-lite.JSLINT.data)
1.  [function <span class="apidocSignatureSpan">jslint-lite.JSLINT.</span>error_report (e)](#apidoc.element.jslint-lite.JSLINT.error_report)
1.  [function <span class="apidocSignatureSpan">jslint-lite.JSLINT.</span>jslint (t, n)](#apidoc.element.jslint-lite.JSLINT.jslint)
1.  [function <span class="apidocSignatureSpan">jslint-lite.JSLINT.</span>properties_report (e)](#apidoc.element.jslint-lite.JSLINT.properties_report)
1.  [function <span class="apidocSignatureSpan">jslint-lite.JSLINT.</span>report (e)](#apidoc.element.jslint-lite.JSLINT.report)
1.  string <span class="apidocSignatureSpan">jslint-lite.JSLINT.</span>edition



# <a name="apidoc.module.jslint-lite"></a>[module jslint-lite](#apidoc.module.jslint-lite)

#### <a name="apidoc.element.jslint-lite.CSSLint._Reporter"></a>[function <span class="apidocSignatureSpan">jslint-lite.</span>CSSLint._Reporter (e, t)](#apidoc.element.jslint-lite.CSSLint._Reporter)
- description and source-code
```javascript
function Reporter(e, t){this.messages=
[],this.stats=[],this.lines=e,this.ruleset=t}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint-lite.JSLINT"></a>[function <span class="apidocSignatureSpan">jslint-lite.</span>JSLINT (t, n)](#apidoc.element.jslint-lite.JSLINT)
- description and source-code
```javascript
JSLINT = function (t, n){var r,o,u;S.errors=[],S.tree="",S.properties="",i=P=X=O=Object
.create(W["(begin)"]),V=[],_=Object.create(null),st(U),H=Object.create(null);if(
n){M=Object.create(n),o=M.predef;if(o)if(Array.isArray(o))for(r=0;r<o.length;r+=1
)_[o[r]]=!0;else typeof o=="object"&&st(o)}else M=Object.create(null);M.indent=+
M.indent||4,M.maxerr=+M.maxerr||50,b=q=Object.create(null),y=m={scope:q,loopage:0
,level:0},g=[m],s=[],f=[],l=!1,w=!1,E=null,x=!1,C=[],L=!1,D=!0,z=!1,$=null,J=0,T
.init(t),ot();try{dt();if(O.id==="(number)")O.stop("unexpected_a");else switch(O
.id){case"{":case"[":l=!0,x=!0,ln();break;default:bt(1),O.id===";"&&!L&&(O.edge=!0
,dt(";")),u=tn(),i.first=u,S.tree=i,u.disrupt&&P.warn("weird_program")}E=null,dt
("(end)"),S.property=H}catch(a){a&&S.errors.push({reason:a.message,line:a.line||
O.line,character:a.character||O.from},null)}return S.errors.length===0}
```
- example usage
```shell
...
                '\u001b[90m \/\/ Line ' + (error.line + 1) +
                ', Pos ' + (error.column + 1) + '\u001b[39m\n';
        });
// jslint es5 script
} else {
    // comment shebang
    scriptParsed = scriptParsed.replace((/^#!/), '//');
    if (local.JSLINT(scriptParsed)) {
        return script;
    }
    // if error occurred, then print colorized error messages
    local.errorText = '\n\u001b[1m' + file + '\u001b[22m\n';
    local.JSLINT.errors
        .filter(function (error) {
            return error;
...
```

#### <a name="apidoc.element.jslint-lite.jslintAndPrint"></a>[function <span class="apidocSignatureSpan">jslint-lite.</span>jslintAndPrint (script, file)](#apidoc.element.jslint-lite.jslintAndPrint)
- description and source-code
```javascript
jslintAndPrint = function (script, file) {
<span class="apidocCodeCommentSpan">/*
 * this function will jslint / csslint the script and print any errors to stderr
 */
</span>    var ignoreDict, lineno, scriptParsed;
    // cleanup errors
    local.errorCounter = 0;
    local.errorText = '';
    // do nothing for empty script
    if (!script.length) {
        return script;
    }
    // init ignoreDict
    ignoreDict = {};
    // init lineno
    lineno = 0;
    // parse script
    scriptParsed = script
        // indent text-block
        // /* jslint-indent-begin */ ... /* jslint-indent-end */
        .replace(
/* jslint-indent-begin 20 */
(function () {
    /*jslint maxlen: 256*/
    return (/^ *?\/\* jslint-indent-begin (\d+?) \*\/$[\S\s]+?^ *?\/\* jslint-indent-end \*\/$/gm);
}()),
/* jslint-indent-end */
            function (match0, match1) {
                return match0.replace(
                    (/(^ *\S)/gm),
                    new Array(Number(match1) + 1).join(' ') + '$1'
                );
            }
        )
        // ignore text-block
        // /* jslint-ignore-begin */ ... /* jslint-ignore-end */
        .replace(
/* jslint-ignore-begin */
(/^ *?\/\* jslint-ignore-begin \*\/$[\S\s]+?^ *?\/\* jslint-ignore-end \*\/$/gm),
/* jslint-ignore-end */
            function (match0) {
                return match0.replace((/.*/g), '');
            }
        )
        // ignore next-line
        // /* jslint-ignore-next-line */
        .replace(
/* jslint-ignore-next-line */
(/^ *?\/\* jslint-ignore-next-line \*\/\n.*/gm),
            function (match0) {
                return match0.replace((/.*/g), '');
            }
        );
    // csslint script
    if (file.slice(-4) === '.css') {
        scriptParsed = scriptParsed.replace(new RegExp([
            // handle flexbox
            ' display: flex;',
            ' flex: .+?;',
            ' flex-.+?: .+?;'
        ].join('|'), 'g'), function () {
            return ' background: url(' + Math.random() + ');';
        });
        local.CSSLint.errors = local.CSSLint.verify(scriptParsed).messages
            .filter(function (error) {
                return !ignoreDict[error.rule.id];
            });
        // if error occurred, then print colorized error messages
        if (!local.CSSLint.errors.length) {
            return script;
        }
        local.errorText = '\n\u001b[1m' + file + '\u001b[22m\n';
        local.CSSLint.errors
            .filter(function (error) {
                return error;
            })
            .forEach(function (error) {
                local.errorCounter += 1;
                lineno += 1;
                local.errorText +=
                    (' #' + String(lineno) + ' ').slice(-4) +
                    '\u001b[33m' + error.type + ' - ' + error.rule.id +
                    ' - ' + error.message + '\n    ' + error.rule.desc +
                    '\u001b[39m\n    ' + String(error.evidence).trim() +
                    '\u001b[90m \/\/ line ' + error.line +
                    ', col ' + error.col + '\u001b[39m\n';
            });
    // jslint es6-script
    } else if ((/^\/\*jslint\b[\s\w,:]*?\bes6: true\b/m)
            .test(scriptParsed.slice(0, 0x1000))) {
        // comment shebang
        scriptParsed = scriptParsed.replace((/^#!/), '//');
        local.jslintEs6.errors = local.jslintEs6(scriptParsed).warnings;
        if (!local.jslintEs6.errors.length) {
            return script;
        }
        // if error occurred, then print colorized error messages
        local.errorText = '\n\u001b[1m' + file + '\u001b[22m\n';
        local.jslintEs6.errors
            .filter(function (error) {
                return error;
            })
            .forEach(function (error) {
                local.errorCounter += 1;
                lineno += 1;
                local.errorText +=
                    (' #' + String(lineno) + ' ').slice(-4) +
                    '\u001b[33m' + error.message +
                    '\u001b[39m\n    ' + String(error.a).trim() +
                    '\u001b[90m \/\/ Line ' + (error.line + 1) +
                    ', Pos ' + (error.column + 1) + '\u001 ...
```
- example usage
```shell
...
        document.querySelector('#testReportDiv1').style.display = 'none';
        document.querySelector('#testRunButton1').textContent = 'run internal test';
    }
    break;
// custom-case
default:
    // jslint #inputTextareaEval1
    local.jslint.jslintAndPrint(
        document.querySelector('#inputTextareaEval1').value,
        'inputTextareaEval1.js'
    );
    document.querySelector('#outputPreJslint1').textContent =
        local.jslint.errorText
        .replace((/\u001b\[\d+m/g), '')
        .trim();
...
```

#### <a name="apidoc.element.jslint-lite.jslintEs6"></a>[function <span class="apidocSignatureSpan">jslint-lite.</span>jslintEs6 (e, i, s)](#apidoc.element.jslint-lite.jslintEs6)
- description and source-code
```javascript
jslintEs6 = function (e, i, s){try{ft=[],Y=i||t(),H="anonymous",j=[],F=t(),q=!0,I=[],R=!0,U=t(
),z=[],W=Y.fudge?1:0,V=[],$={id:"(global)",body:!0,context:t(),from:0,level:0,line
:0,live:[],loop:0,"switch":0,thru:0},B=$,X=$,J=!1,et=!1,Q=!1,G=$,Z=t(),tt=[],ot=
undefined,rt=$,it=0,at=undefined,n(F,a,!1),s!==undefined&&n(F,s,!1),Object.keys(
Y).forEach(function(e){if(Y[e]===!0){var t=r[e];Array.isArray(t)&&n(F,t,!1)}}),gt
(e),Et(),J?(ut=St(),Et("(end)")):(Y.browser?G.id===";"&&Et(";"):G.value==="use strict"&&
($.strict=G,Et("(string)"),Et(";")),ut=Ot(),Et("(end)"),X=$,on(ut),Q&&$.strict!==
undefined&&vt("unexpected_a",$.strict),gn(),Y.white||yn()),Y.browser||I.forEach(
function(e){e.directive==="global"&&vt("missing_browser",e)}),R=!1}catch(o){o.name!=="JSLintError"&&
ft.push(o)}return{directives:I,edition:"2016-10-24",exports:U,froms:z,functions:
V,global:$,id:"(JSLint)",json:J,lines:K,module:Q===!0,ok:ft.length===0&&!R,option
:Y,property:Z,stop:R,tokens:st,tree:ut,warnings:ft.sort(function(e,t){return e.line-
t.line||e.column-t.column})}}
```
- example usage
```shell
...
                ', col ' + error.col + '\u001b[39m\n';
        });
// jslint es6-script
} else if ((/^\/\*jslint\b[\s\w,:]*?\bes6: true\b/m)
        .test(scriptParsed.slice(0, 0x1000))) {
    // comment shebang
    scriptParsed = scriptParsed.replace((/^#!/), '//');
    local.jslintEs6.errors = local.jslintEs6(scriptParsed).warnings;
    if (!local.jslintEs6.errors.length) {
        return script;
    }
    // if error occurred, then print colorized error messages
    local.errorText = '\n\u001b[1m' + file + '\u001b[22m\n';
    local.jslintEs6.errors
        .filter(function (error) {
...
```



# <a name="apidoc.module.jslint-lite.CSSLint"></a>[module jslint-lite.CSSLint](#apidoc.module.jslint-lite.CSSLint)

#### <a name="apidoc.element.jslint-lite.CSSLint._Reporter"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>_Reporter (e, t)](#apidoc.element.jslint-lite.CSSLint._Reporter)
- description and source-code
```javascript
function Reporter(e, t){this.messages=
[],this.stats=[],this.lines=e,this.ruleset=t}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint-lite.CSSLint.addFormatter"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>addFormatter (e)](#apidoc.element.jslint-lite.CSSLint.addFormatter)
- description and source-code
```javascript
addFormatter = function (e){
t[e.id]=e}
```
- example usage
```shell
...
({id:"checkstyle-xml",name:"Checkstyle XML format",startFormat:function(){return'<?xml version="1.0" encoding="utf-8"?><checkstyle
>'
},endFormat:function(){return"</checkstyle>"},readError:function(t,n){return'<file name="'+
e(t)+'"><error line="0" column="0" severty="error" message="'+e(n)+'"></error></file>'
},formatResults:function(t,n,r){var i=t.messages,s=[],o=function(e){return!!e&&"name"in
e?"net.csslint."+e.name.replace(/\s/g,""):""};return i.length>0&&(s.push('<file name="'+
n+'">'),CSSLint.Util.forEach(i,function(t,n){t.rollup||s.push('<error line="'+t.
line+'" column="'+t.col+'" severity="'+t.type+'"'+' message="'+e(t.message)+'" source="'+
o(t.rule)+'"/>')}),s.push("</file>")),s.join("")}})}(),CSSLint.addFormatter({id:"compact"
,name:"Compact, 'porcelain' format",startFormat:function(){return""},endFormat:function(
){return""},formatResults:function(e,t,n){var r=e.messages,i="";n=n||{};var s=function(
e){return e.charAt(0).toUpperCase()+e.slice(1)};return r.length===0?n.quiet?"":t+": Lint Free!"
:(CSSLint.Util.forEach(r,function(e,n){e.rollup?i+=t+": "+s(e.type)+" - "+e.message+"\n"
:i+=t+": "+"line "+e.line+", col "+e.col+", "+s(e.type)+" - "+e.message+"\n"}),i
)}}),CSSLint.addFormatter({id:"csslint-xml",name:"CSSLint XML format",startFormat
:function(){return'<?xml version="1.0" encoding="utf-8"?><csslint>'},endFormat:function(
...
```

#### <a name="apidoc.element.jslint-lite.CSSLint.addRule"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>addRule (t )](#apidoc.element.jslint-lite.CSSLint.addRule)
- description and source-code
```javascript
addRule = function (t ){e.push(t),e[t.id]=t}
```
- example usage
```shell
...
.push({type:"info",line:t,col:n,message:e,evidence:this.lines[t-1],rule:r})},rollupError
:function(e,t){this.messages.push({type:"error",rollup:!0,message:e,rule:t})},rollupWarn
:function(e,t){this.messages.push({type:"warning",rollup:!0,message:e,rule:t})},
stat:function(e,t){this.stats[e]=t}},CSSLint._Reporter=Reporter,CSSLint.Util={mix
:function(e,t){var n;for(n in t)t.hasOwnProperty(n)&&(e[n]=t[n]);return n},indexOf
:function(e,t){if(e.indexOf)return e.indexOf(t);for(var n=0,r=e.length;n<r;n++)if(
e[n]===t)return n;return-1},forEach:function(e,t){if(e.forEach)return e.forEach(
t);for(var n=0,r=e.length;n<r;n++)t(e[n],n,e)}},CSSLint.addRule({id:"adjoining-classes"
,name:"Disallow adjoining classes",desc:"Don't use adjoining classes.",browsers:"IE6"
,init:function(e,t){var n=this;e.addListener("startrule",function(r){var i=r.selectors
,s,o,u,a,f,l,c;for(f=0;f<i.length;f++){s=i[f];for(l=0;l<s.parts.length;l++){o=s.
parts[l];if(o.type==e.SELECTOR_PART_TYPE){a=0;for(c=0;c<o.modifiers.length;c++)u=
o.modifiers[c],u.type=="class"&&a++,a>1&&t.report("Don't use adjoining classes."
,o.line,o.col,n)}}}})}}),CSSLint.addRule({id:"box-model",name:"Beware of broken box size"
,desc:"Don't use width or height when using padding or border.",browsers:"All",init
...
```

#### <a name="apidoc.element.jslint-lite.CSSLint.clearRules"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>clearRules ()](#apidoc.element.jslint-lite.CSSLint.clearRules)
- description and source-code
```javascript
clearRules = function (){e=[]}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint-lite.CSSLint.format"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>format (e, t, n, r)](#apidoc.element.jslint-lite.CSSLint.format)
- description and source-code
```javascript
format = function (e, t, n, r){var i=
this.getFormatter(n),s=null;return i&&(s=i.startFormat(),s+=i.formatResults(e,t,
r||{}),s+=i.endFormat()),s}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint-lite.CSSLint.getFormatter"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>getFormatter (e)](#apidoc.element.jslint-lite.CSSLint.getFormatter)
- description and source-code
```javascript
getFormatter = function (e){return t[e]}
```
- example usage
```shell
...
:0,2:2,1:1,0:0},s.toLowerCase().split(",").forEach(function(e){var n=e.split(":"
),i=n[0]||"",s=n[1]||"";t[i.trim()]=r[s.trim()]})),t}var e=[],t=[],n=/\/\*csslint([^\*]*)\*\//
,r=new parserlib.util.EventTarget;return r.version="0.10.0",r.addRule=function(t
){e.push(t),e[t.id]=t},r.clearRules=function(){e=[]},r.getRules=function(){return[
].concat(e).sort(function(e,t){return e.id>t.id?1:0})},r.getRuleset=function(){var t=
{},n=0,r=e.length;while(n<r)t[e[n++].id]=1;return t},r.addFormatter=function(e){
t[e.id]=e},r.getFormatter=function(e){return t[e]},r.format=function(e,t,n,r){var i=
this.getFormatter(n),s=null;return i&&(s=i.startFormat(),s+=i.formatResults(e,t,
r||{}),s+=i.endFormat()),s},r.hasFormat=function(e){return t.hasOwnProperty(e)},
r.verify=function(t,r){var s=0,o=e.length,u,a,f,l=new parserlib.css.Parser({starHack
:!0,ieFilters:!0,underscoreHack:!0,strict:!1});a=t.replace(/\n\r?/g,"$split$").split
("$split$"),r||(r=this.getRuleset()),n.test(t)&&(r=i(t,r)),u=new Reporter(a,r),r
.errors=2;for(s in r)r.hasOwnProperty(s)&&r[s]&&e[s]&&e[s].init(l,u);try{l.parse
(t)}catch(c){u.error("Fatal error, cannot continue: "+c.message,c.line,c.col,{})
}return f={messages:u.messages,stats:u.stats,ruleset:u.ruleset},f.messages.sort(
...
```

#### <a name="apidoc.element.jslint-lite.CSSLint.getRules"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>getRules ()](#apidoc.element.jslint-lite.CSSLint.getRules)
- description and source-code
```javascript
getRules = function (){return[
].concat(e).sort(function(e,t){return e.id>t.id?1:0})}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint-lite.CSSLint.getRuleset"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>getRuleset ()](#apidoc.element.jslint-lite.CSSLint.getRuleset)
- description and source-code
```javascript
getRuleset = function (){var t=
{},n=0,r=e.length;while(n<r)t[e[n++].id]=1;return t}
```
- example usage
```shell
...
].concat(e).sort(function(e,t){return e.id>t.id?1:0})},r.getRuleset=function(){var t=
{},n=0,r=e.length;while(n<r)t[e[n++].id]=1;return t},r.addFormatter=function(e){
t[e.id]=e},r.getFormatter=function(e){return t[e]},r.format=function(e,t,n,r){var i=
this.getFormatter(n),s=null;return i&&(s=i.startFormat(),s+=i.formatResults(e,t,
r||{}),s+=i.endFormat()),s},r.hasFormat=function(e){return t.hasOwnProperty(e)},
r.verify=function(t,r){var s=0,o=e.length,u,a,f,l=new parserlib.css.Parser({starHack
:!0,ieFilters:!0,underscoreHack:!0,strict:!1});a=t.replace(/\n\r?/g,"$split$").split
("$split$"),r||(r=this.getRuleset()),n.test(t)&&(r=i(t,r)),u=new Reporter(a,r),r
.errors=2;for(s in r)r.hasOwnProperty(s)&&r[s]&&e[s]&&e[s].init(l,u);try{l.parse
(t)}catch(c){u.error("Fatal error, cannot continue: "+c.message,c.line,c.col,{})
}return f={messages:u.messages,stats:u.stats,ruleset:u.ruleset},f.messages.sort(
function(e,t){return e.rollup&&!t.rollup?1:!e.rollup&&t.rollup?-1:e.line-t.line}
),f},r}();return Reporter.prototype={constructor:Reporter,error:function(e,t,n,r
){this.messages.push({type:"error",line:t,col:n,message:e,evidence:this.lines[t-1
],rule:r||{}})},warn:function(e,t,n,r){this.report(e,t,n,r)},report:function(e,t
...
```

#### <a name="apidoc.element.jslint-lite.CSSLint.hasFormat"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>hasFormat (e)](#apidoc.element.jslint-lite.CSSLint.hasFormat)
- description and source-code
```javascript
hasFormat = function (e){return t.hasOwnProperty(e)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint-lite.CSSLint.verify"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>verify (t, r)](#apidoc.element.jslint-lite.CSSLint.verify)
- description and source-code
```javascript
verify = function (t, r){var s=0,o=e.length,u,a,f,l=new parserlib.css.Parser({starHack
:!0,ieFilters:!0,underscoreHack:!0,strict:!1});a=t.replace(/\n\r?/g,"$split$").split
("$split$"),r||(r=this.getRuleset()),n.test(t)&&(r=i(t,r)),u=new Reporter(a,r),r
.errors=2;for(s in r)r.hasOwnProperty(s)&&r[s]&&e[s]&&e[s].init(l,u);try{l.parse
(t)}catch(c){u.error("Fatal error, cannot continue: "+c.message,c.line,c.col,{})
}return f={messages:u.messages,stats:u.stats,ruleset:u.ruleset},f.messages.sort(
function(e,t){return e.rollup&&!t.rollup?1:!e.rollup&&t.rollup?-1:e.line-t.line}
),f}
```
- example usage
```shell
...
    // handle flexbox
    ' display: flex;',
    ' flex: .+?;',
    ' flex-.+?: .+?;'
].join('|'), 'g'), function () {
    return ' background: url(' + Math.random() + ');';
});
local.CSSLint.errors = local.CSSLint.verify(scriptParsed).messages
    .filter(function (error) {
        return !ignoreDict[error.rule.id];
    });
// if error occurred, then print colorized error messages
if (!local.CSSLint.errors.length) {
    return script;
}
...
```



# <a name="apidoc.module.jslint-lite.CSSLint.Util"></a>[module jslint-lite.CSSLint.Util](#apidoc.module.jslint-lite.CSSLint.Util)

#### <a name="apidoc.element.jslint-lite.CSSLint.Util.forEach"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint.Util.</span>forEach (e, t)](#apidoc.element.jslint-lite.CSSLint.Util.forEach)
- description and source-code
```javascript
forEach = function (e, t){if(e.forEach)return e.forEach(
t);for(var n=0,r=e.length;n<r;n++)t(e[n],n,e)}
```
- example usage
```shell
...
    event.currentTarget &&
    event.currentTarget.className &&
    event.currentTarget.className.includes &&
    event.currentTarget.className.includes('onreset'))) {
// reset output
Array.from(
    document.querySelectorAll('body > .resettable')
).forEach(function (element) {
    switch (element.tagName) {
    case 'INPUT':
    case 'TEXTAREA':
        element.value = '';
        break;
    default:
        element.textContent = '';
...
```

#### <a name="apidoc.element.jslint-lite.CSSLint.Util.indexOf"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint.Util.</span>indexOf (e, t)](#apidoc.element.jslint-lite.CSSLint.Util.indexOf)
- description and source-code
```javascript
indexOf = function (e, t){if(e.indexOf)return e.indexOf(t);for(var n=0,r=e.length;n<r;n++)if(
e[n]===t)return n;return-1}
```
- example usage
```shell
...
mark:function(){this._bookmark={cursor:this._cursor,line:this._line,col:this._col
}},reset:function(){this._bookmark&&(this._cursor=this._bookmark.cursor,this._line=
this._bookmark.line,this._col=this._bookmark.col,delete this._bookmark)},readTo:
function(e){var t="",n;while(t.length<e.length||t.lastIndexOf(e)!=t.length-e.length
){n=this.read();if(!n)throw new Error('Expected "'+e+'" at line '+this._line+", col "+
this._col+".");t+=n}return t},readWhile:function(e){var t="",n=this.read();while(
n!==null&&e(n))t+=n,n=this.read();return t},readMatch:function(e){var t=this._input
.substring(this._cursor),n=null;return typeof e=="string"?t.indexOf(e)===0&&(n=this
.readCount(e.length)):e instanceof RegExp&&e.test(t)&&(n=this.readCount(RegExp.lastMatch
.length)),n},readCount:function(e){var t="";while(e--)t+=this.read();return t}},
n.prototype=new Error,r.fromToken=function(e){return new r(e.value,e.startLine,e
.startCol)},r.prototype={constructor:r,valueOf:function(){return this.toString()
},toString:function(){return this.text}},i.createTokenData=function(e){var t=[],
n={},r=e.concat([]),i=0,s=r.length+1;r.UNKNOWN=-1,r.unshift({name:"EOF"});for(;i<
s;i++)t.push(r[i].name),r[r[i].name]=i,r[i].text&&(n[r[i].text]=i);return r.name=
...
```

#### <a name="apidoc.element.jslint-lite.CSSLint.Util.mix"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint.Util.</span>mix (e, t)](#apidoc.element.jslint-lite.CSSLint.Util.mix)
- description and source-code
```javascript
mix = function (e, t){var n;for(n in t)t.hasOwnProperty(n)&&(e[n]=t[n]);return n}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint-lite.CSSLint._Reporter"></a>[module jslint-lite.CSSLint._Reporter](#apidoc.module.jslint-lite.CSSLint._Reporter)

#### <a name="apidoc.element.jslint-lite.CSSLint._Reporter._Reporter"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint.</span>_Reporter (e, t)](#apidoc.element.jslint-lite.CSSLint._Reporter._Reporter)
- description and source-code
```javascript
function Reporter(e, t){this.messages=
[],this.stats=[],this.lines=e,this.ruleset=t}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint-lite.CSSLint._Reporter.prototype"></a>[module jslint-lite.CSSLint._Reporter.prototype](#apidoc.module.jslint-lite.CSSLint._Reporter.prototype)

#### <a name="apidoc.element.jslint-lite.CSSLint._Reporter.prototype.constructor"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint._Reporter.prototype.</span>constructor (e, t)](#apidoc.element.jslint-lite.CSSLint._Reporter.prototype.constructor)
- description and source-code
```javascript
function Reporter(e, t){this.messages=
[],this.stats=[],this.lines=e,this.ruleset=t}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint-lite.CSSLint._Reporter.prototype.error"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint._Reporter.prototype.</span>error (e, t, n, r )](#apidoc.element.jslint-lite.CSSLint._Reporter.prototype.error)
- description and source-code
```javascript
error = function (e, t, n, r ){this.messages.push({type:"error",line:t,col:n,message:e,evidence:this.lines[t-1
],rule:r||{}})}
```
- example usage
```shell
...
            event.currentTarget.className.includes &&
            event.currentTarget.className.includes('oneval')))) {
        // try to eval input-code
        try {
            /*jslint evil: true*/
            eval(document.querySelector('#inputTextareaEval1').value);
        } catch (errorCaught) {
            console.error(errorCaught.stack);
        }
    }
};
// log stderr and stdout to #outputTextareaStdout1
['error', 'log'].forEach(function (key) {
    console[key + '_original'] = console[key];
    console[key] = function () {
...
```

#### <a name="apidoc.element.jslint-lite.CSSLint._Reporter.prototype.info"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint._Reporter.prototype.</span>info (e, t, n, r)](#apidoc.element.jslint-lite.CSSLint._Reporter.prototype.info)
- description and source-code
```javascript
info = function (e, t, n, r){this.messages
.push({type:"info",line:t,col:n,message:e,evidence:this.lines[t-1],rule:r})}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint-lite.CSSLint._Reporter.prototype.report"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint._Reporter.prototype.</span>report (e, t , n, r)](#apidoc.element.jslint-lite.CSSLint._Reporter.prototype.report)
- description and source-code
```javascript
report = function (e, t , n, r){this.messages.push({type:this.ruleset[r.id]==2?"error":"warning",line:t,col
:n,message:e,evidence:this.lines[t-1],rule:r})}
```
- example usage
```shell
...
("$split$"),r||(r=this.getRuleset()),n.test(t)&&(r=i(t,r)),u=new Reporter(a,r),r
.errors=2;for(s in r)r.hasOwnProperty(s)&&r[s]&&e[s]&&e[s].init(l,u);try{l.parse
(t)}catch(c){u.error("Fatal error, cannot continue: "+c.message,c.line,c.col,{})
}return f={messages:u.messages,stats:u.stats,ruleset:u.ruleset},f.messages.sort(
function(e,t){return e.rollup&&!t.rollup?1:!e.rollup&&t.rollup?-1:e.line-t.line}
),f},r}();return Reporter.prototype={constructor:Reporter,error:function(e,t,n,r
){this.messages.push({type:"error",line:t,col:n,message:e,evidence:this.lines[t-1
],rule:r||{}})},warn:function(e,t,n,r){this.report(e,t,n,r)},report:function(e,t
,n,r){this.messages.push({type:this.ruleset[r.id]==2?"error":"warning",line:t,col
:n,message:e,evidence:this.lines[t-1],rule:r})},info:function(e,t,n,r){this.messages
.push({type:"info",line:t,col:n,message:e,evidence:this.lines[t-1],rule:r})},rollupError
:function(e,t){this.messages.push({type:"error",rollup:!0,message:e,rule:t})},rollupWarn
:function(e,t){this.messages.push({type:"warning",rollup:!0,message:e,rule:t})},
stat:function(e,t){this.stats[e]=t}},CSSLint._Reporter=Reporter,CSSLint.Util={mix
:function(e,t){var n;for(n in t)t.hasOwnProperty(n)&&(e[n]=t[n]);return n},indexOf
...
```

#### <a name="apidoc.element.jslint-lite.CSSLint._Reporter.prototype.rollupError"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint._Reporter.prototype.</span>rollupError (e, t)](#apidoc.element.jslint-lite.CSSLint._Reporter.prototype.rollupError)
- description and source-code
```javascript
rollupError = function (e, t){this.messages.push({type:"error",rollup:!0,message:e,rule:t})}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint-lite.CSSLint._Reporter.prototype.rollupWarn"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint._Reporter.prototype.</span>rollupWarn (e, t)](#apidoc.element.jslint-lite.CSSLint._Reporter.prototype.rollupWarn)
- description and source-code
```javascript
rollupWarn = function (e, t){this.messages.push({type:"warning",rollup:!0,message:e,rule:t})}
```
- example usage
```shell
...
a<l)u[a].type=="color"&&("alpha"in u[a]||"hue"in u[a]?(/([^\)]+)\(/.test(u[a])&&
(f=RegExp.$1.toUpperCase()),(!r||r.property.text.toLowerCase()!=o||r.colorType!="compat"
)&&t.report("Fallback "+o+" (hex or RGB) should precede "+f+" "+o+".",e.line,e.col
,n)):e.colorType="compat"),a++;r=e})}}),CSSLint.addRule({id:"floats",name:"Disallow too many floats"
,desc:"This rule tests if the float property is used too many times",browsers:"All"
,init:function(e,t){var n=this,r=0;e.addListener("property",function(e){e.property
.text.toLowerCase()=="float"&&e.value.text.toLowerCase()!="none"&&r++}),e.addListener
("endstylesheet",function(){t.stat("floats",r),r>=10&&t.rollupWarn("Too many floats ("+
r+"), you're probably using them for layout. Consider using a grid system instead."
,n)})}}),CSSLint.addRule({id:"font-faces",name:"Don't use too many web fonts",desc
:"Too many different web fonts in the same stylesheet.",browsers:"All",init:function(
e,t){var n=this,r=0;e.addListener("startfontface",function(){r++}),e.addListener
("endstylesheet",function(){r>5&&t.rollupWarn("Too many @font-face declarations ("+
r+").",n)})}}),CSSLint.addRule({id:"font-sizes",name:"Disallow too many font sizes"
,desc:"Checks the number of font-size declarations.",browsers:"All",init:function(
...
```

#### <a name="apidoc.element.jslint-lite.CSSLint._Reporter.prototype.stat"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint._Reporter.prototype.</span>stat (e, t)](#apidoc.element.jslint-lite.CSSLint._Reporter.prototype.stat)
- description and source-code
```javascript
stat = function (e, t){this.stats[e]=t}
```
- example usage
```shell
...
a<l)u[a].type=="color"&&("alpha"in u[a]||"hue"in u[a]?(/([^\)]+)\(/.test(u[a])&&
(f=RegExp.$1.toUpperCase()),(!r||r.property.text.toLowerCase()!=o||r.colorType!="compat"
)&&t.report("Fallback "+o+" (hex or RGB) should precede "+f+" "+o+".",e.line,e.col
,n)):e.colorType="compat"),a++;r=e})}}),CSSLint.addRule({id:"floats",name:"Disallow too many floats"
,desc:"This rule tests if the float property is used too many times",browsers:"All"
,init:function(e,t){var n=this,r=0;e.addListener("property",function(e){e.property
.text.toLowerCase()=="float"&&e.value.text.toLowerCase()!="none"&&r++}),e.addListener
("endstylesheet",function(){t.stat("floats",r),r>=10&&t.rollupWarn("Too many floats ("+
r+"), you're probably using them for layout. Consider using a grid system instead."
,n)})}}),CSSLint.addRule({id:"font-faces",name:"Don't use too many web fonts",desc
:"Too many different web fonts in the same stylesheet.",browsers:"All",init:function(
e,t){var n=this,r=0;e.addListener("startfontface",function(){r++}),e.addListener
("endstylesheet",function(){r>5&&t.rollupWarn("Too many @font-face declarations ("+
r+").",n)})}}),CSSLint.addRule({id:"font-sizes",name:"Disallow too many font sizes"
,desc:"Checks the number of font-size declarations.",browsers:"All",init:function(
...
```

#### <a name="apidoc.element.jslint-lite.CSSLint._Reporter.prototype.warn"></a>[function <span class="apidocSignatureSpan">jslint-lite.CSSLint._Reporter.prototype.</span>warn (e, t, n, r)](#apidoc.element.jslint-lite.CSSLint._Reporter.prototype.warn)
- description and source-code
```javascript
warn = function (e, t, n, r){this.report(e,t,n,r)}
```
- example usage
```shell
...
),M.rhino&&(st(I),M.rhino=!1)}function ut(e){return e||(e=O),e.id==="(number)"?e
.number:e.string}function at(e,t,n){throw{name:"JSLintError",line:t,character:n,
message:u.scanned_a_b.supplant({a:u[e]||e,b:Math.floor(t/N.length*100)})}}function ft
(e,t,n,r,i,s,o){var a={id:"(error)",raw:u[e]||e,code:e,evidence:N[t-1]||"",line:
t,character:n,a:r||ut(this),b:i,c:s,d:o};return a.reason=a.raw.supplant(a),S.errors
.push(a),M.passfail&&at("stopping",t,n),J+=1,J>=M.maxerr&&at("too_many",t,n),a}function lt
(e,t,n,r,i,s,o){var u=ft(e,t,n,r,i,s,o);at("stopping",u.line,u.character)}function ct
(e){!M.white&&O.from!==e&&O.warn("expected_a_at_b_c","",e,O.from)}function ht(e,
t){var n=t.string,r=q[n];t.dead=!1,t.init=!1,t.kind=e,t.master=r,t.used=0,t.writeable=!0
,e==="var"&&m===y?r||(_[n]===!1&&(t.writeable=!1),b[n]=t):(r&&(r.function===m?(r
.kind!=="exception"||e!=="exception"||!r.dead)&&t.warn("already_defined",n):r.function!==
y&&e==="var"&&t.warn("redefinition_a_b",n,r.line)),q[n]=t,e==="var"&&s.push(n))}
function pt(e){var t,n=0;e=e||0;while(n<=e)t=C[n],t||(t=C[n]=T.token()),n+=1;return t
}function dt(e,t){if(E){if($&&O.line!==X.line){if(($!==E||!O.edge)&&O.from===E.at-
(O.edge?M.indent:0)){var r=E;for(;;){r.at-=M.indent;if(r===$)break;r=r.was}r.open=!1
...
```



# <a name="apidoc.module.jslint-lite.JSLINT"></a>[module jslint-lite.JSLINT](#apidoc.module.jslint-lite.JSLINT)

#### <a name="apidoc.element.jslint-lite.JSLINT.JSLINT"></a>[function <span class="apidocSignatureSpan">jslint-lite.</span>JSLINT (t, n)](#apidoc.element.jslint-lite.JSLINT.JSLINT)
- description and source-code
```javascript
JSLINT = function (t, n){var r,o,u;S.errors=[],S.tree="",S.properties="",i=P=X=O=Object
.create(W["(begin)"]),V=[],_=Object.create(null),st(U),H=Object.create(null);if(
n){M=Object.create(n),o=M.predef;if(o)if(Array.isArray(o))for(r=0;r<o.length;r+=1
)_[o[r]]=!0;else typeof o=="object"&&st(o)}else M=Object.create(null);M.indent=+
M.indent||4,M.maxerr=+M.maxerr||50,b=q=Object.create(null),y=m={scope:q,loopage:0
,level:0},g=[m],s=[],f=[],l=!1,w=!1,E=null,x=!1,C=[],L=!1,D=!0,z=!1,$=null,J=0,T
.init(t),ot();try{dt();if(O.id==="(number)")O.stop("unexpected_a");else switch(O
.id){case"{":case"[":l=!0,x=!0,ln();break;default:bt(1),O.id===";"&&!L&&(O.edge=!0
,dt(";")),u=tn(),i.first=u,S.tree=i,u.disrupt&&P.warn("weird_program")}E=null,dt
("(end)"),S.property=H}catch(a){a&&S.errors.push({reason:a.message,line:a.line||
O.line,character:a.character||O.from},null)}return S.errors.length===0}
```
- example usage
```shell
...
                '\u001b[90m \/\/ Line ' + (error.line + 1) +
                ', Pos ' + (error.column + 1) + '\u001b[39m\n';
        });
// jslint es5 script
} else {
    // comment shebang
    scriptParsed = scriptParsed.replace((/^#!/), '//');
    if (local.JSLINT(scriptParsed)) {
        return script;
    }
    // if error occurred, then print colorized error messages
    local.errorText = '\n\u001b[1m' + file + '\u001b[22m\n';
    local.JSLINT.errors
        .filter(function (error) {
            return error;
...
```

#### <a name="apidoc.element.jslint-lite.JSLINT.color"></a>[function <span class="apidocSignatureSpan">jslint-lite.JSLINT.</span>color (e)](#apidoc.element.jslint-lite.JSLINT.color)
- description and source-code
```javascript
color = function (e){var t,n=1,r,i,s=[],o,u=e.tokens[0];
while(u&&u.id!=="(end)"){t=u.from,i=u.line,o=u.thru,r=u.function.level;do o=u.thru
,u=e.tokens[n],n+=1;while(u&&u.line===i&&u.from-o<5&&r===u.function.level);s.push
({line:i,level:r,from:t,thru:o})}return s}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint-lite.JSLINT.data"></a>[function <span class="apidocSignatureSpan">jslint-lite.JSLINT.</span>data ( )](#apidoc.element.jslint-lite.JSLINT.data)
- description and source-code
```javascript
data = function ( ){function s(e){var n=i[e].kind;switch(n){case"var":case"exception":case"label":
t[n].push(e)}}var e={functions:[]},t,n,r,i;e.errors=S.errors,e.json=x,e.global=cn
(Object.keys(b));for(n=1;n<g.length;n+=1)r=g[n],t={name:r.name,line:r.line,level
:r.level,parameter:r.parameter,"var":[],exception:[],closure:cn(r.closure),outer
:cn(r.outer),global:cn(r.global),label:[]},i=r.scope,Object.keys(i).forEach(s),t
.var.sort(),t.exception.sort(),t.label.sort(),e.functions.push(t);return e.tokens=
V,e}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint-lite.JSLINT.error_report"></a>[function <span class="apidocSignatureSpan">jslint-lite.JSLINT.</span>error_report (e)](#apidoc.element.jslint-lite.JSLINT.error_report)
- description and source-code
```javascript
error_report = function (e){var t,n,r=[],i;if(e.errors.length){e.json&&r.push
("<cite>JSON: bad.</cite><br>");for(n=0;n<e.errors.length;n+=1)i=e.errors[n],i&&
(t=i.evidence||"",r.push("<cite>"),isFinite(i.line)&&r.push("<address>line "+String
(i.line)+" character "+String(i.character)+"</address>"),r.push(i.reason.entityify
()+"</cite>"),t&&r.push("<pre>"+t.entityify()+"</pre>"))}return r.join("")}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint-lite.JSLINT.jslint"></a>[function <span class="apidocSignatureSpan">jslint-lite.JSLINT.</span>jslint (t, n)](#apidoc.element.jslint-lite.JSLINT.jslint)
- description and source-code
```javascript
jslint = function (t, n){var r,o,u;S.errors=[],S.tree="",S.properties="",i=P=X=O=Object
.create(W["(begin)"]),V=[],_=Object.create(null),st(U),H=Object.create(null);if(
n){M=Object.create(n),o=M.predef;if(o)if(Array.isArray(o))for(r=0;r<o.length;r+=1
)_[o[r]]=!0;else typeof o=="object"&&st(o)}else M=Object.create(null);M.indent=+
M.indent||4,M.maxerr=+M.maxerr||50,b=q=Object.create(null),y=m={scope:q,loopage:0
,level:0},g=[m],s=[],f=[],l=!1,w=!1,E=null,x=!1,C=[],L=!1,D=!0,z=!1,$=null,J=0,T
.init(t),ot();try{dt();if(O.id==="(number)")O.stop("unexpected_a");else switch(O
.id){case"{":case"[":l=!0,x=!0,ln();break;default:bt(1),O.id===";"&&!L&&(O.edge=!0
,dt(";")),u=tn(),i.first=u,S.tree=i,u.disrupt&&P.warn("weird_program")}E=null,dt
("(end)"),S.property=H}catch(a){a&&S.errors.push({reason:a.message,line:a.line||
O.line,character:a.character||O.from},null)}return S.errors.length===0}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint-lite.JSLINT.properties_report"></a>[function <span class="apidocSignatureSpan">jslint-lite.JSLINT.</span>properties_report (e)](#apidoc.element.jslint-lite.JSLINT.properties_report)
- description and source-code
```javascript
properties_report = function (e){if(!
e)return"";var t,n,r=Object.keys(e).sort(),i="   ",s,o=!1,u=["/*properties"];for(
t=0;t<r.length;t+=1)n=r[t],e[n]>0&&(o&&(i+=","),s=G.test(n)?n:"'"+n.replace(et,it
)+"'",i.length+s.length>=80?(u.push(i),i="    "):i+=" ",i+=s,o=!0);return u.push
(i,"*/\n"),u.join("\n")}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint-lite.JSLINT.report"></a>[function <span class="apidocSignatureSpan">jslint-lite.JSLINT.</span>report (e)](#apidoc.element.jslint-lite.JSLINT.report)
- description and source-code
```javascript
report = function (e){function u(e,t){var n=!1;t.length&&(s.push("<dt>"+e+"</dt><dd>"),t.forEach
(function(e){s.push((n?", ":"")+e),n=!0}),s.push("</dd>"))}var t,n,r,i,s=[],o;s.
push("<dl class=level0>"),e.global.length?(u("global",e.global),t=!0):e.json?e.errors
.length||s.push("<dt>JSON: good.</dt>"):s.push("<dt><i>No new global variables introduced.</i></dt>"
),t?s.push("</dl>"):s[0]="";if(e.functions)for(n=0;n<e.functions.length;n+=1){o=
e.functions[n],i=[];if(o.params)for(r=0;r<o.params.length;r+=1)i[r]=o.params[r].
string;s.push("<dl class=level"+o.level+"><address>line "+String(o.line)+"</address>"+
o.name.entityify()),u("parameter",o.parameter),u("variable",o.var),u("exception"
,o.exception),u("closure",o.closure),u("outer",o.outer),u("global",o.global),u("label"
,o.label),s.push("</dl>")}return s.join("")}
```
- example usage
```shell
...
("$split$"),r||(r=this.getRuleset()),n.test(t)&&(r=i(t,r)),u=new Reporter(a,r),r
.errors=2;for(s in r)r.hasOwnProperty(s)&&r[s]&&e[s]&&e[s].init(l,u);try{l.parse
(t)}catch(c){u.error("Fatal error, cannot continue: "+c.message,c.line,c.col,{})
}return f={messages:u.messages,stats:u.stats,ruleset:u.ruleset},f.messages.sort(
function(e,t){return e.rollup&&!t.rollup?1:!e.rollup&&t.rollup?-1:e.line-t.line}
),f},r}();return Reporter.prototype={constructor:Reporter,error:function(e,t,n,r
){this.messages.push({type:"error",line:t,col:n,message:e,evidence:this.lines[t-1
],rule:r||{}})},warn:function(e,t,n,r){this.report(e,t,n,r)},report:function(e,t
,n,r){this.messages.push({type:this.ruleset[r.id]==2?"error":"warning",line:t,col
:n,message:e,evidence:this.lines[t-1],rule:r})},info:function(e,t,n,r){this.messages
.push({type:"info",line:t,col:n,message:e,evidence:this.lines[t-1],rule:r})},rollupError
:function(e,t){this.messages.push({type:"error",rollup:!0,message:e,rule:t})},rollupWarn
:function(e,t){this.messages.push({type:"warning",rollup:!0,message:e,rule:t})},
stat:function(e,t){this.stats[e]=t}},CSSLint._Reporter=Reporter,CSSLint.Util={mix
:function(e,t){var n;for(n in t)t.hasOwnProperty(n)&&(e[n]=t[n]);return n},indexOf
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
