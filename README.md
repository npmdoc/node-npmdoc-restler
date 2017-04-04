# api documentation for  [restler (v3.4.0)](https://github.com/danwrong/restler)  [![npm package](https://img.shields.io/npm/v/npmdoc-restler.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-restler) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-restler.svg)](https://travis-ci.org/npmdoc/node-npmdoc-restler)
#### An HTTP client library for node.js

[![NPM](https://nodei.co/npm/restler.png?downloads=true)](https://www.npmjs.com/package/restler)

[![apidoc](https://npmdoc.github.io/node-npmdoc-restler/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-restler_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-restler/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-restler/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-restler/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/danwrong/restler/issues"
    },
    "contributors": [
        {
            "name": "Dan Webb",
            "email": "dan@danwebb.net"
        },
        {
            "name": "Ben Marvell",
            "email": "ben@marvell-consulting.com"
        }
    ],
    "dependencies": {
        "iconv-lite": "0.2.11",
        "qs": "1.2.0",
        "xml2js": "0.4.0",
        "yaml": "0.2.3"
    },
    "description": "An HTTP client library for node.js",
    "devDependencies": {
        "nodeunit": "0.8.2"
    },
    "directories": {
        "lib": "./lib"
    },
    "dist": {
        "shasum": "741ec0b3d16b949feea2813d0c3c68529e888d9b",
        "tarball": "https://registry.npmjs.org/restler/-/restler-3.4.0.tgz"
    },
    "engines": {
        "node": ">= 0.10.x"
    },
    "gitHead": "f31e457eaedb54def4a5e3fc84b3a161be0889e0",
    "homepage": "https://github.com/danwrong/restler",
    "license": "MIT",
    "main": "./lib/restler",
    "maintainers": [
        {
            "name": "danwrong",
            "email": "dan@danwebb.net"
        },
        {
            "name": "ayoung",
            "email": "andrewdyoung@gmail.com"
        },
        {
            "name": "easternbloc",
            "email": "ben@marvell-consulting.com"
        }
    ],
    "name": "restler",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/danwrong/restler.git"
    },
    "scripts": {
        "test": "node test/all.js"
    },
    "version": "3.4.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module restler](#apidoc.module.restler)
1.  [function <span class="apidocSignatureSpan">restler.</span>Request (uri, options)](#apidoc.element.restler.Request)
1.  [function <span class="apidocSignatureSpan">restler.</span>Service (defaults)](#apidoc.element.restler.Service)
1.  [function <span class="apidocSignatureSpan">restler.</span>data (filename, contentType, data)](#apidoc.element.restler.data)
1.  [function <span class="apidocSignatureSpan">restler.</span>del (url, options)](#apidoc.element.restler.del)
1.  [function <span class="apidocSignatureSpan">restler.</span>file (path, filename, fileSize, encoding, contentType)](#apidoc.element.restler.file)
1.  [function <span class="apidocSignatureSpan">restler.</span>get (url, options)](#apidoc.element.restler.get)
1.  [function <span class="apidocSignatureSpan">restler.</span>head (url, options)](#apidoc.element.restler.head)
1.  [function <span class="apidocSignatureSpan">restler.</span>json (url, data, options, method)](#apidoc.element.restler.json)
1.  [function <span class="apidocSignatureSpan">restler.</span>patch (url, options)](#apidoc.element.restler.patch)
1.  [function <span class="apidocSignatureSpan">restler.</span>patchJson (url, data, options)](#apidoc.element.restler.patchJson)
1.  [function <span class="apidocSignatureSpan">restler.</span>post (url, options)](#apidoc.element.restler.post)
1.  [function <span class="apidocSignatureSpan">restler.</span>postJson (url, data, options)](#apidoc.element.restler.postJson)
1.  [function <span class="apidocSignatureSpan">restler.</span>put (url, options)](#apidoc.element.restler.put)
1.  [function <span class="apidocSignatureSpan">restler.</span>putJson (url, data, options)](#apidoc.element.restler.putJson)
1.  [function <span class="apidocSignatureSpan">restler.</span>request (url, options)](#apidoc.element.restler.request)
1.  [function <span class="apidocSignatureSpan">restler.</span>service (constructor, defaults, methods)](#apidoc.element.restler.service)
1.  object <span class="apidocSignatureSpan">restler.</span>Request.prototype
1.  object <span class="apidocSignatureSpan">restler.</span>Service.prototype
1.  object <span class="apidocSignatureSpan">restler.</span>multipartform
1.  object <span class="apidocSignatureSpan">restler.</span>parsers

#### [module restler.Request](#apidoc.module.restler.Request)
1.  [function <span class="apidocSignatureSpan">restler.</span>Request (uri, options)](#apidoc.element.restler.Request.Request)
1.  [function <span class="apidocSignatureSpan">restler.Request.</span>super_ ()](#apidoc.element.restler.Request.super_)

#### [module restler.Request.prototype](#apidoc.module.restler.Request.prototype)
1.  [function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_applyAuth ()](#apidoc.element.restler.Request.prototype._applyAuth)
1.  [function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_decode (body, response, callback)](#apidoc.element.restler.Request.prototype._decode)
1.  [function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_encode (body, response, callback)](#apidoc.element.restler.Request.prototype._encode)
1.  [function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_fireCancelTimeout ()](#apidoc.element.restler.Request.prototype._fireCancelTimeout)
1.  [function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_fireError (err, response)](#apidoc.element.restler.Request.prototype._fireError)
1.  [function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_fireSuccess (body, response)](#apidoc.element.restler.Request.prototype._fireSuccess)
1.  [function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_fireTimeout (err)](#apidoc.element.restler.Request.prototype._fireTimeout)
1.  [function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_fullPath ()](#apidoc.element.restler.Request.prototype._fullPath)
1.  [function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_iconv (body, response)](#apidoc.element.restler.Request.prototype._iconv)
1.  [function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_isRedirect (response)](#apidoc.element.restler.Request.prototype._isRedirect)
1.  [function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_makeRequest ()](#apidoc.element.restler.Request.prototype._makeRequest)
1.  [function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_responseHandler (response)](#apidoc.element.restler.Request.prototype._responseHandler)
1.  [function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_retry ()](#apidoc.element.restler.Request.prototype._retry)
1.  [function <span class="apidocSignatureSpan">restler.Request.prototype.</span>abort (err)](#apidoc.element.restler.Request.prototype.abort)
1.  [function <span class="apidocSignatureSpan">restler.Request.prototype.</span>retry (timeout)](#apidoc.element.restler.Request.prototype.retry)
1.  [function <span class="apidocSignatureSpan">restler.Request.prototype.</span>run ()](#apidoc.element.restler.Request.prototype.run)

#### [module restler.Service](#apidoc.module.restler.Service)
1.  [function <span class="apidocSignatureSpan">restler.</span>Service (defaults)](#apidoc.element.restler.Service.Service)

#### [module restler.Service.prototype](#apidoc.module.restler.Service.prototype)
1.  [function <span class="apidocSignatureSpan">restler.Service.prototype.</span>_url (path)](#apidoc.element.restler.Service.prototype._url)
1.  [function <span class="apidocSignatureSpan">restler.Service.prototype.</span>_withDefaults (options)](#apidoc.element.restler.Service.prototype._withDefaults)
1.  [function <span class="apidocSignatureSpan">restler.Service.prototype.</span>del (path, options)](#apidoc.element.restler.Service.prototype.del)
1.  [function <span class="apidocSignatureSpan">restler.Service.prototype.</span>get (path, options)](#apidoc.element.restler.Service.prototype.get)
1.  [function <span class="apidocSignatureSpan">restler.Service.prototype.</span>json (method, path, data, options)](#apidoc.element.restler.Service.prototype.json)
1.  [function <span class="apidocSignatureSpan">restler.Service.prototype.</span>patch (path, options)](#apidoc.element.restler.Service.prototype.patch)
1.  [function <span class="apidocSignatureSpan">restler.Service.prototype.</span>post (path, options)](#apidoc.element.restler.Service.prototype.post)
1.  [function <span class="apidocSignatureSpan">restler.Service.prototype.</span>put (path, options)](#apidoc.element.restler.Service.prototype.put)
1.  [function <span class="apidocSignatureSpan">restler.Service.prototype.</span>request (path, options)](#apidoc.element.restler.Service.prototype.request)

#### [module restler.multipartform](#apidoc.module.restler.multipartform)
1.  [function <span class="apidocSignatureSpan">restler.multipartform.</span>data (filename, contentType, data)](#apidoc.element.restler.multipartform.data)
1.  [function <span class="apidocSignatureSpan">restler.multipartform.</span>file (path, filename, fileSize, encoding, contentType)](#apidoc.element.restler.multipartform.file)
1.  [function <span class="apidocSignatureSpan">restler.multipartform.</span>sizeOf (parts, boundary)](#apidoc.element.restler.multipartform.sizeOf)
1.  [function <span class="apidocSignatureSpan">restler.multipartform.</span>write (stream, data, callback, boundary)](#apidoc.element.restler.multipartform.write)
1.  string <span class="apidocSignatureSpan">restler.multipartform.</span>defaultBoundary

#### [module restler.parsers](#apidoc.module.restler.parsers)
1.  [function <span class="apidocSignatureSpan">restler.parsers.</span>auto (data, callback)](#apidoc.element.restler.parsers.auto)
1.  [function <span class="apidocSignatureSpan">restler.parsers.</span>json (data, callback)](#apidoc.element.restler.parsers.json)
1.  [function <span class="apidocSignatureSpan">restler.parsers.</span>xml (data, callback)](#apidoc.element.restler.parsers.xml)
1.  [function <span class="apidocSignatureSpan">restler.parsers.</span>yaml (data, callback)](#apidoc.element.restler.parsers.yaml)



# <a name="apidoc.module.restler"></a>[module restler](#apidoc.module.restler)

#### <a name="apidoc.element.restler.Request"></a>[function <span class="apidocSignatureSpan">restler.</span>Request (uri, options)](#apidoc.element.restler.Request)
- description and source-code
```javascript
function Request(uri, options) {
  events.EventEmitter.call(this);
  this.url = url.parse(uri);
  this.options = options;
  this.headers = {
    'Accept': '*/*',
    'User-Agent': 'Restler for node.js',
    'Host': this.url.host
  };

  this.headers['Accept-Encoding'] = 'gzip, deflate';

  mixin(this.headers, options.headers || {});

  // set port and method defaults
  if (!this.url.port) this.url.port = (this.url.protocol == 'https:') ? '443' : '80';
  if (!this.options.method) this.options.method = (this.options.data) ? 'POST' : 'GET';
  if (typeof this.options.followRedirects == 'undefined') this.options.followRedirects = true;

  // stringify query given in options of not given in URL
  if (this.options.query && !this.url.query) {
    if (typeof this.options.query == 'object')
      this.url.query = qs.stringify(this.options.query);
    else this.url.query = this.options.query;
  }

  this._applyAuth();

  if (this.options.multipart) {
    this.headers['Content-Type'] = 'multipart/form-data; boundary=' + multipart.defaultBoundary;
    var multipart_size = multipart.sizeOf(this.options.data, multipart.defaultBoundary);
    if (typeof multipart_size === 'number' && multipart_size === multipart_size) {
        this.headers['Content-Length'] = multipart_size;
    }
    else {
        console.log("Building multipart request without Content-Length header, please specify all file sizes");
    }
  } else {
    if (typeof this.options.data == 'object' && !Buffer.isBuffer(this.options.data)) {
      this.options.data = qs.stringify(this.options.data);
      this.headers['Content-Type'] = 'application/x-www-form-urlencoded';
      this.headers['Content-Length'] = this.options.data.length;
    }
    if (typeof this.options.data == 'string') {
      var buffer = new Buffer(this.options.data, this.options.encoding || 'utf8');
      this.options.data = buffer;
      this.headers['Content-Length'] = buffer.length;
    }
    if (!this.options.data) {
      this.headers['Content-Length'] = 0;
    }
  }

  var proto = (this.url.protocol == 'https:') ? https : http;

  this.request = proto.request({
    host: this.url.hostname,
    port: this.url.port,
    path: this._fullPath(),
    method: this.options.method,
    headers: this.headers,
    rejectUnauthorized: this.options.rejectUnauthorized,
    agent: this.options.agent
  });

  this._makeRequest();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Service"></a>[function <span class="apidocSignatureSpan">restler.</span>Service (defaults)](#apidoc.element.restler.Service)
- description and source-code
```javascript
function Service(defaults) {
  if (defaults.baseURL) {
   this.baseURL = defaults.baseURL;
   delete defaults.baseURL;
  }

  this.defaults = defaults;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.data"></a>[function <span class="apidocSignatureSpan">restler.</span>data (filename, contentType, data)](#apidoc.element.restler.data)
- description and source-code
```javascript
data = function (filename, contentType, data) {
  return new Data(filename, contentType, data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.del"></a>[function <span class="apidocSignatureSpan">restler.</span>del (url, options)](#apidoc.element.restler.del)
- description and source-code
```javascript
function del(url, options) {
  return request(url, shortcutOptions(options, 'DELETE'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.file"></a>[function <span class="apidocSignatureSpan">restler.</span>file (path, filename, fileSize, encoding, contentType)](#apidoc.element.restler.file)
- description and source-code
```javascript
file = function (path, filename, fileSize, encoding, contentType) {
  return new File(path, filename, fileSize, encoding, contentType)
}
```
- example usage
```shell
...
// multipart request sending a 321567 byte long file using https
rest.post('https://twaud.io/api/v1/upload.json', {
  multipart: true,
  username: 'danwrong',
  password: 'wouldntyouliketoknow',
  data: {
    'sound[message]': 'hello from restler!',
    'sound[file]': rest.file('doug-e-fresh_the-show.mp3', null, 321567, null, 'audio/mpeg')
  }
}).on('complete', function(data) {
  console.log(data.audio_url);
});

// create a service constructor for very easy API wrappers a la HTTParty...
Twitter = rest.service(function(u, p) {
...
```

#### <a name="apidoc.element.restler.get"></a>[function <span class="apidocSignatureSpan">restler.</span>get (url, options)](#apidoc.element.restler.get)
- description and source-code
```javascript
function get(url, options) {
 return request(url, shortcutOptions(options, 'GET'));
}
```
- example usage
```shell
...

Example usage
-------------

'''javascript
var rest = require('./restler');

rest.get('http://google.com').on('complete', function(result) {
  if (result instanceof Error) {
    console.log('Error:', result.message);
    this.retry(5000); // try again after 5 sec
  } else {
    console.log(result);
  }
});
...
```

#### <a name="apidoc.element.restler.head"></a>[function <span class="apidocSignatureSpan">restler.</span>head (url, options)](#apidoc.element.restler.head)
- description and source-code
```javascript
function head(url, options) {
  return request(url, shortcutOptions(options, 'HEAD'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.json"></a>[function <span class="apidocSignatureSpan">restler.</span>json (url, data, options, method)](#apidoc.element.restler.json)
- description and source-code
```javascript
function json(url, data, options, method) {
  options = options || {};
  options.parser = (typeof options.parser !== "undefined") ? options.parser : parsers.auto;
  options.headers = options.headers || {};
  options.headers['content-type'] = 'application/json';
  options.data = JSON.stringify(data || {});
  options.method = method || 'GET';
  return request(url, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.patch"></a>[function <span class="apidocSignatureSpan">restler.</span>patch (url, options)](#apidoc.element.restler.patch)
- description and source-code
```javascript
function patch(url, options) {
  return request(url, shortcutOptions(options, 'PATCH'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.patchJson"></a>[function <span class="apidocSignatureSpan">restler.</span>patchJson (url, data, options)](#apidoc.element.restler.patchJson)
- description and source-code
```javascript
function patchJson(url, data, options) {
  return json(url, data, options, 'PATCH');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.post"></a>[function <span class="apidocSignatureSpan">restler.</span>post (url, options)](#apidoc.element.restler.post)
- description and source-code
```javascript
function post(url, options) {
  return request(url, shortcutOptions(options, 'POST'));
}
```
- example usage
```shell
...

rest.get('http://someslowdomain.com',{timeout: 10000}).on('timeout', function(ms){
  console.log('did not return within '+ms+' ms');
}).on('complete',function(data,response){
  console.log('did not time out');
});

rest.post('http://user:pass@service.com/action', {
  data: { id: 334 },
}).on('complete', function(data, response) {
  if (response.statusCode == 201) {
    // you can get at the raw response like this...
  }
});
...
```

#### <a name="apidoc.element.restler.postJson"></a>[function <span class="apidocSignatureSpan">restler.</span>postJson (url, data, options)](#apidoc.element.restler.postJson)
- description and source-code
```javascript
function postJson(url, data, options) {
  return json(url, data, options, 'POST');
}
```
- example usage
```shell
...
var client = new Twitter('danwrong', 'password');
client.update('Tweeting using a Restler service thingy').on('complete', function(data) {
console.log(data);
});

// post JSON
var jsonData = { id: 334 };
rest.postJson('http://example.com/action', jsonData).on('complete', function(data, response) {
// handle response
});

// put JSON
var jsonData = { id: 334 };
rest.putJson('http://example.com/action', jsonData).on('complete', function(data, response) {
// handle response
...
```

#### <a name="apidoc.element.restler.put"></a>[function <span class="apidocSignatureSpan">restler.</span>put (url, options)](#apidoc.element.restler.put)
- description and source-code
```javascript
function put(url, options) {
  return request(url, shortcutOptions(options, 'PUT'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.putJson"></a>[function <span class="apidocSignatureSpan">restler.</span>putJson (url, data, options)](#apidoc.element.restler.putJson)
- description and source-code
```javascript
function putJson(url, data, options) {
  return json(url, data, options, 'PUT');
}
```
- example usage
```shell
...
var jsonData = { id: 334 };
rest.postJson('http://example.com/action', jsonData).on('complete', function(data, response) {
  // handle response
});

// put JSON
var jsonData = { id: 334 };
rest.putJson('http://example.com/action', jsonData).on('complete', function(data, response) {
  // handle response
});

'''

TODO
----
...
```

#### <a name="apidoc.element.restler.request"></a>[function <span class="apidocSignatureSpan">restler.</span>request (url, options)](#apidoc.element.restler.request)
- description and source-code
```javascript
function request(url, options) {
  var request = new Request(url, options);
  request.on('error', function() {});
  process.nextTick(request.run.bind(request));
  return request;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.service"></a>[function <span class="apidocSignatureSpan">restler.</span>service (constructor, defaults, methods)](#apidoc.element.restler.service)
- description and source-code
```javascript
function service(constructor, defaults, methods) {
  constructor.prototype = new Service(defaults || {});
  mixin(constructor.prototype, methods);
  return constructor;
}
```
- example usage
```shell
...
  'sound[file]': rest.file('doug-e-fresh_the-show.mp3', null, 321567, null, 'audio/mpeg')
}
}).on('complete', function(data) {
console.log(data.audio_url);
});

// create a service constructor for very easy API wrappers a la HTTParty...
Twitter = rest.service(function(u, p) {
this.defaults.username = u;
this.defaults.password = p;
}, {
baseURL: 'http://twitter.com'
}, {
update: function(message) {
  return this.post('/statuses/update.json', { data: { status: message } });
...
```



# <a name="apidoc.module.restler.Request"></a>[module restler.Request](#apidoc.module.restler.Request)

#### <a name="apidoc.element.restler.Request.Request"></a>[function <span class="apidocSignatureSpan">restler.</span>Request (uri, options)](#apidoc.element.restler.Request.Request)
- description and source-code
```javascript
function Request(uri, options) {
  events.EventEmitter.call(this);
  this.url = url.parse(uri);
  this.options = options;
  this.headers = {
    'Accept': '*/*',
    'User-Agent': 'Restler for node.js',
    'Host': this.url.host
  };

  this.headers['Accept-Encoding'] = 'gzip, deflate';

  mixin(this.headers, options.headers || {});

  // set port and method defaults
  if (!this.url.port) this.url.port = (this.url.protocol == 'https:') ? '443' : '80';
  if (!this.options.method) this.options.method = (this.options.data) ? 'POST' : 'GET';
  if (typeof this.options.followRedirects == 'undefined') this.options.followRedirects = true;

  // stringify query given in options of not given in URL
  if (this.options.query && !this.url.query) {
    if (typeof this.options.query == 'object')
      this.url.query = qs.stringify(this.options.query);
    else this.url.query = this.options.query;
  }

  this._applyAuth();

  if (this.options.multipart) {
    this.headers['Content-Type'] = 'multipart/form-data; boundary=' + multipart.defaultBoundary;
    var multipart_size = multipart.sizeOf(this.options.data, multipart.defaultBoundary);
    if (typeof multipart_size === 'number' && multipart_size === multipart_size) {
        this.headers['Content-Length'] = multipart_size;
    }
    else {
        console.log("Building multipart request without Content-Length header, please specify all file sizes");
    }
  } else {
    if (typeof this.options.data == 'object' && !Buffer.isBuffer(this.options.data)) {
      this.options.data = qs.stringify(this.options.data);
      this.headers['Content-Type'] = 'application/x-www-form-urlencoded';
      this.headers['Content-Length'] = this.options.data.length;
    }
    if (typeof this.options.data == 'string') {
      var buffer = new Buffer(this.options.data, this.options.encoding || 'utf8');
      this.options.data = buffer;
      this.headers['Content-Length'] = buffer.length;
    }
    if (!this.options.data) {
      this.headers['Content-Length'] = 0;
    }
  }

  var proto = (this.url.protocol == 'https:') ? https : http;

  this.request = proto.request({
    host: this.url.hostname,
    port: this.url.port,
    path: this._fullPath(),
    method: this.options.method,
    headers: this.headers,
    rejectUnauthorized: this.options.rejectUnauthorized,
    agent: this.options.agent
  });

  this._makeRequest();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Request.super_"></a>[function <span class="apidocSignatureSpan">restler.Request.</span>super_ ()](#apidoc.element.restler.Request.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.restler.Request.prototype"></a>[module restler.Request.prototype](#apidoc.module.restler.Request.prototype)

#### <a name="apidoc.element.restler.Request.prototype._applyAuth"></a>[function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_applyAuth ()](#apidoc.element.restler.Request.prototype._applyAuth)
- description and source-code
```javascript
_applyAuth = function () {
  var authParts;

  if (this.url.auth) {
    authParts = this.url.auth.split(':');
    this.options.username = authParts[0];
    this.options.password = authParts[1];
  }

  if (this.options.username && this.options.password !== undefined) {
    var b = new Buffer([this.options.username, this.options.password].join(':'));
    this.headers['Authorization'] = "Basic " + b.toString('base64');
  } else if (this.options.accessToken) {
    this.headers['Authorization'] = "Bearer " + this.options.accessToken;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Request.prototype._decode"></a>[function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_decode (body, response, callback)](#apidoc.element.restler.Request.prototype._decode)
- description and source-code
```javascript
_decode = function (body, response, callback) {
  var decoder = response.headers['content-encoding'];
  if (decoder in decoders) {
    decoders[decoder].call(response, body, callback);
  } else {
    callback(null, body);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Request.prototype._encode"></a>[function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_encode (body, response, callback)](#apidoc.element.restler.Request.prototype._encode)
- description and source-code
```javascript
_encode = function (body, response, callback) {
  var self = this;
  if (self.options.decoding == 'buffer') {
    callback(null, body);
  } else {
    body = body.toString(self.options.decoding);
    if (self.options.parser) {
      self.options.parser.call(response, body, callback);
    } else {
      callback(null, body);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Request.prototype._fireCancelTimeout"></a>[function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_fireCancelTimeout ()](#apidoc.element.restler.Request.prototype._fireCancelTimeout)
- description and source-code
```javascript
_fireCancelTimeout = function (){
  var self = this;
  if(self.options.timeout){
    clearTimeout(self.options.timeoutFn);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Request.prototype._fireError"></a>[function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_fireError (err, response)](#apidoc.element.restler.Request.prototype._fireError)
- description and source-code
```javascript
_fireError = function (err, response) {
  this._fireCancelTimeout();
  this.emit('error', err, response);
  this.emit('complete', err, response);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Request.prototype._fireSuccess"></a>[function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_fireSuccess (body, response)](#apidoc.element.restler.Request.prototype._fireSuccess)
- description and source-code
```javascript
_fireSuccess = function (body, response) {
  if (parseInt(response.statusCode) >= 400) {
    this.emit('fail', body, response);
  } else {
    this.emit('success', body, response);
  }
  this.emit(response.statusCode.toString().replace(/\d{2}$/, 'XX'), body, response);
  this.emit(response.statusCode.toString(), body, response);
  this.emit('complete', body, response);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Request.prototype._fireTimeout"></a>[function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_fireTimeout (err)](#apidoc.element.restler.Request.prototype._fireTimeout)
- description and source-code
```javascript
_fireTimeout = function (err){
  this.emit('timeout', err);
  this.aborted = true;
  this.timedout = true;
  this.request.abort();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Request.prototype._fullPath"></a>[function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_fullPath ()](#apidoc.element.restler.Request.prototype._fullPath)
- description and source-code
```javascript
_fullPath = function () {
  var path = this.url.pathname || '/';
  if (this.url.hash) path += this.url.hash;
  if (this.url.query) path += '?' + this.url.query;
  return path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Request.prototype._iconv"></a>[function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_iconv (body, response)](#apidoc.element.restler.Request.prototype._iconv)
- description and source-code
```javascript
_iconv = function (body, response) {
  var charset = response.headers['content-type'];
  if (charset) {
    charset = /\bcharset=(.+)(?:;|$)/i.exec(charset);
    if (charset) {
      charset = charset[1].trim().toUpperCase();
      if (charset != 'UTF-8') {
        try {
          return iconv.decode(body, charset);
        } catch (err) {}
      }
    }
  }
  return body;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Request.prototype._isRedirect"></a>[function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_isRedirect (response)](#apidoc.element.restler.Request.prototype._isRedirect)
- description and source-code
```javascript
_isRedirect = function (response) {
  return ([301, 302, 303, 307].indexOf(response.statusCode) >= 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Request.prototype._makeRequest"></a>[function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_makeRequest ()](#apidoc.element.restler.Request.prototype._makeRequest)
- description and source-code
```javascript
_makeRequest = function () {
  var self = this;
  var timeoutMs = self.options.timeout;
  if(timeoutMs){
    self.options.timeoutFn = setTimeout(function(){
      self._fireTimeout(timeoutMs);
    },timeoutMs);
  }
  this.request.on('response', function(response) {
    self._fireCancelTimeout();
    self.emit('response', response);
    self._responseHandler(response);
  }).on('error', function(err) {
    self._fireCancelTimeout();
    if (!self.aborted) {
      self._fireError(err, null);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Request.prototype._responseHandler"></a>[function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_responseHandler (response)](#apidoc.element.restler.Request.prototype._responseHandler)
- description and source-code
```javascript
_responseHandler = function (response) {
  var self = this;

  if (self._isRedirect(response) && self.options.followRedirects) {
    try {
      // 303 should redirect and retrieve content with the GET method
      // http://www.w3.org/Protocols/rfc2616/rfc2616-sec10.html#sec10.3.4
      if (response.statusCode === 303) {
          self.url    = url.parse(url.resolve(self.url.href, response.headers['location']));
          self.options.method = 'GET';
          delete self.options.data;
          self._retry();
      } else {
          self.url = url.parse(url.resolve(self.url.href, response.headers['location']));
          self._retry();
          // todo handle somehow infinite redirects
      }
    } catch(err) {
      err.message = 'Failed to follow redirect: ' + err.message;
      self._fireError(err, response);
    }
  } else {
    var body = '';

    // When using browserify, response.setEncoding is not defined
    if (typeof response.setEncoding == 'function')
      response.setEncoding('binary');

    response.on('data', function(chunk) {
      body += chunk;
    });

    response.on('end', function() {
      response.rawEncoded = body;
      self._decode(new Buffer(body, 'binary'), response, function(err, body) {
        if (err) {
          self._fireError(err, response);
          return;
        }
        response.raw = body;
        body = self._iconv(body, response);
        self._encode(body, response, function(err, body) {
          if (err) {
            self._fireError(err, response);
          } else {
            self._fireSuccess(body, response);
          }
        });
      });
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Request.prototype._retry"></a>[function <span class="apidocSignatureSpan">restler.Request.prototype.</span>_retry ()](#apidoc.element.restler.Request.prototype._retry)
- description and source-code
```javascript
_retry = function () {
  this.request.removeAllListeners().on('error', function() {});
  if (this.request.finished) {
    this.request.abort();
  }
  Request.call(this, this.url.href, this.options); // reusing request object to handle recursive calls and remember listeners
  this.run();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Request.prototype.abort"></a>[function <span class="apidocSignatureSpan">restler.Request.prototype.</span>abort (err)](#apidoc.element.restler.Request.prototype.abort)
- description and source-code
```javascript
abort = function (err) {
  var self = this;

  if (err) {
    if (typeof err == 'string') {
      err = new Error(err);
    } else if (!(err instanceof Error)) {
      err = new Error('AbortError');
    }
    err.type = 'abort';
  } else {
    err = null;
  }

  self.request.on('close', function() {
    if (err) {
      self._fireError(err, null);
    } else {
      self.emit('complete', null, null);
    }
  });

  self.aborted = true;
  self.request.abort();
  self.emit('abort', err);
  return this;
}
```
- example usage
```shell
...

#### events

* 'complete: function(result, response)' - emitted when the request has finished whether it was successful or not. Gets passed the
 response result and the response object as arguments. If some error has occurred, 'result' is always instance of 'Error', otherwise
 it contains response data.
* 'success: function(data, response)' - emitted when the request was successful. Gets passed the response data and the response
object as arguments.
* 'fail: function(data, response)' - emitted when the request was successful, but 4XX or 5XX status code returned. Gets passed the
 response data and the response object as arguments.
* 'error: function(err, response)' - emitted when some errors have occurred (eg. connection aborted, parse, encoding, decoding failed
 or some other unhandled errors). Gets passed the 'Error' object and the response object (when available) as arguments.
* 'abort: function()' - emitted when 'request.abort()' is called.
* 'timeout: function(ms)' - when a request takes more than the timeout option eg: {timeout:5000}, the request will be aborted. error
 and abort events will not be called, instead timeout will be emitted.
* '2XX', '3XX', '4XX', '5XX: function(data, response)' - emitted for all requests with response codes in the range (eg. '2XX' emitted
 for 200, 201, 203).
* <code><i>actual response code</i>: function(data, response)</code> - emitted for every single response code (eg. 404, 201, etc
).

#### members

* 'abort([error])' Cancels request. 'abort' event is emitted. 'request.aborted' is set to 'true'. If non-falsy 'error' is passed
, then 'error' will be additionally emitted (with 'error' passed as a param and 'error.type' is set to '"abort"'). Otherwise only
 'complete' event will raise.
...
```

#### <a name="apidoc.element.restler.Request.prototype.retry"></a>[function <span class="apidocSignatureSpan">restler.Request.prototype.</span>retry (timeout)](#apidoc.element.restler.Request.prototype.retry)
- description and source-code
```javascript
retry = function (timeout) {
  var self = this;
  timeout = parseInt(timeout);
  var fn = self._retry.bind(self);
  if (!isFinite(timeout) || timeout <= 0) {
    process.nextTick(fn, timeout);
  } else {
    setTimeout(fn, timeout);
  }
  return this;
}
```
- example usage
```shell
...

'''javascript
var rest = require('./restler');

rest.get('http://google.com').on('complete', function(result) {
if (result instanceof Error) {
  console.log('Error:', result.message);
  this.retry(5000); // try again after 5 sec
} else {
  console.log(result);
}
});

rest.get('http://twaud.io/api/v1/users/danwrong.json').on('complete', function(data) {
console.log(data[0].message); // auto convert to object
...
```

#### <a name="apidoc.element.restler.Request.prototype.run"></a>[function <span class="apidocSignatureSpan">restler.Request.prototype.</span>run ()](#apidoc.element.restler.Request.prototype.run)
- description and source-code
```javascript
run = function () {
  var self = this;
  if (this.options.multipart) {
    multipart.write(this.request, this.options.data, function() {
      self.request.end();
    });
  } else {
    if (this.options.data) {
      this.request.write(this.options.data, this.options.encoding || 'utf8');
    }
    this.request.end();
  }

  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.restler.Service"></a>[module restler.Service](#apidoc.module.restler.Service)

#### <a name="apidoc.element.restler.Service.Service"></a>[function <span class="apidocSignatureSpan">restler.</span>Service (defaults)](#apidoc.element.restler.Service.Service)
- description and source-code
```javascript
function Service(defaults) {
  if (defaults.baseURL) {
   this.baseURL = defaults.baseURL;
   delete defaults.baseURL;
  }

  this.defaults = defaults;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.restler.Service.prototype"></a>[module restler.Service.prototype](#apidoc.module.restler.Service.prototype)

#### <a name="apidoc.element.restler.Service.prototype._url"></a>[function <span class="apidocSignatureSpan">restler.Service.prototype.</span>_url (path)](#apidoc.element.restler.Service.prototype._url)
- description and source-code
```javascript
_url = function (path) {
  if (this.baseURL) return url.resolve(this.baseURL, path);
  else return path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Service.prototype._withDefaults"></a>[function <span class="apidocSignatureSpan">restler.Service.prototype.</span>_withDefaults (options)](#apidoc.element.restler.Service.prototype._withDefaults)
- description and source-code
```javascript
_withDefaults = function (options) {
  var o = mixin({}, this.defaults);
  return mixin(o, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Service.prototype.del"></a>[function <span class="apidocSignatureSpan">restler.Service.prototype.</span>del (path, options)](#apidoc.element.restler.Service.prototype.del)
- description and source-code
```javascript
del = function (path, options) {
  return del(this._url(path), this._withDefaults(options));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Service.prototype.get"></a>[function <span class="apidocSignatureSpan">restler.Service.prototype.</span>get (path, options)](#apidoc.element.restler.Service.prototype.get)
- description and source-code
```javascript
get = function (path, options) {
  return get(this._url(path), this._withDefaults(options));
}
```
- example usage
```shell
...

Example usage
-------------

'''javascript
var rest = require('./restler');

rest.get('http://google.com').on('complete', function(result) {
  if (result instanceof Error) {
    console.log('Error:', result.message);
    this.retry(5000); // try again after 5 sec
  } else {
    console.log(result);
  }
});
...
```

#### <a name="apidoc.element.restler.Service.prototype.json"></a>[function <span class="apidocSignatureSpan">restler.Service.prototype.</span>json (method, path, data, options)](#apidoc.element.restler.Service.prototype.json)
- description and source-code
```javascript
json = function (method, path, data, options) {
  return json(this._url(path), data, this._withDefaults(options), method);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Service.prototype.patch"></a>[function <span class="apidocSignatureSpan">restler.Service.prototype.</span>patch (path, options)](#apidoc.element.restler.Service.prototype.patch)
- description and source-code
```javascript
patch = function (path, options) {
  return patch(this._url(path), this._withDefaults(options));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Service.prototype.post"></a>[function <span class="apidocSignatureSpan">restler.Service.prototype.</span>post (path, options)](#apidoc.element.restler.Service.prototype.post)
- description and source-code
```javascript
post = function (path, options) {
  return post(this._url(path), this._withDefaults(options));
}
```
- example usage
```shell
...

rest.get('http://someslowdomain.com',{timeout: 10000}).on('timeout', function(ms){
  console.log('did not return within '+ms+' ms');
}).on('complete',function(data,response){
  console.log('did not time out');
});

rest.post('http://user:pass@service.com/action', {
  data: { id: 334 },
}).on('complete', function(data, response) {
  if (response.statusCode == 201) {
    // you can get at the raw response like this...
  }
});
...
```

#### <a name="apidoc.element.restler.Service.prototype.put"></a>[function <span class="apidocSignatureSpan">restler.Service.prototype.</span>put (path, options)](#apidoc.element.restler.Service.prototype.put)
- description and source-code
```javascript
put = function (path, options) {
  return put(this._url(path), this._withDefaults(options));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.Service.prototype.request"></a>[function <span class="apidocSignatureSpan">restler.Service.prototype.</span>request (path, options)](#apidoc.element.restler.Service.prototype.request)
- description and source-code
```javascript
request = function (path, options) {
  return request(this._url(path), this._withDefaults(options));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.restler.multipartform"></a>[module restler.multipartform](#apidoc.module.restler.multipartform)

#### <a name="apidoc.element.restler.multipartform.data"></a>[function <span class="apidocSignatureSpan">restler.multipartform.</span>data (filename, contentType, data)](#apidoc.element.restler.multipartform.data)
- description and source-code
```javascript
data = function (filename, contentType, data) {
  return new Data(filename, contentType, data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.multipartform.file"></a>[function <span class="apidocSignatureSpan">restler.multipartform.</span>file (path, filename, fileSize, encoding, contentType)](#apidoc.element.restler.multipartform.file)
- description and source-code
```javascript
file = function (path, filename, fileSize, encoding, contentType) {
  return new File(path, filename, fileSize, encoding, contentType)
}
```
- example usage
```shell
...
// multipart request sending a 321567 byte long file using https
rest.post('https://twaud.io/api/v1/upload.json', {
  multipart: true,
  username: 'danwrong',
  password: 'wouldntyouliketoknow',
  data: {
    'sound[message]': 'hello from restler!',
    'sound[file]': rest.file('doug-e-fresh_the-show.mp3', null, 321567, null, 'audio/mpeg')
  }
}).on('complete', function(data) {
  console.log(data.audio_url);
});

// create a service constructor for very easy API wrappers a la HTTParty...
Twitter = rest.service(function(u, p) {
...
```

#### <a name="apidoc.element.restler.multipartform.sizeOf"></a>[function <span class="apidocSignatureSpan">restler.multipartform.</span>sizeOf (parts, boundary)](#apidoc.element.restler.multipartform.sizeOf)
- description and source-code
```javascript
sizeOf = function (parts, boundary) {
  var totalSize = 0;
	  boundary = boundary || exports.defaultBoundary;
	for (var name in parts) totalSize += new Part(name, parts[name], boundary).sizeOf();
	return totalSize + boundary.length + 6;
}
```
- example usage
```shell
...
},
data: function(filename, contentType, data) {
  return new Data(filename, contentType, data);
},
sizeOf: function(parts, boundary) {
  var totalSize = 0;
	  boundary = boundary || exports.defaultBoundary;
	for (var name in parts) totalSize += new Part(name, parts[name], boundary).sizeOf();
	return totalSize + boundary.length + 6;
},
write: function(stream, data, callback, boundary) {
  var r = new MultiPartRequest(data, boundary);
  r.write(stream, callback);
  return r;
}
...
```

#### <a name="apidoc.element.restler.multipartform.write"></a>[function <span class="apidocSignatureSpan">restler.multipartform.</span>write (stream, data, callback, boundary)](#apidoc.element.restler.multipartform.write)
- description and source-code
```javascript
write = function (stream, data, callback, boundary) {
  var r = new MultiPartRequest(data, boundary);
  r.write(stream, callback);
  return r;
}
```
- example usage
```shell
...

Stream.prototype = {
//write to an internal String or to the Stream
write: function(data) {
	if (this.string != undefined) {
		this.string += data;
	} else {
		this.stream.write(data, "binary");
	}
},

//stolen from underscore.js
_isString: function(obj) {
  return !!(obj === '' || (obj && obj.charCodeAt && obj.substr));
}
...
```



# <a name="apidoc.module.restler.parsers"></a>[module restler.parsers](#apidoc.module.restler.parsers)

#### <a name="apidoc.element.restler.parsers.auto"></a>[function <span class="apidocSignatureSpan">restler.parsers.</span>auto (data, callback)](#apidoc.element.restler.parsers.auto)
- description and source-code
```javascript
auto = function (data, callback) {
  var contentType = this.headers['content-type'];
  var contentParser;
  if (contentType) {
    contentType = contentType.replace(/;.+/, ''); // remove all except mime type (eg. text/html; charset=UTF-8)
    if (contentType in parsers.auto.matchers) {
      contentParser = parsers.auto.matchers[contentType];
    } else {
      // custom (vendor) mime types
      var parts = contentType.match(/^([\w-]+)\/vnd((?:\.(?:[\w-]+))+)\+([\w-]+)$/i);
      if (parts) {
        var type = parts[1];
        var vendors = parts[2].substr(1).split('.');
        var subtype = parts[3];
        var vendorType;
        while (vendors.pop() && !(vendorType in parsers.auto.matchers)) {
          vendorType = vendors.length
            ? type + '/vnd.' + vendors.join('.') + '+' + subtype
            : vendorType = type + '/' + subtype;
        }
        contentParser = parsers.auto.matchers[vendorType];
      }
    }
  }
  if (typeof contentParser == 'function') {
    contentParser.call(this, data, callback);
  } else {
    callback(null, data);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.parsers.json"></a>[function <span class="apidocSignatureSpan">restler.parsers.</span>json (data, callback)](#apidoc.element.restler.parsers.json)
- description and source-code
```javascript
json = function (data, callback) {
  if (data && data.length) {
    var parsedData;
    try {
      parsedData = JSON.parse(data);
    } catch (err) {
      err.message = 'Failed to parse JSON body: ' + err.message;
      callback(err, null);
    }
    if (parsedData !== undefined) {
      callback(null, parsedData);
    }
  } else {
    callback(null, null);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.parsers.xml"></a>[function <span class="apidocSignatureSpan">restler.parsers.</span>xml (data, callback)](#apidoc.element.restler.parsers.xml)
- description and source-code
```javascript
xml = function (data, callback) {
  if (data) {
    var parser = new xml2js.Parser(parsers.xml.options);
    parser.parseString(data, function(err, data) {
      if (err) {
        err.message = 'Failed to parse XML body: ' + err.message;
      }
      callback(err, data);
    });
  } else {
    callback(null, null);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.restler.parsers.yaml"></a>[function <span class="apidocSignatureSpan">restler.parsers.</span>yaml (data, callback)](#apidoc.element.restler.parsers.yaml)
- description and source-code
```javascript
yaml = function (data, callback) {
  if (data) {
    try {
      callback(null, yaml.eval(data));
    } catch (err) {
      err.message = 'Failed to parse YAML body: ' + err.message;
      callback(err, null);
    }
  } else {
    callback(null, null);
  }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
