# api documentation for  [fast-csv (v2.4.0)](http://c2fo.github.com/fast-csv/index.html)  [![npm package](https://img.shields.io/npm/v/npmdoc-fast-csv.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-fast-csv) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-fast-csv.svg)](https://travis-ci.org/npmdoc/node-npmdoc-fast-csv)
#### CSV parser and writer

[![NPM](https://nodei.co/npm/fast-csv.png?downloads=true)](https://www.npmjs.com/package/fast-csv)

[![apidoc](https://npmdoc.github.io/node-npmdoc-fast-csv/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-fast-csv_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-fast-csv/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-fast-csv/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-fast-csv/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Doug Martin"
    },
    "bugs": {
        "url": "https://github.com/C2FO/fast-csv/issues"
    },
    "dependencies": {
        "extended": "0.0.6",
        "is-extended": "0.0.10",
        "object-extended": "0.0.7",
        "string-extended": "0.0.8"
    },
    "description": "CSV parser and writer",
    "devDependencies": {
        "grunt": "~0.4.1",
        "grunt-contrib-jshint": "~0.10.0",
        "grunt-exec": "^0.4.5",
        "grunt-gh-pages": "^2.0.0",
        "grunt-it": "^1.0.0",
        "it": "^1.0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "f6e93185b6d290e5808948869c3fd09f64fbc842",
        "tarball": "https://registry.npmjs.org/fast-csv/-/fast-csv-2.4.0.tgz"
    },
    "engines": {
        "node": ">=4.0.0"
    },
    "gitHead": "5cf10be9bc9dbc87abfce04ccf2a03dd5d1f8a9e",
    "homepage": "http://c2fo.github.com/fast-csv/index.html",
    "keywords": [
        "csv",
        "parser",
        "fast",
        "writer",
        "csv writer",
        "CSV"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "damartin",
            "email": "doug@dougamartin.com"
        },
        {
            "name": "dustinsmith1024",
            "email": "dds1024@gmail.com"
        }
    ],
    "name": "fast-csv",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/C2FO/fast-csv.git"
    },
    "scripts": {
        "test": "grunt jshint it"
    },
    "version": "2.4.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module fast-csv](#apidoc.module.fast-csv)
1.  [function <span class="apidocSignatureSpan">fast-csv.</span>createReadStream (options)](#apidoc.element.fast-csv.createReadStream)
1.  [function <span class="apidocSignatureSpan">fast-csv.</span>createWriteStream (options)](#apidoc.element.fast-csv.createWriteStream)
1.  [function <span class="apidocSignatureSpan">fast-csv.</span>extended (obj)](#apidoc.element.fast-csv.extended)
1.  [function <span class="apidocSignatureSpan">fast-csv.</span>format (options)](#apidoc.element.fast-csv.format)
1.  [function <span class="apidocSignatureSpan">fast-csv.</span>fromPath (location, options)](#apidoc.element.fast-csv.fromPath)
1.  [function <span class="apidocSignatureSpan">fast-csv.</span>fromStream (stream, options)](#apidoc.element.fast-csv.fromStream)
1.  [function <span class="apidocSignatureSpan">fast-csv.</span>fromString (string, options)](#apidoc.element.fast-csv.fromString)
1.  [function <span class="apidocSignatureSpan">fast-csv.</span>parse ()](#apidoc.element.fast-csv.parse)
1.  [function <span class="apidocSignatureSpan">fast-csv.</span>write (arr, options, ws)](#apidoc.element.fast-csv.write)
1.  [function <span class="apidocSignatureSpan">fast-csv.</span>writeToBuffer (arr, options, cb)](#apidoc.element.fast-csv.writeToBuffer)
1.  [function <span class="apidocSignatureSpan">fast-csv.</span>writeToPath (path, arr, options)](#apidoc.element.fast-csv.writeToPath)
1.  [function <span class="apidocSignatureSpan">fast-csv.</span>writeToStream (ws, arr, options)](#apidoc.element.fast-csv.writeToStream)
1.  [function <span class="apidocSignatureSpan">fast-csv.</span>writeToString (arr, options, cb)](#apidoc.element.fast-csv.writeToString)

#### [module fast-csv.extended](#apidoc.module.fast-csv.extended)
1.  [function <span class="apidocSignatureSpan">fast-csv.</span>extended (obj)](#apidoc.element.fast-csv.extended.extended)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>asyncEach (arr, iter, cb)](#apidoc.element.fast-csv.extended.asyncEach)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>contains (arr, obj)](#apidoc.element.fast-csv.extended.contains)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>containsAt (arr, obj, index)](#apidoc.element.fast-csv.extended.containsAt)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>deepEqual (actual, expected)](#apidoc.element.fast-csv.extended.deepEqual)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>deepMerge (obj)](#apidoc.element.fast-csv.extended.deepMerge)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>define (tester, decorate)](#apidoc.element.fast-csv.extended.define)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>escape (str, except)](#apidoc.element.fast-csv.extended.escape)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>expose ()](#apidoc.element.fast-csv.extended.expose)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>extend (supr)](#apidoc.element.fast-csv.extended.extend)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>format (str, obj)](#apidoc.element.fast-csv.extended.format)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>has (obj, prop)](#apidoc.element.fast-csv.extended.has)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>instanceOf (obj, clazz)](#apidoc.element.fast-csv.extended.instanceOf)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isArguments (object)](#apidoc.element.fast-csv.extended.isArguments)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isArray ()](#apidoc.element.fast-csv.extended.isArray)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isBoolean (obj)](#apidoc.element.fast-csv.extended.isBoolean)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isDate (obj)](#apidoc.element.fast-csv.extended.isDate)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isDefined (obj)](#apidoc.element.fast-csv.extended.isDefined)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isEmpty (str)](#apidoc.element.fast-csv.extended.isEmpty)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isEq (obj, obj2)](#apidoc.element.fast-csv.extended.isEq)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isFalse (obj)](#apidoc.element.fast-csv.extended.isFalse)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isFunction (obj)](#apidoc.element.fast-csv.extended.isFunction)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isGt (obj, obj2)](#apidoc.element.fast-csv.extended.isGt)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isGte (obj, obj2)](#apidoc.element.fast-csv.extended.isGte)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isHash (obj)](#apidoc.element.fast-csv.extended.isHash)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isIn (obj, arr)](#apidoc.element.fast-csv.extended.isIn)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isLength (obj, l)](#apidoc.element.fast-csv.extended.isLength)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isLike (obj, reg)](#apidoc.element.fast-csv.extended.isLike)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isLt (obj, obj2)](#apidoc.element.fast-csv.extended.isLt)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isLte (obj, obj2)](#apidoc.element.fast-csv.extended.isLte)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isNeq (obj, obj2)](#apidoc.element.fast-csv.extended.isNeq)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isNotIn (obj, arr)](#apidoc.element.fast-csv.extended.isNotIn)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isNotLength (obj, l)](#apidoc.element.fast-csv.extended.isNotLength)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isNotLike (obj, reg)](#apidoc.element.fast-csv.extended.isNotLike)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isNotNull (obj)](#apidoc.element.fast-csv.extended.isNotNull)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isNull (obj)](#apidoc.element.fast-csv.extended.isNull)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isNumber (obj)](#apidoc.element.fast-csv.extended.isNumber)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isObject (obj)](#apidoc.element.fast-csv.extended.isObject)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isRegExp (obj)](#apidoc.element.fast-csv.extended.isRegExp)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isSeq (obj, obj2)](#apidoc.element.fast-csv.extended.isSeq)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isSneq (obj, obj2)](#apidoc.element.fast-csv.extended.isSneq)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isString (obj)](#apidoc.element.fast-csv.extended.isString)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isTrue (obj)](#apidoc.element.fast-csv.extended.isTrue)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isUndefined (obj)](#apidoc.element.fast-csv.extended.isUndefined)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>isUndefinedOrNull (obj)](#apidoc.element.fast-csv.extended.isUndefinedOrNull)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>keys (obj)](#apidoc.element.fast-csv.extended.keys)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>merge (obj)](#apidoc.element.fast-csv.extended.merge)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>multiply (str, times)](#apidoc.element.fast-csv.extended.multiply)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>notContains (arr, obj)](#apidoc.element.fast-csv.extended.notContains)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>notContainsAt (arr, obj, index)](#apidoc.element.fast-csv.extended.notContainsAt)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>notHas (obj, prop)](#apidoc.element.fast-csv.extended.notHas)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>omit (hash, omitted)](#apidoc.element.fast-csv.extended.omit)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>pad (string, length, ch, end)](#apidoc.element.fast-csv.extended.pad)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>register (alias, extendWith)](#apidoc.element.fast-csv.extended.register)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>spreadArgs (f, args, scope)](#apidoc.element.fast-csv.extended.spreadArgs)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>style (str, options)](#apidoc.element.fast-csv.extended.style)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>switcher (obj)](#apidoc.element.fast-csv.extended.switcher)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>tester (obj)](#apidoc.element.fast-csv.extended.tester)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>toArray (testStr, delim)](#apidoc.element.fast-csv.extended.toArray)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>trim (str)](#apidoc.element.fast-csv.extended.trim)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>trimLeft (str)](#apidoc.element.fast-csv.extended.trimLeft)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>trimRight (str)](#apidoc.element.fast-csv.extended.trimRight)
1.  [function <span class="apidocSignatureSpan">fast-csv.extended.</span>truncate (string, length, end)](#apidoc.element.fast-csv.extended.truncate)
1.  object <span class="apidocSignatureSpan">fast-csv.extended.</span>__defined__
1.  object <span class="apidocSignatureSpan">fast-csv.extended.</span>characters
1.  object <span class="apidocSignatureSpan">fast-csv.extended.</span>hash
1.  string <span class="apidocSignatureSpan">fast-csv.extended.</span>LINE_BREAK

#### [module fast-csv.format](#apidoc.module.fast-csv.format)
1.  [function <span class="apidocSignatureSpan">fast-csv.</span>format (options)](#apidoc.element.fast-csv.format.format)
1.  [function <span class="apidocSignatureSpan">fast-csv.format.</span>createWriteStream (options)](#apidoc.element.fast-csv.format.createWriteStream)
1.  [function <span class="apidocSignatureSpan">fast-csv.format.</span>write (arr, options, ws)](#apidoc.element.fast-csv.format.write)
1.  [function <span class="apidocSignatureSpan">fast-csv.format.</span>writeToBuffer (arr, options, cb)](#apidoc.element.fast-csv.format.writeToBuffer)
1.  [function <span class="apidocSignatureSpan">fast-csv.format.</span>writeToPath (path, arr, options)](#apidoc.element.fast-csv.format.writeToPath)
1.  [function <span class="apidocSignatureSpan">fast-csv.format.</span>writeToStream (ws, arr, options)](#apidoc.element.fast-csv.format.writeToStream)
1.  [function <span class="apidocSignatureSpan">fast-csv.format.</span>writeToString (arr, options, cb)](#apidoc.element.fast-csv.format.writeToString)



# <a name="apidoc.module.fast-csv"></a>[module fast-csv](#apidoc.module.fast-csv)

#### <a name="apidoc.element.fast-csv.createReadStream"></a>[function <span class="apidocSignatureSpan">fast-csv.</span>createReadStream (options)](#apidoc.element.fast-csv.createReadStream)
- description and source-code
```javascript
function createWriteStream(options) {
    return new CsvTransformStream(options);
}
```
- example usage
```shell
...
* 'data': Emitted with the object or 'stringified' version if the 'objectMode' is set to 'false'.

**'([options])' or '.parse(options)'**

If you use 'fast-csv' as a function it returns a transform stream that can be piped into.

'''javascript
var stream = fs.createReadStream("my.csv");

var csvStream = csv()
.on("data", function(data){
     console.log(data);
})
.on("end", function(){
     console.log("done");
...
```

#### <a name="apidoc.element.fast-csv.createWriteStream"></a>[function <span class="apidocSignatureSpan">fast-csv.</span>createWriteStream (options)](#apidoc.element.fast-csv.createWriteStream)
- description and source-code
```javascript
function createWriteStream(options) {
    return new CsvTransformStream(options);
}
```
- example usage
```shell
...
### Formatting Functions

**'createWriteStream(options)' or '.format(options)'**

This is the lowest level of the write methods, it creates a stream that can be used to create a CSV of unknown size and pipe to
an output CSV.

'''javascript
var csvStream = csv.createWriteStream({headers: true}),
    writableStream = fs.createWriteStream("my.csv");

writableStream.on("finish", function(){
  console.log("DONE!");
});

csvStream.pipe(writableStream);
...
```

#### <a name="apidoc.element.fast-csv.extended"></a>[function <span class="apidocSignatureSpan">fast-csv.</span>extended (obj)](#apidoc.element.fast-csv.extended)
- description and source-code
```javascript
function _extender(obj) {
    var ret = obj, i, l;
    if (!(obj instanceof Base)) {
        var OurBase = Base;
        for (i = 0, l = defined.length; i < l; i++) {
            var definer = defined[i];
            if (definer[0](obj)) {
                OurBase = OurBase.extend({instance: definer[1]});
            }
        }
        ret = new OurBase(obj);
        ret["__extender__"] = _extender;
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.format"></a>[function <span class="apidocSignatureSpan">fast-csv.</span>format (options)](#apidoc.element.fast-csv.format)
- description and source-code
```javascript
function createWriteStream(options) {
    return new CsvTransformStream(options);
}
```
- example usage
```shell
...
//Generated CSV
//a,a,b,b,c,c
//a1,a2,b1,b2,c1,c2
'''

### Formatting Functions

**'createWriteStream(options)' or '.format(options)'**

This is the lowest level of the write methods, it creates a stream that can be used to create a CSV of unknown size and pipe to
an output CSV.

'''javascript
var csvStream = csv.createWriteStream({headers: true}),
writableStream = fs.createWriteStream("my.csv");
...
```

#### <a name="apidoc.element.fast-csv.fromPath"></a>[function <span class="apidocSignatureSpan">fast-csv.</span>fromPath (location, options)](#apidoc.element.fast-csv.fromPath)
- description and source-code
```javascript
function fromPath(location, options) {
    return fs.createReadStream(location).pipe(new ParserStream(options));
}
```
- example usage
```shell
...
    })
    .on("end", function () {
        console.log("done");
    });
'''


**'.fromPath(path[, options])'**

This method parses a file from the specified path.

'''javascript
var csv = require("fast-csv");

csv
...
```

#### <a name="apidoc.element.fast-csv.fromStream"></a>[function <span class="apidocSignatureSpan">fast-csv.</span>fromStream (stream, options)](#apidoc.element.fast-csv.fromStream)
- description and source-code
```javascript
function fromStream(stream, options) {
    return stream.pipe(new ParserStream(options));
}
```
- example usage
```shell
...
     console.log(data);
 })
 .on("end", function(){
     console.log("done");
 });
'''

**'.fromStream(stream[, options])'**

This accepted a readable stream to parse data from.

'''javascript
var stream = fs.createReadStream("my.csv");

csv
...
```

#### <a name="apidoc.element.fast-csv.fromString"></a>[function <span class="apidocSignatureSpan">fast-csv.</span>fromString (string, options)](#apidoc.element.fast-csv.fromString)
- description and source-code
```javascript
function fromString(string, options) {
    var rs = new stream.Readable();
    rs.push(string);
    rs.push(null);
    return rs.pipe(new ParserStream(options));
}
```
- example usage
```shell
...
     console.log(data);
 })
 .on("end", function(){
     console.log("done");
 });
'''

**'.fromString(string[, options])'**

This method parses a string

'''javascript
var csv = require("fast-csv");

var CSV_STRING = 'a,b\n' +
...
```

#### <a name="apidoc.element.fast-csv.parse"></a>[function <span class="apidocSignatureSpan">fast-csv.</span>parse ()](#apidoc.element.fast-csv.parse)
- description and source-code
```javascript
function csv() {
    return parser.apply(void 0, arguments);
}
```
- example usage
```shell
...

**events**

* 'data': Emitted when a record is parsed.
* 'data-invalid': Emitted if there was invalid row encounted, **only emitted if the 'validate' function is used or 'strictColumnHandling
=true'**.
* 'data': Emitted with the object or 'stringified' version if the 'objectMode' is set to 'false'.

**'([options])' or '.parse(options)'**

If you use 'fast-csv' as a function it returns a transform stream that can be piped into.

'''javascript
var stream = fs.createReadStream("my.csv");

var csvStream = csv()
...
```

#### <a name="apidoc.element.fast-csv.write"></a>[function <span class="apidocSignatureSpan">fast-csv.</span>write (arr, options, ws)](#apidoc.element.fast-csv.write)
- description and source-code
```javascript
function write(arr, options, ws) {
    var csvStream = createWriteStream(options), i = -1, l = arr.length;
    extended.asyncEach(arr, function (item, cb) {
        csvStream.write(item, null, cb);
    }, function (err) {
        if (err) {
            csvStream.emit("error", err);
        } else {
            csvStream.end();
        }
    });
    return csvStream;
}
```
- example usage
```shell
...
var fileStream = fs.createReadStream("my.csv"),
    parser = fastCsv();

fileStream
    .on("readable", function () {
        var data;
        while ((data = fileStream.read()) !== null) {
            parser.write(data);
        }
    })
    .on("end", function () {
        parser.end();
    });

parser
...
```

#### <a name="apidoc.element.fast-csv.writeToBuffer"></a>[function <span class="apidocSignatureSpan">fast-csv.</span>writeToBuffer (arr, options, cb)](#apidoc.element.fast-csv.writeToBuffer)
- description and source-code
```javascript
function writeToBuffer(arr, options, cb) {
    if (extended.isFunction(options)) {
        cb = options;
        options = {};
    }
    var ws = new stream.Writable(), buffers = [], l = 0;
    ws._write = function (data, enc, cb) {
        buffers.push(data);
        l++;
        cb();
    };
    ws
        .on("error", cb)
        .on("finish", function () {
            cb(null, Buffer.concat(buffers));
        });
    write(arr, options).pipe(ws);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.writeToPath"></a>[function <span class="apidocSignatureSpan">fast-csv.</span>writeToPath (path, arr, options)](#apidoc.element.fast-csv.writeToPath)
- description and source-code
```javascript
function writeToPath(path, arr, options) {
    var stream = fs.createWriteStream(path, {encoding: "utf8"});
    return write(arr, options).pipe(stream);
}
```
- example usage
```shell
...

**'writeToPath(path, arr[, options])'**

Write an array of values to the specified path

'''javascript
csv
.writeToPath("my.csv", [
    ["a", "b"],
    ["a1", "b1"],
    ["a2", "b2"]
], {headers: true})
.on("finish", function(){
    console.log("done!");
});
...
```

#### <a name="apidoc.element.fast-csv.writeToStream"></a>[function <span class="apidocSignatureSpan">fast-csv.</span>writeToStream (ws, arr, options)](#apidoc.element.fast-csv.writeToStream)
- description and source-code
```javascript
function writeToStream(ws, arr, options) {
    return write(arr, options).pipe(ws);
}
```
- example usage
```shell
...

**'writeToStream(stream, arr[, options])'**

Write an array of values to a 'WritableStream'

'''javascript
csv
   .writeToStream(fs.createWriteStream("my.csv"), [
       ["a", "b"],
       ["a1", "b1"],
       ["a2", "b2"]
   ], {headers: true});
'''

'''javascript
...
```

#### <a name="apidoc.element.fast-csv.writeToString"></a>[function <span class="apidocSignatureSpan">fast-csv.</span>writeToString (arr, options, cb)](#apidoc.element.fast-csv.writeToString)
- description and source-code
```javascript
function writeToString(arr, options, cb) {
    if (extended.isFunction(options)) {
        cb = options;
        options = {};
    }
    var ws = new stream.Writable(), written = [];
    ws._write = function (data, enc, cb) {
        written.push(data + "");
        cb();
    };
    ws
        .on("error", cb)
        .on("finish", function () {
            cb(null, written.join(""));
        });
    write(arr, options).pipe(ws);
}
```
- example usage
```shell
...
  console.log("done!");
   });
'''

**'writeToString(arr[, options], cb)'**

'''javascript
csv.writeToString(
[
    ["a", "b"],
    ["a1", "b1"],
    ["a2", "b2"]
],
{headers: true},
function(err, data){
...
```



# <a name="apidoc.module.fast-csv.extended"></a>[module fast-csv.extended](#apidoc.module.fast-csv.extended)

#### <a name="apidoc.element.fast-csv.extended.extended"></a>[function <span class="apidocSignatureSpan">fast-csv.</span>extended (obj)](#apidoc.element.fast-csv.extended.extended)
- description and source-code
```javascript
function _extender(obj) {
    var ret = obj, i, l;
    if (!(obj instanceof Base)) {
        var OurBase = Base;
        for (i = 0, l = defined.length; i < l; i++) {
            var definer = defined[i];
            if (definer[0](obj)) {
                OurBase = OurBase.extend({instance: definer[1]});
            }
        }
        ret = new OurBase(obj);
        ret["__extender__"] = _extender;
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.asyncEach"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>asyncEach (arr, iter, cb)](#apidoc.element.fast-csv.extended.asyncEach)
- description and source-code
```javascript
asyncEach = function (arr, iter, cb) {


    (function asyncIterator(i, l, rows, cb) {
        if (++i < l) {
            iter(rows[i], function (err) {
                if (err) {
                    cb(err);
                } else {
                    if ((i % 100) === 0) {
                        //dont overflow the stack
                        setImmediate(function () {
                            asyncIterator(i, l, rows, cb);
                        });
                    } else {
                        asyncIterator(i, l, rows, cb);
                    }
                }
            });
        } else {
            //get out of stack
            cb(null, arr);
        }
    }(-1, arr.length, arr, cb));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.contains"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>contains (arr, obj)](#apidoc.element.fast-csv.extended.contains)
- description and source-code
```javascript
function contains(arr, obj) {
    return isIn(obj, arr);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.containsAt"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>containsAt (arr, obj, index)](#apidoc.element.fast-csv.extended.containsAt)
- description and source-code
```javascript
function containsAt(arr, obj, index) {
    if (isArray(arr) && arr.length > index) {
        return isEq(arr[index], obj);
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.deepEqual"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>deepEqual (actual, expected)](#apidoc.element.fast-csv.extended.deepEqual)
- description and source-code
```javascript
function deepEqual(actual, expected) {
    // 7.1. All identical values are equivalent, as determined by ===.
    if (actual === expected) {
        return true;

    } else if (typeof Buffer !== "undefined" && Buffer.isBuffer(actual) && Buffer.isBuffer(expected)) {
        if (actual.length !== expected.length) {
            return false;
        }
        for (var i = 0; i < actual.length; i++) {
            if (actual[i] !== expected[i]) {
                return false;
            }
        }
        return true;

        // 7.2. If the expected value is a Date object, the actual value is
        // equivalent if it is also a Date object that refers to the same time.
    } else if (isDate(actual) && isDate(expected)) {
        return actual.getTime() === expected.getTime();

        // 7.3 If the expected value is a RegExp object, the actual value is
        // equivalent if it is also a RegExp object with the same source and
        // properties ('global', 'multiline', 'lastIndex', 'ignoreCase').
    } else if (isRegExp(actual) && isRegExp(expected)) {
        return actual.source === expected.source &&
            actual.global === expected.global &&
            actual.multiline === expected.multiline &&
            actual.lastIndex === expected.lastIndex &&
            actual.ignoreCase === expected.ignoreCase;

        // 7.4. Other pairs that do not both pass typeof value == 'object',
        // equivalence is determined by ==.
    } else if (isString(actual) && isString(expected) && actual !== expected) {
        return false;
    } else if (typeof actual !== 'object' && typeof expected !== 'object') {
        return actual === expected;

        // 7.5 For all other Object pairs, including Array objects, equivalence is
        // determined by having the same number of owned properties (as verified
        // with Object.prototype.hasOwnProperty.call), the same set of keys
        // (although not necessarily the same order), equivalent values for every
        // corresponding key, and an identical 'prototype' property. Note: this
        // accounts for both named and indexed properties on Arrays.
    } else {
        return objEquiv(actual, expected);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.deepMerge"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>deepMerge (obj)](#apidoc.element.fast-csv.extended.deepMerge)
- description and source-code
```javascript
function deepMerge(obj) {
    if (!obj) {
        obj = {};
    }
    for (var i = 1, l = arguments.length; i < l; i++) {
        _deepMerge(obj, arguments[i]);
    }
    return obj; // Object
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.define"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>define (tester, decorate)](#apidoc.element.fast-csv.extended.define)
- description and source-code
```javascript
function define(tester, decorate) {
    if (arguments.length) {
        if (typeof tester === "object") {
            decorate = tester;
            tester = always;
        }
        decorate = decorate || {};
        var proto = {};
        decorateProto(proto, decorate);
        //handle browsers like which skip over the constructor while looping
        if (!proto.hasOwnProperty("constructor")) {
            if (decorate.hasOwnProperty("constructor")) {
                addMethod(proto, "constructor", decorate.constructor);
            } else {
                proto.constructor = function () {
                    this._super(arguments);
                };
            }
        }
        defined.push([tester, proto]);
    }
    return _extender;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.escape"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>escape (str, except)](#apidoc.element.fast-csv.extended.escape)
- description and source-code
```javascript
function escape(str, except) {
    return str.replace(/([\.$?*|{}\(\)\[\]\\\/\+^])/g, function (ch) {
        if (except && arr.indexOf(except, ch) !== -1) {
            return ch;
        }
        return "\\" + ch;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.expose"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>expose ()](#apidoc.element.fast-csv.extended.expose)
- description and source-code
```javascript
function expose() {
    var methods;
    for (var i = 0, l = arguments.length; i < l; i++) {
        methods = arguments[i];
        if (typeof methods === "object") {
            merge(_extender, methods, ["define", "extend", "expose", "__defined__"]);
        }
    }
    return _extender;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.extend"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>extend (supr)](#apidoc.element.fast-csv.extended.extend)
- description and source-code
```javascript
function extend(supr) {
    if (supr && supr.hasOwnProperty("__defined__")) {
        _extender["__defined__"] = defined = defined.concat(supr["__defined__"]);
    }
    merge(_extender, supr, ["define", "extend", "expose", "__defined__"]);
    return _extender;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.format"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>format (str, obj)](#apidoc.element.fast-csv.extended.format)
- description and source-code
```javascript
function format(str, obj) {
    if (obj instanceof Array) {
        var i = 0, len = obj.length;
        //find the matches
        return str.replace(FORMAT_REGEX, function (m, format, type) {
            var replacer, ret;
            if (i < len) {
                replacer = obj[i++];
            } else {
                //we are out of things to replace with so
                //just return the match?
                return m;
            }
            if (m === "%s" || m === "%d" || m === "%D") {
                //fast path!
                ret = replacer + "";
            } else if (m === "%Z") {
                ret = replacer.toUTCString();
            } else if (m === "%j") {
                try {
                    ret = stringify(replacer);
                } catch (e) {
                    throw new Error("stringExtended.format : Unable to parse json from ", replacer);
                }
            } else {
                format = format.replace(/^\[|\]$/g, "");
                switch (type) {
                case "s":
                    ret = formatString(replacer, format);
                    break;
                case "d":
                    ret = formatNumber(replacer, format);
                    break;
                case "j":
                    ret = formatObject(replacer, format);
                    break;
                case "D":
                    ret = date.format(replacer, format);
                    break;
                case "Z":
                    ret = date.format(replacer, format, true);
                    break;
                }
            }
            return ret;
        });
    } else if (isHash(obj)) {
        return str.replace(INTERP_REGEX, function (m, format, value) {
            value = obj[value];
            if (!is.isUndefined(value)) {
                if (format) {
                    if (is.isString(value)) {
                        return formatString(value, format);
                    } else if (is.isNumber(value)) {
                        return formatNumber(value, format);
                    } else if (is.isDate(value)) {
                        return date.format(value, format);
                    } else if (is.isObject(value)) {
                        return formatObject(value, format);
                    }
                } else {
                    return "" + value;
                }
            }
            return m;
        });
    } else {
        var args = aSlice.call(arguments).slice(1);
        return format(str, args);
    }
}
```
- example usage
```shell
...
//Generated CSV
//a,a,b,b,c,c
//a1,a2,b1,b2,c1,c2
'''

### Formatting Functions

**'createWriteStream(options)' or '.format(options)'**

This is the lowest level of the write methods, it creates a stream that can be used to create a CSV of unknown size and pipe to
an output CSV.

'''javascript
var csvStream = csv.createWriteStream({headers: true}),
writableStream = fs.createWriteStream("my.csv");
...
```

#### <a name="apidoc.element.fast-csv.extended.has"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>has (obj, prop)](#apidoc.element.fast-csv.extended.has)
- description and source-code
```javascript
function has(obj, prop) {
    return hasOwn.call(obj, prop);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.instanceOf"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>instanceOf (obj, clazz)](#apidoc.element.fast-csv.extended.instanceOf)
- description and source-code
```javascript
function isInstanceOf(obj, clazz) {
    if (isFunction(clazz)) {
        return obj instanceof clazz;
    } else {
        return false;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isArguments"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isArguments (object)](#apidoc.element.fast-csv.extended.isArguments)
- description and source-code
```javascript
function _isArguments(object) {
    return toStr.call(object) === '[object Arguments]';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isArray"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isArray ()](#apidoc.element.fast-csv.extended.isArray)
- description and source-code
```javascript
function isArray() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isBoolean"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isBoolean (obj)](#apidoc.element.fast-csv.extended.isBoolean)
- description and source-code
```javascript
function isBoolean(obj) {
    return obj === true || obj === false || toStr.call(obj) === "[object Boolean]";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isDate"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isDate (obj)](#apidoc.element.fast-csv.extended.isDate)
- description and source-code
```javascript
function isDate(obj) {
    return toStr.call(obj) === '[object Date]';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isDefined"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isDefined (obj)](#apidoc.element.fast-csv.extended.isDefined)
- description and source-code
```javascript
function isDefined(obj) {
    return !isUndefined(obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isEmpty"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isEmpty (str)](#apidoc.element.fast-csv.extended.isEmpty)
- description and source-code
```javascript
function isEmpty(str) {
    return str.length === 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isEq"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isEq (obj, obj2)](#apidoc.element.fast-csv.extended.isEq)
- description and source-code
```javascript
function isEq(obj, obj2) {
<span class="apidocCodeCommentSpan">    /*jshint eqeqeq:false*/
</span>    return obj == obj2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isFalse"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isFalse (obj)](#apidoc.element.fast-csv.extended.isFalse)
- description and source-code
```javascript
function isFalse(obj) {
    return obj === false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isFunction"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isFunction (obj)](#apidoc.element.fast-csv.extended.isFunction)
- description and source-code
```javascript
isFunction = function (obj) {
    return toStr.call(obj) === '[object Function]';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isGt"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isGt (obj, obj2)](#apidoc.element.fast-csv.extended.isGt)
- description and source-code
```javascript
function isGt(obj, obj2) {
    return obj > obj2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isGte"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isGte (obj, obj2)](#apidoc.element.fast-csv.extended.isGte)
- description and source-code
```javascript
function isGte(obj, obj2) {
    return obj >= obj2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isHash"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isHash (obj)](#apidoc.element.fast-csv.extended.isHash)
- description and source-code
```javascript
function isHash(obj) {
    var ret = isObject(obj);
    return ret && obj.constructor === Object && !obj.nodeType && !obj.setInterval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isIn"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isIn (obj, arr)](#apidoc.element.fast-csv.extended.isIn)
- description and source-code
```javascript
function isIn(obj, arr) {
    if ((isArray(arr) && Array.prototype.indexOf) || isString(arr)) {
        return arr.indexOf(obj) > -1;
    } else if (isArray(arr)) {
        for (var i = 0, l = arr.length; i < l; i++) {
            if (isEq(obj, arr[i])) {
                return true;
            }
        }
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isLength"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isLength (obj, l)](#apidoc.element.fast-csv.extended.isLength)
- description and source-code
```javascript
function length(obj, l) {
    if (has(obj, "length")) {
        return obj.length === l;
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isLike"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isLike (obj, reg)](#apidoc.element.fast-csv.extended.isLike)
- description and source-code
```javascript
function isLike(obj, reg) {
    if (isString(reg)) {
        return ("" + obj).match(reg) !== null;
    } else if (isRegExp(reg)) {
        return reg.test(obj);
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isLt"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isLt (obj, obj2)](#apidoc.element.fast-csv.extended.isLt)
- description and source-code
```javascript
function isLt(obj, obj2) {
    return obj < obj2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isLte"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isLte (obj, obj2)](#apidoc.element.fast-csv.extended.isLte)
- description and source-code
```javascript
function isLte(obj, obj2) {
    return obj <= obj2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isNeq"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isNeq (obj, obj2)](#apidoc.element.fast-csv.extended.isNeq)
- description and source-code
```javascript
function isNeq(obj, obj2) {
<span class="apidocCodeCommentSpan">    /*jshint eqeqeq:false*/
</span>    return obj != obj2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isNotIn"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isNotIn (obj, arr)](#apidoc.element.fast-csv.extended.isNotIn)
- description and source-code
```javascript
function isNotIn(obj, arr) {
    return !isIn(obj, arr);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isNotLength"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isNotLength (obj, l)](#apidoc.element.fast-csv.extended.isNotLength)
- description and source-code
```javascript
function notLength(obj, l) {
    if (has(obj, "length")) {
        return obj.length !== l;
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isNotLike"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isNotLike (obj, reg)](#apidoc.element.fast-csv.extended.isNotLike)
- description and source-code
```javascript
function isNotLike(obj, reg) {
    return !isLike(obj, reg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isNotNull"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isNotNull (obj)](#apidoc.element.fast-csv.extended.isNotNull)
- description and source-code
```javascript
function isNotNull(obj) {
    return !isNull(obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isNull"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isNull (obj)](#apidoc.element.fast-csv.extended.isNull)
- description and source-code
```javascript
function isNull(obj) {
    return obj === null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isNumber"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isNumber (obj)](#apidoc.element.fast-csv.extended.isNumber)
- description and source-code
```javascript
function isNumber(obj) {
    return toStr.call(obj) === '[object Number]';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isObject"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isObject (obj)](#apidoc.element.fast-csv.extended.isObject)
- description and source-code
```javascript
function isObject(obj) {
    var undef;
    return obj !== null && typeof obj === "object";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isRegExp"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isRegExp (obj)](#apidoc.element.fast-csv.extended.isRegExp)
- description and source-code
```javascript
function isRegExp(obj) {
    return toStr.call(obj) === '[object RegExp]';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isSeq"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isSeq (obj, obj2)](#apidoc.element.fast-csv.extended.isSeq)
- description and source-code
```javascript
function isSeq(obj, obj2) {
    return obj === obj2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isSneq"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isSneq (obj, obj2)](#apidoc.element.fast-csv.extended.isSneq)
- description and source-code
```javascript
function isSneq(obj, obj2) {
    return obj !== obj2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isString"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isString (obj)](#apidoc.element.fast-csv.extended.isString)
- description and source-code
```javascript
function isString(obj) {
    return toStr.call(obj) === '[object String]';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isTrue"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isTrue (obj)](#apidoc.element.fast-csv.extended.isTrue)
- description and source-code
```javascript
function isTrue(obj) {
    return obj === true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isUndefined"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isUndefined (obj)](#apidoc.element.fast-csv.extended.isUndefined)
- description and source-code
```javascript
function isUndefined(obj) {
    return typeof obj === 'undefined';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.isUndefinedOrNull"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>isUndefinedOrNull (obj)](#apidoc.element.fast-csv.extended.isUndefinedOrNull)
- description and source-code
```javascript
function isUndefinedOrNull(obj) {
    return isUndefined(obj) || isNull(obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.keys"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>keys (obj)](#apidoc.element.fast-csv.extended.keys)
- description and source-code
```javascript
keys = function (obj) {
    var ret = [];
    for (var i in obj) {
        if (hasOwn.call(obj, i)) {
            ret.push(i);
        }
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.merge"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>merge (obj)](#apidoc.element.fast-csv.extended.merge)
- description and source-code
```javascript
function merge(obj) {
    if (!obj) {
        obj = {};
    }
    for (var i = 1, l = arguments.length; i < l; i++) {
        _merge(obj, arguments[i]);
    }
    return obj; // Object
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.multiply"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>multiply (str, times)](#apidoc.element.fast-csv.extended.multiply)
- description and source-code
```javascript
function multiply(str, times) {
    var ret = [];
    if (times) {
        for (var i = 0; i < times; i++) {
            ret.push(str);
        }
    }
    return ret.join("");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.notContains"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>notContains (arr, obj)](#apidoc.element.fast-csv.extended.notContains)
- description and source-code
```javascript
function notContains(arr, obj) {
    return !isIn(obj, arr);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.notContainsAt"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>notContainsAt (arr, obj, index)](#apidoc.element.fast-csv.extended.notContainsAt)
- description and source-code
```javascript
function notContainsAt(arr, obj, index) {
    if (isArray(arr)) {
        return !isEq(arr[index], obj);
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.notHas"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>notHas (obj, prop)](#apidoc.element.fast-csv.extended.notHas)
- description and source-code
```javascript
function notHas(obj, prop) {
    return !has(obj, prop);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.omit"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>omit (hash, omitted)](#apidoc.element.fast-csv.extended.omit)
- description and source-code
```javascript
function omit(hash, omitted) {
    if (!isHash(hash)) {
        throw new TypeError();
    }
    if (isString(omitted)) {
        omitted = [omitted];
    }
    var objKeys = difference(keys(hash), omitted), key, ret = {};
    for (var i = 0, len = objKeys.length; i < len; ++i) {
        key = objKeys[i];
        ret[key] = hash[key];
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.pad"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>pad (string, length, ch, end)](#apidoc.element.fast-csv.extended.pad)
- description and source-code
```javascript
function pad(string, length, ch, end) {
    string = "" + string; //check for numbers
    ch = ch || " ";
    var strLen = string.length;
    while (strLen < length) {
        if (end) {
            string += ch;
        } else {
            string = ch + string;
        }
        strLen++;
    }
    return string;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.register"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>register (alias, extendWith)](#apidoc.element.fast-csv.extended.register)
- description and source-code
```javascript
function register(alias, extendWith) {
    if (!extendWith) {
        extendWith = alias;
        alias = null;
    }
    var type = typeof extendWith;
    if (alias) {
        extended[alias] = extendWith;
    } else if (extendWith && type === "function") {
        extended.extend(extendWith);
    } else if (type === "object") {
        extended.expose(extendWith);
    } else {
        throw new TypeError("extended.register must be called with an extender function");
    }
    return extended;
}
```
- example usage
```shell
...




var is = require("is-extended"),
    hasOwn = Object.prototype.hasOwnProperty;
module.exports = require("extended")()
    .register(is)
    .register(require("object-extended"))
    .register(require("string-extended"))
    .register("LINE_BREAK", require("os").EOL)
    .register("asyncEach", function (arr, iter, cb) {


(function asyncIterator(i, l, rows, cb) {
...
```

#### <a name="apidoc.element.fast-csv.extended.spreadArgs"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>spreadArgs (f, args, scope)](#apidoc.element.fast-csv.extended.spreadArgs)
- description and source-code
```javascript
function spreadArgs(f, args, scope) {
    var ret;
    switch ((args || []).length) {
        case 0:
            ret = f.call(scope);
            break;
        case 1:
            ret = f.call(scope, args[0]);
            break;
        case 2:
            ret = f.call(scope, args[0], args[1]);
            break;
        case 3:
            ret = f.call(scope, args[0], args[1], args[2]);
            break;
        default:
            ret = f.apply(scope, args);
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.style"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>style (str, options)](#apidoc.element.fast-csv.extended.style)
- description and source-code
```javascript
function style(str, options) {
    var ret, i, l;
    if (options) {
        if (is.isArray(str)) {
            ret = [];
            for (i = 0, l = str.length; i < l; i++) {
                ret.push(style(str[i], options));
            }
        } else if (options instanceof Array) {
            ret = str;
            for (i = 0, l = options.length; i < l; i++) {
                ret = style(ret, options[i]);
            }
        } else if (options in styles) {
            ret = '\x1B[' + styles[options] + 'm' + str + '\x1B[0m';
        }
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.switcher"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>switcher (obj)](#apidoc.element.fast-csv.extended.switcher)
- description and source-code
```javascript
function _extender(obj) {
    var ret = obj, i, l;
    if (!(obj instanceof Base)) {
        var OurBase = Base;
        for (i = 0, l = defined.length; i < l; i++) {
            var definer = defined[i];
            if (definer[0](obj)) {
                OurBase = OurBase.extend({instance: definer[1]});
            }
        }
        ret = new OurBase(obj);
        ret["__extender__"] = _extender;
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.tester"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>tester (obj)](#apidoc.element.fast-csv.extended.tester)
- description and source-code
```javascript
function _extender(obj) {
    var ret = obj, i, l;
    if (!(obj instanceof Base)) {
        var OurBase = Base;
        for (i = 0, l = defined.length; i < l; i++) {
            var definer = defined[i];
            if (definer[0](obj)) {
                OurBase = OurBase.extend({instance: definer[1]});
            }
        }
        ret = new OurBase(obj);
        ret["__extender__"] = _extender;
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.toArray"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>toArray (testStr, delim)](#apidoc.element.fast-csv.extended.toArray)
- description and source-code
```javascript
function toArray(testStr, delim) {
    var ret = [];
    if (testStr) {
        if (testStr.indexOf(delim) > 0) {
            ret = testStr.replace(/\s+/g, "").split(delim);
        }
        else {
            ret.push(testStr);
        }
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.trim"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>trim (str)](#apidoc.element.fast-csv.extended.trim)
- description and source-code
```javascript
function trim(str) {
    return str.replace(/^\s*|\s*$/g, "");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.trimLeft"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>trimLeft (str)](#apidoc.element.fast-csv.extended.trimLeft)
- description and source-code
```javascript
function trimLeft(str) {
    return str.replace(/^\s*/, "");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.trimRight"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>trimRight (str)](#apidoc.element.fast-csv.extended.trimRight)
- description and source-code
```javascript
function trimRight(str) {
    return str.replace(/\s*$/, "");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.extended.truncate"></a>[function <span class="apidocSignatureSpan">fast-csv.extended.</span>truncate (string, length, end)](#apidoc.element.fast-csv.extended.truncate)
- description and source-code
```javascript
function truncate(string, length, end) {
    var ret = string;
    if (is.isString(ret)) {
        if (string.length > length) {
            if (end) {
                var l = string.length;
                ret = string.substring(l - length, l);
            } else {
                ret = string.substring(0, length);
            }
        }
    } else {
        ret = truncate("" + ret, length);
    }
    return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fast-csv.format"></a>[module fast-csv.format](#apidoc.module.fast-csv.format)

#### <a name="apidoc.element.fast-csv.format.format"></a>[function <span class="apidocSignatureSpan">fast-csv.</span>format (options)](#apidoc.element.fast-csv.format.format)
- description and source-code
```javascript
function createWriteStream(options) {
    return new CsvTransformStream(options);
}
```
- example usage
```shell
...
//Generated CSV
//a,a,b,b,c,c
//a1,a2,b1,b2,c1,c2
'''

### Formatting Functions

**'createWriteStream(options)' or '.format(options)'**

This is the lowest level of the write methods, it creates a stream that can be used to create a CSV of unknown size and pipe to
an output CSV.

'''javascript
var csvStream = csv.createWriteStream({headers: true}),
writableStream = fs.createWriteStream("my.csv");
...
```

#### <a name="apidoc.element.fast-csv.format.createWriteStream"></a>[function <span class="apidocSignatureSpan">fast-csv.format.</span>createWriteStream (options)](#apidoc.element.fast-csv.format.createWriteStream)
- description and source-code
```javascript
function createWriteStream(options) {
    return new CsvTransformStream(options);
}
```
- example usage
```shell
...
### Formatting Functions

**'createWriteStream(options)' or '.format(options)'**

This is the lowest level of the write methods, it creates a stream that can be used to create a CSV of unknown size and pipe to
an output CSV.

'''javascript
var csvStream = csv.createWriteStream({headers: true}),
    writableStream = fs.createWriteStream("my.csv");

writableStream.on("finish", function(){
  console.log("DONE!");
});

csvStream.pipe(writableStream);
...
```

#### <a name="apidoc.element.fast-csv.format.write"></a>[function <span class="apidocSignatureSpan">fast-csv.format.</span>write (arr, options, ws)](#apidoc.element.fast-csv.format.write)
- description and source-code
```javascript
function write(arr, options, ws) {
    var csvStream = createWriteStream(options), i = -1, l = arr.length;
    extended.asyncEach(arr, function (item, cb) {
        csvStream.write(item, null, cb);
    }, function (err) {
        if (err) {
            csvStream.emit("error", err);
        } else {
            csvStream.end();
        }
    });
    return csvStream;
}
```
- example usage
```shell
...
var fileStream = fs.createReadStream("my.csv"),
    parser = fastCsv();

fileStream
    .on("readable", function () {
        var data;
        while ((data = fileStream.read()) !== null) {
            parser.write(data);
        }
    })
    .on("end", function () {
        parser.end();
    });

parser
...
```

#### <a name="apidoc.element.fast-csv.format.writeToBuffer"></a>[function <span class="apidocSignatureSpan">fast-csv.format.</span>writeToBuffer (arr, options, cb)](#apidoc.element.fast-csv.format.writeToBuffer)
- description and source-code
```javascript
function writeToBuffer(arr, options, cb) {
    if (extended.isFunction(options)) {
        cb = options;
        options = {};
    }
    var ws = new stream.Writable(), buffers = [], l = 0;
    ws._write = function (data, enc, cb) {
        buffers.push(data);
        l++;
        cb();
    };
    ws
        .on("error", cb)
        .on("finish", function () {
            cb(null, Buffer.concat(buffers));
        });
    write(arr, options).pipe(ws);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fast-csv.format.writeToPath"></a>[function <span class="apidocSignatureSpan">fast-csv.format.</span>writeToPath (path, arr, options)](#apidoc.element.fast-csv.format.writeToPath)
- description and source-code
```javascript
function writeToPath(path, arr, options) {
    var stream = fs.createWriteStream(path, {encoding: "utf8"});
    return write(arr, options).pipe(stream);
}
```
- example usage
```shell
...

**'writeToPath(path, arr[, options])'**

Write an array of values to the specified path

'''javascript
csv
.writeToPath("my.csv", [
    ["a", "b"],
    ["a1", "b1"],
    ["a2", "b2"]
], {headers: true})
.on("finish", function(){
    console.log("done!");
});
...
```

#### <a name="apidoc.element.fast-csv.format.writeToStream"></a>[function <span class="apidocSignatureSpan">fast-csv.format.</span>writeToStream (ws, arr, options)](#apidoc.element.fast-csv.format.writeToStream)
- description and source-code
```javascript
function writeToStream(ws, arr, options) {
    return write(arr, options).pipe(ws);
}
```
- example usage
```shell
...

**'writeToStream(stream, arr[, options])'**

Write an array of values to a 'WritableStream'

'''javascript
csv
   .writeToStream(fs.createWriteStream("my.csv"), [
       ["a", "b"],
       ["a1", "b1"],
       ["a2", "b2"]
   ], {headers: true});
'''

'''javascript
...
```

#### <a name="apidoc.element.fast-csv.format.writeToString"></a>[function <span class="apidocSignatureSpan">fast-csv.format.</span>writeToString (arr, options, cb)](#apidoc.element.fast-csv.format.writeToString)
- description and source-code
```javascript
function writeToString(arr, options, cb) {
    if (extended.isFunction(options)) {
        cb = options;
        options = {};
    }
    var ws = new stream.Writable(), written = [];
    ws._write = function (data, enc, cb) {
        written.push(data + "");
        cb();
    };
    ws
        .on("error", cb)
        .on("finish", function () {
            cb(null, written.join(""));
        });
    write(arr, options).pipe(ws);
}
```
- example usage
```shell
...
  console.log("done!");
   });
'''

**'writeToString(arr[, options], cb)'**

'''javascript
csv.writeToString(
[
    ["a", "b"],
    ["a1", "b1"],
    ["a2", "b2"]
],
{headers: true},
function(err, data){
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
