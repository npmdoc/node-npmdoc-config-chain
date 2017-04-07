# api documentation for  [config-chain (v1.1.11)](http://github.com/dominictarr/config-chain)  [![npm package](https://img.shields.io/npm/v/npmdoc-config-chain.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-config-chain) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-config-chain.svg)](https://travis-ci.org/npmdoc/node-npmdoc-config-chain)
#### HANDLE CONFIGURATION ONCE AND FOR ALL

[![NPM](https://nodei.co/npm/config-chain.png?downloads=true)](https://www.npmjs.com/package/config-chain)

[![apidoc](https://npmdoc.github.io/node-npmdoc-config-chain/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-config-chain%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-config-chain/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-config-chain/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-config-chain/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Dominic Tarr",
        "email": "dominic.tarr@gmail.com",
        "url": "http://dominictarr.com"
    },
    "bugs": {
        "url": "https://github.com/dominictarr/config-chain/issues"
    },
    "dependencies": {
        "ini": "^1.3.4",
        "proto-list": "~1.2.1"
    },
    "description": "HANDLE CONFIGURATION ONCE AND FOR ALL",
    "devDependencies": {
        "tap": "0.3.0"
    },
    "directories": {},
    "dist": {
        "shasum": "aba09747dfbe4c3e70e766a6e41586e1859fc6f2",
        "tarball": "https://registry.npmjs.org/config-chain/-/config-chain-1.1.11.tgz"
    },
    "gitHead": "0976c33f2f126a060a289284bb031a5f7aeba329",
    "homepage": "http://github.com/dominictarr/config-chain",
    "licenses": [
        {
            "type": "MIT",
            "url": "https://raw.githubusercontent.com/dominictarr/config-chain/master/LICENCE"
        }
    ],
    "maintainers": [
        {
            "name": "dominictarr",
            "email": "dominic.tarr@gmail.com"
        },
        {
            "name": "isaacs",
            "email": "i@izs.me"
        }
    ],
    "name": "config-chain",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/dominictarr/config-chain.git"
    },
    "scripts": {
        "test": "tap test/"
    },
    "version": "1.1.11"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module config-chain](#apidoc.module.config-chain)
1.  [function <span class="apidocSignatureSpan">config-chain.</span>ConfigChain ()](#apidoc.element.config-chain.ConfigChain)
1.  [function <span class="apidocSignatureSpan">config-chain.</span>env (prefix, env)](#apidoc.element.config-chain.env)
1.  [function <span class="apidocSignatureSpan">config-chain.</span>find ()](#apidoc.element.config-chain.find)
1.  [function <span class="apidocSignatureSpan">config-chain.</span>json ()](#apidoc.element.config-chain.json)
1.  [function <span class="apidocSignatureSpan">config-chain.</span>parse (content, file, type)](#apidoc.element.config-chain.parse)
1.  object <span class="apidocSignatureSpan">config-chain.</span>ConfigChain.prototype

#### [module config-chain.ConfigChain](#apidoc.module.config-chain.ConfigChain)
1.  [function <span class="apidocSignatureSpan">config-chain.</span>ConfigChain ()](#apidoc.element.config-chain.ConfigChain.ConfigChain)

#### [module config-chain.ConfigChain.prototype](#apidoc.module.config-chain.ConfigChain.prototype)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>_await ()](#apidoc.element.config-chain.ConfigChain.prototype._await)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>_resolve ()](#apidoc.element.config-chain.ConfigChain.prototype._resolve)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>add (data, marker)](#apidoc.element.config-chain.ConfigChain.prototype.add)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>addEnv (prefix, env, name)](#apidoc.element.config-chain.ConfigChain.prototype.addEnv)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>addFile (file, type, name)](#apidoc.element.config-chain.ConfigChain.prototype.addFile)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>addListener (type, listener)](#apidoc.element.config-chain.ConfigChain.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>addString (data, file, type, marker)](#apidoc.element.config-chain.ConfigChain.prototype.addString)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>addUrl (req, type, name)](#apidoc.element.config-chain.ConfigChain.prototype.addUrl)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>del (key, where)](#apidoc.element.config-chain.ConfigChain.prototype.del)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>emit (type)](#apidoc.element.config-chain.ConfigChain.prototype.emit)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>eventNames ()](#apidoc.element.config-chain.ConfigChain.prototype.eventNames)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>get (key, where)](#apidoc.element.config-chain.ConfigChain.prototype.get)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>getMaxListeners ()](#apidoc.element.config-chain.ConfigChain.prototype.getMaxListeners)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>listenerCount (type)](#apidoc.element.config-chain.ConfigChain.prototype.listenerCount)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>listeners (type)](#apidoc.element.config-chain.ConfigChain.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>on (type, listener)](#apidoc.element.config-chain.ConfigChain.prototype.on)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>once (type, listener)](#apidoc.element.config-chain.ConfigChain.prototype.once)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>parse (content, file, type)](#apidoc.element.config-chain.ConfigChain.prototype.parse)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>prependListener (type, listener)](#apidoc.element.config-chain.ConfigChain.prototype.prependListener)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>prependOnceListener (type, listener)](#apidoc.element.config-chain.ConfigChain.prototype.prependOnceListener)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>removeAllListeners (type)](#apidoc.element.config-chain.ConfigChain.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>removeListener (type, listener)](#apidoc.element.config-chain.ConfigChain.prototype.removeListener)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>save (where, type, cb)](#apidoc.element.config-chain.ConfigChain.prototype.save)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>set (key, value, where)](#apidoc.element.config-chain.ConfigChain.prototype.set)
1.  [function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>setMaxListeners (n)](#apidoc.element.config-chain.ConfigChain.prototype.setMaxListeners)
1.  undefined <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>domain



# <a name="apidoc.module.config-chain"></a>[module config-chain](#apidoc.module.config-chain)

#### <a name="apidoc.element.config-chain.ConfigChain"></a>[function <span class="apidocSignatureSpan">config-chain.</span>ConfigChain ()](#apidoc.element.config-chain.ConfigChain)
- description and source-code
```javascript
function ConfigChain() {
  EE.apply(this)
  ProtoList.apply(this, arguments)
  this._awaiting = 0
  this._saving = 0
  this.sources = {}
}
```
- example usage
```shell
...
Get all the keys on the provided env object (or process.env) which are
prefixed by the specified prefix, and put the values on a new object.

RETURN THE RESULTING OBJECT!

NO I/O!

## cc.ConfigChain()

The ConfigChain class for CRAY CRAY JQUERY STYLE METHOD CHAINING!

One of these is returned by the main exported function, as well.

It inherits (prototypically) from
[ProtoList](https://github.com/isaacs/proto-list/), and also inherits
...
```

#### <a name="apidoc.element.config-chain.env"></a>[function <span class="apidocSignatureSpan">config-chain.</span>env (prefix, env)](#apidoc.element.config-chain.env)
- description and source-code
```javascript
env = function (prefix, env) {
  env = env || process.env
  var obj = {}
  var l = prefix.length
  for(var k in env) {
    if(k.indexOf(prefix) === 0)
      obj[k.substring(l)] = env[k]
  }

  return obj
}
```
- example usage
```shell
...
  this.addString(data, file, type, marker)
}.bind(this))
return this
}

ConfigChain.prototype.addEnv = function (prefix, env, name) {
name = name || 'env'
var data = exports.env(prefix, env)
this.sources[name] = { data: data, source: env, prefix: prefix }
return this.add(data, name)
}

ConfigChain.prototype.addUrl = function (req, type, name) {
this._await()
var href = url.format(req)
...
```

#### <a name="apidoc.element.config-chain.find"></a>[function <span class="apidocSignatureSpan">config-chain.</span>find ()](#apidoc.element.config-chain.find)
- description and source-code
```javascript
find = function () {
  var rel = path.join.apply(null, [].slice.call(arguments))

  function find(start, rel) {
    var file = path.join(start, rel)
    try {
      fs.statSync(file)
      return file
    } catch (err) {
      if(path.dirname(start) !== start) // root
        return find(path.dirname(start), rel)
    }
  }
  return find(__dirname, rel)
}
```
- example usage
```shell
...
  ? path.join(__dirname, 'special.json') //load a special file
  : null //NULL IS IGNORED!

//SUBDIR FOR ENV CONFIG
path.join(__dirname,  'config', env, 'config.json'),

//SEARCH PARENT DIRECTORIES FROM CURRENT DIR FOR FILE
cc.find('config.json'),

//PUT DEFAULTS LAST
{
  host: 'localhost'
  port: 8000
})
...
```

#### <a name="apidoc.element.config-chain.json"></a>[function <span class="apidocSignatureSpan">config-chain.</span>json ()](#apidoc.element.config-chain.json)
- description and source-code
```javascript
json = function () {
  var args = [].slice.call(arguments).filter(function (arg) { return arg != null })
  var file = path.join.apply(null, args)
  var content
  try {
    content = fs.readFileSync(file,'utf-8')
  } catch (err) {
    return
  }
  return parse(content, file, 'json')
}
```
- example usage
```shell
...

If the arg is a STRING, then it shall be a JSON FILENAME.

SYNC I/O!

RETURN THE CHAIN!

## cc.json(...args)

Join the args INTO A JSON FILENAME!

SYNC I/O!

## cc.find(relativePath)
...
```

#### <a name="apidoc.element.config-chain.parse"></a>[function <span class="apidocSignatureSpan">config-chain.</span>parse (content, file, type)](#apidoc.element.config-chain.parse)
- description and source-code
```javascript
parse = function (content, file, type) {
  content = '' + content
  // if we don't know what it is, try json and fall back to ini
  // if we know what it is, then it must be that.
  if (!type) {
    try { return JSON.parse(content) }
    catch (er) { return ini.parse(content) }
  } else if (type === 'json') {
    if (this.emit) {
      try { return JSON.parse(content) }
      catch (er) { this.emit('error', er) }
    } else {
      return JSON.parse(content)
    }
  } else {
    return ini.parse(content)
  }
}
```
- example usage
```shell
...
}

var parse = exports.parse = function (content, file, type) {
content = '' + content
// if we don't know what it is, try json and fall back to ini
// if we know what it is, then it must be that.
if (!type) {
  try { return JSON.parse(content) }
  catch (er) { return ini.parse(content) }
} else if (type === 'json') {
  if (this.emit) {
    try { return JSON.parse(content) }
    catch (er) { this.emit('error', er) }
  } else {
    return JSON.parse(content)
...
```



# <a name="apidoc.module.config-chain.ConfigChain"></a>[module config-chain.ConfigChain](#apidoc.module.config-chain.ConfigChain)

#### <a name="apidoc.element.config-chain.ConfigChain.ConfigChain"></a>[function <span class="apidocSignatureSpan">config-chain.</span>ConfigChain ()](#apidoc.element.config-chain.ConfigChain.ConfigChain)
- description and source-code
```javascript
function ConfigChain() {
  EE.apply(this)
  ProtoList.apply(this, arguments)
  this._awaiting = 0
  this._saving = 0
  this.sources = {}
}
```
- example usage
```shell
...
Get all the keys on the provided env object (or process.env) which are
prefixed by the specified prefix, and put the values on a new object.

RETURN THE RESULTING OBJECT!

NO I/O!

## cc.ConfigChain()

The ConfigChain class for CRAY CRAY JQUERY STYLE METHOD CHAINING!

One of these is returned by the main exported function, as well.

It inherits (prototypically) from
[ProtoList](https://github.com/isaacs/proto-list/), and also inherits
...
```



# <a name="apidoc.module.config-chain.ConfigChain.prototype"></a>[module config-chain.ConfigChain.prototype](#apidoc.module.config-chain.ConfigChain.prototype)

#### <a name="apidoc.element.config-chain.ConfigChain.prototype._await"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>_await ()](#apidoc.element.config-chain.ConfigChain.prototype._await)
- description and source-code
```javascript
_await = function () {
  this._awaiting++
}
```
- example usage
```shell
...
}

ConfigChain.prototype.addFile = function (file, type, name) {
  name = name || file
  var marker = {__source__:name}
  this.sources[name] = { path: file, type: type }
  this.push(marker)
  this._await()
  fs.readFile(file, 'utf8', function (er, data) {
    if (er) this.emit('error', er)
    this.addString(data, file, type, marker)
  }.bind(this))
  return this
}
...
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype._resolve"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>_resolve ()](#apidoc.element.config-chain.ConfigChain.prototype._resolve)
- description and source-code
```javascript
_resolve = function () {
  this._awaiting--
  if (this._awaiting === 0) this.emit('load', this)
}
```
- example usage
```shell
...
    return this.emit('error', new Error('bad marker'))
  }
  this.splice(i, 1, data)
  marker = marker.__source__
  this.sources[marker] = this.sources[marker] || {}
  this.sources[marker].data = data
  // we were waiting for this.  maybe emit 'load'
  this._resolve()
} else {
  if (typeof marker === 'string') {
    this.sources[marker] = this.sources[marker] || {}
    this.sources[marker].data = data
  }
  // trigger the load event if nothing was already going to do so.
  this._await()
...
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.add"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>add (data, marker)](#apidoc.element.config-chain.ConfigChain.prototype.add)
- description and source-code
```javascript
add = function (data, marker) {
  if (marker && typeof marker === 'object') {
    var i = this.list.indexOf(marker)
    if (i === -1) {
      return this.emit('error', new Error('bad marker'))
    }
    this.splice(i, 1, data)
    marker = marker.__source__
    this.sources[marker] = this.sources[marker] || {}
    this.sources[marker].data = data
    // we were waiting for this.  maybe emit 'load'
    this._resolve()
  } else {
    if (typeof marker === 'string') {
      this.sources[marker] = this.sources[marker] || {}
      this.sources[marker].data = data
    }
    // trigger the load event if nothing was already going to do so.
    this._await()
    this.push(data)
    process.nextTick(this._resolve.bind(this))
  }
  return this
}
```
- example usage
```shell
...
return this
}

ConfigChain.prototype.addEnv = function (prefix, env, name) {
name = name || 'env'
var data = exports.env(prefix, env)
this.sources[name] = { data: data, source: env, prefix: prefix }
return this.add(data, name)
}

ConfigChain.prototype.addUrl = function (req, type, name) {
this._await()
var href = url.format(req)
name = name || href
var marker = {__source__:name}
...
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.addEnv"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>addEnv (prefix, env, name)](#apidoc.element.config-chain.ConfigChain.prototype.addEnv)
- description and source-code
```javascript
addEnv = function (prefix, env, name) {
  name = name || 'env'
  var data = exports.env(prefix, env)
  this.sources[name] = { data: data, source: env, prefix: prefix }
  return this.add(data, name)
}
```
- example usage
```shell
...

## chain.addUrl(url, type, [name=url])

Same as the filename thing, but with a url.

Can't be saved later.

## chain.addEnv(prefix, env, [name='env'])

Add all the keys from the env object that start with the prefix.

## chain.addString(data, file, type, [name])

Parse the string and add it to the set.  (Mainly used internally.)
...
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.addFile"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>addFile (file, type, name)](#apidoc.element.config-chain.ConfigChain.prototype.addFile)
- description and source-code
```javascript
addFile = function (file, type, name) {
  name = name || file
  var marker = {__source__:name}
  this.sources[name] = { path: file, type: type }
  this.push(marker)
  this._await()
  fs.readFile(file, 'utf8', function (er, data) {
    if (er) this.emit('error', er)
    this.addString(data, file, type, marker)
  }.bind(this))
  return this
}
```
- example usage
```shell
...
  },
  cc.find('config.json'),
  cc.env('myApp_')
)
// CONFIGS AS A SERVICE, aka "CaaS", aka EVERY DEVOPS DREAM OMG!
.addUrl('http://configurator:1234/my-configs')
// ASYNC FTW!
.addFile('/path/to/file.json')

// OBJECTS ARE OK TOO, they're SYNC but they still ORDER RIGHT
// BECAUSE PROMISES ARE USED BUT NO, NOT *THOSE* PROMISES, JUST
// ACTUAL PROMISES LIKE YOU MAKE TO YOUR MOM, KEPT OUT OF LOVE
.add({ another: 'object' })

// DIE A THOUSAND DEATHS IF THIS EVER HAPPENS!!
...
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.addListener"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>addListener (type, listener)](#apidoc.element.config-chain.ConfigChain.prototype.addListener)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.addString"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>addString (data, file, type, marker)](#apidoc.element.config-chain.ConfigChain.prototype.addString)
- description and source-code
```javascript
addString = function (data, file, type, marker) {
  data = this.parse(data, file, type)
  this.add(data, marker)
  return this
}
```
- example usage
```shell
...
name = name || file
var marker = {__source__:name}
this.sources[name] = { path: file, type: type }
this.push(marker)
this._await()
fs.readFile(file, 'utf8', function (er, data) {
  if (er) this.emit('error', er)
  this.addString(data, file, type, marker)
}.bind(this))
return this
}

ConfigChain.prototype.addEnv = function (prefix, env, name) {
name = name || 'env'
var data = exports.env(prefix, env)
...
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.addUrl"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>addUrl (req, type, name)](#apidoc.element.config-chain.ConfigChain.prototype.addUrl)
- description and source-code
```javascript
addUrl = function (req, type, name) {
  this._await()
  var href = url.format(req)
  name = name || href
  var marker = {__source__:name}
  this.sources[name] = { href: href, type: type }
  this.push(marker)
  http.request(req, function (res) {
    var c = []
    var ct = res.headers['content-type']
    if (!type) {
      type = ct.indexOf('json') !== -1 ? 'json'
           : ct.indexOf('ini') !== -1 ? 'ini'
           : href.match(/\.json$/) ? 'json'
           : href.match(/\.ini$/) ? 'ini'
           : null
      marker.type = type
    }

    res.on('data', c.push.bind(c))
    .on('end', function () {
      this.addString(Buffer.concat(c), href, type, marker)
    }.bind(this))
    .on('error', this.emit.bind(this, 'error'))

  }.bind(this))
  .on('error', this.emit.bind(this, 'error'))
  .end()

  return this
}
```
- example usage
```shell
...
var config = cc({
    some: 'object'
  },
  cc.find('config.json'),
  cc.env('myApp_')
)
// CONFIGS AS A SERVICE, aka "CaaS", aka EVERY DEVOPS DREAM OMG!
.addUrl('http://configurator:1234/my-configs')
// ASYNC FTW!
.addFile('/path/to/file.json')

// OBJECTS ARE OK TOO, they're SYNC but they still ORDER RIGHT
// BECAUSE PROMISES ARE USED BUT NO, NOT *THOSE* PROMISES, JUST
// ACTUAL PROMISES LIKE YOU MAKE TO YOUR MOM, KEPT OUT OF LOVE
.add({ another: 'object' })
...
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.del"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>del (key, where)](#apidoc.element.config-chain.ConfigChain.prototype.del)
- description and source-code
```javascript
del = function (key, where) {
  // if not specified where, then delete from the whole chain, scorched
  // earth style
  if (where) {
    var target = this.sources[where]
    target = target && target.data
    if (!target) {
      return this.emit('error', new Error('not found '+where))
    }
    delete target[key]
  } else {
    for (var i = 0, l = this.list.length; i < l; i ++) {
      delete this.list[i][key]
    }
  }
  return this
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.emit"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>emit (type)](#apidoc.element.config-chain.ConfigChain.prototype.emit)
- description and source-code
```javascript
function emit(type) {
  var er, handler, len, args, i, events, domain;
  var needDomainExit = false;
  var doError = (type === 'error');

  events = this._events;
  if (events)
    doError = (doError && events.error == null);
  else if (!doError)
    return false;

  domain = this.domain;

  // If there is no 'error' event listener then throw.
  if (doError) {
    er = arguments[1];
    if (domain) {
      if (!er)
        er = new Error('Uncaught, unspecified "error" event');
      er.domainEmitter = this;
      er.domain = domain;
      er.domainThrown = false;
      domain.emit('error', er);
    } else if (er instanceof Error) {
      throw er; // Unhandled 'error' event
    } else {
      // At least give some kind of context to the user
      var err = new Error('Uncaught, unspecified "error" event. (' + er + ')');
      err.context = er;
      throw err;
    }
    return false;
  }

  handler = events[type];

  if (!handler)
    return false;

  if (domain && this !== process) {
    domain.enter();
    needDomainExit = true;
  }

  var isFn = typeof handler === 'function';
  len = arguments.length;
  switch (len) {
    // fast cases
    case 1:
      emitNone(handler, isFn, this);
      break;
    case 2:
      emitOne(handler, isFn, this, arguments[1]);
      break;
    case 3:
      emitTwo(handler, isFn, this, arguments[1], arguments[2]);
      break;
    case 4:
      emitThree(handler, isFn, this, arguments[1], arguments[2], arguments[3]);
      break;
    // slower
    default:
      args = new Array(len - 1);
      for (i = 1; i < len; i++)
        args[i - 1] = arguments[i];
      emitMany(handler, isFn, this, args);
  }

  if (needDomainExit)
    domain.exit();

  return true;
}
```
- example usage
```shell
...
  // if we know what it is, then it must be that.
  if (!type) {
    try { return JSON.parse(content) }
    catch (er) { return ini.parse(content) }
  } else if (type === 'json') {
    if (this.emit) {
      try { return JSON.parse(content) }
      catch (er) { this.emit('error', er) }
    } else {
      return JSON.parse(content)
    }
  } else {
    return ini.parse(content)
  }
}
...
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.eventNames"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>eventNames ()](#apidoc.element.config-chain.ConfigChain.prototype.eventNames)
- description and source-code
```javascript
function eventNames() {
  return this._eventsCount > 0 ? Reflect.ownKeys(this._events) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.get"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>get (key, where)](#apidoc.element.config-chain.ConfigChain.prototype.get)
- description and source-code
```javascript
get = function (key, where) {
  if (where) {
    where = this.sources[where]
    if (where) where = where.data
    if (where && Object.hasOwnProperty.call(where, key)) return where[key]
    return undefined
  }
  return this.list[0][key]
}
```
- example usage
```shell
...

    //PUT DEFAULTS LAST
    {
      host: 'localhost'
      port: 8000
    })

  var host = conf.get('host')

  // or

  var host = conf.store.host

'''
...
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.getMaxListeners"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>getMaxListeners ()](#apidoc.element.config-chain.ConfigChain.prototype.getMaxListeners)
- description and source-code
```javascript
function getMaxListeners() {
  return $getMaxListeners(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.listenerCount"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>listenerCount (type)](#apidoc.element.config-chain.ConfigChain.prototype.listenerCount)
- description and source-code
```javascript
function listenerCount(type) {
  const events = this._events;

  if (events) {
    const evlistener = events[type];

    if (typeof evlistener === 'function') {
      return 1;
    } else if (evlistener) {
      return evlistener.length;
    }
  }

  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.listeners"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>listeners (type)](#apidoc.element.config-chain.ConfigChain.prototype.listeners)
- description and source-code
```javascript
function listeners(type) {
  var evlistener;
  var ret;
  var events = this._events;

  if (!events)
    ret = [];
  else {
    evlistener = events[type];
    if (!evlistener)
      ret = [];
    else if (typeof evlistener === 'function')
      ret = [evlistener];
    else
      ret = arrayClone(evlistener, evlistener.length);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.on"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>on (type, listener)](#apidoc.element.config-chain.ConfigChain.prototype.on)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
...
         : ct.indexOf('ini') !== -1 ? 'ini'
         : href.match(/\.json$/) ? 'json'
         : href.match(/\.ini$/) ? 'ini'
         : null
    marker.type = type
  }

  res.on('data', c.push.bind(c))
  .on('end', function () {
    this.addString(Buffer.concat(c), href, type, marker)
  }.bind(this))
  .on('error', this.emit.bind(this, 'error'))

}.bind(this))
.on('error', this.emit.bind(this, 'error'))
...
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.once"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>once (type, listener)](#apidoc.element.config-chain.ConfigChain.prototype.once)
- description and source-code
```javascript
function once(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.on(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.parse"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>parse (content, file, type)](#apidoc.element.config-chain.ConfigChain.prototype.parse)
- description and source-code
```javascript
parse = function (content, file, type) {
  content = '' + content
  // if we don't know what it is, try json and fall back to ini
  // if we know what it is, then it must be that.
  if (!type) {
    try { return JSON.parse(content) }
    catch (er) { return ini.parse(content) }
  } else if (type === 'json') {
    if (this.emit) {
      try { return JSON.parse(content) }
      catch (er) { this.emit('error', er) }
    } else {
      return JSON.parse(content)
    }
  } else {
    return ini.parse(content)
  }
}
```
- example usage
```shell
...
}

var parse = exports.parse = function (content, file, type) {
content = '' + content
// if we don't know what it is, try json and fall back to ini
// if we know what it is, then it must be that.
if (!type) {
  try { return JSON.parse(content) }
  catch (er) { return ini.parse(content) }
} else if (type === 'json') {
  if (this.emit) {
    try { return JSON.parse(content) }
    catch (er) { this.emit('error', er) }
  } else {
    return JSON.parse(content)
...
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.prependListener"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>prependListener (type, listener)](#apidoc.element.config-chain.ConfigChain.prototype.prependListener)
- description and source-code
```javascript
function prependListener(type, listener) {
  return _addListener(this, type, listener, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.prependOnceListener"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>prependOnceListener (type, listener)](#apidoc.element.config-chain.ConfigChain.prototype.prependOnceListener)
- description and source-code
```javascript
function prependOnceListener(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.prependListener(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>removeAllListeners (type)](#apidoc.element.config-chain.ConfigChain.prototype.removeAllListeners)
- description and source-code
```javascript
function removeAllListeners(type) {
  var listeners, events;

  events = this._events;
  if (!events)
    return this;

  // not listening for removeListener, no need to emit
  if (!events.removeListener) {
    if (arguments.length === 0) {
      this._events = new EventHandlers();
      this._eventsCount = 0;
    } else if (events[type]) {
      if (--this._eventsCount === 0)
        this._events = new EventHandlers();
      else
        delete events[type];
    }
    return this;
  }

  // emit removeListener for all listeners on all events
  if (arguments.length === 0) {
    var keys = Object.keys(events);
    for (var i = 0, key; i < keys.length; ++i) {
      key = keys[i];
      if (key === 'removeListener') continue;
      this.removeAllListeners(key);
    }
    this.removeAllListeners('removeListener');
    this._events = new EventHandlers();
    this._eventsCount = 0;
    return this;
  }

  listeners = events[type];

  if (typeof listeners === 'function') {
    this.removeListener(type, listeners);
  } else if (listeners) {
    // LIFO order
    do {
      this.removeListener(type, listeners[listeners.length - 1]);
    } while (listeners[0]);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>removeListener (type, listener)](#apidoc.element.config-chain.ConfigChain.prototype.removeListener)
- description and source-code
```javascript
function removeListener(type, listener) {
  var list, events, position, i, originalListener;

  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');

  events = this._events;
  if (!events)
    return this;

  list = events[type];
  if (!list)
    return this;

  if (list === listener || list.listener === listener) {
    if (--this._eventsCount === 0)
      this._events = new EventHandlers();
    else {
      delete events[type];
      if (events.removeListener)
        this.emit('removeListener', type, list.listener || listener);
    }
  } else if (typeof list !== 'function') {
    position = -1;

    for (i = list.length; i-- > 0;) {
      if (list[i] === listener || list[i].listener === listener) {
        originalListener = list[i].listener;
        position = i;
        break;
      }
    }

    if (position < 0)
      return this;

    if (list.length === 1) {
      list[0] = undefined;
      if (--this._eventsCount === 0) {
        this._events = new EventHandlers();
        return this;
      } else {
        delete events[type];
      }
    } else {
      spliceOne(list, position);
    }

    if (events.removeListener)
      this.emit('removeListener', type, originalListener || listener);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.save"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>save (where, type, cb)](#apidoc.element.config-chain.ConfigChain.prototype.save)
- description and source-code
```javascript
save = function (where, type, cb) {
  if (typeof type === 'function') cb = type, type = null
  var target = this.sources[where]
  if (!target || !(target.path || target.source) || !target.data) {
    // TODO: maybe save() to a url target could be a PUT or something?
    // would be easy to swap out with a reddis type thing, too
    return this.emit('error', new Error('bad save target: '+where))
  }

  if (target.source) {
    var pref = target.prefix || ''
    Object.keys(target.data).forEach(function (k) {
      target.source[pref + k] = target.data[k]
    })
    return this
  }

  var type = type || target.type
  var data = target.data
  if (target.type === 'json') {
    data = JSON.stringify(data)
  } else {
    data = ini.stringify(data)
  }

  this._saving ++
  fs.writeFile(target.path, data, 'utf8', function (er) {
    this._saving --
    if (er) {
      if (cb) return cb(er)
      else return this.emit('error', er)
    }
    if (this._saving === 0) {
      if (cb) cb()
      this.emit('save')
    }
  }.bind(this))
  return this
}
```
- example usage
```shell
...
the one with the highest priority, which was added first.)

## chain.get(key, [name])

Get the key from the named config object explicitly, or from the
resolved configs if not specified.

## chain.save(name, type)

Write the named config object back to its origin.

Currently only supported for env and file config types.

For files, encode the data according to the type.
...
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.set"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>set (key, value, where)](#apidoc.element.config-chain.ConfigChain.prototype.set)
- description and source-code
```javascript
set = function (key, value, where) {
  var target

  if (where) {
    target = this.sources[where]
    target = target && target.data
    if (!target) {
      return this.emit('error', new Error('not found '+where))
    }
  } else {
    target = this.list[0]
    if (!target) {
      return this.emit('error', new Error('cannot set, no confs!'))
    }
  }
  target[key] = value
  return this
}
```
- example usage
```shell
...
## chain.root {Object}

The root from which all the other config objects in the set descend
prototypically.

Put your defaults here.

## chain.set(key, value, name)

Set the key to the value on the named config object.  If name is
unset, then set it on the first config object in the set.  (That is,
the one with the highest priority, which was added first.)

## chain.get(key, [name])
...
```

#### <a name="apidoc.element.config-chain.ConfigChain.prototype.setMaxListeners"></a>[function <span class="apidocSignatureSpan">config-chain.ConfigChain.prototype.</span>setMaxListeners (n)](#apidoc.element.config-chain.ConfigChain.prototype.setMaxListeners)
- description and source-code
```javascript
function setMaxListeners(n) {
  if (typeof n !== 'number' || n < 0 || isNaN(n))
    throw new TypeError('"n" argument must be a positive number');
  this._maxListeners = n;
  return this;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
