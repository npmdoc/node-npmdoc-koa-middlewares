# api documentation for  [koa-middlewares (v6.0.0)](https://github.com/cnpm/koa-middlewares)  [![npm package](https://img.shields.io/npm/v/npmdoc-koa-middlewares.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-koa-middlewares) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-koa-middlewares.svg)](https://travis-ci.org/npmdoc/node-npmdoc-koa-middlewares)
#### easy way to require some useful koa middlewares

[![NPM](https://nodei.co/npm/koa-middlewares.png?downloads=true)](https://www.npmjs.com/package/koa-middlewares)

[![apidoc](https://npmdoc.github.io/node-npmdoc-koa-middlewares/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-koa-middlewares_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-koa-middlewares/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-koa-middlewares/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-koa-middlewares/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "dead_horse",
        "email": "dead_horse@qq.com",
        "url": "http://deadhorse.me"
    },
    "bugs": {
        "url": "https://github.com/cnpm/koa-middlewares/issues"
    },
    "contributors": [
        {
            "name": "dead-horse",
            "email": "dead_horse@qq.com",
            "url": "https://github.com/dead-horse"
        },
        {
            "name": "fengmk2",
            "email": "fengmk2@gmail.com",
            "url": "https://github.com/fengmk2"
        }
    ],
    "dependencies": {
        "koa-bodyparser": "^2.0.1",
        "koa-compress": "^1.0.9",
        "koa-conditional-get": "^1.0.3",
        "koa-csrf": "^2.4.0",
        "koa-ejs": "^3.0.0",
        "koa-etag": "^2.1.1",
        "koa-favicon": "^1.2.1",
        "koa-generic-session": "^1.10.2",
        "koa-logger": "^1.3.0",
        "koa-onerror": "^2.0.0",
        "koa-redis": "^2.0.1",
        "koa-resource-router": "^0.4.0",
        "koa-rewrite": "^1.1.1",
        "koa-router": "^5.4.0",
        "koa-rt": "^0.0.2",
        "koa-safe-jsonp": "^0.3.1",
        "koa-session": "^3.3.1",
        "koa-static-cache": "^3.1.7"
    },
    "description": "easy way to require some useful koa middlewares",
    "devDependencies": {
        "autod": "2",
        "koa": "1"
    },
    "directories": {},
    "dist": {
        "shasum": "0c8bfdad0ee278145a2fbb1448c139b2aa4ddc12",
        "tarball": "https://registry.npmjs.org/koa-middlewares/-/koa-middlewares-6.0.0.tgz"
    },
    "files": [
        "index.js"
    ],
    "gitHead": "252f773dbb313fed474e17629c671fc0c19fce32",
    "homepage": "https://github.com/cnpm/koa-middlewares",
    "keywords": [
        "koa",
        "middlewares",
        "session",
        "render",
        "jsonp",
        "body"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "dead_horse",
            "email": "dead_horse@qq.com"
        }
    ],
    "name": "koa-middlewares",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/cnpm/koa-middlewares.git"
    },
    "scripts": {
        "test": "node index.js"
    },
    "version": "6.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module koa-middlewares](#apidoc.module.koa-middlewares)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>RedisStore (options)](#apidoc.element.koa-middlewares.RedisStore)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>ResourceRouter (name, actions, options)](#apidoc.element.koa-middlewares.ResourceRouter)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>bodyParser (opts)](#apidoc.element.koa-middlewares.bodyParser)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>bodyparser (opts)](#apidoc.element.koa-middlewares.bodyparser)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>compress (options)](#apidoc.element.koa-middlewares.compress)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>conditional ()](#apidoc.element.koa-middlewares.conditional)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>cookieSession (opts, app)](#apidoc.element.koa-middlewares.cookieSession)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>csrf (app, opts)](#apidoc.element.koa-middlewares.csrf)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>ejs (app, settings)](#apidoc.element.koa-middlewares.ejs)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>etag (options)](#apidoc.element.koa-middlewares.etag)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>favicon (path, options)](#apidoc.element.koa-middlewares.favicon)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>jsonp (app, options)](#apidoc.element.koa-middlewares.jsonp)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>logger (opts)](#apidoc.element.koa-middlewares.logger)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>onerror (app, options)](#apidoc.element.koa-middlewares.onerror)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>redisStore (options)](#apidoc.element.koa-middlewares.redisStore)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>resourceRouter (name, actions, options)](#apidoc.element.koa-middlewares.resourceRouter)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>rewrite (src, dst)](#apidoc.element.koa-middlewares.rewrite)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>router (opts)](#apidoc.element.koa-middlewares.router)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>rt (options)](#apidoc.element.koa-middlewares.rt)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>session (options)](#apidoc.element.koa-middlewares.session)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>session.MemoryStore ()](#apidoc.element.koa-middlewares.session.MemoryStore)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>staticCache (dir, options, files)](#apidoc.element.koa-middlewares.staticCache)
1.  object <span class="apidocSignatureSpan">koa-middlewares.</span>RedisStore.prototype
1.  object <span class="apidocSignatureSpan">koa-middlewares.</span>ResourceRouter.prototype
1.  object <span class="apidocSignatureSpan">koa-middlewares.</span>router.prototype
1.  object <span class="apidocSignatureSpan">koa-middlewares.</span>session.MemoryStore.prototype

#### [module koa-middlewares.RedisStore](#apidoc.module.koa-middlewares.RedisStore)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>RedisStore (options)](#apidoc.element.koa-middlewares.RedisStore.RedisStore)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.RedisStore.</span>super_ ()](#apidoc.element.koa-middlewares.RedisStore.super_)

#### [module koa-middlewares.RedisStore.prototype](#apidoc.module.koa-middlewares.RedisStore.prototype)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.RedisStore.prototype.</span>destroy (sid)](#apidoc.element.koa-middlewares.RedisStore.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.RedisStore.prototype.</span>end ()](#apidoc.element.koa-middlewares.RedisStore.prototype.end)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.RedisStore.prototype.</span>get (sid)](#apidoc.element.koa-middlewares.RedisStore.prototype.get)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.RedisStore.prototype.</span>quit ()](#apidoc.element.koa-middlewares.RedisStore.prototype.quit)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.RedisStore.prototype.</span>set (sid, sess, ttl)](#apidoc.element.koa-middlewares.RedisStore.prototype.set)

#### [module koa-middlewares.ResourceRouter](#apidoc.module.koa-middlewares.ResourceRouter)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>ResourceRouter (name, actions, options)](#apidoc.element.koa-middlewares.ResourceRouter.ResourceRouter)

#### [module koa-middlewares.ResourceRouter.prototype](#apidoc.module.koa-middlewares.ResourceRouter.prototype)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.ResourceRouter.prototype.</span>add (resource)](#apidoc.element.koa-middlewares.ResourceRouter.prototype.add)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.ResourceRouter.prototype.</span>match (path, params)](#apidoc.element.koa-middlewares.ResourceRouter.prototype.match)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.ResourceRouter.prototype.</span>middleware ()](#apidoc.element.koa-middlewares.ResourceRouter.prototype.middleware)

#### [module koa-middlewares.csrf](#apidoc.module.koa-middlewares.csrf)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>csrf (app, opts)](#apidoc.element.koa-middlewares.csrf.csrf)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.csrf.</span>middleware (next)](#apidoc.element.koa-middlewares.csrf.middleware)

#### [module koa-middlewares.router](#apidoc.module.koa-middlewares.router)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>router (opts)](#apidoc.element.koa-middlewares.router.router)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.</span>url (path, params)](#apidoc.element.koa-middlewares.router.url)

#### [module koa-middlewares.router.prototype](#apidoc.module.koa-middlewares.router.prototype)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>acl (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.acl)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>all (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.all)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>allowedMethods (options)](#apidoc.element.koa-middlewares.router.prototype.allowedMethods)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>bind (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.bind)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>checkout (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.checkout)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>connect (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.connect)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>copy (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.copy)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>del (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.del)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>delete (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.delete)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>get (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.get)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>head (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.head)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>link (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.link)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>lock (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.lock)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>m-search (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.m-search)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>match (path, method)](#apidoc.element.koa-middlewares.router.prototype.match)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>merge (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.merge)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>middleware ()](#apidoc.element.koa-middlewares.router.prototype.middleware)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>mkactivity (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.mkactivity)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>mkcalendar (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.mkcalendar)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>mkcol (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.mkcol)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>move (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.move)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>notify (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.notify)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>options (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.options)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>param (param, middleware)](#apidoc.element.koa-middlewares.router.prototype.param)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>patch (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.patch)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>post (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.post)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>prefix (prefix)](#apidoc.element.koa-middlewares.router.prototype.prefix)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>propfind (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.propfind)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>proppatch (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.proppatch)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>purge (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.purge)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>put (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.put)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>rebind (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.rebind)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>redirect (source, destination, code)](#apidoc.element.koa-middlewares.router.prototype.redirect)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>register (path, methods, middleware, opts)](#apidoc.element.koa-middlewares.router.prototype.register)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>report (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.report)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>route (name)](#apidoc.element.koa-middlewares.router.prototype.route)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>routes ()](#apidoc.element.koa-middlewares.router.prototype.routes)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>search (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.search)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>subscribe (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.subscribe)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>trace (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.trace)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>unbind (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.unbind)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>unlink (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.unlink)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>unlock (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.unlock)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>unsubscribe (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.unsubscribe)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>url (name, params)](#apidoc.element.koa-middlewares.router.prototype.url)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>use ()](#apidoc.element.koa-middlewares.router.prototype.use)

#### [module koa-middlewares.session](#apidoc.module.koa-middlewares.session)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.</span>session (options)](#apidoc.element.koa-middlewares.session.session)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.session.</span>MemoryStore ()](#apidoc.element.koa-middlewares.session.MemoryStore)

#### [module koa-middlewares.session.MemoryStore](#apidoc.module.koa-middlewares.session.MemoryStore)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.session.</span>MemoryStore ()](#apidoc.element.koa-middlewares.session.MemoryStore.MemoryStore)

#### [module koa-middlewares.session.MemoryStore.prototype](#apidoc.module.koa-middlewares.session.MemoryStore.prototype)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.session.MemoryStore.prototype.</span>destroy (sid)](#apidoc.element.koa-middlewares.session.MemoryStore.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.session.MemoryStore.prototype.</span>get (sid)](#apidoc.element.koa-middlewares.session.MemoryStore.prototype.get)
1.  [function <span class="apidocSignatureSpan">koa-middlewares.session.MemoryStore.prototype.</span>set (sid, val)](#apidoc.element.koa-middlewares.session.MemoryStore.prototype.set)



# <a name="apidoc.module.koa-middlewares"></a>[module koa-middlewares](#apidoc.module.koa-middlewares)

#### <a name="apidoc.element.koa-middlewares.RedisStore"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>RedisStore (options)](#apidoc.element.koa-middlewares.RedisStore)
- description and source-code
```javascript
RedisStore = function (options) {
  if (!(this instanceof RedisStore)) {
    return new RedisStore(options);
  }
  EventEmitter.call(this);
  options = options || {};

  var client;
  options.auth_pass = options.auth_pass || options.pass || null;     // For backwards compatibility
  options.path = options.path || options.socket || null;             // For backwards compatibility
  if (!options.client) {
    debug('Init redis new client');
    client = redis.createClient(options);
  } else {
    if (options.duplicate) {                                         // Duplicate client and update with options provided
      debug('Duplicating provided client with new options (if provided)');
      var dupClient = options.client;
      delete options.client;
      delete options.duplicate;
      client = dupClient.duplicate(options);                         // Useful if you want to use the DB option without adjusting
 the client DB outside koa-redis
    } else {
      debug('Using provided client');
      client = options.client;
    }
  }

  if (options.db) {
    debug('selecting db %s', options.db)
    client.select(options.db);
    client.on('connect', function() {
      client.send_anyways = true;
      client.select(options.db);
      client.send_anyways = false;
    });
  }

  client.on('error', this.emit.bind(this, 'error'));
  client.on('end', this.emit.bind(this, 'end'));
  client.on('end', this.emit.bind(this, 'disconnect'));              // For backwards compatibility
  client.on('connect', this.emit.bind(this, 'connect'));
  client.on('reconnecting', this.emit.bind(this, 'reconnecting'));
  client.on('ready', this.emit.bind(this, 'ready'));
  client.on('warning', this.emit.bind(this, 'warning'));
  this.on('connect', function() {
    debug('connected to redis');
    this.connected = client.connected;
  });
  this.on('ready', function() {
    debug('redis ready');
  });
  this.on('end', function() {
    debug('redis ended');
    this.connected = client.connected;
  });
  // No good way to test error
<span class="apidocCodeCommentSpan">  /* istanbul ignore next */
</span>  this.on('error', function() {
    debug('redis error');
    this.connected = client.connected;
  });
  // No good way to test reconnect
  /* istanbul ignore next */
  this.on('reconnecting', function() {
    debug('redis reconnecting');
    this.connected = client.connected;
  });
  // No good way to test warning
  /* istanbul ignore next */
  this.on('warning', function() {
    debug('redis warning');
    this.connected = client.connected;
  });

  //wrap redis
  this._redisClient = client;
  this.client = redisWrapper(client);
  this.connected = client.connected;
}
```
- example usage
```shell
...

* **koa-generic-session**: A session like connect with memory,
has friendly APIs for work with other Stores such as 'redis', 'mongo'.
* **koa-redis**: Work togather with 'koa-generic-session', provide a redis store from koa-sess.

'''js
app.use(middlewares.session({
store: middlewares.RedisStore(),
defer: true
}));

app.use(function *() {
var session = yield this.session;
session.foo = 'bar';
this.body = this.session.foo;
...
```

#### <a name="apidoc.element.koa-middlewares.ResourceRouter"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>ResourceRouter (name, actions, options)](#apidoc.element.koa-middlewares.ResourceRouter)
- description and source-code
```javascript
function Resource(name, actions, options) {
  if (!(this instanceof Resource)) {
    var args = Array.prototype.slice.call(arguments);
    var resource = Object.create(Resource.prototype);
    Resource.apply(resource, args);
    return resource;
  }
  options = options || {};
  this.name = typeof name == 'string' ? name : null;

  this.id = this.name ? pluralize.singular(name) : 'id';
  this.base = this.name ? '/' + this.name : '/';

  var middleware = Array.prototype.slice.call(arguments, this.name ? 1 : 0);

  this.actions = middleware.pop();

  // if last object has 'methods' property or 'id' property, assume it is 'options'
  if (this.actions.methods || this.actions.id) {
    options = this.actions;
    this.actions = middleware.pop();
  }

  this.routes = [];
  this.resources = [];

  this.options = {
    id: options.id,
    methods: defaults(options.methods || {}, {
      'options': 'OPTIONS',
      'new':     'GET',
      'create':  'POST',
      'edit':    'GET',
      'update':  'PUT',
      'index':   'GET',
      'list':    'GET',
      'read':    'GET',
      'show':    'GET',
      'destroy': 'DELETE',
      'remove':  'DELETE'
    })
  };

  // Set a custom id param name if one was provided.
  this.id = this.options.id || this.id;

  // create route definition (used for routing) for each resource action
  Object.keys(this.actions).forEach(function(name) {
    var action = this.actions[name];
    var url = this.base;
    var urlTrailing = this.base;
    var params = [];

    if (!this.options.methods[name]) return;

    if (url[url.length-1] != '/') {
      urlTrailing = url + '/';
    }

    if (name == 'new') {
      url = urlTrailing + 'new';
    }
    else if (name == 'edit') {
      url = urlTrailing + ':' + this.id + '/edit';
    }
    else if (name.match(/(show|read|update|remove|destroy)/)) {
      url = urlTrailing + ':' + this.id;
    }

    // compose multiple action middleware
    if (action instanceof Array) {
      this.actions[name] = compose(action);
    }

    // compose resource middleware
    if (middleware.length) {
      this.actions[name] = compose(middleware.concat(Array.isArray(action) ? action : [action]));
    }

    this.routes.push({
      method: this.options.methods[name].toUpperCase(),
      url: url,
      regexp: pathToRegExp(url, params),
      params: params,
      action: this.actions[name]
    });
  }, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.bodyParser"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>bodyParser (opts)](#apidoc.element.koa-middlewares.bodyParser)
- description and source-code
```javascript
bodyParser = function (opts) {
  opts = opts || {};
  var detectJSON = opts.detectJSON;
  var onerror = opts.onerror;

  var enableTypes = opts.enableTypes || ['json', 'form'];
  var enableForm = checkEnable(enableTypes, 'form');
  var enableJson = checkEnable(enableTypes, 'json');
  var enableText = checkEnable(enableTypes, 'text');

  opts.detectJSON = undefined;
  opts.onerror = undefined;

  // force co-body return raw body
  opts.returnRawBody = true;

  // default json types
  var jsonTypes = [
    'application/json',
    'application/json-patch+json',
    'application/vnd.api+json',
    'application/csp-report',
  ];

  // default form types
  var formTypes = [
    'application/x-www-form-urlencoded',
  ];

  // default text types
  var textTypes = [
    'text/plain',
  ];

  var jsonOpts = formatOptions(opts, 'json');
  var formOpts = formatOptions(opts, 'form');
  var textOpts = formatOptions(opts, 'text');

  var extendTypes = opts.extendTypes || {};

  extendType(jsonTypes, extendTypes.json);
  extendType(formTypes, extendTypes.form);
  extendType(textTypes, extendTypes.text);

  return function *bodyParser(next) {
    if (this.request.body !== undefined) return yield next;
    if (this.disableBodyParser) return yield next;
    try {
      var res = yield parseBody(this);
      this.request.body = 'parsed' in res ? res.parsed : {};
      if (this.request.rawBody === undefined) this.request.rawBody = res.raw;
    } catch (err) {
      if (onerror) {
        onerror(err, this);
      } else {
        throw err;
      }
    }
    yield next;
  };

  function* parseBody(ctx) {
    if (enableJson && ((detectJSON && detectJSON(ctx)) || ctx.request.is(jsonTypes))) {
      return yield parse.json(ctx, jsonOpts);
    }
    if (enableForm && ctx.request.is(formTypes)) {
      return yield parse.form(ctx, formOpts);
    }
    if (enableText && ctx.request.is(textTypes)) {
      return yield parse.text(ctx, textOpts) || '';
    }
    return {};
  }
}
```
- example usage
```shell
...
'''js

var koa = require('koa');
var middlewares = require('koa-middlewares');

var app = koa();

app.use(middlewares.bodyParser());
app.use(middlewares.router(app));
app.use(middlewares.conditional());
app.use(middlewares.etag());
app.use(middlewares.compress());
middlewares.csrf(app);

app.use(function *() {
...
```

#### <a name="apidoc.element.koa-middlewares.bodyparser"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>bodyparser (opts)](#apidoc.element.koa-middlewares.bodyparser)
- description and source-code
```javascript
bodyparser = function (opts) {
  opts = opts || {};
  var detectJSON = opts.detectJSON;
  var onerror = opts.onerror;

  var enableTypes = opts.enableTypes || ['json', 'form'];
  var enableForm = checkEnable(enableTypes, 'form');
  var enableJson = checkEnable(enableTypes, 'json');
  var enableText = checkEnable(enableTypes, 'text');

  opts.detectJSON = undefined;
  opts.onerror = undefined;

  // force co-body return raw body
  opts.returnRawBody = true;

  // default json types
  var jsonTypes = [
    'application/json',
    'application/json-patch+json',
    'application/vnd.api+json',
    'application/csp-report',
  ];

  // default form types
  var formTypes = [
    'application/x-www-form-urlencoded',
  ];

  // default text types
  var textTypes = [
    'text/plain',
  ];

  var jsonOpts = formatOptions(opts, 'json');
  var formOpts = formatOptions(opts, 'form');
  var textOpts = formatOptions(opts, 'text');

  var extendTypes = opts.extendTypes || {};

  extendType(jsonTypes, extendTypes.json);
  extendType(formTypes, extendTypes.form);
  extendType(textTypes, extendTypes.text);

  return function *bodyParser(next) {
    if (this.request.body !== undefined) return yield next;
    if (this.disableBodyParser) return yield next;
    try {
      var res = yield parseBody(this);
      this.request.body = 'parsed' in res ? res.parsed : {};
      if (this.request.rawBody === undefined) this.request.rawBody = res.raw;
    } catch (err) {
      if (onerror) {
        onerror(err, this);
      } else {
        throw err;
      }
    }
    yield next;
  };

  function* parseBody(ctx) {
    if (enableJson && ((detectJSON && detectJSON(ctx)) || ctx.request.is(jsonTypes))) {
      return yield parse.json(ctx, jsonOpts);
    }
    if (enableForm && ctx.request.is(formTypes)) {
      return yield parse.form(ctx, formOpts);
    }
    if (enableText && ctx.request.is(textTypes)) {
      return yield parse.text(ctx, textOpts) || '';
    }
    return {};
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.compress"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>compress (options)](#apidoc.element.koa-middlewares.compress)
- description and source-code
```javascript
compress = function (options) {
  options = options || {}

  var filter = options.filter || compressible

  var threshold = !options.threshold ? 1024
    : typeof options.threshold === 'number' ? options.threshold
    : typeof options.threshold === 'string' ? bytes(options.threshold)
    : 1024

  return function* compress(next) {
    this.vary('Accept-Encoding')

    yield* next

    var body = this.body
    if (!body) return
    if (this.compress === false) return
    if (this.request.method === 'HEAD') return
    if (status.empty[this.response.status]) return
    if (this.response.get('Content-Encoding')) return

    // forced compression or implied
    if (!(this.compress === true || filter(this.response.type))) return

    // identity
    var encoding = this.acceptsEncodings('gzip', 'deflate', 'identity')
    if (!encoding) this.throw(406, 'supported encodings: gzip, deflate, identity')
    if (encoding === 'identity') return

    // json
    if (isJSON(body)) body = this.body = JSON.stringify(body)

    // threshold
    if (threshold && this.response.length < threshold) return

    this.set('Content-Encoding', encoding)
    this.res.removeHeader('Content-Length')

    var stream =
    this.body = encodingMethods[encoding](options)

    if (body instanceof Stream) {
      body.pipe(stream)
    } else {
      stream.end(body)
    }
  }
}
```
- example usage
```shell
...

var app = koa();

app.use(middlewares.bodyParser());
app.use(middlewares.router(app));
app.use(middlewares.conditional());
app.use(middlewares.etag());
app.use(middlewares.compress());
middlewares.csrf(app);

app.use(function *() {
  this.body = 'hello koa-middlewares';
});

app.listen(7001);
...
```

#### <a name="apidoc.element.koa-middlewares.conditional"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>conditional ()](#apidoc.element.koa-middlewares.conditional)
- description and source-code
```javascript
function conditional() {
  return function *conditional(next){
    yield* next;
    if (this.fresh) {
      this.status = 304;
      this.body = null;
    }
  }
}
```
- example usage
```shell
...
var koa = require('koa');
var middlewares = require('koa-middlewares');

var app = koa();

app.use(middlewares.bodyParser());
app.use(middlewares.router(app));
app.use(middlewares.conditional());
app.use(middlewares.etag());
app.use(middlewares.compress());
middlewares.csrf(app);

app.use(function *() {
  this.body = 'hello koa-middlewares';
});
...
```

#### <a name="apidoc.element.koa-middlewares.cookieSession"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>cookieSession (opts, app)](#apidoc.element.koa-middlewares.cookieSession)
- description and source-code
```javascript
cookieSession = function (opts, app){
  // session(app[, opts])
  if (opts && typeof opts.use === 'function') {
    var tmp = app;
    app = opts;
    opts = tmp;
  }

  opts = opts || {};

  // key
  opts.key = opts.key || 'koa:sess';

  // back-compat maxage
  if (!('maxAge' in opts)) opts.maxAge = opts.maxage;

  // defaults
  if (null == opts.overwrite) opts.overwrite = true;
  if (null == opts.httpOnly) opts.httpOnly = true;
  if (null == opts.signed) opts.signed = true;

  debug('session options %j', opts);

  if (!app || typeof app.use !== 'function') {
    throw new TypeError('app instance required: 'session(opts, app)'');
  }

  // setup encoding/decoding
  if (typeof opts.encode !== 'function') {
    opts.encode = encode
  }
  if (typeof opts.decode !== 'function') {
    opts.decode = decode
  }

  // to pass to Session()
  app.context.sessionKey = opts.key;

  app.context.__defineGetter__('session', function(){
    var sess = this._sess;
    // already retrieved
    if (sess) return sess;

    // unset
    if (false === sess) return null;

    var json = this.cookies.get(opts.key, opts);

    if (json) {
      debug('parse %s', json);
      try {
        // make sure sessionOptions exists
        initSessionOptions(this, opts);
        var obj = opts.decode(json);
        if (typeof opts.valid === 'function' && !opts.valid(this, obj)) {
          // valid session value fail, ignore this session
          sess = new Session(this);
          json = obj;
          debug('invalid %j', obj);
        } else {
          sess = new Session(this, obj);
          // make prev a different object from sess
          json = opts.decode(json);
        }
      } catch (err) {
        // backwards compatibility:
        // create a new session if parsing fails.
        // new Buffer(string, 'base64') does not seem to crash
        // when 'string' is not base64-encoded.
        // but 'JSON.parse(string)' will crash.
        debug('decode %j error: %s', json, err);
        if (!(err instanceof SyntaxError)) throw err;
        sess = new Session(this);
        json = null;
      }
    } else {
      debug('new session');
      sess = new Session(this);
    }

    this._sess = sess;
    this._prevjson = json;
    return sess;
  });

  app.context.__defineSetter__('session', function(val){
    if (null == val) return this._sess = false;
    if ('object' == typeof val) return this._sess = new Session(this, val);
    throw new Error('this.session can only be set as null or an object.');
  });

  return function* session(next){
    // make sessionOptions independent in each request
    initSessionOptions(this, opts);
    try {
      yield* next;
    } catch (err) {
      throw err;
    } finally {
      commit(this, this._prevjson, this._sess, opts);
    }
  };
}
```
- example usage
```shell
...
'''js
app.use(middlewares.logger());
'''

* **koa-session**: cookie base session.

'''js
app.use(middlewares.cookieSession());
'''

* **koa-generic-session**: A session like connect with memory,
has friendly APIs for work with other Stores such as 'redis', 'mongo'.
* **koa-redis**: Work togather with 'koa-generic-session', provide a redis store from koa-sess.

'''js
...
```

#### <a name="apidoc.element.koa-middlewares.csrf"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>csrf (app, opts)](#apidoc.element.koa-middlewares.csrf)
- description and source-code
```javascript
csrf = function (app, opts) {
  if (isApp(app)) {
    opts = opts || {}
  } else {
    opts = app || {}
    app = null
  }

  var tokens = require('csrf')(opts)
  var middleware = opts.middleware || exports.middleware

  if (app) {
    define(app)
    return app
  }

  return function* csrf(next) {
    define(this)
    yield middleware.call(this, next)
  }

  function define(ctx) {
    var context = ctx.context || ctx
    var response = ctx.response
    var request = ctx.request

<span class="apidocCodeCommentSpan">    /*
     * Lazily creates a CSRF token.
     * Creates one per request.
     *
     * @api public
     */
</span>
    context.__defineGetter__('csrf', function () {
      if (this._csrf) return this._csrf
      if (!this.session) return null
      var secret = this.session.secret
        || (this.session.secret = tokens.secretSync())
      return this._csrf = tokens.create(secret)
    })

    response.__defineGetter__('csrf', function () {
      return this.ctx.csrf
    })

    /**
     * Asserts that a CSRF token exists and is valid.
     * Throws a 403 error otherwise.
     * var body = yield this.request.json()
     * try {
     *   this.assertCSRF(body)
     * } catch (err) {
     *   this.status = 403
     *   this.body = {
     *     message: 'invalid CSRF token'
     *   }
     * }
     *
     * @param {Object} body
     * @return {Context} this
     * @api public
     **/

    context.assertCSRF =
    context.assertCsrf = function (body) {
      // no session
      var secret = this.session.secret
      if (!secret) this.throw(403, 'secret is missing')

      var token = (body && body._csrf)
        || (!opts.disableQuery && this.query && this.query._csrf)
        || (this.get('x-csrf-token'))
        || (this.get('x-xsrf-token'))
        || body
      if (!token) this.throw(403, 'token is missing')
      if (!tokens.verify(secret, token)) this.throw(403, 'invalid csrf token')

      return this
    }

    request.assertCSRF =
    request.assertCsrf = function (body) {
      this.ctx.assertCsrf(body)
      return this
    }

  }
}
```
- example usage
```shell
...
var app = koa();

app.use(middlewares.bodyParser());
app.use(middlewares.router(app));
app.use(middlewares.conditional());
app.use(middlewares.etag());
app.use(middlewares.compress());
middlewares.csrf(app);

app.use(function *() {
  this.body = 'hello koa-middlewares';
});

app.listen(7001);
'''
...
```

#### <a name="apidoc.element.koa-middlewares.ejs"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>ejs (app, settings)](#apidoc.element.koa-middlewares.ejs)
- description and source-code
```javascript
ejs = function (app, settings) {
  if (app.context.render) {
    return;
  }

  if (!settings || !settings.root) {
    throw new Error('settings.root required');
  }

  settings.root = path.resolve(process.cwd(), settings.root);

<span class="apidocCodeCommentSpan">  /**
  * cache the generate package
  * @type {Object}
  */
</span>  var cache = Object.create(null);

  copy(defaultSettings).to(settings);

  settings.viewExt = settings.viewExt
    ? '.' + settings.viewExt.replace(/^\./, '')
    : '';

  /**
   * generate html with view name and options
   * @param {String} view
   * @param {Object} options
   * @return {String} html
   */
  function *render(view, options) {
    view += settings.viewExt;
    var viewPath = path.join(settings.root, view);
    // get from cache
    if (settings.cache && cache[viewPath]) {
      return cache[viewPath].call(options.scope, options);
    }

    var tpl = yield fs.readFile(viewPath, 'utf8');
    var fn = ejs.compile(tpl, {
      filename: viewPath,
      _with: settings._with,
      compileDebug: settings.debug,
      delimiter: settings.delimiter
    });
    if (settings.cache) {
      cache[viewPath] = fn;
    }

    return fn.call(options.scope, options);
  }


  app.context.render = function *(view, _context) {
    var context = {};
    merge(context, this.state);
    merge(context, _context);

    var html = yield *render(view, context);

    var layout = context.layout === false ? false : (context.layout || settings.layout);
    if (layout) {
      // if using layout
      context.body = html;
      html = yield *render(layout, context);
    }

    var writeResp = context.writeResp === false ? false : (context.writeResp || settings.writeResp);
    if (writeResp) {
      //normal operation
      this.type = 'html';
      this.body = html;
    }else{
      //only return the html
      return html;
    }
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.etag"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>etag (options)](#apidoc.element.koa-middlewares.etag)
- description and source-code
```javascript
function etag(options) {
  return function *etag(next){
    yield* next;

    // no body
    var body = this.body;
    if (!body || this.response.get('ETag')) return;

    // type
    var status = this.status / 100 | 0;

    // 2xx
    if (2 != status) return;

    // hash
    var etag;
    if (body instanceof Stream) {
      if (!body.path) return;
      var s = yield fs.stat(body.path).catch(noop);
      if (!s) return;
      etag = calculate(s, options);
    } else if (('string' == typeof body) || Buffer.isBuffer(body)) {
      etag = calculate(body, options);
    } else {
      etag = calculate(JSON.stringify(body), options);
    }

    // add etag
    if (etag) this.response.etag = etag;
  }
}
```
- example usage
```shell
...
var middlewares = require('koa-middlewares');

var app = koa();

app.use(middlewares.bodyParser());
app.use(middlewares.router(app));
app.use(middlewares.conditional());
app.use(middlewares.etag());
app.use(middlewares.compress());
middlewares.csrf(app);

app.use(function *() {
  this.body = 'hello koa-middlewares';
});
...
```

#### <a name="apidoc.element.koa-middlewares.favicon"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>favicon (path, options)](#apidoc.element.koa-middlewares.favicon)
- description and source-code
```javascript
favicon = function (path, options){
  var icon;

  if (path) path = resolve(path);
  options = options || {};

  var maxAge = options.maxAge == null
    ? 86400000
    : Math.min(Math.max(0, options.maxAge), 31556926000);

  return function *favicon(next){
    if ('/favicon.ico' != this.path) return yield next;

    if (!path) return;

    if ('GET' !== this.method && 'HEAD' !== this.method) {
      this.status = 'OPTIONS' == this.method ? 200 : 405;
      this.set('Allow', 'GET, HEAD, OPTIONS');
      return;
    }

    if (!icon) icon = yield fs.readFile(path);

    this.set('Cache-Control', 'public, max-age=' + (maxAge / 1000 | 0));
    this.type = 'image/x-icon';
    this.body = icon;
  };
}
```
- example usage
```shell
...
app.use(middlewares.conditional());
app.use(middlewares.etag());
'''

* **koa-favicon**: Bounce favicon requests with a 404.

'''js
app.use(middlewares.favicon());
'''

* **koa-safe-jsonp**: A safe jsonp plugins for koa.

'''js
middlewares.jsonp(app);
...
```

#### <a name="apidoc.element.koa-middlewares.jsonp"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>jsonp (app, options)](#apidoc.element.koa-middlewares.jsonp)
- description and source-code
```javascript
function jsonp(app, options) {
  options = options || {};
  var callback = options.callback || 'callback';

  Object.defineProperty(app.context, 'jsonp', {
    set: function (obj) {
      var jsonpFunction = this.query[callback];
      if (!jsonpFunction) {
        return this.body = obj;
      }

      this.set('X-Content-Type-Options', 'nosniff');
      this.type = 'js';
      this.body = jsonpBody(obj, jsonpFunction, options);
    },
    configurable: true
  });
}
```
- example usage
```shell
...
'''js
app.use(middlewares.favicon());
'''

* **koa-safe-jsonp**: A safe jsonp plugins for koa.

'''js
middlewares.jsonp(app);

app.use(function* () {
  this.jsonp = {foo: 'bar'};
});
'''

* **koa-logger**: Development style logger.
...
```

#### <a name="apidoc.element.koa-middlewares.logger"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>logger (opts)](#apidoc.element.koa-middlewares.logger)
- description and source-code
```javascript
function dev(opts) {
  return function *logger(next) {
    // request
    var start = new Date;
    console.log('  ' + chalk.gray('<--')
      + ' ' + chalk.bold('%s')
      + ' ' + chalk.gray('%s'),
        this.method,
        this.originalUrl);

    try {
      yield next;
    } catch (err) {
      // log uncaught downstream errors
      log(this, start, null, err);
      throw err;
    }

    // calculate the length of a streaming response
    // by intercepting the stream with a counter.
    // only necessary if a content-length header is currently not set.
    var length = this.response.length;
    var body = this.body;
    var counter;
    if (null == length && body && body.readable) {
      this.body = body
        .pipe(counter = Counter())
        .on('error', this.onerror);
    }

    // log when the response is finished or closed,
    // whichever happens first.
    var ctx = this;
    var res = this.res;

    var onfinish = done.bind(null, 'finish');
    var onclose = done.bind(null, 'close');

    res.once('finish', onfinish);
    res.once('close', onclose);

    function done(event){
      res.removeListener('finish', onfinish);
      res.removeListener('close', onclose);
      log(ctx, start, counter ? counter.length : length, null, event);
    }
  }
}
```
- example usage
```shell
...
  this.jsonp = {foo: 'bar'};
});
'''

* **koa-logger**: Development style logger.

'''js
app.use(middlewares.logger());
'''

* **koa-session**: cookie base session.

'''js
app.use(middlewares.cookieSession());
'''
...
```

#### <a name="apidoc.element.koa-middlewares.onerror"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>onerror (app, options)](#apidoc.element.koa-middlewares.onerror)
- description and source-code
```javascript
function onerror(app, options) {
  options = options || {};

  const defaultOptions = {
    text: text,
    json: json,
    redirect: null,
    template: path.join(__dirname, 'error.html'),
    accepts: null,
  };

  copy(defaultOptions).to(options);
  if (!options.html) {
    options.html = createHtmlHandler(options.template);
  }

  app.context.onerror = function(err) {
    // don't do anything if there is no error.
    // this allows you to pass 'this.onerror'
    // to node-style callbacks.
    if (err == null) {
      return;
    }

    // wrap non-error object
    if (!(err instanceof Error)) {
      err = new Error('non-error thrown: ' + err);
    }

    // delegate
    this.app.emit('error', err, this);

    // nothing we can do here other
    // than delegate to the app-level
    // handler and log.
    if (this.headerSent || !this.writable) {
      err.headerSent = true;
      return;
    }

    // ENOENT support
    if (err.code === 'ENOENT') {
      err.status = 404;
    }

    if (typeof err.status !== 'number' || !http.STATUS_CODES[err.status]) {
      err.status = 500;
    }
    this.status = err.status;

    this.set(err.headers);

    let type = 'text';
    if (options.accepts) {
      type = options.accepts.call(this, 'html', 'text', 'json');
    } else {
      type = this.accepts('html', 'text', 'json');
    }
    type = type || 'text';
    if (options.all) {
      options.all.call(this, err);
    } else {
      if (options.redirect && type !== 'json') {
        this.redirect(options.redirect);
      } else {
        options[type].call(this, err);
        this.type = type;
      }
    }

    if (type === 'json') {
      this.body = JSON.stringify(this.body);
    }
    this.res.end(this.body);
  };



<span class="apidocCodeCommentSpan">  /**
   * default text error handler
   * @param {Error} err
   */
</span>
  function text(err) {
    // unset all headers, and set those specified
    this.res._headers = {};
    this.set(err.headers);

    this.body = isDev || err.expose
      ? err.message
      : http.STATUS_CODES[this.status];
  }

  /**
   * default json error handler
   * @param {Error} err
   */

  function json(err) {
    this.body = isDev || err.expose
      ? { error: err.message }
      : { error: http.STATUS_CODES[this.status] };
  }

  return app;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.redisStore"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>redisStore (options)](#apidoc.element.koa-middlewares.redisStore)
- description and source-code
```javascript
redisStore = function (options) {
  if (!(this instanceof RedisStore)) {
    return new RedisStore(options);
  }
  EventEmitter.call(this);
  options = options || {};

  var client;
  options.auth_pass = options.auth_pass || options.pass || null;     // For backwards compatibility
  options.path = options.path || options.socket || null;             // For backwards compatibility
  if (!options.client) {
    debug('Init redis new client');
    client = redis.createClient(options);
  } else {
    if (options.duplicate) {                                         // Duplicate client and update with options provided
      debug('Duplicating provided client with new options (if provided)');
      var dupClient = options.client;
      delete options.client;
      delete options.duplicate;
      client = dupClient.duplicate(options);                         // Useful if you want to use the DB option without adjusting
 the client DB outside koa-redis
    } else {
      debug('Using provided client');
      client = options.client;
    }
  }

  if (options.db) {
    debug('selecting db %s', options.db)
    client.select(options.db);
    client.on('connect', function() {
      client.send_anyways = true;
      client.select(options.db);
      client.send_anyways = false;
    });
  }

  client.on('error', this.emit.bind(this, 'error'));
  client.on('end', this.emit.bind(this, 'end'));
  client.on('end', this.emit.bind(this, 'disconnect'));              // For backwards compatibility
  client.on('connect', this.emit.bind(this, 'connect'));
  client.on('reconnecting', this.emit.bind(this, 'reconnecting'));
  client.on('ready', this.emit.bind(this, 'ready'));
  client.on('warning', this.emit.bind(this, 'warning'));
  this.on('connect', function() {
    debug('connected to redis');
    this.connected = client.connected;
  });
  this.on('ready', function() {
    debug('redis ready');
  });
  this.on('end', function() {
    debug('redis ended');
    this.connected = client.connected;
  });
  // No good way to test error
<span class="apidocCodeCommentSpan">  /* istanbul ignore next */
</span>  this.on('error', function() {
    debug('redis error');
    this.connected = client.connected;
  });
  // No good way to test reconnect
  /* istanbul ignore next */
  this.on('reconnecting', function() {
    debug('redis reconnecting');
    this.connected = client.connected;
  });
  // No good way to test warning
  /* istanbul ignore next */
  this.on('warning', function() {
    debug('redis warning');
    this.connected = client.connected;
  });

  //wrap redis
  this._redisClient = client;
  this.client = redisWrapper(client);
  this.connected = client.connected;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.resourceRouter"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>resourceRouter (name, actions, options)](#apidoc.element.koa-middlewares.resourceRouter)
- description and source-code
```javascript
function Resource(name, actions, options) {
  if (!(this instanceof Resource)) {
    var args = Array.prototype.slice.call(arguments);
    var resource = Object.create(Resource.prototype);
    Resource.apply(resource, args);
    return resource;
  }
  options = options || {};
  this.name = typeof name == 'string' ? name : null;

  this.id = this.name ? pluralize.singular(name) : 'id';
  this.base = this.name ? '/' + this.name : '/';

  var middleware = Array.prototype.slice.call(arguments, this.name ? 1 : 0);

  this.actions = middleware.pop();

  // if last object has 'methods' property or 'id' property, assume it is 'options'
  if (this.actions.methods || this.actions.id) {
    options = this.actions;
    this.actions = middleware.pop();
  }

  this.routes = [];
  this.resources = [];

  this.options = {
    id: options.id,
    methods: defaults(options.methods || {}, {
      'options': 'OPTIONS',
      'new':     'GET',
      'create':  'POST',
      'edit':    'GET',
      'update':  'PUT',
      'index':   'GET',
      'list':    'GET',
      'read':    'GET',
      'show':    'GET',
      'destroy': 'DELETE',
      'remove':  'DELETE'
    })
  };

  // Set a custom id param name if one was provided.
  this.id = this.options.id || this.id;

  // create route definition (used for routing) for each resource action
  Object.keys(this.actions).forEach(function(name) {
    var action = this.actions[name];
    var url = this.base;
    var urlTrailing = this.base;
    var params = [];

    if (!this.options.methods[name]) return;

    if (url[url.length-1] != '/') {
      urlTrailing = url + '/';
    }

    if (name == 'new') {
      url = urlTrailing + 'new';
    }
    else if (name == 'edit') {
      url = urlTrailing + ':' + this.id + '/edit';
    }
    else if (name.match(/(show|read|update|remove|destroy)/)) {
      url = urlTrailing + ':' + this.id;
    }

    // compose multiple action middleware
    if (action instanceof Array) {
      this.actions[name] = compose(action);
    }

    // compose resource middleware
    if (middleware.length) {
      this.actions[name] = compose(middleware.concat(Array.isArray(action) ? action : [action]));
    }

    this.routes.push({
      method: this.options.methods[name].toUpperCase(),
      url: url,
      regexp: pathToRegExp(url, params),
      params: params,
      action: this.actions[name]
    });
  }, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.rewrite"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>rewrite (src, dst)](#apidoc.element.koa-middlewares.rewrite)
- description and source-code
```javascript
function rewrite(src, dst) {
  var keys = [];
  var re = toRegexp(src, keys);
  var map = toMap(keys);

  debug('rewrite %s -> %s    %s', src, dst, re);

  return function*(next){
    var orig = this.path;
    var m = re.exec(orig);

    if (m) {
      this.path = dst.replace(/\$(\d+)|(?::(\w+))/g, function(_, n, name){
        if (name) return m[map[name].index + 1];
        return m[n];
      });

      debug('rewrite %s -> %s', orig, this.path);

      yield* next;

      this.path = orig;
      return;
    }

    yield* next;
  }
}
```
- example usage
```shell
...
  this.body = [{name: 'Lee'}, {name: 'Han'}];
});
'''

* **koa-rewrite**: URL rewrite middleware.

'''js
app.use(middlewares.rewrite('/js/*', '/public/assets/js/$1'));
'''

* **koa-rt**: Log response time, support custom with microtime.

'''js
var microtime = require('microtime');
app.use(middlewares.rt({
...
```

#### <a name="apidoc.element.koa-middlewares.router"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>router (opts)](#apidoc.element.koa-middlewares.router)
- description and source-code
```javascript
function Router(opts) {
  if (!(this instanceof Router)) {
    return new Router(opts);
  }

  this.opts = opts || {};
  this.methods = this.opts.methods || [
    'HEAD',
    'OPTIONS',
    'GET',
    'PUT',
    'PATCH',
    'POST',
    'DELETE'
  ];

  this.params = {};
  this.stack = [];
}
```
- example usage
```shell
...

var koa = require('koa');
var middlewares = require('koa-middlewares');

var app = koa();

app.use(middlewares.bodyParser());
app.use(middlewares.router(app));
app.use(middlewares.conditional());
app.use(middlewares.etag());
app.use(middlewares.compress());
middlewares.csrf(app);

app.use(function *() {
this.body = 'hello koa-middlewares';
...
```

#### <a name="apidoc.element.koa-middlewares.rt"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>rt (options)](#apidoc.element.koa-middlewares.rt)
- description and source-code
```javascript
function responseTime(options) {
  options = options || {};
  var timer = options.timer || Date;
  var headerName = options.headerName || 'X-Response-Time';

  return function *responseTime(next){
    var start = timer.now();
    yield* next;
    var delta = timer.now() - start;
    this.set(headerName, delta);
  };
}
```
- example usage
```shell
...
app.use(middlewares.rewrite('/js/*', '/public/assets/js/$1'));
'''

* **koa-rt**: Log response time, support custom with microtime.

'''js
var microtime = require('microtime');
app.use(middlewares.rt({
  timer: microtime
}));
'''

* **koa-static-cache**: Static file serving from memory.

'''js
...
```

#### <a name="apidoc.element.koa-middlewares.session"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>session (options)](#apidoc.element.koa-middlewares.session)
- description and source-code
```javascript
session = function (options) {
  options = options || {};
  let key = options.key || 'koa.sid';
  let client = options.store || new MemoryStore();
  let errorHandler = options.errorHandler || defaultErrorHanlder;
  let reconnectTimeout = options.reconnectTimeout || 10000;

  let store = new Store(client, {
    ttl: options.ttl,
    prefix: options.prefix
  });

  let genSid = options.genSid || uid.sync;
  let valid = options.valid || noop;
  let beforeSave = options.beforeSave || noop;

  let cookie = options.cookie || {};
  copy(defaultCookie).to(cookie);

  let storeStatus = 'available';
  let waitStore = Promise.resolve();

  // notify user that this store is not
  // meant for a production environment
  if ('production' === process.env.NODE_ENV
   && client instanceof MemoryStore) console.warn(warning);

  let sessionIdStore = options.sessionIdStore || {

    get: function() {
      return this.cookies.get(key, cookie);
    },

    set: function(sid, session) {
      this.cookies.set(key, sid, session.cookie);
    },

    reset: function() {
      this.cookies.set(key, null);
    }
  };

  store.on('disconnect', function() {
    if (storeStatus !== 'available') return;
    storeStatus = 'pending';
    waitStore = new Promise(function (resolve, reject) {
      setTimeout(function () {
        if (storeStatus === 'pending') storeStatus = 'unavailable';
        reject(new Error('session store is unavailable'));
      }, reconnectTimeout);
      store.once('connect', resolve);
    });

  });

  store.on('connect', function() {
    storeStatus = 'available';
    waitStore = Promise.resolve();
  });

  // save empty session hash for compare
  const EMPTY_SESSION_HASH = hash(generateSession());

  return options.defer ? deferSession : session;

  function addCommonAPI() {

    this._sessionSave = null;

    // more flexible
    this.__defineGetter__('sessionSave', function () {
      return this._sessionSave;
    });

    this.__defineSetter__('sessionSave', function (save) {
      this._sessionSave = save;
    });
  }

<span class="apidocCodeCommentSpan">  /**
   * generate a new session
   */
</span>  function generateSession() {
    let session = {};
    //you can alter the cookie options in nexts
    session.cookie = {};
    for (let prop in cookie) {
      session.cookie[prop] = cookie[prop];
    }
    compatMaxage(session.cookie);
    return session;
  }

  /**
   * check url match cookie's path
   */
  function matchPath(ctx) {
    let pathname = parse(ctx).pathname;
    let cookiePath = cookie.path || '/';
    if (cookiePath === '/') {
      return true;
    }
    if (pathname.indexOf(cookiePath) !== 0) {
      debug('cookie path not match');
      return false;
    }
    return true;
  }

  /**
   * get session from store
   *   get sessionId from cookie
   *   save sessionId into context
   *   get session from store
   */
  function *getSession() {
    if (!matchPath(this)) return;
    if (storeStatus === 'pending') {
      debug('store is disconnect and pending');
      yield waitStore;
    } else if (storeStatus === 'unavailable') {
      debug('store is unavailable');
      throw new Error('session store is unavailable');
    }

    if (!this.sessionId) {
      this.sessionId = sessionIdStore.get.call(this);
    }

    let session;
    let isNew = false;
    if (!this.sessionId) {
      debug('session id not exist, generate a new one');
      session = generateSession();
      this.sessionId = genSid.call(this, 24);
      isNew = true;
    } else {
      try {
        session = yield store.get(this.sessionId);
        debug('get session %j with key %s', session, this.sessionId);
      } catch (err) {
        if (err.code === 'ENOENT') {
          debug('get session error, code = ENOENT');
        } else {
          debug('get session error: ', err.message);
          errorHandler(err, 'get', this);
        }
      }
    }

    // make sure the session is still valid
    if (!session ||
      !valid(this, session)) {
      debug('session is empty or invalid');
      session = generateSession();
      this.sessionId = genSid.call(this, 24);
      sessionIdStore.re ...
```
- example usage
```shell
...
'''

* **koa-generic-session**: A session like connect with memory,
has friendly APIs for work with other Stores such as 'redis', 'mongo'.
* **koa-redis**: Work togather with 'koa-generic-session', provide a redis store from koa-sess.

'''js
app.use(middlewares.session({
store: middlewares.RedisStore(),
defer: true
}));

app.use(function *() {
var session = yield this.session;
session.foo = 'bar';
...
```

#### <a name="apidoc.element.koa-middlewares.session.MemoryStore"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>session.MemoryStore ()](#apidoc.element.koa-middlewares.session.MemoryStore)
- description and source-code
```javascript
session.MemoryStore = function () {
  this.sessions = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.staticCache"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>staticCache (dir, options, files)](#apidoc.element.koa-middlewares.staticCache)
- description and source-code
```javascript
function staticCache(dir, options, files) {
  if (typeof dir === 'object') {
    files = options
    options = dir
    dir = null
  }

  options = options || {}
  options.prefix = (options.prefix || '').replace(/\/$/, '') + path.sep
  files = files || options.files || Object.create(null)
  dir = dir || options.dir || process.cwd()
  var enableGzip = !!options.gzip
  var filePrefix = path.normalize(options.prefix.replace(/^\//, ''))

  // option.filter
  var fileFilter = function () { return true }
  if (Array.isArray(options.filter)) fileFilter = function (file) { return ~options.filter.indexOf(file) }
  if (typeof options.filter === 'function') fileFilter = options.filter

  if (options.preload !== false) {
    readDir(dir).filter(fileFilter).forEach(function (name) {
      loadFile(name, dir, options, files)
    })
  }

  if (options.alias) {
    Object.keys(options.alias).forEach(function (key) {
      var value = options.alias[key]

      if (files[value]) {
        files[key] = files[value]

        debug('aliasing ' + value + ' as ' + key)
      }
    })
  }

  return function* staticCache(next) {
    // only accept HEAD and GET
    if (this.method !== 'HEAD' && this.method !== 'GET') return yield next

    // decode for '/%E4%B8%AD%E6%96%87'
    // normalize for '//index'
    var filename = safeDecodeURIComponent(path.normalize(this.path))

    var file = files[filename]

    // try to load file
    if (!file) {
      if (!options.dynamic) return yield next
      if (path.basename(filename)[0] === '.') return yield next
      if (filename.charAt(0) === path.sep) filename = filename.slice(1)

      // trim prefix
      if (options.prefix !== path.sep) {
        if (filename.indexOf(filePrefix) !== 0) return yield next
        filename = filename.slice(filePrefix.length)
      }

      var s
      try {
        s = yield fs.stat(path.join(dir, filename))
      } catch (err) {
        return yield next
      }
      if (!s.isFile()) return yield next

      file = loadFile(filename, dir, options, files)
    }

    this.status = 200

    if (enableGzip) this.vary('Accept-Encoding')

    if (!file.buffer) {
      var stats = yield fs.stat(file.path)
      if (stats.mtime > file.mtime) {
        file.mtime = stats.mtime
        file.md5 = null
        file.length = stats.size
      }
    }

    this.response.lastModified = file.mtime
    if (file.md5) this.response.etag = file.md5

    if (this.fresh)
      return this.status = 304

    this.type = file.type
    this.length = file.zipBuffer ? file.zipBuffer.length : file.length
    this.set('Cache-Control', file.cacheControl || 'public, max-age=' + file.maxAge)
    if (file.md5) this.set('Content-MD5', file.md5)

    if (this.method === 'HEAD')
      return

    var acceptGzip = this.acceptsEncodings('gzip') === 'gzip'

    if (file.zipBuffer) {
      if (acceptGzip) {
        this.set('Content-Encoding', 'gzip')
        this.body = file.zipBuffer
      } else {
        this.body = file.buffer
      }
      return
    }

    var shouldGzip = enableGzip
      && file.length > 1024
      && acceptGzip
      && compressible(file.type)

    if (file.buffer) {
      if (shouldGzip) {

        var gzFile = files[filename + '.gz']
        if (options.usePrecompiledGzip && gzFile && gzFile.buffer) { // if .gz file already read from disk
          file.zipBuffer = gzFile.buffer
        } else {
          file.zipBuffer = yield zlib.gzip(file.buffer)
        }
        this.set('Content-Encoding', 'gzip')
        this.body = file.zipBuffer
      } else {
        this.body = file.buffer
      }
      return
    }

    var stream = fs.createReadStream(file.path)

    // update file hash
    if (!file.md5) {
      var hash = crypto.createHash('md5')
      stream.on('data', hash.update.bind(hash))
      stream.on('end', function () {
        file.md5 = hash.digest('base64')
      })
    }

    this.body = stream
    // enable gzip will remove content length
    if (shouldGzip) {
      this.remove('Content-Length')
      this.set('Content-Encoding', 'gzip')
      this.body = stream.pip ...
```
- example usage
```shell
...
  timer: microtime
}));
'''

* **koa-static-cache**: Static file serving from memory.

'''js
app.use(middlewares.staticCache(path.join(__dirname, 'public'), {
  buffer: true,
  maxAge: 60 * 60 * 24 * 7,
  dir: path.join(rootdir, 'public')
}));
'''

* **koa-compress**: Compress middleware for Koa, support 'gzip' and 'deflate'
...
```



# <a name="apidoc.module.koa-middlewares.RedisStore"></a>[module koa-middlewares.RedisStore](#apidoc.module.koa-middlewares.RedisStore)

#### <a name="apidoc.element.koa-middlewares.RedisStore.RedisStore"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>RedisStore (options)](#apidoc.element.koa-middlewares.RedisStore.RedisStore)
- description and source-code
```javascript
RedisStore = function (options) {
  if (!(this instanceof RedisStore)) {
    return new RedisStore(options);
  }
  EventEmitter.call(this);
  options = options || {};

  var client;
  options.auth_pass = options.auth_pass || options.pass || null;     // For backwards compatibility
  options.path = options.path || options.socket || null;             // For backwards compatibility
  if (!options.client) {
    debug('Init redis new client');
    client = redis.createClient(options);
  } else {
    if (options.duplicate) {                                         // Duplicate client and update with options provided
      debug('Duplicating provided client with new options (if provided)');
      var dupClient = options.client;
      delete options.client;
      delete options.duplicate;
      client = dupClient.duplicate(options);                         // Useful if you want to use the DB option without adjusting
 the client DB outside koa-redis
    } else {
      debug('Using provided client');
      client = options.client;
    }
  }

  if (options.db) {
    debug('selecting db %s', options.db)
    client.select(options.db);
    client.on('connect', function() {
      client.send_anyways = true;
      client.select(options.db);
      client.send_anyways = false;
    });
  }

  client.on('error', this.emit.bind(this, 'error'));
  client.on('end', this.emit.bind(this, 'end'));
  client.on('end', this.emit.bind(this, 'disconnect'));              // For backwards compatibility
  client.on('connect', this.emit.bind(this, 'connect'));
  client.on('reconnecting', this.emit.bind(this, 'reconnecting'));
  client.on('ready', this.emit.bind(this, 'ready'));
  client.on('warning', this.emit.bind(this, 'warning'));
  this.on('connect', function() {
    debug('connected to redis');
    this.connected = client.connected;
  });
  this.on('ready', function() {
    debug('redis ready');
  });
  this.on('end', function() {
    debug('redis ended');
    this.connected = client.connected;
  });
  // No good way to test error
<span class="apidocCodeCommentSpan">  /* istanbul ignore next */
</span>  this.on('error', function() {
    debug('redis error');
    this.connected = client.connected;
  });
  // No good way to test reconnect
  /* istanbul ignore next */
  this.on('reconnecting', function() {
    debug('redis reconnecting');
    this.connected = client.connected;
  });
  // No good way to test warning
  /* istanbul ignore next */
  this.on('warning', function() {
    debug('redis warning');
    this.connected = client.connected;
  });

  //wrap redis
  this._redisClient = client;
  this.client = redisWrapper(client);
  this.connected = client.connected;
}
```
- example usage
```shell
...

* **koa-generic-session**: A session like connect with memory,
has friendly APIs for work with other Stores such as 'redis', 'mongo'.
* **koa-redis**: Work togather with 'koa-generic-session', provide a redis store from koa-sess.

'''js
app.use(middlewares.session({
store: middlewares.RedisStore(),
defer: true
}));

app.use(function *() {
var session = yield this.session;
session.foo = 'bar';
this.body = this.session.foo;
...
```

#### <a name="apidoc.element.koa-middlewares.RedisStore.super_"></a>[function <span class="apidocSignatureSpan">koa-middlewares.RedisStore.</span>super_ ()](#apidoc.element.koa-middlewares.RedisStore.super_)
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



# <a name="apidoc.module.koa-middlewares.RedisStore.prototype"></a>[module koa-middlewares.RedisStore.prototype](#apidoc.module.koa-middlewares.RedisStore.prototype)

#### <a name="apidoc.element.koa-middlewares.RedisStore.prototype.destroy"></a>[function <span class="apidocSignatureSpan">koa-middlewares.RedisStore.prototype.</span>destroy (sid)](#apidoc.element.koa-middlewares.RedisStore.prototype.destroy)
- description and source-code
```javascript
function* (sid) {
  debug('DEL %s', sid);
  yield this.client.del(sid);
  debug('DEL %s complete', sid);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.RedisStore.prototype.end"></a>[function <span class="apidocSignatureSpan">koa-middlewares.RedisStore.prototype.</span>end ()](#apidoc.element.koa-middlewares.RedisStore.prototype.end)
- description and source-code
```javascript
function* () {                         // End connection SAFELY
  debug('quitting redis client');
  yield this.client.quit();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.RedisStore.prototype.get"></a>[function <span class="apidocSignatureSpan">koa-middlewares.RedisStore.prototype.</span>get (sid)](#apidoc.element.koa-middlewares.RedisStore.prototype.get)
- description and source-code
```javascript
function* (sid) {
  var data = yield this.client.get(sid);
  debug('get session: %s', data || 'none');
  if (!data) {
    return null;
  }
  try {
    return JSON.parse(data.toString());
  } catch (err) {
    // ignore err
    debug('parse session error: %s', err.message);
  }
}
```
- example usage
```shell
...
});
'''

* **koa-router**: Provide express-style routing using app.get, app.put, app.post.

'''js
app.use(middlewares.router(app));
app.get('/', function *() {
  this.body = 'Hello koa-router';
});
'''

* **koa-resource-router**: RESTful resource routing for koa.

'''js
...
```

#### <a name="apidoc.element.koa-middlewares.RedisStore.prototype.quit"></a>[function <span class="apidocSignatureSpan">koa-middlewares.RedisStore.prototype.</span>quit ()](#apidoc.element.koa-middlewares.RedisStore.prototype.quit)
- description and source-code
```javascript
function* () {                         // End connection SAFELY
  debug('quitting redis client');
  yield this.client.quit();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.RedisStore.prototype.set"></a>[function <span class="apidocSignatureSpan">koa-middlewares.RedisStore.prototype.</span>set (sid, sess, ttl)](#apidoc.element.koa-middlewares.RedisStore.prototype.set)
- description and source-code
```javascript
function* (sid, sess, ttl) {
  if (typeof ttl === 'number') {
    ttl = Math.ceil(ttl / 1000);
  }
  sess = JSON.stringify(sess);
  if (ttl) {
    debug('SETEX %s %s %s', sid, ttl, sess);
    yield this.client.setex(sid, ttl, sess);
  } else {
    debug('SET %s %s', sid, sess);
    yield this.client.set(sid, sess);
  }
  debug('SET %s complete', sid);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.koa-middlewares.ResourceRouter"></a>[module koa-middlewares.ResourceRouter](#apidoc.module.koa-middlewares.ResourceRouter)

#### <a name="apidoc.element.koa-middlewares.ResourceRouter.ResourceRouter"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>ResourceRouter (name, actions, options)](#apidoc.element.koa-middlewares.ResourceRouter.ResourceRouter)
- description and source-code
```javascript
function Resource(name, actions, options) {
  if (!(this instanceof Resource)) {
    var args = Array.prototype.slice.call(arguments);
    var resource = Object.create(Resource.prototype);
    Resource.apply(resource, args);
    return resource;
  }
  options = options || {};
  this.name = typeof name == 'string' ? name : null;

  this.id = this.name ? pluralize.singular(name) : 'id';
  this.base = this.name ? '/' + this.name : '/';

  var middleware = Array.prototype.slice.call(arguments, this.name ? 1 : 0);

  this.actions = middleware.pop();

  // if last object has 'methods' property or 'id' property, assume it is 'options'
  if (this.actions.methods || this.actions.id) {
    options = this.actions;
    this.actions = middleware.pop();
  }

  this.routes = [];
  this.resources = [];

  this.options = {
    id: options.id,
    methods: defaults(options.methods || {}, {
      'options': 'OPTIONS',
      'new':     'GET',
      'create':  'POST',
      'edit':    'GET',
      'update':  'PUT',
      'index':   'GET',
      'list':    'GET',
      'read':    'GET',
      'show':    'GET',
      'destroy': 'DELETE',
      'remove':  'DELETE'
    })
  };

  // Set a custom id param name if one was provided.
  this.id = this.options.id || this.id;

  // create route definition (used for routing) for each resource action
  Object.keys(this.actions).forEach(function(name) {
    var action = this.actions[name];
    var url = this.base;
    var urlTrailing = this.base;
    var params = [];

    if (!this.options.methods[name]) return;

    if (url[url.length-1] != '/') {
      urlTrailing = url + '/';
    }

    if (name == 'new') {
      url = urlTrailing + 'new';
    }
    else if (name == 'edit') {
      url = urlTrailing + ':' + this.id + '/edit';
    }
    else if (name.match(/(show|read|update|remove|destroy)/)) {
      url = urlTrailing + ':' + this.id;
    }

    // compose multiple action middleware
    if (action instanceof Array) {
      this.actions[name] = compose(action);
    }

    // compose resource middleware
    if (middleware.length) {
      this.actions[name] = compose(middleware.concat(Array.isArray(action) ? action : [action]));
    }

    this.routes.push({
      method: this.options.methods[name].toUpperCase(),
      url: url,
      regexp: pathToRegExp(url, params),
      params: params,
      action: this.actions[name]
    });
  }, this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.koa-middlewares.ResourceRouter.prototype"></a>[module koa-middlewares.ResourceRouter.prototype](#apidoc.module.koa-middlewares.ResourceRouter.prototype)

#### <a name="apidoc.element.koa-middlewares.ResourceRouter.prototype.add"></a>[function <span class="apidocSignatureSpan">koa-middlewares.ResourceRouter.prototype.</span>add (resource)](#apidoc.element.koa-middlewares.ResourceRouter.prototype.add)
- description and source-code
```javascript
add = function (resource) {
  var base = this.base[this.base.length-1] == '/' ? this.base : this.base + '/';
  this.resources.push(resource);

  // Re-define base path for nested resource
  resource.base = resource.name ? '/' + resource.name : '/';
  resource.base = base + ':' + this.id + resource.base;

  // Re-define route paths for nested resource
  for (var len = resource.routes.length, i=0; i<len; i++) {
    var route = resource.routes[i];
    route.url = base + ':' + this.id + route.url;
    route.params = [];
    route.regexp = pathToRegExp(route.url, route.params);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.ResourceRouter.prototype.match"></a>[function <span class="apidocSignatureSpan">koa-middlewares.ResourceRouter.prototype.</span>match (path, params)](#apidoc.element.koa-middlewares.ResourceRouter.prototype.match)
- description and source-code
```javascript
match = function (path, params) {
  var matched = [];

  for (var len = this.routes.length, i=0; i<len; i++) {
    var route = this.routes[i];

    if (route.regexp.test(path)) {
      var captures = path.match(route.regexp);
      if (captures && captures.length) {
        captures = captures.slice(1);
      }

      if (params && route.params.length) {
        for (var l = captures.length, n=0; n<l; n++) {
          if (route.params[n]) {
            params[route.params[n].name] = captures[n];
          }
        }
      }

      matched.push(route);
    }
  }

  return matched.length ? matched : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.ResourceRouter.prototype.middleware"></a>[function <span class="apidocSignatureSpan">koa-middlewares.ResourceRouter.prototype.</span>middleware ()](#apidoc.element.koa-middlewares.ResourceRouter.prototype.middleware)
- description and source-code
```javascript
middleware = function () {
  var resource = this;

  return function *(next) {
    var matched;

    this.params = [];

    if (matched = resource.match(this.path, this.params)) {
      var allowedMethods = [];

      for (var len = matched.length, i=0; i<len; i++) {
        var route = matched[i];

        if (this.method == route.method) {
          if (this.params.user !== 'new' || route.url.match(/new$/i)) {
            return yield route.action.call(this, next);
          }
        }
        else {
          if (!~allowedMethods.indexOf(route.method)) {
            allowedMethods.push(route.method);
          }

        }
      }

      this.status = (this.method == 'OPTIONS' ? 204 : 405);
      this.set('Allow', allowedMethods.join(", "));
    }

    return yield next;
  };
}
```
- example usage
```shell
...
});
'''

* **koa-resource-router**: RESTful resource routing for koa.

'''js
var users = new middlewares.Resource('users');
app.use(users.middleware());

app.get('/users', function *() {
  this.body = [{name: 'Lee'}, {name: 'Han'}];
});
'''

* **koa-rewrite**: URL rewrite middleware.
...
```



# <a name="apidoc.module.koa-middlewares.csrf"></a>[module koa-middlewares.csrf](#apidoc.module.koa-middlewares.csrf)

#### <a name="apidoc.element.koa-middlewares.csrf.csrf"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>csrf (app, opts)](#apidoc.element.koa-middlewares.csrf.csrf)
- description and source-code
```javascript
csrf = function (app, opts) {
  if (isApp(app)) {
    opts = opts || {}
  } else {
    opts = app || {}
    app = null
  }

  var tokens = require('csrf')(opts)
  var middleware = opts.middleware || exports.middleware

  if (app) {
    define(app)
    return app
  }

  return function* csrf(next) {
    define(this)
    yield middleware.call(this, next)
  }

  function define(ctx) {
    var context = ctx.context || ctx
    var response = ctx.response
    var request = ctx.request

<span class="apidocCodeCommentSpan">    /*
     * Lazily creates a CSRF token.
     * Creates one per request.
     *
     * @api public
     */
</span>
    context.__defineGetter__('csrf', function () {
      if (this._csrf) return this._csrf
      if (!this.session) return null
      var secret = this.session.secret
        || (this.session.secret = tokens.secretSync())
      return this._csrf = tokens.create(secret)
    })

    response.__defineGetter__('csrf', function () {
      return this.ctx.csrf
    })

    /**
     * Asserts that a CSRF token exists and is valid.
     * Throws a 403 error otherwise.
     * var body = yield this.request.json()
     * try {
     *   this.assertCSRF(body)
     * } catch (err) {
     *   this.status = 403
     *   this.body = {
     *     message: 'invalid CSRF token'
     *   }
     * }
     *
     * @param {Object} body
     * @return {Context} this
     * @api public
     **/

    context.assertCSRF =
    context.assertCsrf = function (body) {
      // no session
      var secret = this.session.secret
      if (!secret) this.throw(403, 'secret is missing')

      var token = (body && body._csrf)
        || (!opts.disableQuery && this.query && this.query._csrf)
        || (this.get('x-csrf-token'))
        || (this.get('x-xsrf-token'))
        || body
      if (!token) this.throw(403, 'token is missing')
      if (!tokens.verify(secret, token)) this.throw(403, 'invalid csrf token')

      return this
    }

    request.assertCSRF =
    request.assertCsrf = function (body) {
      this.ctx.assertCsrf(body)
      return this
    }

  }
}
```
- example usage
```shell
...
var app = koa();

app.use(middlewares.bodyParser());
app.use(middlewares.router(app));
app.use(middlewares.conditional());
app.use(middlewares.etag());
app.use(middlewares.compress());
middlewares.csrf(app);

app.use(function *() {
  this.body = 'hello koa-middlewares';
});

app.listen(7001);
'''
...
```

#### <a name="apidoc.element.koa-middlewares.csrf.middleware"></a>[function <span class="apidocSignatureSpan">koa-middlewares.csrf.</span>middleware (next)](#apidoc.element.koa-middlewares.csrf.middleware)
- description and source-code
```javascript
function* (next) {
  // ignore get, head, options
  if (this.method === 'GET'
    || this.method === 'HEAD'
    || this.method === 'OPTIONS') {
    return yield next
  }

  // bodyparser middlewares maybe store body in request.body
  // or you can just set csrf token header
  this.assertCSRF(this.request.body)

  yield next
}
```
- example usage
```shell
...
});
'''

* **koa-resource-router**: RESTful resource routing for koa.

'''js
var users = new middlewares.Resource('users');
app.use(users.middleware());

app.get('/users', function *() {
  this.body = [{name: 'Lee'}, {name: 'Han'}];
});
'''

* **koa-rewrite**: URL rewrite middleware.
...
```



# <a name="apidoc.module.koa-middlewares.router"></a>[module koa-middlewares.router](#apidoc.module.koa-middlewares.router)

#### <a name="apidoc.element.koa-middlewares.router.router"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>router (opts)](#apidoc.element.koa-middlewares.router.router)
- description and source-code
```javascript
function Router(opts) {
  if (!(this instanceof Router)) {
    return new Router(opts);
  }

  this.opts = opts || {};
  this.methods = this.opts.methods || [
    'HEAD',
    'OPTIONS',
    'GET',
    'PUT',
    'PATCH',
    'POST',
    'DELETE'
  ];

  this.params = {};
  this.stack = [];
}
```
- example usage
```shell
...

var koa = require('koa');
var middlewares = require('koa-middlewares');

var app = koa();

app.use(middlewares.bodyParser());
app.use(middlewares.router(app));
app.use(middlewares.conditional());
app.use(middlewares.etag());
app.use(middlewares.compress());
middlewares.csrf(app);

app.use(function *() {
this.body = 'hello koa-middlewares';
...
```

#### <a name="apidoc.element.koa-middlewares.router.url"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.</span>url (path, params)](#apidoc.element.koa-middlewares.router.url)
- description and source-code
```javascript
url = function (path, params) {
    return Layer.prototype.url.call({path: path}, params);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.koa-middlewares.router.prototype"></a>[module koa-middlewares.router.prototype](#apidoc.module.koa-middlewares.router.prototype)

#### <a name="apidoc.element.koa-middlewares.router.prototype.acl"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>acl (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.acl)
- description and source-code
```javascript
acl = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.all"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>all (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.all)
- description and source-code
```javascript
all = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string') {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, methods, middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.allowedMethods"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>allowedMethods (options)](#apidoc.element.koa-middlewares.router.prototype.allowedMethods)
- description and source-code
```javascript
allowedMethods = function (options) {
  options = options || {};
  var implemented = this.methods;

  return function *allowedMethods(next) {
    yield *next;

    var allowed = {};

    if (!this.status || this.status === 404) {
      this.matched.forEach(function (route) {
        route.methods.forEach(function (method) {
          allowed[method] = method;
        });
      });

      var allowedArr = Object.keys(allowed);

      if (!~implemented.indexOf(this.method)) {
        if (options.throw) {
          var notImplementedThrowable;
          if (typeof options.notImplemented === 'function') {
            notImplementedThrowable = options.notImplemented(); // set whatever the user returns from their function
          } else {
            notImplementedThrowable = new HttpError.NotImplemented();
          }
          throw notImplementedThrowable;
        } else {
          this.status = 501;
          this.set('Allow', allowedArr);
        }
      } else if (allowedArr.length) {
        if (this.method === 'OPTIONS') {
          this.status = 204;
        } else if (!allowed[this.method]) {
          if (options.throw) {
            var notAllowedThrowable;
            if (typeof options.methodNotAllowed === 'function') {
              notAllowedThrowable = options.methodNotAllowed(); // set whatever the user returns from their function
            } else {
              notAllowedThrowable = new HttpError.MethodNotAllowed();
            }
            throw notAllowedThrowable;
          } else {
            this.status = 405;
          }
        }
        this.set('Allow', allowedArr);
      }
    }
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.bind"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>bind (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.bind)
- description and source-code
```javascript
bind = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.checkout"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>checkout (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.checkout)
- description and source-code
```javascript
checkout = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.connect"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>connect (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.connect)
- description and source-code
```javascript
connect = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.copy"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>copy (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.copy)
- description and source-code
```javascript
copy = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.del"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>del (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.del)
- description and source-code
```javascript
del = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.delete"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>delete (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.delete)
- description and source-code
```javascript
delete = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.get"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>get (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.get)
- description and source-code
```javascript
get = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
...
});
'''

* **koa-router**: Provide express-style routing using app.get, app.put, app.post.

'''js
app.use(middlewares.router(app));
app.get('/', function *() {
  this.body = 'Hello koa-router';
});
'''

* **koa-resource-router**: RESTful resource routing for koa.

'''js
...
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.head"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>head (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.head)
- description and source-code
```javascript
head = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.link"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>link (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.link)
- description and source-code
```javascript
link = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.lock"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>lock (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.lock)
- description and source-code
```javascript
lock = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.m-search"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>m-search (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.m-search)
- description and source-code
```javascript
m-search = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.match"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>match (path, method)](#apidoc.element.koa-middlewares.router.prototype.match)
- description and source-code
```javascript
match = function (path, method) {
  var layers = this.stack;
  var layer;
  var matched = {
    path: [],
    pathAndMethod: [],
    route: false
  };

  for (var len = layers.length, i = 0; i < len; i++) {
    layer = layers[i];

    debug('test %s %s', layer.path, layer.regexp);

    if (layer.match(path)) {
      matched.path.push(layer);

      if (layer.methods.length === 0 || ~layer.methods.indexOf(method)) {
        matched.pathAndMethod.push(layer);
        if (layer.methods.length) matched.route = true;
      }
    }
  }

  return matched;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.merge"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>merge (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.merge)
- description and source-code
```javascript
merge = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.middleware"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>middleware ()](#apidoc.element.koa-middlewares.router.prototype.middleware)
- description and source-code
```javascript
middleware = function () {
  var router = this;

  var dispatch = function *dispatch(next) {
    debug('%s %s', this.method, this.path);

    var path = router.opts.routerPath || this.routerPath || this.path;
    var matched = router.match(path, this.method);
    var layer, i, ii;

    if (this.matched) {
      this.matched.push.apply(this.matched, matched.path);
    } else {
      this.matched = matched.path;
    }

    if (matched.pathAndMethod.length) {
      i = matched.pathAndMethod.length;

      var mostSpecificPath = matched.pathAndMethod[matched.pathAndMethod.length - 1].path
      this._matchedRoute = mostSpecificPath

      while (matched.route && i--) {
        layer = matched.pathAndMethod[i];
        ii = layer.stack.length;
        this.captures = layer.captures(path, this.captures);
        this.params = layer.params(path, this.captures, this.params);
        debug('dispatch %s %s', layer.path, layer.regexp);

        while (ii--) {
          if (layer.stack[ii].constructor.name === 'GeneratorFunction') {
            next = layer.stack[ii].call(this, next);
          } else {
            next = Promise.resolve(layer.stack[ii].call(this, next));
          }
        }
      }
    }

    if (typeof next.next === 'function') {
      yield *next;
    } else {
      yield next;
    }
  };

  dispatch.router = this;

  return dispatch;
}
```
- example usage
```shell
...
});
'''

* **koa-resource-router**: RESTful resource routing for koa.

'''js
var users = new middlewares.Resource('users');
app.use(users.middleware());

app.get('/users', function *() {
  this.body = [{name: 'Lee'}, {name: 'Han'}];
});
'''

* **koa-rewrite**: URL rewrite middleware.
...
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.mkactivity"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>mkactivity (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.mkactivity)
- description and source-code
```javascript
mkactivity = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.mkcalendar"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>mkcalendar (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.mkcalendar)
- description and source-code
```javascript
mkcalendar = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.mkcol"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>mkcol (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.mkcol)
- description and source-code
```javascript
mkcol = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.move"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>move (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.move)
- description and source-code
```javascript
move = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.notify"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>notify (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.notify)
- description and source-code
```javascript
notify = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.options"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>options (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.options)
- description and source-code
```javascript
options = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.param"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>param (param, middleware)](#apidoc.element.koa-middlewares.router.prototype.param)
- description and source-code
```javascript
param = function (param, middleware) {
  this.params[param] = middleware;
  this.stack.forEach(function (route) {
    route.param(param, middleware);
  });
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.patch"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>patch (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.patch)
- description and source-code
```javascript
patch = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.post"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>post (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.post)
- description and source-code
```javascript
post = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.prefix"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>prefix (prefix)](#apidoc.element.koa-middlewares.router.prototype.prefix)
- description and source-code
```javascript
prefix = function (prefix) {
  this.opts.prefix = prefix;

  this.stack.forEach(function (route) {
    route.setPrefix(prefix);
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.propfind"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>propfind (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.propfind)
- description and source-code
```javascript
propfind = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.proppatch"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>proppatch (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.proppatch)
- description and source-code
```javascript
proppatch = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.purge"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>purge (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.purge)
- description and source-code
```javascript
purge = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.put"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>put (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.put)
- description and source-code
```javascript
put = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.rebind"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>rebind (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.rebind)
- description and source-code
```javascript
rebind = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.redirect"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>redirect (source, destination, code)](#apidoc.element.koa-middlewares.router.prototype.redirect)
- description and source-code
```javascript
redirect = function (source, destination, code) {
  // lookup source route by name
  if (source[0] !== '/') {
    source = this.url(source);
  }

  // lookup destination route by name
  if (destination[0] !== '/') {
    destination = this.url(destination);
  }

  return this.all(source, function *() {
    this.redirect(destination);
    this.status = code || 301;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.register"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>register (path, methods, middleware, opts)](#apidoc.element.koa-middlewares.router.prototype.register)
- description and source-code
```javascript
register = function (path, methods, middleware, opts) {
  opts = opts || {};

  var stack = this.stack;

  // create route
  var route = new Layer(path, methods, middleware, {
    end: opts.end === false ? opts.end : true,
    name: opts.name,
    sensitive: opts.sensitive || this.opts.sensitive || false,
    strict: opts.strict || this.opts.strict || false,
    prefix: opts.prefix || this.opts.prefix || "",
    ignoreCaptures: opts.ignoreCaptures
  });

  if (this.opts.prefix) {
    route.setPrefix(this.opts.prefix);
  }

  // add parameter middleware
  Object.keys(this.params).forEach(function (param) {
    route.param(param, this.params[param]);
  }, this);

  // register route with router
  if (methods.length || !stack.length) {
    // if we don't have parameters, put before any with same route
    // nesting level but with parameters
    var added = false;

    if (!route.paramNames.length) {
      var routeNestingLevel = route.path.toString().split('/').length;

      added = stack.some(function (m, i) {
        var mNestingLevel = m.path.toString().split('/').length;
        var isParamRoute = !!m.paramNames.length;
        if (routeNestingLevel === mNestingLevel && isParamRoute) {
          return stack.splice(i, 0, route);
        }
      });
    }

    if (!added) stack.push(route);
  } else {
    stack.some(function (m, i) {
      if (!m.methods.length && i === stack.length - 1) {
        return stack.push(route);
      } else if (m.methods.length) {
        if (stack[i - 1]) {
          return stack.splice(i, 0, route);
        } else {
          return stack.unshift(route);
        }
      }
    });
  }

  return route;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.report"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>report (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.report)
- description and source-code
```javascript
report = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.route"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>route (name)](#apidoc.element.koa-middlewares.router.prototype.route)
- description and source-code
```javascript
route = function (name) {
  var routes = this.stack;

  for (var len = routes.length, i=0; i<len; i++) {
    if (routes[i].name && routes[i].name === name) {
      return routes[i];
    }
  }

  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.routes"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>routes ()](#apidoc.element.koa-middlewares.router.prototype.routes)
- description and source-code
```javascript
routes = function () {
  var router = this;

  var dispatch = function *dispatch(next) {
    debug('%s %s', this.method, this.path);

    var path = router.opts.routerPath || this.routerPath || this.path;
    var matched = router.match(path, this.method);
    var layer, i, ii;

    if (this.matched) {
      this.matched.push.apply(this.matched, matched.path);
    } else {
      this.matched = matched.path;
    }

    if (matched.pathAndMethod.length) {
      i = matched.pathAndMethod.length;

      var mostSpecificPath = matched.pathAndMethod[matched.pathAndMethod.length - 1].path
      this._matchedRoute = mostSpecificPath

      while (matched.route && i--) {
        layer = matched.pathAndMethod[i];
        ii = layer.stack.length;
        this.captures = layer.captures(path, this.captures);
        this.params = layer.params(path, this.captures, this.params);
        debug('dispatch %s %s', layer.path, layer.regexp);

        while (ii--) {
          if (layer.stack[ii].constructor.name === 'GeneratorFunction') {
            next = layer.stack[ii].call(this, next);
          } else {
            next = Promise.resolve(layer.stack[ii].call(this, next));
          }
        }
      }
    }

    if (typeof next.next === 'function') {
      yield *next;
    } else {
      yield next;
    }
  };

  dispatch.router = this;

  return dispatch;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.search"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>search (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.search)
- description and source-code
```javascript
search = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.subscribe"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>subscribe (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.subscribe)
- description and source-code
```javascript
subscribe = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.trace"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>trace (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.trace)
- description and source-code
```javascript
trace = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.unbind"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>unbind (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.unbind)
- description and source-code
```javascript
unbind = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.unlink"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>unlink (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.unlink)
- description and source-code
```javascript
unlink = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.unlock"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>unlock (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.unlock)
- description and source-code
```javascript
unlock = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.unsubscribe"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>unsubscribe (name, path, middleware)](#apidoc.element.koa-middlewares.router.prototype.unsubscribe)
- description and source-code
```javascript
unsubscribe = function (name, path, middleware) {
  var middleware;

  if (typeof path === 'string' || path instanceof RegExp) {
    middleware = Array.prototype.slice.call(arguments, 2);
  } else {
    middleware = Array.prototype.slice.call(arguments, 1);
    path = name;
    name = null;
  }

  this.register(path, [method], middleware, {
    name: name
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.url"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>url (name, params)](#apidoc.element.koa-middlewares.router.prototype.url)
- description and source-code
```javascript
url = function (name, params) {
  var route = this.route(name);

  if (route) {
    var args = Array.prototype.slice.call(arguments, 1);
    return route.url.apply(route, args);
  }

  return new Error("No route found for name: " + name);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.router.prototype.use"></a>[function <span class="apidocSignatureSpan">koa-middlewares.router.prototype.</span>use ()](#apidoc.element.koa-middlewares.router.prototype.use)
- description and source-code
```javascript
use = function () {
  var router = this;
  var middleware = Array.prototype.slice.call(arguments);
  var path;

  // support array of paths
  if (Array.isArray(middleware[0]) && typeof middleware[0][0] === 'string') {
    middleware[0].forEach(function (p) {
      router.use.apply(router, [p].concat(middleware.slice(1)));
    });

    return this;
  }

  if (typeof middleware[0] === 'string') {
    path = middleware.shift();
  }

  // filter out nested routers from filter
  middleware = middleware.filter(function (fn) {
    if (fn.router) {
      fn.router.stack.forEach(function (layer) {
        if (path) layer.setPrefix(path);
        if (router.opts.prefix) layer.setPrefix(router.opts.prefix);
        router.stack.push(layer);
      });

      if (router.params) {
        Object.keys(router.params).forEach(function (key) {
          fn.router.param(key, router.params[key]);
        });
      }

      return false;
    }

    return true;
  });

  if (middleware.length) {
    router.register(path || '(.*)', [], middleware, {
      end: false,
      ignoreCaptures: !path
    });
  }

  return this;
}
```
- example usage
```shell
...
'''js

var koa = require('koa');
var middlewares = require('koa-middlewares');

var app = koa();

app.use(middlewares.bodyParser());
app.use(middlewares.router(app));
app.use(middlewares.conditional());
app.use(middlewares.etag());
app.use(middlewares.compress());
middlewares.csrf(app);

app.use(function *() {
...
```



# <a name="apidoc.module.koa-middlewares.session"></a>[module koa-middlewares.session](#apidoc.module.koa-middlewares.session)

#### <a name="apidoc.element.koa-middlewares.session.session"></a>[function <span class="apidocSignatureSpan">koa-middlewares.</span>session (options)](#apidoc.element.koa-middlewares.session.session)
- description and source-code
```javascript
session = function (options) {
  options = options || {};
  let key = options.key || 'koa.sid';
  let client = options.store || new MemoryStore();
  let errorHandler = options.errorHandler || defaultErrorHanlder;
  let reconnectTimeout = options.reconnectTimeout || 10000;

  let store = new Store(client, {
    ttl: options.ttl,
    prefix: options.prefix
  });

  let genSid = options.genSid || uid.sync;
  let valid = options.valid || noop;
  let beforeSave = options.beforeSave || noop;

  let cookie = options.cookie || {};
  copy(defaultCookie).to(cookie);

  let storeStatus = 'available';
  let waitStore = Promise.resolve();

  // notify user that this store is not
  // meant for a production environment
  if ('production' === process.env.NODE_ENV
   && client instanceof MemoryStore) console.warn(warning);

  let sessionIdStore = options.sessionIdStore || {

    get: function() {
      return this.cookies.get(key, cookie);
    },

    set: function(sid, session) {
      this.cookies.set(key, sid, session.cookie);
    },

    reset: function() {
      this.cookies.set(key, null);
    }
  };

  store.on('disconnect', function() {
    if (storeStatus !== 'available') return;
    storeStatus = 'pending';
    waitStore = new Promise(function (resolve, reject) {
      setTimeout(function () {
        if (storeStatus === 'pending') storeStatus = 'unavailable';
        reject(new Error('session store is unavailable'));
      }, reconnectTimeout);
      store.once('connect', resolve);
    });

  });

  store.on('connect', function() {
    storeStatus = 'available';
    waitStore = Promise.resolve();
  });

  // save empty session hash for compare
  const EMPTY_SESSION_HASH = hash(generateSession());

  return options.defer ? deferSession : session;

  function addCommonAPI() {

    this._sessionSave = null;

    // more flexible
    this.__defineGetter__('sessionSave', function () {
      return this._sessionSave;
    });

    this.__defineSetter__('sessionSave', function (save) {
      this._sessionSave = save;
    });
  }

<span class="apidocCodeCommentSpan">  /**
   * generate a new session
   */
</span>  function generateSession() {
    let session = {};
    //you can alter the cookie options in nexts
    session.cookie = {};
    for (let prop in cookie) {
      session.cookie[prop] = cookie[prop];
    }
    compatMaxage(session.cookie);
    return session;
  }

  /**
   * check url match cookie's path
   */
  function matchPath(ctx) {
    let pathname = parse(ctx).pathname;
    let cookiePath = cookie.path || '/';
    if (cookiePath === '/') {
      return true;
    }
    if (pathname.indexOf(cookiePath) !== 0) {
      debug('cookie path not match');
      return false;
    }
    return true;
  }

  /**
   * get session from store
   *   get sessionId from cookie
   *   save sessionId into context
   *   get session from store
   */
  function *getSession() {
    if (!matchPath(this)) return;
    if (storeStatus === 'pending') {
      debug('store is disconnect and pending');
      yield waitStore;
    } else if (storeStatus === 'unavailable') {
      debug('store is unavailable');
      throw new Error('session store is unavailable');
    }

    if (!this.sessionId) {
      this.sessionId = sessionIdStore.get.call(this);
    }

    let session;
    let isNew = false;
    if (!this.sessionId) {
      debug('session id not exist, generate a new one');
      session = generateSession();
      this.sessionId = genSid.call(this, 24);
      isNew = true;
    } else {
      try {
        session = yield store.get(this.sessionId);
        debug('get session %j with key %s', session, this.sessionId);
      } catch (err) {
        if (err.code === 'ENOENT') {
          debug('get session error, code = ENOENT');
        } else {
          debug('get session error: ', err.message);
          errorHandler(err, 'get', this);
        }
      }
    }

    // make sure the session is still valid
    if (!session ||
      !valid(this, session)) {
      debug('session is empty or invalid');
      session = generateSession();
      this.sessionId = genSid.call(this, 24);
      sessionIdStore.re ...
```
- example usage
```shell
...
'''

* **koa-generic-session**: A session like connect with memory,
has friendly APIs for work with other Stores such as 'redis', 'mongo'.
* **koa-redis**: Work togather with 'koa-generic-session', provide a redis store from koa-sess.

'''js
app.use(middlewares.session({
store: middlewares.RedisStore(),
defer: true
}));

app.use(function *() {
var session = yield this.session;
session.foo = 'bar';
...
```

#### <a name="apidoc.element.koa-middlewares.session.MemoryStore"></a>[function <span class="apidocSignatureSpan">koa-middlewares.session.</span>MemoryStore ()](#apidoc.element.koa-middlewares.session.MemoryStore)
- description and source-code
```javascript
MemoryStore = function () {
  this.sessions = {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.koa-middlewares.session.MemoryStore"></a>[module koa-middlewares.session.MemoryStore](#apidoc.module.koa-middlewares.session.MemoryStore)

#### <a name="apidoc.element.koa-middlewares.session.MemoryStore.MemoryStore"></a>[function <span class="apidocSignatureSpan">koa-middlewares.session.</span>MemoryStore ()](#apidoc.element.koa-middlewares.session.MemoryStore.MemoryStore)
- description and source-code
```javascript
MemoryStore = function () {
  this.sessions = {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.koa-middlewares.session.MemoryStore.prototype"></a>[module koa-middlewares.session.MemoryStore.prototype](#apidoc.module.koa-middlewares.session.MemoryStore.prototype)

#### <a name="apidoc.element.koa-middlewares.session.MemoryStore.prototype.destroy"></a>[function <span class="apidocSignatureSpan">koa-middlewares.session.MemoryStore.prototype.</span>destroy (sid)](#apidoc.element.koa-middlewares.session.MemoryStore.prototype.destroy)
- description and source-code
```javascript
function* (sid) {
  delete this.sessions[sid];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-middlewares.session.MemoryStore.prototype.get"></a>[function <span class="apidocSignatureSpan">koa-middlewares.session.MemoryStore.prototype.</span>get (sid)](#apidoc.element.koa-middlewares.session.MemoryStore.prototype.get)
- description and source-code
```javascript
function* (sid) {
  debug('get value %j with key %s', this.sessions[sid], sid);
  return this.sessions[sid];
}
```
- example usage
```shell
...
});
'''

* **koa-router**: Provide express-style routing using app.get, app.put, app.post.

'''js
app.use(middlewares.router(app));
app.get('/', function *() {
  this.body = 'Hello koa-router';
});
'''

* **koa-resource-router**: RESTful resource routing for koa.

'''js
...
```

#### <a name="apidoc.element.koa-middlewares.session.MemoryStore.prototype.set"></a>[function <span class="apidocSignatureSpan">koa-middlewares.session.MemoryStore.prototype.</span>set (sid, val)](#apidoc.element.koa-middlewares.session.MemoryStore.prototype.set)
- description and source-code
```javascript
function* (sid, val) {
  debug('set value %j for key %s', val, sid);
  this.sessions[sid] = val;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
