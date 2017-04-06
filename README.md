# api documentation for  [axon (v2.0.3)](https://github.com/visionmedia/axon#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-axon.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-axon) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-axon.svg)](https://travis-ci.org/npmdoc/node-npmdoc-axon)
#### High-level messaging & socket patterns implemented in pure js

[![NPM](https://nodei.co/npm/axon.png?downloads=true)](https://www.npmjs.com/package/axon)

[![apidoc](https://npmdoc.github.io/node-npmdoc-axon/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-axon_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-axon/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-axon/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-axon/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "TJ Holowaychuk",
        "email": "tj@vision-media.ca"
    },
    "bugs": {
        "url": "https://github.com/visionmedia/axon/issues"
    },
    "dependencies": {
        "amp": "~0.3.1",
        "amp-message": "~0.1.1",
        "configurable": "0.0.1",
        "debug": "*",
        "escape-regexp": "0.0.1"
    },
    "description": "High-level messaging & socket patterns implemented in pure js",
    "devDependencies": {
        "better-assert": "~1.0.1",
        "commander": "~2.4.0",
        "humanize-number": "0.0.1",
        "mocha": "~1.21.5",
        "should": "~4.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "90bc9a31e30acfdaeff795ada7aba22c51079692",
        "tarball": "https://registry.npmjs.org/axon/-/axon-2.0.3.tgz"
    },
    "engines": {
        "node": ">= 0.11.8"
    },
    "gitHead": "df2f5bb1637e39f1391dfd8f355db94f9b768e87",
    "homepage": "https://github.com/visionmedia/axon#readme",
    "keywords": [
        "zmq",
        "zeromq",
        "pubsub",
        "socket",
        "emitter",
        "ipc",
        "rpc"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "tjholowaychuk",
            "email": "tj@vision-media.ca"
        },
        {
            "name": "gjohnson",
            "email": "gjj391@gmail.com"
        },
        {
            "name": "jcrugzz",
            "email": "jcrugzz@gmail.com"
        }
    ],
    "name": "axon",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/visionmedia/axon.git"
    },
    "scripts": {
        "test": "make test"
    },
    "version": "2.0.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module axon](#apidoc.module.axon)
1.  [function <span class="apidocSignatureSpan">axon.</span>PubEmitterSocket ()](#apidoc.element.axon.PubEmitterSocket)
1.  [function <span class="apidocSignatureSpan">axon.</span>PubSocket ()](#apidoc.element.axon.PubSocket)
1.  [function <span class="apidocSignatureSpan">axon.</span>PullSocket ()](#apidoc.element.axon.PullSocket)
1.  [function <span class="apidocSignatureSpan">axon.</span>PushSocket ()](#apidoc.element.axon.PushSocket)
1.  [function <span class="apidocSignatureSpan">axon.</span>RepSocket ()](#apidoc.element.axon.RepSocket)
1.  [function <span class="apidocSignatureSpan">axon.</span>ReqSocket ()](#apidoc.element.axon.ReqSocket)
1.  [function <span class="apidocSignatureSpan">axon.</span>Socket ()](#apidoc.element.axon.Socket)
1.  [function <span class="apidocSignatureSpan">axon.</span>SubEmitterSocket ()](#apidoc.element.axon.SubEmitterSocket)
1.  [function <span class="apidocSignatureSpan">axon.</span>SubSocket ()](#apidoc.element.axon.SubSocket)
1.  [function <span class="apidocSignatureSpan">axon.</span>socket (type, options)](#apidoc.element.axon.socket)
1.  object <span class="apidocSignatureSpan">axon.</span>PubSocket.prototype
1.  object <span class="apidocSignatureSpan">axon.</span>PullSocket.prototype
1.  object <span class="apidocSignatureSpan">axon.</span>RepSocket.prototype
1.  object <span class="apidocSignatureSpan">axon.</span>ReqSocket.prototype
1.  object <span class="apidocSignatureSpan">axon.</span>Socket.prototype
1.  object <span class="apidocSignatureSpan">axon.</span>SubEmitterSocket.prototype
1.  object <span class="apidocSignatureSpan">axon.</span>SubSocket.prototype
1.  object <span class="apidocSignatureSpan">axon.</span>types
1.  object <span class="apidocSignatureSpan">axon.</span>utils

#### [module axon.PubSocket](#apidoc.module.axon.PubSocket)
1.  [function <span class="apidocSignatureSpan">axon.</span>PubSocket ()](#apidoc.element.axon.PubSocket.PubSocket)

#### [module axon.PubSocket.prototype](#apidoc.module.axon.PubSocket.prototype)
1.  [function <span class="apidocSignatureSpan">axon.PubSocket.prototype.</span>send (msg)](#apidoc.element.axon.PubSocket.prototype.send)

#### [module axon.PullSocket](#apidoc.module.axon.PullSocket)
1.  [function <span class="apidocSignatureSpan">axon.</span>PullSocket ()](#apidoc.element.axon.PullSocket.PullSocket)

#### [module axon.PullSocket.prototype](#apidoc.module.axon.PullSocket.prototype)
1.  [function <span class="apidocSignatureSpan">axon.PullSocket.prototype.</span>send ()](#apidoc.element.axon.PullSocket.prototype.send)

#### [module axon.RepSocket](#apidoc.module.axon.RepSocket)
1.  [function <span class="apidocSignatureSpan">axon.</span>RepSocket ()](#apidoc.element.axon.RepSocket.RepSocket)

#### [module axon.RepSocket.prototype](#apidoc.module.axon.RepSocket.prototype)
1.  [function <span class="apidocSignatureSpan">axon.RepSocket.prototype.</span>onmessage (sock)](#apidoc.element.axon.RepSocket.prototype.onmessage)

#### [module axon.ReqSocket](#apidoc.module.axon.ReqSocket)
1.  [function <span class="apidocSignatureSpan">axon.</span>ReqSocket ()](#apidoc.element.axon.ReqSocket.ReqSocket)

#### [module axon.ReqSocket.prototype](#apidoc.module.axon.ReqSocket.prototype)
1.  [function <span class="apidocSignatureSpan">axon.ReqSocket.prototype.</span>id ()](#apidoc.element.axon.ReqSocket.prototype.id)
1.  [function <span class="apidocSignatureSpan">axon.ReqSocket.prototype.</span>onmessage ()](#apidoc.element.axon.ReqSocket.prototype.onmessage)
1.  [function <span class="apidocSignatureSpan">axon.ReqSocket.prototype.</span>send (msg)](#apidoc.element.axon.ReqSocket.prototype.send)

#### [module axon.Socket](#apidoc.module.axon.Socket)
1.  [function <span class="apidocSignatureSpan">axon.</span>Socket ()](#apidoc.element.axon.Socket.Socket)

#### [module axon.Socket.prototype](#apidoc.module.axon.Socket.prototype)
1.  [function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>addSocket (sock)](#apidoc.element.axon.Socket.prototype.addSocket)
1.  [function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>address ()](#apidoc.element.axon.Socket.prototype.address)
1.  [function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>bind (port, host, fn)](#apidoc.element.axon.Socket.prototype.bind)
1.  [function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>close (fn)](#apidoc.element.axon.Socket.prototype.close)
1.  [function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>closeServer (fn)](#apidoc.element.axon.Socket.prototype.closeServer)
1.  [function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>closeSockets ()](#apidoc.element.axon.Socket.prototype.closeSockets)
1.  [function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>connect (port, host, fn)](#apidoc.element.axon.Socket.prototype.connect)
1.  [function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>disable (name)](#apidoc.element.axon.Socket.prototype.disable)
1.  [function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>disabled (name)](#apidoc.element.axon.Socket.prototype.disabled)
1.  [function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>enable (name)](#apidoc.element.axon.Socket.prototype.enable)
1.  [function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>enabled (name)](#apidoc.element.axon.Socket.prototype.enabled)
1.  [function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>get (name)](#apidoc.element.axon.Socket.prototype.get)
1.  [function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>handleErrors (sock)](#apidoc.element.axon.Socket.prototype.handleErrors)
1.  [function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>onconnect (sock)](#apidoc.element.axon.Socket.prototype.onconnect)
1.  [function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>onmessage (sock)](#apidoc.element.axon.Socket.prototype.onmessage)
1.  [function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>pack (args)](#apidoc.element.axon.Socket.prototype.pack)
1.  [function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>removeSocket (sock)](#apidoc.element.axon.Socket.prototype.removeSocket)
1.  [function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>set (name, val)](#apidoc.element.axon.Socket.prototype.set)
1.  [function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>use (plugin)](#apidoc.element.axon.Socket.prototype.use)
1.  object <span class="apidocSignatureSpan">axon.Socket.prototype.</span>settings

#### [module axon.SubEmitterSocket](#apidoc.module.axon.SubEmitterSocket)
1.  [function <span class="apidocSignatureSpan">axon.</span>SubEmitterSocket ()](#apidoc.element.axon.SubEmitterSocket.SubEmitterSocket)

#### [module axon.SubEmitterSocket.prototype](#apidoc.module.axon.SubEmitterSocket.prototype)
1.  [function <span class="apidocSignatureSpan">axon.SubEmitterSocket.prototype.</span>off (event)](#apidoc.element.axon.SubEmitterSocket.prototype.off)
1.  [function <span class="apidocSignatureSpan">axon.SubEmitterSocket.prototype.</span>on (event, fn)](#apidoc.element.axon.SubEmitterSocket.prototype.on)
1.  [function <span class="apidocSignatureSpan">axon.SubEmitterSocket.prototype.</span>onmessage ()](#apidoc.element.axon.SubEmitterSocket.prototype.onmessage)

#### [module axon.SubSocket](#apidoc.module.axon.SubSocket)
1.  [function <span class="apidocSignatureSpan">axon.</span>SubSocket ()](#apidoc.element.axon.SubSocket.SubSocket)

#### [module axon.SubSocket.prototype](#apidoc.module.axon.SubSocket.prototype)
1.  [function <span class="apidocSignatureSpan">axon.SubSocket.prototype.</span>clearSubscriptions ()](#apidoc.element.axon.SubSocket.prototype.clearSubscriptions)
1.  [function <span class="apidocSignatureSpan">axon.SubSocket.prototype.</span>hasSubscriptions ()](#apidoc.element.axon.SubSocket.prototype.hasSubscriptions)
1.  [function <span class="apidocSignatureSpan">axon.SubSocket.prototype.</span>matches (topic)](#apidoc.element.axon.SubSocket.prototype.matches)
1.  [function <span class="apidocSignatureSpan">axon.SubSocket.prototype.</span>onmessage (sock)](#apidoc.element.axon.SubSocket.prototype.onmessage)
1.  [function <span class="apidocSignatureSpan">axon.SubSocket.prototype.</span>send ()](#apidoc.element.axon.SubSocket.prototype.send)
1.  [function <span class="apidocSignatureSpan">axon.SubSocket.prototype.</span>subscribe (re)](#apidoc.element.axon.SubSocket.prototype.subscribe)
1.  [function <span class="apidocSignatureSpan">axon.SubSocket.prototype.</span>unsubscribe (re)](#apidoc.element.axon.SubSocket.prototype.unsubscribe)

#### [module axon.types](#apidoc.module.axon.types)
1.  [function <span class="apidocSignatureSpan">axon.types.</span>pub ()](#apidoc.element.axon.types.pub)
1.  [function <span class="apidocSignatureSpan">axon.types.</span>pub-emitter ()](#apidoc.element.axon.types.pub-emitter)
1.  [function <span class="apidocSignatureSpan">axon.types.</span>pull ()](#apidoc.element.axon.types.pull)
1.  [function <span class="apidocSignatureSpan">axon.types.</span>push ()](#apidoc.element.axon.types.push)
1.  [function <span class="apidocSignatureSpan">axon.types.</span>rep ()](#apidoc.element.axon.types.rep)
1.  [function <span class="apidocSignatureSpan">axon.types.</span>req ()](#apidoc.element.axon.types.req)
1.  [function <span class="apidocSignatureSpan">axon.types.</span>sub ()](#apidoc.element.axon.types.sub)
1.  [function <span class="apidocSignatureSpan">axon.types.</span>sub-emitter ()](#apidoc.element.axon.types.sub-emitter)

#### [module axon.utils](#apidoc.module.axon.utils)
1.  [function <span class="apidocSignatureSpan">axon.utils.</span>slice (args)](#apidoc.element.axon.utils.slice)



# <a name="apidoc.module.axon"></a>[module axon](#apidoc.module.axon)

#### <a name="apidoc.element.axon.PubEmitterSocket"></a>[function <span class="apidocSignatureSpan">axon.</span>PubEmitterSocket ()](#apidoc.element.axon.PubEmitterSocket)
- description and source-code
```javascript
function PubEmitterSocket() {
  this.sock = new PubSocket;
  this.emit = this.sock.send.bind(this.sock);
  this.bind = this.sock.bind.bind(this.sock);
  this.connect = this.sock.connect.bind(this.sock);
  this.close = this.sock.close.bind(this.sock);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.PubSocket"></a>[function <span class="apidocSignatureSpan">axon.</span>PubSocket ()](#apidoc.element.axon.PubSocket)
- description and source-code
```javascript
function PubSocket() {
  Socket.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.PullSocket"></a>[function <span class="apidocSignatureSpan">axon.</span>PullSocket ()](#apidoc.element.axon.PullSocket)
- description and source-code
```javascript
function PullSocket() {
  Socket.call(this);
  // TODO: selective reception
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.PushSocket"></a>[function <span class="apidocSignatureSpan">axon.</span>PushSocket ()](#apidoc.element.axon.PushSocket)
- description and source-code
```javascript
function PushSocket() {
  Socket.call(this);
  this.use(queue());
  this.use(roundrobin({ fallback: this.enqueue }));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.RepSocket"></a>[function <span class="apidocSignatureSpan">axon.</span>RepSocket ()](#apidoc.element.axon.RepSocket)
- description and source-code
```javascript
function RepSocket() {
  Socket.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.ReqSocket"></a>[function <span class="apidocSignatureSpan">axon.</span>ReqSocket ()](#apidoc.element.axon.ReqSocket)
- description and source-code
```javascript
function ReqSocket() {
  Socket.call(this);
  this.n = 0;
  this.ids = 0;
  this.callbacks = {};
  this.identity = this.get('identity');
  this.use(queue());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.Socket"></a>[function <span class="apidocSignatureSpan">axon.</span>Socket ()](#apidoc.element.axon.Socket)
- description and source-code
```javascript
function Socket() {
  this.server = null;
  this.socks = [];
  this.settings = {};
  this.set('hwm', Infinity);
  this.set('identity', String(process.pid));
  this.set('retry timeout', 100);
  this.set('retry max timeout', 5000);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.SubEmitterSocket"></a>[function <span class="apidocSignatureSpan">axon.</span>SubEmitterSocket ()](#apidoc.element.axon.SubEmitterSocket)
- description and source-code
```javascript
function SubEmitterSocket() {
  this.sock = new SubSocket;
  this.sock.onmessage = this.onmessage.bind(this);
  this.bind = this.sock.bind.bind(this.sock);
  this.connect = this.sock.connect.bind(this.sock);
  this.close = this.sock.close.bind(this.sock);
  this.listeners = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.SubSocket"></a>[function <span class="apidocSignatureSpan">axon.</span>SubSocket ()](#apidoc.element.axon.SubSocket)
- description and source-code
```javascript
function SubSocket() {
  Socket.call(this);
  this.subscriptions = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.socket"></a>[function <span class="apidocSignatureSpan">axon.</span>socket (type, options)](#apidoc.element.axon.socket)
- description and source-code
```javascript
socket = function (type, options){
  var fn = exports.types[type];
  if (!fn) throw new Error('invalid socket type "' + type + '"');
  return new fn(options);
}
```
- example usage
```shell
...

## Push / Pull

'PushSocket's distribute messages round-robin:

'''js
var axon = require('axon');
var sock = axon.socket('push');

sock.bind(3000);
console.log('push server started');

setInterval(function(){
  sock.send('hello');
}, 150);
...
```



# <a name="apidoc.module.axon.PubSocket"></a>[module axon.PubSocket](#apidoc.module.axon.PubSocket)

#### <a name="apidoc.element.axon.PubSocket.PubSocket"></a>[function <span class="apidocSignatureSpan">axon.</span>PubSocket ()](#apidoc.element.axon.PubSocket.PubSocket)
- description and source-code
```javascript
function PubSocket() {
  Socket.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.axon.PubSocket.prototype"></a>[module axon.PubSocket.prototype](#apidoc.module.axon.PubSocket.prototype)

#### <a name="apidoc.element.axon.PubSocket.prototype.send"></a>[function <span class="apidocSignatureSpan">axon.PubSocket.prototype.</span>send (msg)](#apidoc.element.axon.PubSocket.prototype.send)
- description and source-code
```javascript
send = function (msg){
  var socks = this.socks;
  var len = socks.length;
  var sock;

  var buf = this.pack(arguments);

  for (var i = 0; i < len; i++) {
    sock = socks[i];
    if (sock.writable) sock.write(buf);
  }

  return this;
}
```
- example usage
```shell
...

## Mixed argument types

  Backed by [node-amp-message](https://github.com/tj/node-amp-message)
  you may pass strings, objects, and buffers as arguments.

'''js
push.send('image', { w: 100, h: 200 }, imageBuffer);
pull.on('message', function(type, size, img){});
'''

## Push / Pull

'PushSocket's distribute messages round-robin:
...
```



# <a name="apidoc.module.axon.PullSocket"></a>[module axon.PullSocket](#apidoc.module.axon.PullSocket)

#### <a name="apidoc.element.axon.PullSocket.PullSocket"></a>[function <span class="apidocSignatureSpan">axon.</span>PullSocket ()](#apidoc.element.axon.PullSocket.PullSocket)
- description and source-code
```javascript
function PullSocket() {
  Socket.call(this);
  // TODO: selective reception
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.axon.PullSocket.prototype"></a>[module axon.PullSocket.prototype](#apidoc.module.axon.PullSocket.prototype)

#### <a name="apidoc.element.axon.PullSocket.prototype.send"></a>[function <span class="apidocSignatureSpan">axon.PullSocket.prototype.</span>send ()](#apidoc.element.axon.PullSocket.prototype.send)
- description and source-code
```javascript
send = function (){
  throw new Error('pull sockets should not send messages');
}
```
- example usage
```shell
...

## Mixed argument types

  Backed by [node-amp-message](https://github.com/tj/node-amp-message)
  you may pass strings, objects, and buffers as arguments.

'''js
push.send('image', { w: 100, h: 200 }, imageBuffer);
pull.on('message', function(type, size, img){});
'''

## Push / Pull

'PushSocket's distribute messages round-robin:
...
```



# <a name="apidoc.module.axon.RepSocket"></a>[module axon.RepSocket](#apidoc.module.axon.RepSocket)

#### <a name="apidoc.element.axon.RepSocket.RepSocket"></a>[function <span class="apidocSignatureSpan">axon.</span>RepSocket ()](#apidoc.element.axon.RepSocket.RepSocket)
- description and source-code
```javascript
function RepSocket() {
  Socket.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.axon.RepSocket.prototype"></a>[module axon.RepSocket.prototype](#apidoc.module.axon.RepSocket.prototype)

#### <a name="apidoc.element.axon.RepSocket.prototype.onmessage"></a>[function <span class="apidocSignatureSpan">axon.RepSocket.prototype.</span>onmessage (sock)](#apidoc.element.axon.RepSocket.prototype.onmessage)
- description and source-code
```javascript
onmessage = function (sock){
  var self = this;

  return function (buf){
    var msg = new Message(buf);
    var args = msg.args;

    var id = args.pop();
    args.unshift('message');
    args.push(reply);
    self.emit.apply(self, args);

    function reply() {
      var fn = function(){};
      var args = slice(arguments);
      args[0] = args[0] || null;

      var hasCallback = 'function' == typeof args[args.length - 1];
      if (hasCallback) fn = args.pop();

      args.push(id);

      if (sock.writable) {
        sock.write(self.pack(args), function(){ fn(true) });
        return true;
      } else {
        debug('peer went away');
        process.nextTick(function(){ fn(false) });
        return false;
      }
    }
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.axon.ReqSocket"></a>[module axon.ReqSocket](#apidoc.module.axon.ReqSocket)

#### <a name="apidoc.element.axon.ReqSocket.ReqSocket"></a>[function <span class="apidocSignatureSpan">axon.</span>ReqSocket ()](#apidoc.element.axon.ReqSocket.ReqSocket)
- description and source-code
```javascript
function ReqSocket() {
  Socket.call(this);
  this.n = 0;
  this.ids = 0;
  this.callbacks = {};
  this.identity = this.get('identity');
  this.use(queue());
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.axon.ReqSocket.prototype"></a>[module axon.ReqSocket.prototype](#apidoc.module.axon.ReqSocket.prototype)

#### <a name="apidoc.element.axon.ReqSocket.prototype.id"></a>[function <span class="apidocSignatureSpan">axon.ReqSocket.prototype.</span>id ()](#apidoc.element.axon.ReqSocket.prototype.id)
- description and source-code
```javascript
id = function (){
  return this.identity + ':' + this.ids++;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.ReqSocket.prototype.onmessage"></a>[function <span class="apidocSignatureSpan">axon.ReqSocket.prototype.</span>onmessage ()](#apidoc.element.axon.ReqSocket.prototype.onmessage)
- description and source-code
```javascript
onmessage = function (){
  var self = this;
  return function(buf){
    var msg = new Message(buf);
    var id = msg.pop();
    var fn = self.callbacks[id];
    if (!fn) return debug('missing callback %s', id);
    fn.apply(null, msg.args);
    delete self.callbacks[id];
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.ReqSocket.prototype.send"></a>[function <span class="apidocSignatureSpan">axon.ReqSocket.prototype.</span>send (msg)](#apidoc.element.axon.ReqSocket.prototype.send)
- description and source-code
```javascript
send = function (msg){
  var socks = this.socks;
  var len = socks.length;
  var sock = socks[this.n++ % len];
  var args = slice(arguments);

  if (sock) {
    var hasCallback = 'function' == typeof args[args.length - 1];
    if (!hasCallback) args.push(function(){});
    var fn = args.pop();
    fn.id = this.id();
    this.callbacks[fn.id] = fn;
    args.push(fn.id);
  }

  if (sock) {
    sock.write(this.pack(args));
  } else {
    debug('no connected peers');
    this.enqueue(args);
  }
}
```
- example usage
```shell
...

## Mixed argument types

  Backed by [node-amp-message](https://github.com/tj/node-amp-message)
  you may pass strings, objects, and buffers as arguments.

'''js
push.send('image', { w: 100, h: 200 }, imageBuffer);
pull.on('message', function(type, size, img){});
'''

## Push / Pull

'PushSocket's distribute messages round-robin:
...
```



# <a name="apidoc.module.axon.Socket"></a>[module axon.Socket](#apidoc.module.axon.Socket)

#### <a name="apidoc.element.axon.Socket.Socket"></a>[function <span class="apidocSignatureSpan">axon.</span>Socket ()](#apidoc.element.axon.Socket.Socket)
- description and source-code
```javascript
function Socket() {
  this.server = null;
  this.socks = [];
  this.settings = {};
  this.set('hwm', Infinity);
  this.set('identity', String(process.pid));
  this.set('retry timeout', 100);
  this.set('retry max timeout', 5000);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.axon.Socket.prototype"></a>[module axon.Socket.prototype](#apidoc.module.axon.Socket.prototype)

#### <a name="apidoc.element.axon.Socket.prototype.addSocket"></a>[function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>addSocket (sock)](#apidoc.element.axon.Socket.prototype.addSocket)
- description and source-code
```javascript
addSocket = function (sock){
  var parser = new Parser;
  var i = this.socks.push(sock) - 1;
  debug('%s add socket %d', this.type, i);
  sock.pipe(parser);
  parser.on('data', this.onmessage(sock));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.Socket.prototype.address"></a>[function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>address ()](#apidoc.element.axon.Socket.prototype.address)
- description and source-code
```javascript
address = function (){
  if (!this.server) return;
  var addr = this.server.address();
  addr.string = 'tcp://' + addr.address + ':' + addr.port;
  return addr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.Socket.prototype.bind"></a>[function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>bind (port, host, fn)](#apidoc.element.axon.Socket.prototype.bind)
- description and source-code
```javascript
bind = function (port, host, fn){
  var self = this;
  if ('client' == this.type) throw new Error('cannot bind() after connect()');
  if ('function' == typeof host) {
    fn = host;
    host = undefined;
  }

  var unixSocket = false;

  if ('string' == typeof port) {
    port = url.parse(port);

    if ('unix:' == port.protocol) {
      host = fn;
      fn = undefined;
      port = port.pathname;
      unixSocket = true;
    } else {
      host = port.hostname || '0.0.0.0';
      port = parseInt(port.port, 10);
    }
  } else {
    host = host || '0.0.0.0';
  }

  this.type = 'server';

  this.server = net.createServer(this.onconnect.bind(this));

  debug('%s bind %s:%s', this.type, host, port);
  this.server.on('listening', this.emit.bind(this, 'bind'));

  if (unixSocket) {
    // TODO: move out
    this.server.on('error', function(e) {
      if (e.code == 'EADDRINUSE') {
        // Unix file socket and error EADDRINUSE is the case if
        // the file socket exists. We check if other processes
        // listen on file socket, otherwise it is a stale socket
        // that we could reopen
        // We try to connect to socket via plain network socket
        var clientSocket = new net.Socket();

        clientSocket.on('error', function(e2) {
          if (e2.code == 'ECONNREFUSED') {
            // No other server listening, so we can delete stale
            // socket file and reopen server socket
            fs.unlink(port);
            self.server.listen(port, host, fn);
          }
        });

        clientSocket.connect({path: port}, function() {
          // Connection is possible, so other server is listening
          // on this file socket
          throw e;
        });
      }
    });
  }

  this.server.listen(port, host, fn);
  return this;
}
```
- example usage
```shell
...

'PushSocket's distribute messages round-robin:

'''js
var axon = require('axon');
var sock = axon.socket('push');

sock.bind(3000);
console.log('push server started');

setInterval(function(){
  sock.send('hello');
}, 150);
'''
...
```

#### <a name="apidoc.element.axon.Socket.prototype.close"></a>[function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>close (fn)](#apidoc.element.axon.Socket.prototype.close)
- description and source-code
```javascript
close = function (fn){
  debug('%s closing', this.type);
  this.closing = true;
  this.closeSockets();
  if (this.server) this.closeServer(fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.Socket.prototype.closeServer"></a>[function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>closeServer (fn)](#apidoc.element.axon.Socket.prototype.closeServer)
- description and source-code
```javascript
closeServer = function (fn){
  debug('%s closing server', this.type);
  this.server.on('close', this.emit.bind(this, 'close'));
  this.server.close();
  fn && fn();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.Socket.prototype.closeSockets"></a>[function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>closeSockets ()](#apidoc.element.axon.Socket.prototype.closeSockets)
- description and source-code
```javascript
closeSockets = function (){
  debug('%s closing %d connections', this.type, this.socks.length);
  this.socks.forEach(function(sock){
    sock.destroy();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.Socket.prototype.connect"></a>[function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>connect (port, host, fn)](#apidoc.element.axon.Socket.prototype.connect)
- description and source-code
```javascript
connect = function (port, host, fn){
  var self = this;
  if ('server' == this.type) throw new Error('cannot connect() after bind()');
  if ('function' == typeof host) {
    fn = host;
    host = undefined;
  }

  if ('string' == typeof port) {
    port = url.parse(port);

    if (port.protocol == "unix:") {
      host = fn;
      fn = undefined;
      port = port.pathname;
    } else {
      host = port.hostname || '0.0.0.0';
      port = parseInt(port.port, 10);
    }
  } else {
    host = host || '0.0.0.0';
  }

  var max = self.get('retry max timeout');
  var sock = new net.Socket;
  sock.setNoDelay();
  this.type = 'client';

  this.handleErrors(sock);

  sock.on('close', function(){
    self.emit('socket close', sock);
    self.connected = false;
    self.removeSocket(sock);
    if (self.closing) return self.emit('close');
    var retry = self.retry || self.get('retry timeout');
    setTimeout(function(){
      debug('%s attempting reconnect', self.type);
      self.emit('reconnect attempt');
      sock.destroy();
      self.connect(port, host);
      self.retry = Math.round(Math.min(max, retry * 1.5));
    }, retry);
  });

  sock.on('connect', function(){
    debug('%s connect', self.type);
    self.connected = true;
    self.addSocket(sock);
    self.retry = self.get('retry timeout');
    self.emit('connect', sock);
    fn && fn();
  });

  debug('%s connect attempt %s:%s', self.type, host, port);
  sock.connect(port, host);
  return this;
}
```
- example usage
```shell
...

Receiver of 'PushSocket' messages:

'''js
var axon = require('axon');
var sock = axon.socket('pull');

sock.connect(3000);

sock.on('message', function(msg){
  console.log(msg.toString());
});
'''
...
```

#### <a name="apidoc.element.axon.Socket.prototype.disable"></a>[function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>disable (name)](#apidoc.element.axon.Socket.prototype.disable)
- description and source-code
```javascript
disable = function (name){
  return this.set(name, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.Socket.prototype.disabled"></a>[function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>disabled (name)](#apidoc.element.axon.Socket.prototype.disabled)
- description and source-code
```javascript
disabled = function (name){
  return ! this.get(name);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.Socket.prototype.enable"></a>[function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>enable (name)](#apidoc.element.axon.Socket.prototype.enable)
- description and source-code
```javascript
enable = function (name){
  return this.set(name, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.Socket.prototype.enabled"></a>[function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>enabled (name)](#apidoc.element.axon.Socket.prototype.enabled)
- description and source-code
```javascript
enabled = function (name){
  return !! this.get(name);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.Socket.prototype.get"></a>[function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>get (name)](#apidoc.element.axon.Socket.prototype.get)
- description and source-code
```javascript
get = function (name){
  return this.settings[name];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.Socket.prototype.handleErrors"></a>[function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>handleErrors (sock)](#apidoc.element.axon.Socket.prototype.handleErrors)
- description and source-code
```javascript
handleErrors = function (sock){
  var self = this;
  sock.on('error', function(err){
    debug('%s error %s', self.type, err.code || err.message);
    self.emit('socket error', err);
    self.removeSocket(sock);
    if (!~ignore.indexOf(err.code)) return self.emit('error', err);
    debug('%s ignored %s', self.type, err.code);
    self.emit('ignored error', err);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.Socket.prototype.onconnect"></a>[function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>onconnect (sock)](#apidoc.element.axon.Socket.prototype.onconnect)
- description and source-code
```javascript
onconnect = function (sock){
  var self = this;
  var addr = sock.remoteAddress + ':' + sock.remotePort;
  debug('%s accept %s', self.type, addr);
  this.addSocket(sock);
  this.handleErrors(sock);
  this.emit('connect', sock);
  sock.on('close', function(){
    debug('%s disconnect %s', self.type, addr);
    self.emit('disconnect', sock);
    self.removeSocket(sock);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.Socket.prototype.onmessage"></a>[function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>onmessage (sock)](#apidoc.element.axon.Socket.prototype.onmessage)
- description and source-code
```javascript
onmessage = function (sock){
  var self = this;
  return function(buf){
    var msg = new Message(buf);
    self.emit.apply(self, ['message'].concat(msg.args));
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.Socket.prototype.pack"></a>[function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>pack (args)](#apidoc.element.axon.Socket.prototype.pack)
- description and source-code
```javascript
pack = function (args){
  var msg = new Message(args);
  return msg.toBuffer();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.Socket.prototype.removeSocket"></a>[function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>removeSocket (sock)](#apidoc.element.axon.Socket.prototype.removeSocket)
- description and source-code
```javascript
removeSocket = function (sock){
  var i = this.socks.indexOf(sock);
  if (!~i) return;
  debug('%s remove socket %d', this.type, i);
  this.socks.splice(i, 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.Socket.prototype.set"></a>[function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>set (name, val)](#apidoc.element.axon.Socket.prototype.set)
- description and source-code
```javascript
set = function (name, val){
  if (1 == arguments.length) {
    for (var key in name) {
      this.set(key, name[key]);
    }
  } else {
    this.settings[name] = val;
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.Socket.prototype.use"></a>[function <span class="apidocSignatureSpan">axon.Socket.prototype.</span>use (plugin)](#apidoc.element.axon.Socket.prototype.use)
- description and source-code
```javascript
use = function (plugin){
  plugin(this);
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.axon.SubEmitterSocket"></a>[module axon.SubEmitterSocket](#apidoc.module.axon.SubEmitterSocket)

#### <a name="apidoc.element.axon.SubEmitterSocket.SubEmitterSocket"></a>[function <span class="apidocSignatureSpan">axon.</span>SubEmitterSocket ()](#apidoc.element.axon.SubEmitterSocket.SubEmitterSocket)
- description and source-code
```javascript
function SubEmitterSocket() {
  this.sock = new SubSocket;
  this.sock.onmessage = this.onmessage.bind(this);
  this.bind = this.sock.bind.bind(this.sock);
  this.connect = this.sock.connect.bind(this.sock);
  this.close = this.sock.close.bind(this.sock);
  this.listeners = [];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.axon.SubEmitterSocket.prototype"></a>[module axon.SubEmitterSocket.prototype](#apidoc.module.axon.SubEmitterSocket.prototype)

#### <a name="apidoc.element.axon.SubEmitterSocket.prototype.off"></a>[function <span class="apidocSignatureSpan">axon.SubEmitterSocket.prototype.</span>off (event)](#apidoc.element.axon.SubEmitterSocket.prototype.off)
- description and source-code
```javascript
off = function (event){
  for (var i = 0; i < this.listeners.length; ++i) {
    if (this.listeners[i].event === event) {
      this.sock.unsubscribe(this.listeners[i].re);
      this.listeners.splice(i--, 1);
    }
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.SubEmitterSocket.prototype.on"></a>[function <span class="apidocSignatureSpan">axon.SubEmitterSocket.prototype.</span>on (event, fn)](#apidoc.element.axon.SubEmitterSocket.prototype.on)
- description and source-code
```javascript
on = function (event, fn){
  var re = this.sock.subscribe(event);
  this.listeners.push({
    event: event,
    re: re,
    fn: fn
  });
  return this;
}
```
- example usage
```shell
...
## Mixed argument types

  Backed by [node-amp-message](https://github.com/tj/node-amp-message)
  you may pass strings, objects, and buffers as arguments.

'''js
push.send('image', { w: 100, h: 200 }, imageBuffer);
pull.on('message', function(type, size, img){});
'''

## Push / Pull

'PushSocket's distribute messages round-robin:

'''js
...
```

#### <a name="apidoc.element.axon.SubEmitterSocket.prototype.onmessage"></a>[function <span class="apidocSignatureSpan">axon.SubEmitterSocket.prototype.</span>onmessage ()](#apidoc.element.axon.SubEmitterSocket.prototype.onmessage)
- description and source-code
```javascript
onmessage = function (){
  var listeners = this.listeners;
  var self = this;

  return function(buf){
    var msg = new Message(buf);
    var topic = msg.shift();

    for (var i = 0; i < listeners.length; ++i) {
      var listener = listeners[i];

      var m = listener.re.exec(topic);
      if (!m) continue;

      listener.fn.apply(self, m.slice(1).concat(msg.args));
    }
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.axon.SubSocket"></a>[module axon.SubSocket](#apidoc.module.axon.SubSocket)

#### <a name="apidoc.element.axon.SubSocket.SubSocket"></a>[function <span class="apidocSignatureSpan">axon.</span>SubSocket ()](#apidoc.element.axon.SubSocket.SubSocket)
- description and source-code
```javascript
function SubSocket() {
  Socket.call(this);
  this.subscriptions = [];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.axon.SubSocket.prototype"></a>[module axon.SubSocket.prototype](#apidoc.module.axon.SubSocket.prototype)

#### <a name="apidoc.element.axon.SubSocket.prototype.clearSubscriptions"></a>[function <span class="apidocSignatureSpan">axon.SubSocket.prototype.</span>clearSubscriptions ()](#apidoc.element.axon.SubSocket.prototype.clearSubscriptions)
- description and source-code
```javascript
clearSubscriptions = function (){
  this.subscriptions = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.SubSocket.prototype.hasSubscriptions"></a>[function <span class="apidocSignatureSpan">axon.SubSocket.prototype.</span>hasSubscriptions ()](#apidoc.element.axon.SubSocket.prototype.hasSubscriptions)
- description and source-code
```javascript
hasSubscriptions = function (){
  return !! this.subscriptions.length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.SubSocket.prototype.matches"></a>[function <span class="apidocSignatureSpan">axon.SubSocket.prototype.</span>matches (topic)](#apidoc.element.axon.SubSocket.prototype.matches)
- description and source-code
```javascript
matches = function (topic){
  for (var i = 0; i < this.subscriptions.length; ++i) {
    if (this.subscriptions[i].test(topic)) {
      return true;
    }
  }
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.SubSocket.prototype.onmessage"></a>[function <span class="apidocSignatureSpan">axon.SubSocket.prototype.</span>onmessage (sock)](#apidoc.element.axon.SubSocket.prototype.onmessage)
- description and source-code
```javascript
onmessage = function (sock){
  var subs = this.hasSubscriptions();
  var self = this;

  return function(buf){
    var msg = new Message(buf);

    if (subs) {
      var topic = msg.args[0];
      if (!self.matches(topic)) return debug('not subscribed to "%s"', topic);
    }

    self.emit.apply(self, ['message'].concat(msg.args));
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.SubSocket.prototype.send"></a>[function <span class="apidocSignatureSpan">axon.SubSocket.prototype.</span>send ()](#apidoc.element.axon.SubSocket.prototype.send)
- description and source-code
```javascript
send = function (){
  throw new Error('subscribers cannot send messages');
}
```
- example usage
```shell
...

## Mixed argument types

  Backed by [node-amp-message](https://github.com/tj/node-amp-message)
  you may pass strings, objects, and buffers as arguments.

'''js
push.send('image', { w: 100, h: 200 }, imageBuffer);
pull.on('message', function(type, size, img){});
'''

## Push / Pull

'PushSocket's distribute messages round-robin:
...
```

#### <a name="apidoc.element.axon.SubSocket.prototype.subscribe"></a>[function <span class="apidocSignatureSpan">axon.SubSocket.prototype.</span>subscribe (re)](#apidoc.element.axon.SubSocket.prototype.subscribe)
- description and source-code
```javascript
subscribe = function (re){
  debug('subscribe to "%s"', re);
  this.subscriptions.push(re = toRegExp(re));
  return re;
}
```
- example usage
```shell
...
sock.connect(3000);

sock.on('message', function(msg){
  console.log(msg.toString());
});
'''

 'SubSocket's may optionally '.subscribe()' to one or more "topics" (the first multipart value),
 using string patterns or regular expressions:

'''js
var axon = require('axon');
var sock = axon.socket('sub');

sock.connect(3000);
...
```

#### <a name="apidoc.element.axon.SubSocket.prototype.unsubscribe"></a>[function <span class="apidocSignatureSpan">axon.SubSocket.prototype.</span>unsubscribe (re)](#apidoc.element.axon.SubSocket.prototype.unsubscribe)
- description and source-code
```javascript
unsubscribe = function (re){
  debug('unsubscribe from "%s"', re);
  re = toRegExp(re);
  for (var i = 0; i < this.subscriptions.length; ++i) {
    if (this.subscriptions[i].toString() === re.toString()) {
      this.subscriptions.splice(i--, 1);
    }
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.axon.types"></a>[module axon.types](#apidoc.module.axon.types)

#### <a name="apidoc.element.axon.types.pub"></a>[function <span class="apidocSignatureSpan">axon.types.</span>pub ()](#apidoc.element.axon.types.pub)
- description and source-code
```javascript
function PubSocket() {
  Socket.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.types.pub-emitter"></a>[function <span class="apidocSignatureSpan">axon.types.</span>pub-emitter ()](#apidoc.element.axon.types.pub-emitter)
- description and source-code
```javascript
function PubEmitterSocket() {
  this.sock = new PubSocket;
  this.emit = this.sock.send.bind(this.sock);
  this.bind = this.sock.bind.bind(this.sock);
  this.connect = this.sock.connect.bind(this.sock);
  this.close = this.sock.close.bind(this.sock);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.types.pull"></a>[function <span class="apidocSignatureSpan">axon.types.</span>pull ()](#apidoc.element.axon.types.pull)
- description and source-code
```javascript
function PullSocket() {
  Socket.call(this);
  // TODO: selective reception
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.types.push"></a>[function <span class="apidocSignatureSpan">axon.types.</span>push ()](#apidoc.element.axon.types.push)
- description and source-code
```javascript
function PushSocket() {
  Socket.call(this);
  this.use(queue());
  this.use(roundrobin({ fallback: this.enqueue }));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.types.rep"></a>[function <span class="apidocSignatureSpan">axon.types.</span>rep ()](#apidoc.element.axon.types.rep)
- description and source-code
```javascript
function RepSocket() {
  Socket.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.types.req"></a>[function <span class="apidocSignatureSpan">axon.types.</span>req ()](#apidoc.element.axon.types.req)
- description and source-code
```javascript
function ReqSocket() {
  Socket.call(this);
  this.n = 0;
  this.ids = 0;
  this.callbacks = {};
  this.identity = this.get('identity');
  this.use(queue());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.types.sub"></a>[function <span class="apidocSignatureSpan">axon.types.</span>sub ()](#apidoc.element.axon.types.sub)
- description and source-code
```javascript
function SubSocket() {
  Socket.call(this);
  this.subscriptions = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.axon.types.sub-emitter"></a>[function <span class="apidocSignatureSpan">axon.types.</span>sub-emitter ()](#apidoc.element.axon.types.sub-emitter)
- description and source-code
```javascript
function SubEmitterSocket() {
  this.sock = new SubSocket;
  this.sock.onmessage = this.onmessage.bind(this);
  this.bind = this.sock.bind.bind(this.sock);
  this.connect = this.sock.connect.bind(this.sock);
  this.close = this.sock.close.bind(this.sock);
  this.listeners = [];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.axon.utils"></a>[module axon.utils](#apidoc.module.axon.utils)

#### <a name="apidoc.element.axon.utils.slice"></a>[function <span class="apidocSignatureSpan">axon.utils.</span>slice (args)](#apidoc.element.axon.utils.slice)
- description and source-code
```javascript
slice = function (args){
  var len = args.length;
  var ret = new Array(len);

  for (var i = 0; i < len; i++) {
    ret[i] = args[i];
  }

  return ret;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
