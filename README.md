# api documentation for  [engine.io (v3.0.0)](https://github.com/socketio/engine.io)  [![npm package](https://img.shields.io/npm/v/npmdoc-engine.io.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-engine.io) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-engine.io.svg)](https://travis-ci.org/npmdoc/node-npmdoc-engine.io)
#### The realtime engine behind Socket.IO. Provides the foundation of a bidirectional connection between client and server

[![NPM](https://nodei.co/npm/engine.io.png?downloads=true)](https://www.npmjs.com/package/engine.io)

[![apidoc](https://npmdoc.github.io/node-npmdoc-engine.io/build/screenCapture.buildApidoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-engine.io%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-engine.io/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-engine.io/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-engine.io/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Guillermo Rauch",
        "email": "guillermo@learnboost.com"
    },
    "bugs": {
        "url": "https://github.com/socketio/engine.io/issues"
    },
    "contributors": [
        {
            "name": "Eugen Dueck",
            "url": "https://github.com/EugenDueck"
        },
        {
            "name": "Afshin Mehrabani",
            "url": "https://github.com/afshinm"
        },
        {
            "name": "Christoph Dorn",
            "url": "https://github.com/cadorn"
        },
        {
            "name": "Mark Mokryn",
            "email": "mokesmokes@gmail.com"
        }
    ],
    "dependencies": {
        "accepts": "1.3.3",
        "base64id": "1.0.0",
        "cookie": "0.3.1",
        "debug": "2.3.3",
        "engine.io-parser": "2.0.3",
        "uws": "0.14.1",
        "ws": "2.2.3"
    },
    "description": "The realtime engine behind Socket.IO. Provides the foundation of a bidirectional connection between client and server",
    "devDependencies": {
        "babel-eslint": "5.0.0",
        "babel-preset-es2015": "^6.24.0",
        "engine.io-client": "3.0.0",
        "eslint-config-standard": "4.4.0",
        "eslint-plugin-standard": "1.3.2",
        "expect.js": "^0.3.1",
        "gulp": "^3.9.1",
        "gulp-babel": "^6.1.2",
        "gulp-eslint": "1.1.1",
        "gulp-mocha": "^4.3.0",
        "gulp-nsp": "^2.4.1",
        "mocha": "^3.2.0",
        "s": "0.1.1",
        "superagent": "0.15.4"
    },
    "directories": {},
    "dist": {
        "shasum": "fde0f460686f09e295bc55933663c1cf37759933",
        "tarball": "https://registry.npmjs.org/engine.io/-/engine.io-3.0.0.tgz"
    },
    "files": [
        "index.js",
        "lib/"
    ],
    "gitHead": "07d57d553f1da9c04a4c903d971346b339df2404",
    "homepage": "https://github.com/socketio/engine.io",
    "license": "MIT",
    "main": "./lib/engine.io",
    "maintainers": [
        {
            "name": "darrachequesne",
            "email": "damien.arrachequesne@gmail.com"
        },
        {
            "name": "rauchg",
            "email": "rauchg@gmail.com"
        }
    ],
    "name": "engine.io",
    "optionalDependencies": {
        "uws": "0.14.1"
    },
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/socketio/engine.io.git"
    },
    "scripts": {
        "test": "gulp test; EIO_WS_ENGINE=ws gulp test;"
    },
    "version": "3.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module engine.io](#apidoc.module.engine.io)
1.  [function <span class="apidocSignatureSpan">engine.io.</span>Server (opts)](#apidoc.element.engine.io.Server)
1.  [function <span class="apidocSignatureSpan">engine.io.</span>Socket (id, server, transport, req)](#apidoc.element.engine.io.Socket)
1.  [function <span class="apidocSignatureSpan">engine.io.</span>Transport (req)](#apidoc.element.engine.io.Transport)
1.  [function <span class="apidocSignatureSpan">engine.io.</span>attach (server, options)](#apidoc.element.engine.io.attach)
1.  [function <span class="apidocSignatureSpan">engine.io.</span>io.Server (opts)](#apidoc.element.engine.io.io.Server)
1.  [function <span class="apidocSignatureSpan">engine.io.</span>io.Socket (id, server, transport, req)](#apidoc.element.engine.io.io.Socket)
1.  [function <span class="apidocSignatureSpan">engine.io.</span>io.Transport (req)](#apidoc.element.engine.io.io.Transport)
1.  [function <span class="apidocSignatureSpan">engine.io.</span>io.transports.websocket (req)](#apidoc.element.engine.io.io.transports.websocket)
1.  [function <span class="apidocSignatureSpan">engine.io.</span>listen (port, options, fn)](#apidoc.element.engine.io.listen)
1.  number <span class="apidocSignatureSpan">engine.io.</span>protocol
1.  object <span class="apidocSignatureSpan">engine.io.</span>io.Server.prototype
1.  object <span class="apidocSignatureSpan">engine.io.</span>io.Socket.prototype
1.  object <span class="apidocSignatureSpan">engine.io.</span>io.Transport.prototype
1.  object <span class="apidocSignatureSpan">engine.io.</span>io.parser
1.  object <span class="apidocSignatureSpan">engine.io.</span>io.transports
1.  object <span class="apidocSignatureSpan">engine.io.</span>io.transports.websocket.prototype
1.  object <span class="apidocSignatureSpan">engine.io.</span>parser
1.  object <span class="apidocSignatureSpan">engine.io.</span>transports

#### [module engine.io.Server](#apidoc.module.engine.io.Server)
1.  [function <span class="apidocSignatureSpan">engine.io.</span>Server (opts)](#apidoc.element.engine.io.Server.Server)
1.  [function <span class="apidocSignatureSpan">engine.io.Server.</span>super_ ()](#apidoc.element.engine.io.Server.super_)
1.  object <span class="apidocSignatureSpan">engine.io.Server.</span>errorMessages
1.  object <span class="apidocSignatureSpan">engine.io.Server.</span>errors

#### [module engine.io.Server.prototype](#apidoc.module.engine.io.Server.prototype)
1.  [function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>attach (server, options)](#apidoc.element.engine.io.Server.prototype.attach)
1.  [function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>close ()](#apidoc.element.engine.io.Server.prototype.close)
1.  [function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>generateId (req)](#apidoc.element.engine.io.Server.prototype.generateId)
1.  [function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>handleRequest (req, res)](#apidoc.element.engine.io.Server.prototype.handleRequest)
1.  [function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>handleUpgrade (req, socket, upgradeHead)](#apidoc.element.engine.io.Server.prototype.handleUpgrade)
1.  [function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>handshake (transportName, req)](#apidoc.element.engine.io.Server.prototype.handshake)
1.  [function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>init ()](#apidoc.element.engine.io.Server.prototype.init)
1.  [function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>onWebSocket (req, socket)](#apidoc.element.engine.io.Server.prototype.onWebSocket)
1.  [function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>prepare (req)](#apidoc.element.engine.io.Server.prototype.prepare)
1.  [function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>upgrades (transport)](#apidoc.element.engine.io.Server.prototype.upgrades)
1.  [function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>verify (req, upgrade, fn)](#apidoc.element.engine.io.Server.prototype.verify)

#### [module engine.io.Socket](#apidoc.module.engine.io.Socket)
1.  [function <span class="apidocSignatureSpan">engine.io.</span>Socket (id, server, transport, req)](#apidoc.element.engine.io.Socket.Socket)
1.  [function <span class="apidocSignatureSpan">engine.io.Socket.</span>super_ ()](#apidoc.element.engine.io.Socket.super_)

#### [module engine.io.Socket.prototype](#apidoc.module.engine.io.Socket.prototype)
1.  [function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>clearTransport ()](#apidoc.element.engine.io.Socket.prototype.clearTransport)
1.  [function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>close (discard)](#apidoc.element.engine.io.Socket.prototype.close)
1.  [function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>closeTransport (discard)](#apidoc.element.engine.io.Socket.prototype.closeTransport)
1.  [function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>flush ()](#apidoc.element.engine.io.Socket.prototype.flush)
1.  [function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>getAvailableUpgrades ()](#apidoc.element.engine.io.Socket.prototype.getAvailableUpgrades)
1.  [function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>maybeUpgrade (transport)](#apidoc.element.engine.io.Socket.prototype.maybeUpgrade)
1.  [function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>onClose (reason, description)](#apidoc.element.engine.io.Socket.prototype.onClose)
1.  [function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>onError (err)](#apidoc.element.engine.io.Socket.prototype.onError)
1.  [function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>onOpen ()](#apidoc.element.engine.io.Socket.prototype.onOpen)
1.  [function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>onPacket (packet)](#apidoc.element.engine.io.Socket.prototype.onPacket)
1.  [function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>send (data, options, callback)](#apidoc.element.engine.io.Socket.prototype.send)
1.  [function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>sendPacket (type, data, options, callback)](#apidoc.element.engine.io.Socket.prototype.sendPacket)
1.  [function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>setPingTimeout ()](#apidoc.element.engine.io.Socket.prototype.setPingTimeout)
1.  [function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>setTransport (transport)](#apidoc.element.engine.io.Socket.prototype.setTransport)
1.  [function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>setupSendCallback ()](#apidoc.element.engine.io.Socket.prototype.setupSendCallback)
1.  [function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>write (data, options, callback)](#apidoc.element.engine.io.Socket.prototype.write)

#### [module engine.io.Transport](#apidoc.module.engine.io.Transport)
1.  [function <span class="apidocSignatureSpan">engine.io.</span>Transport (req)](#apidoc.element.engine.io.Transport.Transport)
1.  [function <span class="apidocSignatureSpan">engine.io.Transport.</span>super_ ()](#apidoc.element.engine.io.Transport.super_)

#### [module engine.io.Transport.prototype](#apidoc.module.engine.io.Transport.prototype)
1.  [function <span class="apidocSignatureSpan">engine.io.Transport.prototype.</span>close (fn)](#apidoc.element.engine.io.Transport.prototype.close)
1.  [function <span class="apidocSignatureSpan">engine.io.Transport.prototype.</span>discard ()](#apidoc.element.engine.io.Transport.prototype.discard)
1.  [function <span class="apidocSignatureSpan">engine.io.Transport.prototype.</span>onClose ()](#apidoc.element.engine.io.Transport.prototype.onClose)
1.  [function <span class="apidocSignatureSpan">engine.io.Transport.prototype.</span>onData (data)](#apidoc.element.engine.io.Transport.prototype.onData)
1.  [function <span class="apidocSignatureSpan">engine.io.Transport.prototype.</span>onError (msg, desc)](#apidoc.element.engine.io.Transport.prototype.onError)
1.  [function <span class="apidocSignatureSpan">engine.io.Transport.prototype.</span>onPacket (packet)](#apidoc.element.engine.io.Transport.prototype.onPacket)
1.  [function <span class="apidocSignatureSpan">engine.io.Transport.prototype.</span>onRequest (req)](#apidoc.element.engine.io.Transport.prototype.onRequest)

#### [module engine.io.parser](#apidoc.module.engine.io.parser)
1.  [function <span class="apidocSignatureSpan">engine.io.parser.</span>decodeBase64Packet (msg, binaryType)](#apidoc.element.engine.io.parser.decodeBase64Packet)
1.  [function <span class="apidocSignatureSpan">engine.io.parser.</span>decodePacket (data, binaryType, utf8decode)](#apidoc.element.engine.io.parser.decodePacket)
1.  [function <span class="apidocSignatureSpan">engine.io.parser.</span>decodePayload (data, binaryType, utf8decode, callback)](#apidoc.element.engine.io.parser.decodePayload)
1.  [function <span class="apidocSignatureSpan">engine.io.parser.</span>decodePayloadAsBinary (data, binaryType, callback)](#apidoc.element.engine.io.parser.decodePayloadAsBinary)
1.  [function <span class="apidocSignatureSpan">engine.io.parser.</span>encodeBase64Packet (packet, callback)](#apidoc.element.engine.io.parser.encodeBase64Packet)
1.  [function <span class="apidocSignatureSpan">engine.io.parser.</span>encodePacket (packet, supportsBinary, utf8encode, callback)](#apidoc.element.engine.io.parser.encodePacket)
1.  [function <span class="apidocSignatureSpan">engine.io.parser.</span>encodePayload (packets, supportsBinary, callback)](#apidoc.element.engine.io.parser.encodePayload)
1.  [function <span class="apidocSignatureSpan">engine.io.parser.</span>encodePayloadAsBinary (packets, callback)](#apidoc.element.engine.io.parser.encodePayloadAsBinary)
1.  number <span class="apidocSignatureSpan">engine.io.parser.</span>protocol
1.  object <span class="apidocSignatureSpan">engine.io.parser.</span>packets

#### [module engine.io.transports](#apidoc.module.engine.io.transports)
1.  [function <span class="apidocSignatureSpan">engine.io.transports.</span>polling (req)](#apidoc.element.engine.io.transports.polling)
1.  [function <span class="apidocSignatureSpan">engine.io.transports.</span>websocket (req)](#apidoc.element.engine.io.transports.websocket)

#### [module engine.io.transports.websocket](#apidoc.module.engine.io.transports.websocket)
1.  [function <span class="apidocSignatureSpan">engine.io.transports.</span>websocket (req)](#apidoc.element.engine.io.transports.websocket.websocket)
1.  [function <span class="apidocSignatureSpan">engine.io.transports.websocket.</span>super_ (req)](#apidoc.element.engine.io.transports.websocket.super_)

#### [module engine.io.transports.websocket.prototype](#apidoc.module.engine.io.transports.websocket.prototype)
1.  boolean <span class="apidocSignatureSpan">engine.io.transports.websocket.prototype.</span>handlesUpgrades
1.  boolean <span class="apidocSignatureSpan">engine.io.transports.websocket.prototype.</span>supportsFraming
1.  [function <span class="apidocSignatureSpan">engine.io.transports.websocket.prototype.</span>doClose (fn)](#apidoc.element.engine.io.transports.websocket.prototype.doClose)
1.  [function <span class="apidocSignatureSpan">engine.io.transports.websocket.prototype.</span>onData (data)](#apidoc.element.engine.io.transports.websocket.prototype.onData)
1.  [function <span class="apidocSignatureSpan">engine.io.transports.websocket.prototype.</span>send (packets)](#apidoc.element.engine.io.transports.websocket.prototype.send)
1.  string <span class="apidocSignatureSpan">engine.io.transports.websocket.prototype.</span>name



# <a name="apidoc.module.engine.io"></a>[module engine.io](#apidoc.module.engine.io)

#### <a name="apidoc.element.engine.io.Server"></a>[function <span class="apidocSignatureSpan">engine.io.</span>Server (opts)](#apidoc.element.engine.io.Server)
- description and source-code
```javascript
function Server(opts) {
  if (!(this instanceof Server)) {
    return new Server(opts);
  }

  this.clients = {};
  this.clientsCount = 0;

  opts = opts || {};

  this.wsEngine = opts.wsEngine || process.env.EIO_WS_ENGINE || 'uws';
  this.pingTimeout = opts.pingTimeout || 60000;
  this.pingInterval = opts.pingInterval || 25000;
  this.upgradeTimeout = opts.upgradeTimeout || 10000;
  this.maxHttpBufferSize = opts.maxHttpBufferSize || 10E7;
  this.transports = opts.transports || Object.keys(transports);
  this.allowUpgrades = false !== opts.allowUpgrades;
  this.allowRequest = opts.allowRequest;
  this.cookie = false !== opts.cookie ? (opts.cookie || 'io') : false;
  this.cookiePath = false !== opts.cookiePath ? (opts.cookiePath || '/') : false;
  this.cookieHttpOnly = false !== opts.cookieHttpOnly;
  this.perMessageDeflate = false !== opts.perMessageDeflate ? (opts.perMessageDeflate || true) : false;
  this.httpCompression = false !== opts.httpCompression ? (opts.httpCompression || {}) : false;
  this.initialPacket = opts.initialPacket;

  var self = this;

  // initialize compression options
  ['perMessageDeflate', 'httpCompression'].forEach(function (type) {
    var compression = self[type];
    if (true === compression) self[type] = compression = {};
    if (compression && null == compression.threshold) {
      compression.threshold = 1024;
    }
  });

  this.init();
}
```
- example usage
```shell
...
});
'''

#### (C) Passing in requests

'''js
var engine = require('engine.io');
var server = new engine.Server();

server.on('connection', function(socket){
  socket.send('hi');
});

// …
httpServer.on('upgrade', function(req, socket, head){
...
```

#### <a name="apidoc.element.engine.io.Socket"></a>[function <span class="apidocSignatureSpan">engine.io.</span>Socket (id, server, transport, req)](#apidoc.element.engine.io.Socket)
- description and source-code
```javascript
function Socket(id, server, transport, req) {
  this.id = id;
  this.server = server;
  this.upgrading = false;
  this.upgraded = false;
  this.readyState = 'opening';
  this.writeBuffer = [];
  this.packetsFn = [];
  this.sentCallbackFn = [];
  this.cleanupFn = [];
  this.request = req;

  // Cache IP since it might not be in the req later
  this.remoteAddress = req.connection.remoteAddress;

  this.checkIntervalTimer = null;
  this.upgradeTimeoutTimer = null;
  this.pingTimeoutTimer = null;

  this.setTransport(transport);
  this.onOpen();
}
```
- example usage
```shell
...
'''

### Client

'''html
<script src="/path/to/engine.io.js"></script>
<script>
  var socket = new eio.Socket('ws://localhost/');
  socket.on('open', function(){
    socket.on('message', function(data){});
    socket.on('close', function(){});
  });
</script>
'''
...
```

#### <a name="apidoc.element.engine.io.Transport"></a>[function <span class="apidocSignatureSpan">engine.io.</span>Transport (req)](#apidoc.element.engine.io.Transport)
- description and source-code
```javascript
function Transport(req) {
  this.readyState = 'open';
  this.discarded = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.attach"></a>[function <span class="apidocSignatureSpan">engine.io.</span>attach (server, options)](#apidoc.element.engine.io.attach)
- description and source-code
```javascript
function attach(server, options) {
  var engine = new exports.Server(options);
  engine.attach(server, options);
  return engine;
}
```
- example usage
```shell
...
'''

#### (B) Intercepting requests for a http.Server

'''js
var engine = require('engine.io');
var http = require('http').createServer().listen(3000);
var server = engine.attach(http);

server.on('connection', function (socket) {
  socket.on('message', function(data){ });
  socket.on('close', function(){ });
});
'''
...
```

#### <a name="apidoc.element.engine.io.io.Server"></a>[function <span class="apidocSignatureSpan">engine.io.</span>io.Server (opts)](#apidoc.element.engine.io.io.Server)
- description and source-code
```javascript
function Server(opts) {
  if (!(this instanceof Server)) {
    return new Server(opts);
  }

  this.clients = {};
  this.clientsCount = 0;

  opts = opts || {};

  this.wsEngine = opts.wsEngine || process.env.EIO_WS_ENGINE || 'uws';
  this.pingTimeout = opts.pingTimeout || 60000;
  this.pingInterval = opts.pingInterval || 25000;
  this.upgradeTimeout = opts.upgradeTimeout || 10000;
  this.maxHttpBufferSize = opts.maxHttpBufferSize || 10E7;
  this.transports = opts.transports || Object.keys(transports);
  this.allowUpgrades = false !== opts.allowUpgrades;
  this.allowRequest = opts.allowRequest;
  this.cookie = false !== opts.cookie ? (opts.cookie || 'io') : false;
  this.cookiePath = false !== opts.cookiePath ? (opts.cookiePath || '/') : false;
  this.cookieHttpOnly = false !== opts.cookieHttpOnly;
  this.perMessageDeflate = false !== opts.perMessageDeflate ? (opts.perMessageDeflate || true) : false;
  this.httpCompression = false !== opts.httpCompression ? (opts.httpCompression || {}) : false;
  this.initialPacket = opts.initialPacket;

  var self = this;

  // initialize compression options
  ['perMessageDeflate', 'httpCompression'].forEach(function (type) {
    var compression = self[type];
    if (true === compression) self[type] = compression = {};
    if (compression && null == compression.threshold) {
      compression.threshold = 1024;
    }
  });

  this.init();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.io.Socket"></a>[function <span class="apidocSignatureSpan">engine.io.</span>io.Socket (id, server, transport, req)](#apidoc.element.engine.io.io.Socket)
- description and source-code
```javascript
function Socket(id, server, transport, req) {
  this.id = id;
  this.server = server;
  this.upgrading = false;
  this.upgraded = false;
  this.readyState = 'opening';
  this.writeBuffer = [];
  this.packetsFn = [];
  this.sentCallbackFn = [];
  this.cleanupFn = [];
  this.request = req;

  // Cache IP since it might not be in the req later
  this.remoteAddress = req.connection.remoteAddress;

  this.checkIntervalTimer = null;
  this.upgradeTimeoutTimer = null;
  this.pingTimeoutTimer = null;

  this.setTransport(transport);
  this.onOpen();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.io.Transport"></a>[function <span class="apidocSignatureSpan">engine.io.</span>io.Transport (req)](#apidoc.element.engine.io.io.Transport)
- description and source-code
```javascript
function Transport(req) {
  this.readyState = 'open';
  this.discarded = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.io.transports.websocket"></a>[function <span class="apidocSignatureSpan">engine.io.</span>io.transports.websocket (req)](#apidoc.element.engine.io.io.transports.websocket)
- description and source-code
```javascript
function WebSocket(req) {
  Transport.call(this, req);
  var self = this;
  this.socket = req.websocket;
  this.socket.on('message', this.onData.bind(this));
  this.socket.once('close', this.onClose.bind(this));
  this.socket.on('error', this.onError.bind(this));
  this.socket.on('headers', onHeaders);
  this.writable = true;
  this.perMessageDeflate = null;

  function onHeaders (headers) {
    self.emit('headers', headers);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.listen"></a>[function <span class="apidocSignatureSpan">engine.io.</span>listen (port, options, fn)](#apidoc.element.engine.io.listen)
- description and source-code
```javascript
function listen(port, options, fn) {
  if ('function' === typeof options) {
    fn = options;
    options = {};
  }

  var server = http.createServer(function (req, res) {
    res.writeHead(501);
    res.end('Not Implemented');
  });

  // create engine server
  var engine = exports.attach(server, options);
  engine.httpServer = server;

  server.listen(port, fn);

  return engine;
}
```
- example usage
```shell
...

### Server

#### (A) Listening on a port

'''js
var engine = require('engine.io');
var server = engine.listen(80);

server.on('connection', function(socket){
  socket.send('utf 8 string');
  socket.send(new Buffer([0, 1, 2, 3, 4, 5])); // binary data
});
'''
...
```



# <a name="apidoc.module.engine.io.Server"></a>[module engine.io.Server](#apidoc.module.engine.io.Server)

#### <a name="apidoc.element.engine.io.Server.Server"></a>[function <span class="apidocSignatureSpan">engine.io.</span>Server (opts)](#apidoc.element.engine.io.Server.Server)
- description and source-code
```javascript
function Server(opts) {
  if (!(this instanceof Server)) {
    return new Server(opts);
  }

  this.clients = {};
  this.clientsCount = 0;

  opts = opts || {};

  this.wsEngine = opts.wsEngine || process.env.EIO_WS_ENGINE || 'uws';
  this.pingTimeout = opts.pingTimeout || 60000;
  this.pingInterval = opts.pingInterval || 25000;
  this.upgradeTimeout = opts.upgradeTimeout || 10000;
  this.maxHttpBufferSize = opts.maxHttpBufferSize || 10E7;
  this.transports = opts.transports || Object.keys(transports);
  this.allowUpgrades = false !== opts.allowUpgrades;
  this.allowRequest = opts.allowRequest;
  this.cookie = false !== opts.cookie ? (opts.cookie || 'io') : false;
  this.cookiePath = false !== opts.cookiePath ? (opts.cookiePath || '/') : false;
  this.cookieHttpOnly = false !== opts.cookieHttpOnly;
  this.perMessageDeflate = false !== opts.perMessageDeflate ? (opts.perMessageDeflate || true) : false;
  this.httpCompression = false !== opts.httpCompression ? (opts.httpCompression || {}) : false;
  this.initialPacket = opts.initialPacket;

  var self = this;

  // initialize compression options
  ['perMessageDeflate', 'httpCompression'].forEach(function (type) {
    var compression = self[type];
    if (true === compression) self[type] = compression = {};
    if (compression && null == compression.threshold) {
      compression.threshold = 1024;
    }
  });

  this.init();
}
```
- example usage
```shell
...
});
'''

#### (C) Passing in requests

'''js
var engine = require('engine.io');
var server = new engine.Server();

server.on('connection', function(socket){
  socket.send('hi');
});

// …
httpServer.on('upgrade', function(req, socket, head){
...
```

#### <a name="apidoc.element.engine.io.Server.super_"></a>[function <span class="apidocSignatureSpan">engine.io.Server.</span>super_ ()](#apidoc.element.engine.io.Server.super_)
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



# <a name="apidoc.module.engine.io.Server.prototype"></a>[module engine.io.Server.prototype](#apidoc.module.engine.io.Server.prototype)

#### <a name="apidoc.element.engine.io.Server.prototype.attach"></a>[function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>attach (server, options)](#apidoc.element.engine.io.Server.prototype.attach)
- description and source-code
```javascript
attach = function (server, options) {
  var self = this;
  options = options || {};
  var path = (options.path || '/engine.io').replace(/\/$/, '');

  var destroyUpgradeTimeout = options.destroyUpgradeTimeout || 1000;

  // normalize path
  path += '/';

  function check (req) {
    if ('OPTIONS' === req.method && false === options.handlePreflightRequest) {
      return false;
    }
    return path === req.url.substr(0, path.length);
  }

  // cache and clean up listeners
  var listeners = server.listeners('request').slice(0);
  server.removeAllListeners('request');
  server.on('close', self.close.bind(self));
  server.on('listening', self.init.bind(self));

  // add request handler
  server.on('request', function (req, res) {
    if (check(req)) {
      debug('intercepting request for path "%s"', path);
      if ('OPTIONS' === req.method && 'function' === typeof options.handlePreflightRequest) {
        options.handlePreflightRequest.call(server, req, res);
      } else {
        self.handleRequest(req, res);
      }
    } else {
      for (var i = 0, l = listeners.length; i < l; i++) {
        listeners[i].call(server, req, res);
      }
    }
  });

  if (~self.transports.indexOf('websocket')) {
    server.on('upgrade', function (req, socket, head) {
      if (check(req)) {
        self.handleUpgrade(req, socket, head);
      } else if (false !== options.destroyUpgrade) {
        // default node behavior is to disconnect when no handlers
        // but by adding a handler, we prevent that
        // and if no eio thing handles the upgrade
        // then the socket needs to die!
        setTimeout(function () {
          if (socket.writable && socket.bytesWritten <= 0) {
            return socket.end();
          }
        }, destroyUpgradeTimeout);
      }
    });
  }
}
```
- example usage
```shell
...
'''

#### (B) Intercepting requests for a http.Server

'''js
var engine = require('engine.io');
var http = require('http').createServer().listen(3000);
var server = engine.attach(http);

server.on('connection', function (socket) {
  socket.on('message', function(data){ });
  socket.on('close', function(){ });
});
'''
...
```

#### <a name="apidoc.element.engine.io.Server.prototype.close"></a>[function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>close ()](#apidoc.element.engine.io.Server.prototype.close)
- description and source-code
```javascript
close = function () {
  debug('closing all open clients');
  for (var i in this.clients) {
    if (this.clients.hasOwnProperty(i)) {
      this.clients[i].close(true);
    }
  }
  if (this.ws) {
    debug('closing webSocketServer');
    this.ws.close();
    // don't delete this.ws because it can be used again if the http server starts listening again
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Server.prototype.generateId"></a>[function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>generateId (req)](#apidoc.element.engine.io.Server.prototype.generateId)
- description and source-code
```javascript
generateId = function (req) {
  return base64id.generateId();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Server.prototype.handleRequest"></a>[function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>handleRequest (req, res)](#apidoc.element.engine.io.Server.prototype.handleRequest)
- description and source-code
```javascript
handleRequest = function (req, res) {
  debug('handling "%s" http request "%s"', req.method, req.url);
  this.prepare(req);
  req.res = res;

  var self = this;
  this.verify(req, false, function (err, success) {
    if (!success) {
      sendErrorMessage(req, res, err);
      return;
    }

    if (req._query.sid) {
      debug('setting new request for existing client');
      self.clients[req._query.sid].transport.onRequest(req);
    } else {
      self.handshake(req._query.transport, req);
    }
  });
}
```
- example usage
```shell
...
});

// …
httpServer.on('upgrade', function(req, socket, head){
  server.handleUpgrade(req, socket, head);
});
httpServer.on('request', function(req, res){
  server.handleRequest(req, res);
});
'''

### Client

'''html
<script src="/path/to/engine.io.js"></script>
...
```

#### <a name="apidoc.element.engine.io.Server.prototype.handleUpgrade"></a>[function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>handleUpgrade (req, socket, upgradeHead)](#apidoc.element.engine.io.Server.prototype.handleUpgrade)
- description and source-code
```javascript
handleUpgrade = function (req, socket, upgradeHead) {
  this.prepare(req);

  var self = this;
  this.verify(req, true, function (err, success) {
    if (!success) {
      abortConnection(socket, err);
      return;
    }

    var head = new Buffer(upgradeHead.length);
    upgradeHead.copy(head);
    upgradeHead = null;

    // delegate to ws
    self.ws.handleUpgrade(req, socket, head, function (conn) {
      self.onWebSocket(req, conn);
    });
  });
}
```
- example usage
```shell
...

server.on('connection', function(socket){
  socket.send('hi');
});

// …
httpServer.on('upgrade', function(req, socket, head){
  server.handleUpgrade(req, socket, head);
});
httpServer.on('request', function(req, res){
  server.handleRequest(req, res);
});
'''

### Client
...
```

#### <a name="apidoc.element.engine.io.Server.prototype.handshake"></a>[function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>handshake (transportName, req)](#apidoc.element.engine.io.Server.prototype.handshake)
- description and source-code
```javascript
handshake = function (transportName, req) {
  var id = this.generateId(req);

  debug('handshaking client "%s"', id);

  try {
    var transport = new transports[transportName](req);
    if ('polling' === transportName) {
      transport.maxHttpBufferSize = this.maxHttpBufferSize;
      transport.httpCompression = this.httpCompression;
    } else if ('websocket' === transportName) {
      transport.perMessageDeflate = this.perMessageDeflate;
    }

    if (req._query && req._query.b64) {
      transport.supportsBinary = false;
    } else {
      transport.supportsBinary = true;
    }
  } catch (e) {
    sendErrorMessage(req, req.res, Server.errors.BAD_REQUEST);
    return;
  }
  var socket = new Socket(id, this, transport, req);
  var self = this;

  if (false !== this.cookie) {
    transport.on('headers', function (headers) {
      headers['Set-Cookie'] = cookieMod.serialize(self.cookie, id,
        {
          path: self.cookiePath,
          httpOnly: self.cookiePath ? self.cookieHttpOnly : false
        });
    });
  }

  transport.onRequest(req);

  this.clients[id] = socket;
  this.clientsCount++;

  socket.once('close', function () {
    delete self.clients[id];
    self.clientsCount--;
  });

  this.emit('connection', socket);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Server.prototype.init"></a>[function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>init ()](#apidoc.element.engine.io.Server.prototype.init)
- description and source-code
```javascript
init = function () {
  if (!~this.transports.indexOf('websocket')) return;

  if (this.ws) this.ws.close();

  var wsModule;
  try {
    wsModule = require(this.wsEngine);
  } catch (ex) {
    this.wsEngine = 'ws';
    // keep require('ws') as separate expression for packers (browserify, etc)
    wsModule = require('ws');
  }
  this.ws = new wsModule.Server({
    noServer: true,
    clientTracking: false,
    perMessageDeflate: this.perMessageDeflate,
    maxPayload: this.maxHttpBufferSize
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Server.prototype.onWebSocket"></a>[function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>onWebSocket (req, socket)](#apidoc.element.engine.io.Server.prototype.onWebSocket)
- description and source-code
```javascript
onWebSocket = function (req, socket) {
  socket.on('error', onUpgradeError);

  if (!transports[req._query.transport].prototype.handlesUpgrades) {
    debug('transport doesnt handle upgraded requests');
    socket.close();
    return;
  }

  // get client id
  var id = req._query.sid;

  // keep a reference to the ws.Socket
  req.websocket = socket;

  if (id) {
    var client = this.clients[id];
    if (!client) {
      debug('upgrade attempt for closed client');
      socket.close();
    } else if (client.upgrading) {
      debug('transport has already been trying to upgrade');
      socket.close();
    } else if (client.upgraded) {
      debug('transport had already been upgraded');
      socket.close();
    } else {
      debug('upgrading existing transport');

      // transport error handling takes over
      socket.removeListener('error', onUpgradeError);

      var transport = new transports[req._query.transport](req);
      if (req._query && req._query.b64) {
        transport.supportsBinary = false;
      } else {
        transport.supportsBinary = true;
      }
      transport.perMessageDeflate = this.perMessageDeflate;
      client.maybeUpgrade(transport);
    }
  } else {
    // transport error handling takes over
    socket.removeListener('error', onUpgradeError);

    this.handshake(req._query.transport, req);
  }

  function onUpgradeError () {
    debug('websocket error before upgrade');
    // socket.close() not needed
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Server.prototype.prepare"></a>[function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>prepare (req)](#apidoc.element.engine.io.Server.prototype.prepare)
- description and source-code
```javascript
prepare = function (req) {
  // try to leverage pre-existing 'req._query' (e.g: from connect)
  if (!req._query) {
    req._query = ~req.url.indexOf('?') ? qs.parse(parse(req.url).query) : {};
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Server.prototype.upgrades"></a>[function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>upgrades (transport)](#apidoc.element.engine.io.Server.prototype.upgrades)
- description and source-code
```javascript
upgrades = function (transport) {
  if (!this.allowUpgrades) return [];
  return transports[transport].upgradesTo || [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Server.prototype.verify"></a>[function <span class="apidocSignatureSpan">engine.io.Server.prototype.</span>verify (req, upgrade, fn)](#apidoc.element.engine.io.Server.prototype.verify)
- description and source-code
```javascript
verify = function (req, upgrade, fn) {
  // transport check
  var transport = req._query.transport;
  if (!~this.transports.indexOf(transport)) {
    debug('unknown transport "%s"', transport);
    return fn(Server.errors.UNKNOWN_TRANSPORT, false);
  }

  // sid check
  var sid = req._query.sid;
  if (sid) {
    if (!this.clients.hasOwnProperty(sid)) {
      return fn(Server.errors.UNKNOWN_SID, false);
    }
    if (!upgrade && this.clients[sid].transport.name !== transport) {
      debug('bad request: unexpected transport without upgrade');
      return fn(Server.errors.BAD_REQUEST, false);
    }
  } else {
    // handshake is GET only
    if ('GET' !== req.method) return fn(Server.errors.BAD_HANDSHAKE_METHOD, false);
    if (!this.allowRequest) return fn(null, true);
    return this.allowRequest(req, fn);
  }

  fn(null, true);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.engine.io.Socket"></a>[module engine.io.Socket](#apidoc.module.engine.io.Socket)

#### <a name="apidoc.element.engine.io.Socket.Socket"></a>[function <span class="apidocSignatureSpan">engine.io.</span>Socket (id, server, transport, req)](#apidoc.element.engine.io.Socket.Socket)
- description and source-code
```javascript
function Socket(id, server, transport, req) {
  this.id = id;
  this.server = server;
  this.upgrading = false;
  this.upgraded = false;
  this.readyState = 'opening';
  this.writeBuffer = [];
  this.packetsFn = [];
  this.sentCallbackFn = [];
  this.cleanupFn = [];
  this.request = req;

  // Cache IP since it might not be in the req later
  this.remoteAddress = req.connection.remoteAddress;

  this.checkIntervalTimer = null;
  this.upgradeTimeoutTimer = null;
  this.pingTimeoutTimer = null;

  this.setTransport(transport);
  this.onOpen();
}
```
- example usage
```shell
...
'''

### Client

'''html
<script src="/path/to/engine.io.js"></script>
<script>
  var socket = new eio.Socket('ws://localhost/');
  socket.on('open', function(){
    socket.on('message', function(data){});
    socket.on('close', function(){});
  });
</script>
'''
...
```

#### <a name="apidoc.element.engine.io.Socket.super_"></a>[function <span class="apidocSignatureSpan">engine.io.Socket.</span>super_ ()](#apidoc.element.engine.io.Socket.super_)
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



# <a name="apidoc.module.engine.io.Socket.prototype"></a>[module engine.io.Socket.prototype](#apidoc.module.engine.io.Socket.prototype)

#### <a name="apidoc.element.engine.io.Socket.prototype.clearTransport"></a>[function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>clearTransport ()](#apidoc.element.engine.io.Socket.prototype.clearTransport)
- description and source-code
```javascript
clearTransport = function () {
  var cleanup;

  var toCleanUp = this.cleanupFn.length;

  for (var i = 0; i < toCleanUp; i++) {
    cleanup = this.cleanupFn.shift();
    cleanup();
  }

  // silence further transport errors and prevent uncaught exceptions
  this.transport.on('error', function () {
    debug('error triggered by discarded transport');
  });

  // ensure transport won't stay open
  this.transport.close();

  clearTimeout(this.pingTimeoutTimer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Socket.prototype.close"></a>[function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>close (discard)](#apidoc.element.engine.io.Socket.prototype.close)
- description and source-code
```javascript
close = function (discard) {
  if ('open' !== this.readyState) return;

  this.readyState = 'closing';

  if (this.writeBuffer.length) {
    this.once('drain', this.closeTransport.bind(this, discard));
    return;
  }

  this.closeTransport(discard);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Socket.prototype.closeTransport"></a>[function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>closeTransport (discard)](#apidoc.element.engine.io.Socket.prototype.closeTransport)
- description and source-code
```javascript
closeTransport = function (discard) {
  if (discard) this.transport.discard();
  this.transport.close(this.onClose.bind(this, 'forced close'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Socket.prototype.flush"></a>[function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>flush ()](#apidoc.element.engine.io.Socket.prototype.flush)
- description and source-code
```javascript
flush = function () {
  if ('closed' !== this.readyState &&
                this.transport.writable &&
                this.writeBuffer.length) {
    debug('flushing buffer to transport');
    this.emit('flush', this.writeBuffer);
    this.server.emit('flush', this, this.writeBuffer);
    var wbuf = this.writeBuffer;
    this.writeBuffer = [];
    if (!this.transport.supportsFraming) {
      this.sentCallbackFn.push(this.packetsFn);
    } else {
      this.sentCallbackFn.push.apply(this.sentCallbackFn, this.packetsFn);
    }
    this.packetsFn = [];
    this.transport.send(wbuf);
    this.emit('drain');
    this.server.emit('drain', this);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Socket.prototype.getAvailableUpgrades"></a>[function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>getAvailableUpgrades ()](#apidoc.element.engine.io.Socket.prototype.getAvailableUpgrades)
- description and source-code
```javascript
getAvailableUpgrades = function () {
  var availableUpgrades = [];
  var allUpgrades = this.server.upgrades(this.transport.name);
  for (var i = 0, l = allUpgrades.length; i < l; ++i) {
    var upg = allUpgrades[i];
    if (this.server.transports.indexOf(upg) !== -1) {
      availableUpgrades.push(upg);
    }
  }
  return availableUpgrades;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Socket.prototype.maybeUpgrade"></a>[function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>maybeUpgrade (transport)](#apidoc.element.engine.io.Socket.prototype.maybeUpgrade)
- description and source-code
```javascript
maybeUpgrade = function (transport) {
  debug('might upgrade socket transport from "%s" to "%s"'
    , this.transport.name, transport.name);

  this.upgrading = true;

  var self = this;

  // set transport upgrade timer
  self.upgradeTimeoutTimer = setTimeout(function () {
    debug('client did not complete upgrade - closing transport');
    cleanup();
    if ('open' === transport.readyState) {
      transport.close();
    }
  }, this.server.upgradeTimeout);

  function onPacket (packet) {
    if ('ping' === packet.type && 'probe' === packet.data) {
      transport.send([{ type: 'pong', data: 'probe' }]);
      self.emit('upgrading', transport);
      clearInterval(self.checkIntervalTimer);
      self.checkIntervalTimer = setInterval(check, 100);
    } else if ('upgrade' === packet.type && self.readyState !== 'closed') {
      debug('got upgrade packet - upgrading');
      cleanup();
      self.transport.discard();
      self.upgraded = true;
      self.clearTransport();
      self.setTransport(transport);
      self.emit('upgrade', transport);
      self.setPingTimeout();
      self.flush();
      if (self.readyState === 'closing') {
        transport.close(function () {
          self.onClose('forced close');
        });
      }
    } else {
      cleanup();
      transport.close();
    }
  }

  // we force a polling cycle to ensure a fast upgrade
  function check () {
    if ('polling' === self.transport.name && self.transport.writable) {
      debug('writing a noop packet to polling for fast upgrade');
      self.transport.send([{ type: 'noop' }]);
    }
  }

  function cleanup () {
    self.upgrading = false;

    clearInterval(self.checkIntervalTimer);
    self.checkIntervalTimer = null;

    clearTimeout(self.upgradeTimeoutTimer);
    self.upgradeTimeoutTimer = null;

    transport.removeListener('packet', onPacket);
    transport.removeListener('close', onTransportClose);
    transport.removeListener('error', onError);
    self.removeListener('close', onClose);
  }

  function onError (err) {
    debug('client did not complete upgrade - %s', err);
    cleanup();
    transport.close();
    transport = null;
  }

  function onTransportClose () {
    onError('transport closed');
  }

  function onClose () {
    onError('socket closed');
  }

  transport.on('packet', onPacket);
  transport.once('close', onTransportClose);
  transport.once('error', onError);

  self.once('close', onClose);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Socket.prototype.onClose"></a>[function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>onClose (reason, description)](#apidoc.element.engine.io.Socket.prototype.onClose)
- description and source-code
```javascript
onClose = function (reason, description) {
  if ('closed' !== this.readyState) {
    this.readyState = 'closed';
    clearTimeout(this.pingTimeoutTimer);
    clearInterval(this.checkIntervalTimer);
    this.checkIntervalTimer = null;
    clearTimeout(this.upgradeTimeoutTimer);
    var self = this;
    // clean writeBuffer in next tick, so developers can still
    // grab the writeBuffer on 'close' event
    process.nextTick(function () {
      self.writeBuffer = [];
    });
    this.packetsFn = [];
    this.sentCallbackFn = [];
    this.clearTransport();
    this.emit('close', reason, description);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Socket.prototype.onError"></a>[function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>onError (err)](#apidoc.element.engine.io.Socket.prototype.onError)
- description and source-code
```javascript
onError = function (err) {
  debug('transport error');
  this.onClose('transport error', err);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Socket.prototype.onOpen"></a>[function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>onOpen ()](#apidoc.element.engine.io.Socket.prototype.onOpen)
- description and source-code
```javascript
onOpen = function () {
  this.readyState = 'open';

  // sends an 'open' packet
  this.transport.sid = this.id;
  this.sendPacket('open', JSON.stringify({
    sid: this.id,
    upgrades: this.getAvailableUpgrades(),
    pingInterval: this.server.pingInterval,
    pingTimeout: this.server.pingTimeout
  }));

  if (this.server.initialPacket) {
    this.sendPacket('message', this.server.initialPacket);
  }

  this.emit('open');
  this.setPingTimeout();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Socket.prototype.onPacket"></a>[function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>onPacket (packet)](#apidoc.element.engine.io.Socket.prototype.onPacket)
- description and source-code
```javascript
onPacket = function (packet) {
  if ('open' === this.readyState) {
    // export packet event
    debug('packet');
    this.emit('packet', packet);

    // Reset ping timeout on any packet, incoming data is a good sign of
    // other side's liveness
    this.setPingTimeout();

    switch (packet.type) {

      case 'ping':
        debug('got ping');
        this.sendPacket('pong');
        this.emit('heartbeat');
        break;

      case 'error':
        this.onClose('parse error');
        break;

      case 'message':
        this.emit('data', packet.data);
        this.emit('message', packet.data);
        break;
    }
  } else {
    debug('packet received with closed socket');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Socket.prototype.send"></a>[function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>send (data, options, callback)](#apidoc.element.engine.io.Socket.prototype.send)
- description and source-code
```javascript
send = function (data, options, callback) {
  this.sendPacket('message', data, options, callback);
  return this;
}
```
- example usage
```shell
...
#### (A) Listening on a port

'''js
var engine = require('engine.io');
var server = engine.listen(80);

server.on('connection', function(socket){
  socket.send('utf 8 string');
  socket.send(new Buffer([0, 1, 2, 3, 4, 5])); // binary data
});
'''

#### (B) Intercepting requests for a http.Server

'''js
...
```

#### <a name="apidoc.element.engine.io.Socket.prototype.sendPacket"></a>[function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>sendPacket (type, data, options, callback)](#apidoc.element.engine.io.Socket.prototype.sendPacket)
- description and source-code
```javascript
sendPacket = function (type, data, options, callback) {
  if ('function' === typeof options) {
    callback = options;
    options = null;
  }

  options = options || {};
  options.compress = false !== options.compress;

  if ('closing' !== this.readyState && 'closed' !== this.readyState) {
    debug('sending packet "%s" (%s)', type, data);

    var packet = {
      type: type,
      options: options
    };
    if (data) packet.data = data;

    // exports packetCreate event
    this.emit('packetCreate', packet);

    this.writeBuffer.push(packet);

    // add send callback to object, if defined
    if (callback) this.packetsFn.push(callback);

    this.flush();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Socket.prototype.setPingTimeout"></a>[function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>setPingTimeout ()](#apidoc.element.engine.io.Socket.prototype.setPingTimeout)
- description and source-code
```javascript
setPingTimeout = function () {
  var self = this;
  clearTimeout(self.pingTimeoutTimer);
  self.pingTimeoutTimer = setTimeout(function () {
    self.onClose('ping timeout');
  }, self.server.pingInterval + self.server.pingTimeout);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Socket.prototype.setTransport"></a>[function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>setTransport (transport)](#apidoc.element.engine.io.Socket.prototype.setTransport)
- description and source-code
```javascript
setTransport = function (transport) {
  var onError = this.onError.bind(this);
  var onPacket = this.onPacket.bind(this);
  var flush = this.flush.bind(this);
  var onClose = this.onClose.bind(this, 'transport close');

  this.transport = transport;
  this.transport.once('error', onError);
  this.transport.on('packet', onPacket);
  this.transport.on('drain', flush);
  this.transport.once('close', onClose);
  // this function will manage packet events (also message callbacks)
  this.setupSendCallback();

  this.cleanupFn.push(function () {
    transport.removeListener('error', onError);
    transport.removeListener('packet', onPacket);
    transport.removeListener('drain', flush);
    transport.removeListener('close', onClose);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Socket.prototype.setupSendCallback"></a>[function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>setupSendCallback ()](#apidoc.element.engine.io.Socket.prototype.setupSendCallback)
- description and source-code
```javascript
setupSendCallback = function () {
  var self = this;
  this.transport.on('drain', onDrain);

  this.cleanupFn.push(function () {
    self.transport.removeListener('drain', onDrain);
  });

  // the message was sent successfully, execute the callback
  function onDrain () {
    if (self.sentCallbackFn.length > 0) {
      var seqFn = self.sentCallbackFn.splice(0, 1)[0];
      if ('function' === typeof seqFn) {
        debug('executing send callback');
        seqFn(self.transport);
      } else if (Array.isArray(seqFn)) {
        debug('executing batch send callback');
        for (var l = seqFn.length, i = 0; i < l; i++) {
          if ('function' === typeof seqFn[i]) {
            seqFn[i](self.transport);
          }
        }
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Socket.prototype.write"></a>[function <span class="apidocSignatureSpan">engine.io.Socket.prototype.</span>write (data, options, callback)](#apidoc.element.engine.io.Socket.prototype.write)
- description and source-code
```javascript
write = function (data, options, callback) {
  this.sendPacket('message', data, options, callback);
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.engine.io.Transport"></a>[module engine.io.Transport](#apidoc.module.engine.io.Transport)

#### <a name="apidoc.element.engine.io.Transport.Transport"></a>[function <span class="apidocSignatureSpan">engine.io.</span>Transport (req)](#apidoc.element.engine.io.Transport.Transport)
- description and source-code
```javascript
function Transport(req) {
  this.readyState = 'open';
  this.discarded = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Transport.super_"></a>[function <span class="apidocSignatureSpan">engine.io.Transport.</span>super_ ()](#apidoc.element.engine.io.Transport.super_)
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



# <a name="apidoc.module.engine.io.Transport.prototype"></a>[module engine.io.Transport.prototype](#apidoc.module.engine.io.Transport.prototype)

#### <a name="apidoc.element.engine.io.Transport.prototype.close"></a>[function <span class="apidocSignatureSpan">engine.io.Transport.prototype.</span>close (fn)](#apidoc.element.engine.io.Transport.prototype.close)
- description and source-code
```javascript
close = function (fn) {
  if ('closed' === this.readyState || 'closing' === this.readyState) return;

  this.readyState = 'closing';
  this.doClose(fn || noop);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Transport.prototype.discard"></a>[function <span class="apidocSignatureSpan">engine.io.Transport.prototype.</span>discard ()](#apidoc.element.engine.io.Transport.prototype.discard)
- description and source-code
```javascript
discard = function () {
  this.discarded = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Transport.prototype.onClose"></a>[function <span class="apidocSignatureSpan">engine.io.Transport.prototype.</span>onClose ()](#apidoc.element.engine.io.Transport.prototype.onClose)
- description and source-code
```javascript
onClose = function () {
  this.readyState = 'closed';
  this.emit('close');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Transport.prototype.onData"></a>[function <span class="apidocSignatureSpan">engine.io.Transport.prototype.</span>onData (data)](#apidoc.element.engine.io.Transport.prototype.onData)
- description and source-code
```javascript
onData = function (data) {
  this.onPacket(parser.decodePacket(data));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Transport.prototype.onError"></a>[function <span class="apidocSignatureSpan">engine.io.Transport.prototype.</span>onError (msg, desc)](#apidoc.element.engine.io.Transport.prototype.onError)
- description and source-code
```javascript
onError = function (msg, desc) {
  if (this.listeners('error').length) {
    var err = new Error(msg);
    err.type = 'TransportError';
    err.description = desc;
    this.emit('error', err);
  } else {
    debug('ignored transport error %s (%s)', msg, desc);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Transport.prototype.onPacket"></a>[function <span class="apidocSignatureSpan">engine.io.Transport.prototype.</span>onPacket (packet)](#apidoc.element.engine.io.Transport.prototype.onPacket)
- description and source-code
```javascript
onPacket = function (packet) {
  this.emit('packet', packet);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.Transport.prototype.onRequest"></a>[function <span class="apidocSignatureSpan">engine.io.Transport.prototype.</span>onRequest (req)](#apidoc.element.engine.io.Transport.prototype.onRequest)
- description and source-code
```javascript
onRequest = function (req) {
  debug('setting request');
  this.req = req;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.engine.io.parser"></a>[module engine.io.parser](#apidoc.module.engine.io.parser)

#### <a name="apidoc.element.engine.io.parser.decodeBase64Packet"></a>[function <span class="apidocSignatureSpan">engine.io.parser.</span>decodeBase64Packet (msg, binaryType)](#apidoc.element.engine.io.parser.decodeBase64Packet)
- description and source-code
```javascript
decodeBase64Packet = function (msg, binaryType) {
  var type = packetslist[msg.charAt(0)];
  var data = new Buffer(msg.substr(1), 'base64');
  if (binaryType === 'arraybuffer') {
    var abv = new Uint8Array(data.length);
    for (var i = 0; i < abv.length; i++){
      abv[i] = data[i];
    }
    data = abv.buffer;
  }
  return { type: type, data: data };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.parser.decodePacket"></a>[function <span class="apidocSignatureSpan">engine.io.parser.</span>decodePacket (data, binaryType, utf8decode)](#apidoc.element.engine.io.parser.decodePacket)
- description and source-code
```javascript
decodePacket = function (data, binaryType, utf8decode) {
  if (data === undefined) {
    return err;
  }

  var type;

  // String data
  if (typeof data === 'string') {

    type = data.charAt(0);

    if (type === 'b') {
      return exports.decodeBase64Packet(data.substr(1), binaryType);
    }

    if (utf8decode) {
      data = tryDecode(data);
      if (data === false) {
        return err;
      }
    }

    if (Number(type) != type || !packetslist[type]) {
      return err;
    }

    if (data.length > 1) {
      return { type: packetslist[type], data: data.substring(1) };
    } else {
      return { type: packetslist[type] };
    }
  }

  // Binary data
  if (binaryType === 'arraybuffer') {
    // wrap Buffer/ArrayBuffer data into an Uint8Array
    var intArray = new Uint8Array(data);
    type = intArray[0];
    return { type: packetslist[type], data: intArray.buffer.slice(1) };
  }

  if (data instanceof ArrayBuffer) {
    data = arrayBufferToBuffer(data);
  }
  type = data[0];
  return { type: packetslist[type], data: data.slice(1) };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.parser.decodePayload"></a>[function <span class="apidocSignatureSpan">engine.io.parser.</span>decodePayload (data, binaryType, utf8decode, callback)](#apidoc.element.engine.io.parser.decodePayload)
- description and source-code
```javascript
decodePayload = function (data, binaryType, utf8decode, callback) {
  if (typeof data !== 'string') {
    return exports.decodePayloadAsBinary(data, binaryType, callback);
  }

  if (typeof binaryType === 'function') {
    callback = binaryType;
    binaryType = null;
  }

  if (typeof utf8decode === 'function') {
    callback = utf8decode;
    utf8decode = null;
  }

  if (data === '') {
    // parser error - ignoring payload
    return callback(err, 0, 1);
  }

  if (utf8decode) {
    data = tryDecode(data);
    if (data === false) {
      return callback(err, 0, 1);
    }
  }

  var length = '', n, msg, packet;

  for (var i = 0, l = data.length; i < l; i++) {
    var chr = data.charAt(i);

    if (chr !== ':') {
      length += chr;
      continue;
    }

    if (length === '' || (length != (n = Number(length)))) {
      // parser error - ignoring payload
      return callback(err, 0, 1);
    }

    msg = data.substr(i + 1, n);

    if (length != msg.length) {
      // parser error - ignoring payload
      return callback(err, 0, 1);
    }

    if (msg.length) {
      packet = exports.decodePacket(msg, binaryType, false);

      if (err.type === packet.type && err.data === packet.data) {
        // parser error in individual packet - ignoring payload
        return callback(err, 0, 1);
      }

      var more = callback(packet, i + n, l);
      if (false === more) return;
    }

    // advance cursor
    i += n;
    length = '';
  }

  if (length !== '') {
    // parser error - ignoring payload
    return callback(err, 0, 1);
  }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.parser.decodePayloadAsBinary"></a>[function <span class="apidocSignatureSpan">engine.io.parser.</span>decodePayloadAsBinary (data, binaryType, callback)](#apidoc.element.engine.io.parser.decodePayloadAsBinary)
- description and source-code
```javascript
decodePayloadAsBinary = function (data, binaryType, callback) {
  if (typeof binaryType === 'function') {
    callback = binaryType;
    binaryType = null;
  }

  var bufferTail = data;
  var buffers = [];
  var i;

  while (bufferTail.length > 0) {
    var strLen = '';
    var isString = bufferTail[0] === 0;
    for (i = 1; ; i++) {
      if (bufferTail[i] === 255)  break;
      // 310 = char length of Number.MAX_VALUE
      if (strLen.length > 310) {
        return callback(err, 0, 1);
      }
      strLen += '' + bufferTail[i];
    }
    bufferTail = bufferTail.slice(strLen.length + 1);

    var msgLength = parseInt(strLen, 10);

    var msg = bufferTail.slice(1, msgLength + 1);
    if (isString) msg = bufferToString(msg);
    buffers.push(msg);
    bufferTail = bufferTail.slice(msgLength + 1);
  }

  var total = buffers.length;
  for (i = 0; i < total; i++) {
    var buffer = buffers[i];
    callback(exports.decodePacket(buffer, binaryType, true), i, total);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.parser.encodeBase64Packet"></a>[function <span class="apidocSignatureSpan">engine.io.parser.</span>encodeBase64Packet (packet, callback)](#apidoc.element.engine.io.parser.encodeBase64Packet)
- description and source-code
```javascript
encodeBase64Packet = function (packet, callback){
  if (!Buffer.isBuffer(packet.data)) {
    packet.data = arrayBufferToBuffer(packet.data);
  }

  var message = 'b' + packets[packet.type];
  message += packet.data.toString('base64');
  return callback(message);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.parser.encodePacket"></a>[function <span class="apidocSignatureSpan">engine.io.parser.</span>encodePacket (packet, supportsBinary, utf8encode, callback)](#apidoc.element.engine.io.parser.encodePacket)
- description and source-code
```javascript
encodePacket = function (packet, supportsBinary, utf8encode, callback) {
  if (typeof supportsBinary === 'function') {
    callback = supportsBinary;
    supportsBinary = null;
  }

  if (typeof utf8encode === 'function') {
    callback = utf8encode;
    utf8encode = null;
  }

  if (Buffer.isBuffer(packet.data)) {
    return encodeBuffer(packet, supportsBinary, callback);
  } else if (packet.data && (packet.data.buffer || packet.data) instanceof ArrayBuffer) {
    packet.data = arrayBufferToBuffer(packet.data);
    return encodeBuffer(packet, supportsBinary, callback);
  }

  // Sending data as a utf-8 string
  var encoded = packets[packet.type];

  // data fragment is optional
  if (undefined !== packet.data) {
    encoded += utf8encode ? utf8.encode(String(packet.data), { strict: false }) : String(packet.data);
  }

  return callback('' + encoded);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.parser.encodePayload"></a>[function <span class="apidocSignatureSpan">engine.io.parser.</span>encodePayload (packets, supportsBinary, callback)](#apidoc.element.engine.io.parser.encodePayload)
- description and source-code
```javascript
encodePayload = function (packets, supportsBinary, callback) {
  if (typeof supportsBinary === 'function') {
    callback = supportsBinary;
    supportsBinary = null;
  }

  if (supportsBinary && hasBinary(packets)) {
    return exports.encodePayloadAsBinary(packets, callback);
  }

  if (!packets.length) {
    return callback('0:');
  }

  function encodeOne(packet, doneCallback) {
    exports.encodePacket(packet, supportsBinary, false, function(message) {
      doneCallback(null, setLengthHeader(message));
    });
  }

  map(packets, encodeOne, function(err, results) {
    return callback(results.join(''));
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.parser.encodePayloadAsBinary"></a>[function <span class="apidocSignatureSpan">engine.io.parser.</span>encodePayloadAsBinary (packets, callback)](#apidoc.element.engine.io.parser.encodePayloadAsBinary)
- description and source-code
```javascript
encodePayloadAsBinary = function (packets, callback) {
  if (!packets.length) {
    return callback(new Buffer(0));
  }

  map(packets, encodeOneBinaryPacket, function(err, results) {
    return callback(Buffer.concat(results));
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.engine.io.transports"></a>[module engine.io.transports](#apidoc.module.engine.io.transports)

#### <a name="apidoc.element.engine.io.transports.polling"></a>[function <span class="apidocSignatureSpan">engine.io.transports.</span>polling (req)](#apidoc.element.engine.io.transports.polling)
- description and source-code
```javascript
function polling(req) {
  if ('string' === typeof req._query.j) {
    return new JSONP(req);
  } else {
    return new XHR(req);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.transports.websocket"></a>[function <span class="apidocSignatureSpan">engine.io.transports.</span>websocket (req)](#apidoc.element.engine.io.transports.websocket)
- description and source-code
```javascript
function WebSocket(req) {
  Transport.call(this, req);
  var self = this;
  this.socket = req.websocket;
  this.socket.on('message', this.onData.bind(this));
  this.socket.once('close', this.onClose.bind(this));
  this.socket.on('error', this.onError.bind(this));
  this.socket.on('headers', onHeaders);
  this.writable = true;
  this.perMessageDeflate = null;

  function onHeaders (headers) {
    self.emit('headers', headers);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.engine.io.transports.websocket"></a>[module engine.io.transports.websocket](#apidoc.module.engine.io.transports.websocket)

#### <a name="apidoc.element.engine.io.transports.websocket.websocket"></a>[function <span class="apidocSignatureSpan">engine.io.transports.</span>websocket (req)](#apidoc.element.engine.io.transports.websocket.websocket)
- description and source-code
```javascript
function WebSocket(req) {
  Transport.call(this, req);
  var self = this;
  this.socket = req.websocket;
  this.socket.on('message', this.onData.bind(this));
  this.socket.once('close', this.onClose.bind(this));
  this.socket.on('error', this.onError.bind(this));
  this.socket.on('headers', onHeaders);
  this.writable = true;
  this.perMessageDeflate = null;

  function onHeaders (headers) {
    self.emit('headers', headers);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.transports.websocket.super_"></a>[function <span class="apidocSignatureSpan">engine.io.transports.websocket.</span>super_ (req)](#apidoc.element.engine.io.transports.websocket.super_)
- description and source-code
```javascript
function Transport(req) {
  this.readyState = 'open';
  this.discarded = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.engine.io.transports.websocket.prototype"></a>[module engine.io.transports.websocket.prototype](#apidoc.module.engine.io.transports.websocket.prototype)

#### <a name="apidoc.element.engine.io.transports.websocket.prototype.doClose"></a>[function <span class="apidocSignatureSpan">engine.io.transports.websocket.prototype.</span>doClose (fn)](#apidoc.element.engine.io.transports.websocket.prototype.doClose)
- description and source-code
```javascript
doClose = function (fn) {
  debug('closing');
  this.socket.close();
  fn && fn();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.transports.websocket.prototype.onData"></a>[function <span class="apidocSignatureSpan">engine.io.transports.websocket.prototype.</span>onData (data)](#apidoc.element.engine.io.transports.websocket.prototype.onData)
- description and source-code
```javascript
onData = function (data) {
  debug('received "%s"', data);
  Transport.prototype.onData.call(this, data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.engine.io.transports.websocket.prototype.send"></a>[function <span class="apidocSignatureSpan">engine.io.transports.websocket.prototype.</span>send (packets)](#apidoc.element.engine.io.transports.websocket.prototype.send)
- description and source-code
```javascript
send = function (packets) {
  var self = this;

  for (var i = 0; i < packets.length; i++) {
    var packet = packets[i];
    parser.encodePacket(packet, self.supportsBinary, send);
  }

  function send (data) {
    debug('writing "%s"', data);

    // always creates a new object since ws modifies it
    var opts = {};
    if (packet.options) {
      opts.compress = packet.options.compress;
    }

    if (self.perMessageDeflate) {
      var len = 'string' === typeof data ? Buffer.byteLength(data) : data.length;
      if (len < self.perMessageDeflate.threshold) {
        opts.compress = false;
      }
    }

    self.writable = false;
    self.socket.send(data, opts, onEnd);
  }

  function onEnd (err) {
    if (err) return self.onError('write error', err.stack);
    self.writable = true;
    self.emit('drain');
  }
}
```
- example usage
```shell
...
#### (A) Listening on a port

'''js
var engine = require('engine.io');
var server = engine.listen(80);

server.on('connection', function(socket){
  socket.send('utf 8 string');
  socket.send(new Buffer([0, 1, 2, 3, 4, 5])); // binary data
});
'''

#### (B) Intercepting requests for a http.Server

'''js
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
