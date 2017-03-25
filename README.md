# api documentation for  [hapi (v16.1.0)](http://hapijs.com)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-hapi.svg)](https://travis-ci.org/npmdoc/node-npmdoc-hapi)
#### HTTP Server framework

[![NPM](https://nodei.co/npm/hapi.png?downloads=true)](https://www.npmjs.com/package/hapi)

[![apidoc](https://npmdoc.github.io/node-npmdoc-hapi/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-hapi_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-hapi/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-hapi/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/hapijs/hapi/issues"
    },
    "dependencies": {
        "accept": "2.x.x",
        "ammo": "2.x.x",
        "boom": "4.x.x",
        "call": "4.x.x",
        "catbox": "7.x.x",
        "catbox-memory": "2.x.x",
        "cryptiles": "3.x.x",
        "heavy": "4.x.x",
        "hoek": "4.x.x",
        "iron": "4.x.x",
        "items": "2.x.x",
        "joi": "10.x.x",
        "mimos": "3.x.x",
        "podium": "^1.2.x",
        "shot": "3.x.x",
        "statehood": "5.x.x",
        "subtext": "^4.3.x",
        "topo": "2.x.x"
    },
    "description": "HTTP Server framework",
    "devDependencies": {
        "code": "4.x.x",
        "handlebars": "4.x.x",
        "inert": "4.x.x",
        "lab": "11.x.x",
        "vision": "4.x.x",
        "wreck": "10.x.x"
    },
    "directories": {},
    "dist": {
        "shasum": "419dd86347588821eb5a0a5f493bce019802d33b",
        "tarball": "https://registry.npmjs.org/hapi/-/hapi-16.1.0.tgz"
    },
    "engines": {
        "node": ">=4.5.0"
    },
    "gitHead": "4ecf32856fa5eb3d1420007ec0c90e26636b8b7d",
    "homepage": "http://hapijs.com",
    "keywords": [
        "framework",
        "http",
        "api",
        "web"
    ],
    "license": "BSD-3-Clause",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "hueniverse",
            "email": "eran@hueniverse.com"
        }
    ],
    "name": "hapi",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/hapijs/hapi.git"
    },
    "scripts": {
        "test": "lab -a code -t 100 -L -m 3000",
        "test-cov-html": "lab -a code -r html -o coverage.html -m 3000",
        "test-tap": "lab -a code -r tap -o tests.tap -m 3000"
    },
    "version": "16.1.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module hapi](#apidoc.module.hapi)
1.  [function <span class="apidocSignatureSpan">hapi.</span>Server (options)](#apidoc.element.hapi.Server)
1.  [function <span class="apidocSignatureSpan">hapi.</span>Server.super_ (server, connections, env, parent)](#apidoc.element.hapi.Server.super_)
1.  [function <span class="apidocSignatureSpan">hapi.</span>auth (connection)](#apidoc.element.hapi.auth)
1.  [function <span class="apidocSignatureSpan">hapi.</span>compression ()](#apidoc.element.hapi.compression)
1.  [function <span class="apidocSignatureSpan">hapi.</span>connection (server, options)](#apidoc.element.hapi.connection)
1.  [function <span class="apidocSignatureSpan">hapi.</span>ext (type, server)](#apidoc.element.hapi.ext)
1.  [function <span class="apidocSignatureSpan">hapi.</span>methods (server)](#apidoc.element.hapi.methods)
1.  [function <span class="apidocSignatureSpan">hapi.</span>protect (request)](#apidoc.element.hapi.protect)
1.  [function <span class="apidocSignatureSpan">hapi.</span>reply ()](#apidoc.element.hapi.reply)
1.  [function <span class="apidocSignatureSpan">hapi.</span>request ()](#apidoc.element.hapi.request)
1.  [function <span class="apidocSignatureSpan">hapi.</span>response (source, request, options)](#apidoc.element.hapi.response)
1.  [function <span class="apidocSignatureSpan">hapi.</span>route (route, connection, plugin, options)](#apidoc.element.hapi.route)
1.  object <span class="apidocSignatureSpan">hapi.</span>Server.prototype
1.  object <span class="apidocSignatureSpan">hapi.</span>Server.super_.prototype
1.  object <span class="apidocSignatureSpan">hapi.</span>Server.super_.super_.prototype
1.  object <span class="apidocSignatureSpan">hapi.</span>auth.prototype
1.  object <span class="apidocSignatureSpan">hapi.</span>compression.prototype
1.  object <span class="apidocSignatureSpan">hapi.</span>connection.prototype
1.  object <span class="apidocSignatureSpan">hapi.</span>cors
1.  object <span class="apidocSignatureSpan">hapi.</span>ext.prototype
1.  object <span class="apidocSignatureSpan">hapi.</span>handler
1.  object <span class="apidocSignatureSpan">hapi.</span>methods.prototype
1.  object <span class="apidocSignatureSpan">hapi.</span>promises
1.  object <span class="apidocSignatureSpan">hapi.</span>protect.prototype
1.  object <span class="apidocSignatureSpan">hapi.</span>reply.prototype
1.  object <span class="apidocSignatureSpan">hapi.</span>request.prototype
1.  object <span class="apidocSignatureSpan">hapi.</span>response.prototype
1.  object <span class="apidocSignatureSpan">hapi.</span>route.prototype
1.  object <span class="apidocSignatureSpan">hapi.</span>schema
1.  object <span class="apidocSignatureSpan">hapi.</span>transmit
1.  object <span class="apidocSignatureSpan">hapi.</span>validation

#### [module hapi.Server](#apidoc.module.hapi.Server)
1.  [function <span class="apidocSignatureSpan">hapi.</span>Server (options)](#apidoc.element.hapi.Server.Server)
1.  [function <span class="apidocSignatureSpan">hapi.Server.</span>super_ (server, connections, env, parent)](#apidoc.element.hapi.Server.super_)

#### [module hapi.Server.prototype](#apidoc.module.hapi.Server.prototype)
1.  [function <span class="apidocSignatureSpan">hapi.Server.prototype.</span>_createCache (options, _callback)](#apidoc.element.hapi.Server.prototype._createCache)
1.  [function <span class="apidocSignatureSpan">hapi.Server.prototype.</span>_invoke (type, next)](#apidoc.element.hapi.Server.prototype._invoke)
1.  [function <span class="apidocSignatureSpan">hapi.Server.prototype.</span>_start (callback)](#apidoc.element.hapi.Server.prototype._start)
1.  [function <span class="apidocSignatureSpan">hapi.Server.prototype.</span>_validateDeps ()](#apidoc.element.hapi.Server.prototype._validateDeps)
1.  [function <span class="apidocSignatureSpan">hapi.Server.prototype.</span>connection (options)](#apidoc.element.hapi.Server.prototype.connection)
1.  [function <span class="apidocSignatureSpan">hapi.Server.prototype.</span>initialize (callback)](#apidoc.element.hapi.Server.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">hapi.Server.prototype.</span>start (callback)](#apidoc.element.hapi.Server.prototype.start)
1.  [function <span class="apidocSignatureSpan">hapi.Server.prototype.</span>stop ()](#apidoc.element.hapi.Server.prototype.stop)

#### [module hapi.Server.super_](#apidoc.module.hapi.Server.super_)
1.  [function <span class="apidocSignatureSpan">hapi.Server.</span>super_ (events)](#apidoc.element.hapi.Server.super_.super_)

#### [module hapi.Server.super_.prototype](#apidoc.module.hapi.Server.super_.prototype)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>_apply (type, func, args)](#apidoc.element.hapi.Server.super_.prototype._apply)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>_applyChild (type, child, func, args)](#apidoc.element.hapi.Server.super_.prototype._applyChild)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>_clone (connections, plugin)](#apidoc.element.hapi.Server.super_.prototype._clone)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>_ext (event)](#apidoc.element.hapi.Server.super_.prototype._ext)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>_log (tags, data)](#apidoc.element.hapi.Server.super_.prototype._log)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>_select (labels, plugin)](#apidoc.element.hapi.Server.super_.prototype._select)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>_single ()](#apidoc.element.hapi.Server.super_.prototype._single)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>bind (context)](#apidoc.element.hapi.Server.super_.prototype.bind)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>cache (options, _segment)](#apidoc.element.hapi.Server.super_.prototype.cache)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>decoder (encoding, decoder)](#apidoc.element.hapi.Server.super_.prototype.decoder)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>decorate (type, property, method, options)](#apidoc.element.hapi.Server.super_.prototype.decorate)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>dependency (dependencies, after)](#apidoc.element.hapi.Server.super_.prototype.dependency)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>emit (criteria, data, callback)](#apidoc.element.hapi.Server.super_.prototype.emit)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>encoder (encoding, encoder)](#apidoc.element.hapi.Server.super_.prototype.encoder)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>event (event)](#apidoc.element.hapi.Server.super_.prototype.event)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>expose (key, value)](#apidoc.element.hapi.Server.super_.prototype.expose)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>ext (events)](#apidoc.element.hapi.Server.super_.prototype.ext)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>handler (name, method)](#apidoc.element.hapi.Server.super_.prototype.handler)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>inject (options, callback)](#apidoc.element.hapi.Server.super_.prototype.inject)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>log (tags, data, timestamp, _internal)](#apidoc.element.hapi.Server.super_.prototype.log)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>lookup (id)](#apidoc.element.hapi.Server.super_.prototype.lookup)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>match (method, path, host)](#apidoc.element.hapi.Server.super_.prototype.match)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>method (name, method, options)](#apidoc.element.hapi.Server.super_.prototype.method)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>path (relativeTo)](#apidoc.element.hapi.Server.super_.prototype.path)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>register (plugins)](#apidoc.element.hapi.Server.super_.prototype.register)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>route (options)](#apidoc.element.hapi.Server.super_.prototype.route)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>select ()](#apidoc.element.hapi.Server.super_.prototype.select)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>state (name, options)](#apidoc.element.hapi.Server.super_.prototype.state)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>table (host)](#apidoc.element.hapi.Server.super_.prototype.table)

#### [module hapi.Server.super_.super_.prototype](#apidoc.module.hapi.Server.super_.super_.prototype)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>_emit (criteria, data, generated, callback)](#apidoc.element.hapi.Server.super_.super_.prototype._emit)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>addListener (criteria, listener)](#apidoc.element.hapi.Server.super_.super_.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>emit (criteria, data, callback)](#apidoc.element.hapi.Server.super_.super_.prototype.emit)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>hasListeners (name)](#apidoc.element.hapi.Server.super_.super_.prototype.hasListeners)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>on (criteria, listener)](#apidoc.element.hapi.Server.super_.super_.prototype.on)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>once (criteria, listener)](#apidoc.element.hapi.Server.super_.super_.prototype.once)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>registerEvent (events)](#apidoc.element.hapi.Server.super_.super_.prototype.registerEvent)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>registerPodium (podiums)](#apidoc.element.hapi.Server.super_.super_.prototype.registerPodium)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>removeAllListeners (name)](#apidoc.element.hapi.Server.super_.super_.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>removeListener (name, listener)](#apidoc.element.hapi.Server.super_.super_.prototype.removeListener)

#### [module hapi.auth](#apidoc.module.hapi.auth)
1.  [function <span class="apidocSignatureSpan">hapi.</span>auth (connection)](#apidoc.element.hapi.auth.auth)
1.  [function <span class="apidocSignatureSpan">hapi.auth.</span>access (request, route)](#apidoc.element.hapi.auth.access)
1.  [function <span class="apidocSignatureSpan">hapi.auth.</span>authenticate (request, next)](#apidoc.element.hapi.auth.authenticate)
1.  [function <span class="apidocSignatureSpan">hapi.auth.</span>payload (request, next)](#apidoc.element.hapi.auth.payload)
1.  [function <span class="apidocSignatureSpan">hapi.auth.</span>response (request, next)](#apidoc.element.hapi.auth.response)

#### [module hapi.auth.prototype](#apidoc.module.hapi.auth.prototype)
1.  [function <span class="apidocSignatureSpan">hapi.auth.prototype.</span>_authenticate (request, next)](#apidoc.element.hapi.auth.prototype._authenticate)
1.  [function <span class="apidocSignatureSpan">hapi.auth.prototype.</span>_setupRoute (options, path)](#apidoc.element.hapi.auth.prototype._setupRoute)
1.  [function <span class="apidocSignatureSpan">hapi.auth.prototype.</span>default (options)](#apidoc.element.hapi.auth.prototype.default)
1.  [function <span class="apidocSignatureSpan">hapi.auth.prototype.</span>lookup (route)](#apidoc.element.hapi.auth.prototype.lookup)
1.  [function <span class="apidocSignatureSpan">hapi.auth.prototype.</span>scheme (name, scheme)](#apidoc.element.hapi.auth.prototype.scheme)
1.  [function <span class="apidocSignatureSpan">hapi.auth.prototype.</span>strategy (name, scheme)](#apidoc.element.hapi.auth.prototype.strategy)
1.  [function <span class="apidocSignatureSpan">hapi.auth.prototype.</span>test (name, request, next)](#apidoc.element.hapi.auth.prototype.test)

#### [module hapi.compression](#apidoc.module.hapi.compression)
1.  [function <span class="apidocSignatureSpan">hapi.</span>compression ()](#apidoc.element.hapi.compression.compression)

#### [module hapi.compression.prototype](#apidoc.module.hapi.compression.prototype)
1.  [function <span class="apidocSignatureSpan">hapi.compression.prototype.</span>accept (request)](#apidoc.element.hapi.compression.prototype.accept)
1.  [function <span class="apidocSignatureSpan">hapi.compression.prototype.</span>addDecoder (encoding, decoder)](#apidoc.element.hapi.compression.prototype.addDecoder)
1.  [function <span class="apidocSignatureSpan">hapi.compression.prototype.</span>addEncoder (encoding, encoder)](#apidoc.element.hapi.compression.prototype.addEncoder)
1.  [function <span class="apidocSignatureSpan">hapi.compression.prototype.</span>encoder (request, encoding)](#apidoc.element.hapi.compression.prototype.encoder)
1.  [function <span class="apidocSignatureSpan">hapi.compression.prototype.</span>encoding (response)](#apidoc.element.hapi.compression.prototype.encoding)

#### [module hapi.connection](#apidoc.module.hapi.connection)
1.  [function <span class="apidocSignatureSpan">hapi.</span>connection (server, options)](#apidoc.element.hapi.connection.connection)
1.  [function <span class="apidocSignatureSpan">hapi.connection.</span>super_ (events)](#apidoc.element.hapi.connection.super_)
1.  object <span class="apidocSignatureSpan">hapi.connection.</span>_events

#### [module hapi.connection.prototype](#apidoc.module.hapi.connection.prototype)
1.  [function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>_addRoute (config, plugin)](#apidoc.element.hapi.connection.prototype._addRoute)
1.  [function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>_defaultRoutes ()](#apidoc.element.hapi.connection.prototype._defaultRoutes)
1.  [function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>_dispatch (options)](#apidoc.element.hapi.connection.prototype._dispatch)
1.  [function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>_ext (event)](#apidoc.element.hapi.connection.prototype._ext)
1.  [function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>_init ()](#apidoc.element.hapi.connection.prototype._init)
1.  [function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>_route (configs, plugin)](#apidoc.element.hapi.connection.prototype._route)
1.  [function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>_start (callback)](#apidoc.element.hapi.connection.prototype._start)
1.  [function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>_stop (options, callback)](#apidoc.element.hapi.connection.prototype._stop)
1.  [function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>decoder (encoding, decoder)](#apidoc.element.hapi.connection.prototype.decoder)
1.  [function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>encoder (encoding, encoder)](#apidoc.element.hapi.connection.prototype.encoder)
1.  [function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>inject (options, callback)](#apidoc.element.hapi.connection.prototype.inject)
1.  [function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>lookup (id)](#apidoc.element.hapi.connection.prototype.lookup)
1.  [function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>match (method, path, host)](#apidoc.element.hapi.connection.prototype.match)
1.  [function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>table (host)](#apidoc.element.hapi.connection.prototype.table)

#### [module hapi.cors](#apidoc.module.hapi.cors)
1.  [function <span class="apidocSignatureSpan">hapi.cors.</span>handler (connection)](#apidoc.element.hapi.cors.handler)
1.  [function <span class="apidocSignatureSpan">hapi.cors.</span>headers (response)](#apidoc.element.hapi.cors.headers)
1.  [function <span class="apidocSignatureSpan">hapi.cors.</span>matchOrigin (origin, settings)](#apidoc.element.hapi.cors.matchOrigin)
1.  [function <span class="apidocSignatureSpan">hapi.cors.</span>options (route, connection, server)](#apidoc.element.hapi.cors.options)
1.  [function <span class="apidocSignatureSpan">hapi.cors.</span>route (options)](#apidoc.element.hapi.cors.route)

#### [module hapi.ext](#apidoc.module.hapi.ext)
1.  [function <span class="apidocSignatureSpan">hapi.</span>ext (type, server)](#apidoc.element.hapi.ext.ext)

#### [module hapi.ext.prototype](#apidoc.module.hapi.ext.prototype)
1.  [function <span class="apidocSignatureSpan">hapi.ext.prototype.</span>add (event)](#apidoc.element.hapi.ext.prototype.add)
1.  [function <span class="apidocSignatureSpan">hapi.ext.prototype.</span>merge (others)](#apidoc.element.hapi.ext.prototype.merge)
1.  [function <span class="apidocSignatureSpan">hapi.ext.prototype.</span>subscribe (route)](#apidoc.element.hapi.ext.prototype.subscribe)

#### [module hapi.handler](#apidoc.module.hapi.handler)
1.  [function <span class="apidocSignatureSpan">hapi.handler.</span>configure (handler, route)](#apidoc.element.hapi.handler.configure)
1.  [function <span class="apidocSignatureSpan">hapi.handler.</span>defaults (method, handler, server)](#apidoc.element.hapi.handler.defaults)
1.  [function <span class="apidocSignatureSpan">hapi.handler.</span>execute (request, next)](#apidoc.element.hapi.handler.execute)
1.  [function <span class="apidocSignatureSpan">hapi.handler.</span>prerequisitesConfig (config, server)](#apidoc.element.hapi.handler.prerequisitesConfig)

#### [module hapi.methods](#apidoc.module.hapi.methods)
1.  [function <span class="apidocSignatureSpan">hapi.</span>methods (server)](#apidoc.element.hapi.methods.methods)
1.  object <span class="apidocSignatureSpan">hapi.methods.</span>methodNameRx

#### [module hapi.methods.prototype](#apidoc.module.hapi.methods.prototype)
1.  [function <span class="apidocSignatureSpan">hapi.methods.prototype.</span>_add (name, method, options, realm)](#apidoc.element.hapi.methods.prototype._add)
1.  [function <span class="apidocSignatureSpan">hapi.methods.prototype.</span>_assign (name, method, normalized)](#apidoc.element.hapi.methods.prototype._assign)
1.  [function <span class="apidocSignatureSpan">hapi.methods.prototype.</span>add (name, method, options, realm)](#apidoc.element.hapi.methods.prototype.add)

#### [module hapi.promises](#apidoc.module.hapi.promises)
1.  [function <span class="apidocSignatureSpan">hapi.promises.</span>wrap (bind, method, args)](#apidoc.element.hapi.promises.wrap)

#### [module hapi.protect](#apidoc.module.hapi.protect)
1.  [function <span class="apidocSignatureSpan">hapi.</span>protect (request)](#apidoc.element.hapi.protect.protect)

#### [module hapi.protect.prototype](#apidoc.module.hapi.protect.prototype)
1.  [function <span class="apidocSignatureSpan">hapi.protect.prototype.</span>_onError (err)](#apidoc.element.hapi.protect.prototype._onError)
1.  [function <span class="apidocSignatureSpan">hapi.protect.prototype.</span>enter (func)](#apidoc.element.hapi.protect.prototype.enter)
1.  [function <span class="apidocSignatureSpan">hapi.protect.prototype.</span>reset ()](#apidoc.element.hapi.protect.prototype.reset)
1.  [function <span class="apidocSignatureSpan">hapi.protect.prototype.</span>run (next, enter)](#apidoc.element.hapi.protect.prototype.run)

#### [module hapi.reply](#apidoc.module.hapi.reply)
1.  [function <span class="apidocSignatureSpan">hapi.</span>reply ()](#apidoc.element.hapi.reply.reply)

#### [module hapi.reply.prototype](#apidoc.module.hapi.reply.prototype)
1.  [function <span class="apidocSignatureSpan">hapi.reply.prototype.</span>decorate (property, method)](#apidoc.element.hapi.reply.prototype.decorate)
1.  [function <span class="apidocSignatureSpan">hapi.reply.prototype.</span>interface (request, realm, options, next)](#apidoc.element.hapi.reply.prototype.interface)

#### [module hapi.request](#apidoc.module.hapi.request)
1.  [function <span class="apidocSignatureSpan">hapi.</span>request ()](#apidoc.element.hapi.request.request)

#### [module hapi.request.prototype](#apidoc.module.hapi.request.prototype)
1.  [function <span class="apidocSignatureSpan">hapi.request.prototype.</span>decorate (property, method, options)](#apidoc.element.hapi.request.prototype.decorate)
1.  [function <span class="apidocSignatureSpan">hapi.request.prototype.</span>request (connection, req, res, options)](#apidoc.element.hapi.request.prototype.request)

#### [module hapi.response](#apidoc.module.hapi.response)
1.  [function <span class="apidocSignatureSpan">hapi.</span>response (source, request, options)](#apidoc.element.hapi.response.response)
1.  [function <span class="apidocSignatureSpan">hapi.response.</span>Payload (payload, options)](#apidoc.element.hapi.response.Payload)
1.  [function <span class="apidocSignatureSpan">hapi.response.</span>Peek (podium)](#apidoc.element.hapi.response.Peek)
1.  [function <span class="apidocSignatureSpan">hapi.response.</span>super_ (events)](#apidoc.element.hapi.response.super_)
1.  [function <span class="apidocSignatureSpan">hapi.response.</span>unmodified (request, options)](#apidoc.element.hapi.response.unmodified)
1.  [function <span class="apidocSignatureSpan">hapi.response.</span>wrap (result, request)](#apidoc.element.hapi.response.wrap)

#### [module hapi.response.prototype](#apidoc.module.hapi.response.prototype)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_close ()](#apidoc.element.hapi.response.prototype._close)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_header (key, value, options)](#apidoc.element.hapi.response.prototype._header)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_isPayloadSupported ()](#apidoc.element.hapi.response.prototype._isPayloadSupported)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_isRewritable ()](#apidoc.element.hapi.response.prototype._isRewritable)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_isTemporary ()](#apidoc.element.hapi.response.prototype._isTemporary)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_marshal (next)](#apidoc.element.hapi.response.prototype._marshal)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_passThrough ()](#apidoc.element.hapi.response.prototype._passThrough)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_permanent (isPermanent)](#apidoc.element.hapi.response.prototype._permanent)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_prepare (next)](#apidoc.element.hapi.response.prototype._prepare)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_processPrepare (next)](#apidoc.element.hapi.response.prototype._processPrepare)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_rewritable (isRewritable)](#apidoc.element.hapi.response.prototype._rewritable)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_setRewritable (isRewritable)](#apidoc.element.hapi.response.prototype._setRewritable)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_setSource (source, variety)](#apidoc.element.hapi.response.prototype._setSource)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_setTemporary (isTemporary)](#apidoc.element.hapi.response.prototype._setTemporary)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_streamify (source, next)](#apidoc.element.hapi.response.prototype._streamify)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_tap ()](#apidoc.element.hapi.response.prototype._tap)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_temporary (isTemporary)](#apidoc.element.hapi.response.prototype._temporary)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>bytes (bytes)](#apidoc.element.hapi.response.prototype.bytes)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>charset (charset)](#apidoc.element.hapi.response.prototype.charset)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>code (statusCode)](#apidoc.element.hapi.response.prototype.code)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>created (location)](#apidoc.element.hapi.response.prototype.created)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>encoding (encoding)](#apidoc.element.hapi.response.prototype.encoding)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>etag (tag, options)](#apidoc.element.hapi.response.prototype.etag)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>header (key, value, options)](#apidoc.element.hapi.response.prototype.header)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>location (uri)](#apidoc.element.hapi.response.prototype.location)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>message (httpMessage)](#apidoc.element.hapi.response.prototype.message)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>passThrough (enabled)](#apidoc.element.hapi.response.prototype.passThrough)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>redirect (location)](#apidoc.element.hapi.response.prototype.redirect)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>replacer (method)](#apidoc.element.hapi.response.prototype.replacer)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>spaces (count)](#apidoc.element.hapi.response.prototype.spaces)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>state (name, value, options)](#apidoc.element.hapi.response.prototype.state)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>suffix (suffix)](#apidoc.element.hapi.response.prototype.suffix)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>takeover ()](#apidoc.element.hapi.response.prototype.takeover)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>ttl (ttl)](#apidoc.element.hapi.response.prototype.ttl)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>type (type)](#apidoc.element.hapi.response.prototype.type)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>unstate (name, options)](#apidoc.element.hapi.response.prototype.unstate)
1.  [function <span class="apidocSignatureSpan">hapi.response.prototype.</span>vary (value)](#apidoc.element.hapi.response.prototype.vary)

#### [module hapi.route](#apidoc.module.hapi.route)
1.  [function <span class="apidocSignatureSpan">hapi.</span>route (route, connection, plugin, options)](#apidoc.element.hapi.route.route)

#### [module hapi.route.prototype](#apidoc.module.hapi.route.prototype)
1.  [function <span class="apidocSignatureSpan">hapi.route.prototype.</span>_combineExtensions (type, subscribe)](#apidoc.element.hapi.route.prototype._combineExtensions)
1.  [function <span class="apidocSignatureSpan">hapi.route.prototype.</span>rebuild (event)](#apidoc.element.hapi.route.prototype.rebuild)

#### [module hapi.schema](#apidoc.module.hapi.schema)
1.  [function <span class="apidocSignatureSpan">hapi.schema.</span>apply (type, options, message)](#apidoc.element.hapi.schema.apply)

#### [module hapi.transmit](#apidoc.module.hapi.transmit)
1.  [function <span class="apidocSignatureSpan">hapi.transmit.</span>send (request, callback)](#apidoc.element.hapi.transmit.send)

#### [module hapi.validation](#apidoc.module.hapi.validation)
1.  [function <span class="apidocSignatureSpan">hapi.validation.</span>compile (rule)](#apidoc.element.hapi.validation.compile)
1.  [function <span class="apidocSignatureSpan">hapi.validation.</span>headers (request, next)](#apidoc.element.hapi.validation.headers)
1.  [function <span class="apidocSignatureSpan">hapi.validation.</span>params (request, next)](#apidoc.element.hapi.validation.params)
1.  [function <span class="apidocSignatureSpan">hapi.validation.</span>payload (request, next)](#apidoc.element.hapi.validation.payload)
1.  [function <span class="apidocSignatureSpan">hapi.validation.</span>query (request, next)](#apidoc.element.hapi.validation.query)
1.  [function <span class="apidocSignatureSpan">hapi.validation.</span>response (request, next)](#apidoc.element.hapi.validation.response)



# <a name="apidoc.module.hapi"></a>[module hapi](#apidoc.module.hapi)

#### <a name="apidoc.element.hapi.Server"></a>[function <span class="apidocSignatureSpan">hapi.</span>Server (options)](#apidoc.element.hapi.Server)
- description and source-code
```javascript
Server = function (options) {

    Hoek.assert(this instanceof internals.Server, 'Server must be instantiated using new');

    options = Schema.apply('server', options || {});

    this._settings = Hoek.applyToDefaultsWithShallow(Defaults.server, options, ['connections.routes.bind']);
    this._settings.connections = Hoek.applyToDefaultsWithShallow(Defaults.connection, this._settings.connections || {}, ['routes
.bind']);
    this._settings.connections.routes.cors = Hoek.applyToDefaults(Defaults.cors, this._settings.connections.routes.cors);
    this._settings.connections.routes.security = Hoek.applyToDefaults(Defaults.security, this._settings.connections.routes.security
);

    this._caches = {};                                                              // Cache clients
    this._handlers = {};                                                            // Registered handlers
    this._methods = new Methods(this);                                              // Server methods

    this._events = new Podium([{ name: 'log', tags: true }, 'start', 'stop']);      // Server-only events
    this._dependencies = [];                                                        // Plugin dependencies
    this._registrations = {};                                                       // Tracks plugins registered before connection
 added
    this._heavy = new Heavy(this._settings.load);
    this._mime = new Mimos(this._settings.mime);
    this._replier = new Reply();
    this._requestor = new Request();
    this._decorations = {};
    this._plugins = {};                                                             // Exposed plugin properties by name
    this._app = {};
    this._registring = false;                                                       // true while register() is waiting for plugin
 callbacks
    this._state = 'stopped';                                                        // 'stopped', 'initializing', 'initialized', '
starting', 'started', 'stopping', 'invalid'

    this._extensionsSeq = 0;                                                        // Used to keep absolute order of extensions
 based on the order added across locations
    this._extensions = {
        onPreStart: new Ext('onPreStart', this),
        onPostStart: new Ext('onPostStart', this),
        onPreStop: new Ext('onPreStop', this),
        onPostStop: new Ext('onPostStop', this)
    };

    if (options.cache) {
        this._createCache(options.cache);
    }

    if (!this._caches._default) {
        this._createCache([{ engine: CatboxMemory }]);                              // Defaults to memory-based
    }

    Plugin.call(this, this, [], '', null);

    // Subscribe to server log events

    if (this._settings.debug) {
        const debug = (request, event) => {

            const data = event.data;
            console.error('Debug:', event.tags.join(', '), (data ? '\n    ' + (data.stack || (typeof data === 'object' ? Hoek.stringify
(data) : data)) : ''));
        };

        if (this._settings.debug.log) {
            this._events.on({ name: 'log', filter: this._settings.debug.log }, (event) => debug(null, event));
        }

        if (this._settings.debug.request) {
            this.on({ name: 'request', filter: this._settings.debug.request }, debug);
            this.on({ name: 'request-internal', filter: this._settings.debug.request }, debug);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_"></a>[function <span class="apidocSignatureSpan">hapi.</span>Server.super_ (server, connections, env, parent)](#apidoc.element.hapi.Server.super_)
- description and source-code
```javascript
Server.super_ = function (server, connections, env, parent) {         // env can be a realm or plugin name

    Podium.call(this, [connections && connections.length ? connections : Connection._events, server._events]);

    this._parent = parent;

    // Public interface

    this.root = server;
    this.app = this.root._app;
    this.connections = connections;
    this.load = this.root._heavy.load;
    this.methods = this.root._methods.methods;
    this.mime = this.root._mime;
    this.plugins = this.root._plugins;
    this.settings = this.root._settings;
    this.version = Package.version;

    this.realm = typeof env !== 'string' ? env : {
        _extensions: {
            onPreAuth: new Ext('onPreAuth', this.root),
            onPostAuth: new Ext('onPostAuth', this.root),
            onPreHandler: new Ext('onPreHandler', this.root),
            onPostHandler: new Ext('onPostHandler', this.root),
            onPreResponse: new Ext('onPreResponse', this.root)
        },
        modifiers: {
            route: {}
        },
        plugin: env,
        pluginOptions: {},
        plugins: {},
        settings: {
            bind: undefined,
            files: {
                relativeTo: undefined
            }
        }
    };

    this.auth = {
        default: (opts) => this._applyChild('auth.default', 'auth', 'default', [opts]),
        scheme: (name, scheme) => this._applyChild('auth.scheme', 'auth', 'scheme', [name, scheme]),
        strategy: (name, scheme, mode, opts) => this._applyChild('auth.strategy', 'auth', 'strategy', [name, scheme, mode, opts]),
        test: (name, request, next) => request.connection.auth.test(name, request, next)
    };

    this.cache.provision = (opts, callback) => {

        if (!callback) {
            return Promises.wrap(null, this.cache.provision, [opts]);
        }

        return this.root._createCache(opts, callback);
    };

    this._single();

    // Decorations

    const methods = Object.keys(this.root._decorations);
    for (let i = 0; i < methods.length; ++i) {
        const method = methods[i];
        this[method] = this.root._decorations[method];
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.auth"></a>[function <span class="apidocSignatureSpan">hapi.</span>auth (connection)](#apidoc.element.hapi.auth)
- description and source-code
```javascript
auth = function (connection) {

    this.connection = connection;
    this._schemes = {};
    this._strategies = {};
    this.settings = {
        default: null           // Strategy used as default if route has no auth settings
    };

    this.api = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.compression"></a>[function <span class="apidocSignatureSpan">hapi.</span>compression ()](#apidoc.element.hapi.compression)
- description and source-code
```javascript
compression = function () {

    this.encodings = ['identity', 'gzip', 'deflate'];
    this._encoders = {
        identity: null,
        gzip: (options) => Zlib.createGzip(options),
        deflate: (options) => Zlib.createDeflate(options)
    };

    this._decoders = {
        gzip: (options) => Zlib.createGunzip(options),
        deflate: (options) => Zlib.createInflate(options)
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.connection"></a>[function <span class="apidocSignatureSpan">hapi.</span>connection (server, options)](#apidoc.element.hapi.connection)
- description and source-code
```javascript
connection = function (server, options) {

    const now = Date.now();

    Podium.call(this, internals.Connection._events);

    this.settings = options;                                                        // options cloned in server.connection()
    this.server = server;

    // Normalize settings

    this.settings.labels = Hoek.unique(this.settings.labels || []);                 // Remove duplicates
    if (this.settings.port === undefined) {
        this.settings.port = 0;
    }

    this.type = (typeof this.settings.port === 'string' ? 'socket' : 'tcp');
    if (this.type === 'socket') {
        this.settings.port = (this.settings.port.indexOf('/') !== -1 ? Path.resolve(this.settings.port) : this.settings.port.toLowerCase
());
    }

    if (this.settings.autoListen === undefined) {
        this.settings.autoListen = true;
    }

    Hoek.assert(this.settings.autoListen || !this.settings.port, 'Cannot specify port when autoListen is false');
    Hoek.assert(this.settings.autoListen || !this.settings.address, 'Cannot specify address when autoListen is false');

    // Connection facilities

    this._started = false;
    this._connections = {};
    this._onConnection = null;          // Used to remove event listener on stop
    this.registrations = {};            // Tracks plugin for dependency validation { name -> { version } }

    this._extensions = {
        onRequest: new Ext('onRequest', this.server),
        onPreAuth: new Ext('onPreAuth', this.server),
        onPostAuth: new Ext('onPostAuth', this.server),
        onPreHandler: new Ext('onPreHandler', this.server),
        onPostHandler: new Ext('onPostHandler', this.server),
        onPreResponse: new Ext('onPreResponse', this.server)
    };

    this._requestCounter = { value: internals.counter.min, min: internals.counter.min, max: internals.counter.max };
    this._load = server._heavy.policy(this.settings.load);
    this._compression = new Compression();
    this.states = new Statehood.Definitions(this.settings.state);
    this.auth = new Auth(this);
    this._router = new Call.Router(this.settings.router);
    this._defaultRoutes();

    this.plugins = {};                  // Registered plugin APIs by plugin name
    this.app = {};                      // Place for application-specific state without conflicts with hapi, should not be used
by plugins

    // Create listener

    this.listener = this.settings.listener || (this.settings.tls ? Https.createServer(this.settings.tls) : Http.createServer());
    this.listener.on('request', this._dispatch());
    this._init();

    this.listener.on('clientError', (err, socket) => {

        this.server._log(['connection', 'client', 'error'], err);
    });

    // Connection information

    this.info = {
        created: now,
        started: 0,
        host: this.settings.host || Os.hostname() || 'localhost',
        port: this.settings.port,
        protocol: this.type === 'tcp' ? (this.settings.tls ? 'https' : 'http') : this.type,
        id: Os.hostname() + ':' + process.pid + ':' + now.toString(36)
    };

    this.info.uri = (this.settings.uri || (this.info.protocol + ':' + (this.type === 'tcp' ? '//' + this.info.host + (this.info.
port ? ':' + this.info.port : '') : this.info.port)));

    this.on('route', Cors.options);
}
```
- example usage
```shell
...

exports = module.exports = internals.Connection = function (server, options) {

const now = Date.now();

Podium.call(this, internals.Connection._events);

this.settings = options;                                                        // options cloned in server.connection()
this.server = server;

// Normalize settings

this.settings.labels = Hoek.unique(this.settings.labels || []);                 // Remove duplicates
if (this.settings.port === undefined) {
    this.settings.port = 0;
...
```

#### <a name="apidoc.element.hapi.ext"></a>[function <span class="apidocSignatureSpan">hapi.</span>ext (type, server)](#apidoc.element.hapi.ext)
- description and source-code
```javascript
ext = function (type, server) {

    this._topo = new Topo();
    this._server = server;
    this._routes = [];

    this.type = type;
    this.nodes = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.methods"></a>[function <span class="apidocSignatureSpan">hapi.</span>methods (server)](#apidoc.element.hapi.methods)
- description and source-code
```javascript
methods = function (server) {

    this.server = server;
    this.methods = {};
    this._normalized = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.protect"></a>[function <span class="apidocSignatureSpan">hapi.</span>protect (request)](#apidoc.element.hapi.protect)
- description and source-code
```javascript
protect = function (request) {

    this._error = null;
    this.logger = request;                          // Replaced with server when request completes

    if (!request.server.settings.useDomains) {
        this.domain = null;
        return;
    }

    Domain = Domain || require('domain');

    this.domain = Domain.create();
    this.domain.on('error', (err) => {

        return this._onError(err);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.reply"></a>[function <span class="apidocSignatureSpan">hapi.</span>reply ()](#apidoc.element.hapi.reply)
- description and source-code
```javascript
reply = function () {

    this._decorations = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.request"></a>[function <span class="apidocSignatureSpan">hapi.</span>request ()](#apidoc.element.hapi.request)
- description and source-code
```javascript
request = function () {

    this._decorations = null;
}
```
- example usage
```shell
...
            req.socket.end();
        }
    });
}

// Create request

const request = this.server._requestor.request(this, req, res, options);

// Check load

const overload = this._load.check();
if (overload) {
    this.server._log(['load'], this.server.load);
    request._reply(overload);
...
```

#### <a name="apidoc.element.hapi.response"></a>[function <span class="apidocSignatureSpan">hapi.</span>response (source, request, options)](#apidoc.element.hapi.response)
- description and source-code
```javascript
response = function (source, request, options) {

    Podium.call(this, ['finish', { name: 'peek', spread: true }]);

    options = options || {};

    this.request = request;
    this.statusCode = null;
    this.headers = {};                          // Incomplete as some headers are stored in flags
    this.variety = null;
    this.source = null;
    this.app = {};
    this.plugins = {};
    this.send = null;                           // Set by reply()
    this.hold = null;                           // Set by reply()

    this.settings = {
        encoding: 'utf8',
        charset: 'utf-8',                       // '-' required by IANA
        ttl: null,
        stringify: null,                        // JSON.stringify options
        passThrough: true,
        varyEtag: false,
        message: null
    };

    this._payload = null;                       // Readable stream
    this._takeover = false;
    this._contentEncoding = null;               // Set during transmit
    this._contentType = null;                   // Used if no explicit content-type is set and type is known
    this._error = null;                         // The boom object when created from an error

    this._processors = {
        marshal: options.marshal,
        prepare: options.prepare,
        close: options.close
    };

    this._setSource(source, options.variety);
}
```
- example usage
```shell
...
if (!strategy.methods.response) {
    return next();
}

request._protect.run(next, (exit) => {

    const reply = request.server._replier.interface(request, strategy.realm, {}, exit);
    strategy.methods.response(request, reply);
});
};


internals.Authenticator = class {
constructor(config, request, manager) {
...
```

#### <a name="apidoc.element.hapi.route"></a>[function <span class="apidocSignatureSpan">hapi.</span>route (route, connection, plugin, options)](#apidoc.element.hapi.route)
- description and source-code
```javascript
route = function (route, connection, plugin, options) {

    options = options || {};

    // Apply plugin environment (before schema validation)

    const realm = plugin.realm;
    if (realm.modifiers.route.vhost ||
        realm.modifiers.route.prefix) {

        route = Hoek.cloneWithShallow(route, ['config']);       // config is left unchanged
        route.path = (realm.modifiers.route.prefix ? realm.modifiers.route.prefix + (route.path !== '/' ? route.path : '') : route
.path);
        route.vhost = realm.modifiers.route.vhost || route.vhost;
    }

    // Setup and validate route configuration

    Hoek.assert(route.path, 'Route missing path');
    const routeDisplay = route.method + ' ' + route.path;

    let config = route.config;
    if (typeof config === 'function') {
        config = config.call(realm.settings.bind, connection.server);
    }

    Hoek.assert(route.handler || (config && config.handler), 'Missing or undefined handler:', routeDisplay);
    Hoek.assert(!!route.handler ^ !!(config && config.handler), 'Handler must only appear once:', routeDisplay);            // XOR
    Hoek.assert(route.path === '/' || route.path[route.path.length - 1] !== '/' || !connection.settings.router.stripTrailingSlash
, 'Path cannot end with a trailing slash when connection configured to strip:', routeDisplay);

    route = Schema.apply('route', route, routeDisplay);

    const handler = route.handler || config.handler;
    const method = route.method.toLowerCase();
    Hoek.assert(method !== 'head', 'Method name not allowed:', routeDisplay);

    // Apply settings in order: {connection} <- {handler} <- {realm} <- {route}

    const handlerDefaults = Handler.defaults(method, handler, connection.server);
    let base = Hoek.applyToDefaultsWithShallow(connection.settings.routes, handlerDefaults, ['bind']);
    base = Hoek.applyToDefaultsWithShallow(base, realm.settings, ['bind']);
    this.settings = Hoek.applyToDefaultsWithShallow(base, config || {}, ['bind', 'validate.headers', 'validate.payload', 'validate
.params', 'validate.query']);
    this.settings.handler = handler;
    this.settings = Schema.apply('routeConfig', this.settings, routeDisplay);

    const socketTimeout = (this.settings.timeout.socket === undefined ? 2 * 60 * 1000 : this.settings.timeout.socket);
    Hoek.assert(!this.settings.timeout.server || !socketTimeout || this.settings.timeout.server < socketTimeout, 'Server timeout
 must be shorter than socket timeout:', routeDisplay);
    Hoek.assert(!this.settings.payload.timeout || !socketTimeout || this.settings.payload.timeout < socketTimeout, 'Payload timeout
 must be shorter than socket timeout:', routeDisplay);

    this.connection = connection;
    this.server = connection.server;
    this.path = route.path;
    this.method = method;
    this.plugin = plugin;

    this.settings.vhost = route.vhost;
    this.settings.plugins = this.settings.plugins || {};            // Route-specific plugins settings, namespaced using plugin
name
    this.settings.app = this.settings.app || {};                    // Route-specific application settings

    // Path parsing

    this._special = !!options.special;
    this._analysis = this.connection._router.analyze(this.path);
    this.params = this._analysis.params;
    this.fingerprint = this._analysis.fingerprint;

    this.public = {
        method: this.method,
        path: this.path,
        vhost: this.vhost,
        realm: this.plugin.realm,
        settings: this.settings,
        fingerprint: this.fingerprint,
        auth: {
            access: (request) => Auth.access(request, this.public)
        }
    };

    // Validation

    const validation = this.settings.validate;
    if (this.method === 'get') {

        // Assert on config, not on merged settings

        Hoek.assert(!config || !config.payload, 'Cannot set payload settings on HEAD or GET request:', routeDisplay);
        Hoek.assert(!config || !config.validate || !config.validate.payload, 'Cannot validate HEAD or GET requests:', routeDisplay
);

        validation.payload = null;
    }

    ['headers', ' ...
```
- example usage
```shell
...

internals.Connection.prototype.match = function (method, path, host) {

    Hoek.assert(method && typeof method === 'string', 'Invalid method:', method);
    Hoek.assert(path && typeof path === 'string' && path[0] === '/', 'Invalid path:', path);
    Hoek.assert(!host || typeof host === 'string', 'Invalid host:', host);

    const match = this._router.route(method.toLowerCase(), path, host);
    Hoek.assert(match !== this._router.specials.badRequest, 'Invalid path:', path);
    if (match === this._router.specials.notFound) {
        return null;
    }

    return match.route.public;
};
...
```



# <a name="apidoc.module.hapi.Server"></a>[module hapi.Server](#apidoc.module.hapi.Server)

#### <a name="apidoc.element.hapi.Server.Server"></a>[function <span class="apidocSignatureSpan">hapi.</span>Server (options)](#apidoc.element.hapi.Server.Server)
- description and source-code
```javascript
Server = function (options) {

    Hoek.assert(this instanceof internals.Server, 'Server must be instantiated using new');

    options = Schema.apply('server', options || {});

    this._settings = Hoek.applyToDefaultsWithShallow(Defaults.server, options, ['connections.routes.bind']);
    this._settings.connections = Hoek.applyToDefaultsWithShallow(Defaults.connection, this._settings.connections || {}, ['routes
.bind']);
    this._settings.connections.routes.cors = Hoek.applyToDefaults(Defaults.cors, this._settings.connections.routes.cors);
    this._settings.connections.routes.security = Hoek.applyToDefaults(Defaults.security, this._settings.connections.routes.security
);

    this._caches = {};                                                              // Cache clients
    this._handlers = {};                                                            // Registered handlers
    this._methods = new Methods(this);                                              // Server methods

    this._events = new Podium([{ name: 'log', tags: true }, 'start', 'stop']);      // Server-only events
    this._dependencies = [];                                                        // Plugin dependencies
    this._registrations = {};                                                       // Tracks plugins registered before connection
 added
    this._heavy = new Heavy(this._settings.load);
    this._mime = new Mimos(this._settings.mime);
    this._replier = new Reply();
    this._requestor = new Request();
    this._decorations = {};
    this._plugins = {};                                                             // Exposed plugin properties by name
    this._app = {};
    this._registring = false;                                                       // true while register() is waiting for plugin
 callbacks
    this._state = 'stopped';                                                        // 'stopped', 'initializing', 'initialized', '
starting', 'started', 'stopping', 'invalid'

    this._extensionsSeq = 0;                                                        // Used to keep absolute order of extensions
 based on the order added across locations
    this._extensions = {
        onPreStart: new Ext('onPreStart', this),
        onPostStart: new Ext('onPostStart', this),
        onPreStop: new Ext('onPreStop', this),
        onPostStop: new Ext('onPostStop', this)
    };

    if (options.cache) {
        this._createCache(options.cache);
    }

    if (!this._caches._default) {
        this._createCache([{ engine: CatboxMemory }]);                              // Defaults to memory-based
    }

    Plugin.call(this, this, [], '', null);

    // Subscribe to server log events

    if (this._settings.debug) {
        const debug = (request, event) => {

            const data = event.data;
            console.error('Debug:', event.tags.join(', '), (data ? '\n    ' + (data.stack || (typeof data === 'object' ? Hoek.stringify
(data) : data)) : ''));
        };

        if (this._settings.debug.log) {
            this._events.on({ name: 'log', filter: this._settings.debug.log }, (event) => debug(null, event));
        }

        if (this._settings.debug.request) {
            this.on({ name: 'request', filter: this._settings.debug.request }, debug);
            this.on({ name: 'request-internal', filter: this._settings.debug.request }, debug);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_"></a>[function <span class="apidocSignatureSpan">hapi.Server.</span>super_ (server, connections, env, parent)](#apidoc.element.hapi.Server.super_)
- description and source-code
```javascript
super_ = function (server, connections, env, parent) {         // env can be a realm or plugin name

    Podium.call(this, [connections && connections.length ? connections : Connection._events, server._events]);

    this._parent = parent;

    // Public interface

    this.root = server;
    this.app = this.root._app;
    this.connections = connections;
    this.load = this.root._heavy.load;
    this.methods = this.root._methods.methods;
    this.mime = this.root._mime;
    this.plugins = this.root._plugins;
    this.settings = this.root._settings;
    this.version = Package.version;

    this.realm = typeof env !== 'string' ? env : {
        _extensions: {
            onPreAuth: new Ext('onPreAuth', this.root),
            onPostAuth: new Ext('onPostAuth', this.root),
            onPreHandler: new Ext('onPreHandler', this.root),
            onPostHandler: new Ext('onPostHandler', this.root),
            onPreResponse: new Ext('onPreResponse', this.root)
        },
        modifiers: {
            route: {}
        },
        plugin: env,
        pluginOptions: {},
        plugins: {},
        settings: {
            bind: undefined,
            files: {
                relativeTo: undefined
            }
        }
    };

    this.auth = {
        default: (opts) => this._applyChild('auth.default', 'auth', 'default', [opts]),
        scheme: (name, scheme) => this._applyChild('auth.scheme', 'auth', 'scheme', [name, scheme]),
        strategy: (name, scheme, mode, opts) => this._applyChild('auth.strategy', 'auth', 'strategy', [name, scheme, mode, opts]),
        test: (name, request, next) => request.connection.auth.test(name, request, next)
    };

    this.cache.provision = (opts, callback) => {

        if (!callback) {
            return Promises.wrap(null, this.cache.provision, [opts]);
        }

        return this.root._createCache(opts, callback);
    };

    this._single();

    // Decorations

    const methods = Object.keys(this.root._decorations);
    for (let i = 0; i < methods.length; ++i) {
        const method = methods[i];
        this[method] = this.root._decorations[method];
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.hapi.Server.prototype"></a>[module hapi.Server.prototype](#apidoc.module.hapi.Server.prototype)

#### <a name="apidoc.element.hapi.Server.prototype._createCache"></a>[function <span class="apidocSignatureSpan">hapi.Server.prototype.</span>_createCache (options, _callback)](#apidoc.element.hapi.Server.prototype._createCache)
- description and source-code
```javascript
_createCache = function (options, _callback) {

    Hoek.assert(this._state !== 'initializing', 'Cannot provision server cache while server is initializing');

    options = Schema.apply('cache', options);

    const added = [];
    for (let i = 0; i < options.length; ++i) {
        let config = options[i];
        if (typeof config === 'function') {
            config = { engine: config };
        }

        const name = config.name || '_default';
        Hoek.assert(!this._caches[name], 'Cannot configure the same cache more than once: ', name === '_default' ? 'default cache
' : name);

        let client = null;
        if (typeof config.engine === 'object') {
            client = new Catbox.Client(config.engine);
        }
        else {
            const settings = Hoek.clone(config);
            settings.partition = settings.partition || 'hapi-cache';
            delete settings.name;
            delete settings.engine;
            delete settings.shared;

            client = new Catbox.Client(config.engine, settings);
        }

        this._caches[name] = {
            client,
            segments: {},
            shared: config.shared || false
        };

        added.push(client);
    }

    if (!_callback) {
        return;
    }

    // Start cache

    if (['initialized', 'starting', 'started'].indexOf(this._state) !== -1) {
        const each = (client, next) => client.start(next);
        return Items.parallel(added, each, _callback);
    }

    return Hoek.nextTick(_callback)();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.prototype._invoke"></a>[function <span class="apidocSignatureSpan">hapi.Server.prototype.</span>_invoke (type, next)](#apidoc.element.hapi.Server.prototype._invoke)
- description and source-code
```javascript
_invoke = function (type, next) {

    const exts = this._extensions[type];
    if (!exts.nodes) {
        return next();
    }

    Items.serial(exts.nodes, (ext, nextExt) => {

        const bind = (ext.bind || ext.plugin.realm.settings.bind);
        ext.func.call(bind, ext.plugin._select(), nextExt);
    }, next);
}
```
- example usage
```shell
...

    // Execute onRequest extensions (can change request method and url)

    if (!this.connection._extensions.onRequest.nodes) {
        return this._lifecycle();
    }

    this._invoke(this.connection._extensions.onRequest, (err) => {

        return this._lifecycle(err);
    });
};


internals.Request.prototype._lifecycle = function (err) {
...
```

#### <a name="apidoc.element.hapi.Server.prototype._start"></a>[function <span class="apidocSignatureSpan">hapi.Server.prototype.</span>_start (callback)](#apidoc.element.hapi.Server.prototype._start)
- description and source-code
```javascript
_start = function (callback) {

    this._state = 'starting';

    const each = (connection, next) => connection._start(next);
    Items.parallel(this.connections, each, (err) => {

        if (err) {
            this._state = 'invalid';
            return Hoek.nextTick(callback)(err);
        }

        this._events.emit('start', null, () => {

            this._invoke('onPostStart', (err) => {

                if (err) {
                    this._state = 'invalid';
                    return callback(err);
                }

                this._state = 'started';
                return callback();
            });
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.prototype._validateDeps"></a>[function <span class="apidocSignatureSpan">hapi.Server.prototype.</span>_validateDeps ()](#apidoc.element.hapi.Server.prototype._validateDeps)
- description and source-code
```javascript
_validateDeps = function () {

    for (let i = 0; i < this._dependencies.length; ++i) {
        const dependency = this._dependencies[i];
        if (dependency.connections) {
            for (let j = 0; j < dependency.connections.length; ++j) {
                const connection = dependency.connections[j];
                for (let k = 0; k < dependency.deps.length; ++k) {
                    const dep = dependency.deps[k];
                    if (!connection.registrations[dep]) {
                        return new Error('Plugin ' + dependency.plugin + ' missing dependency ' + dep + ' in connection: ' + connection
.info.uri);
                    }
                }
            }
        }
        else {
            for (let j = 0; j < dependency.deps.length; ++j) {
                const dep = dependency.deps[j];
                if (!this._registrations[dep]) {
                    return new Error('Plugin ' + dependency.plugin + ' missing dependency ' + dep);
                }
            }
        }
    }

    return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.prototype.connection"></a>[function <span class="apidocSignatureSpan">hapi.Server.prototype.</span>connection (options)](#apidoc.element.hapi.Server.prototype.connection)
- description and source-code
```javascript
connection = function (options) {

    const root = this.root;                                     // Explicitly use the root reference (for plugin invocation)

    const connections = [];
    [].concat(options).forEach((item) => {

        let settings = Hoek.applyToDefaultsWithShallow(root._settings.connections, item || {}, ['listener', 'routes.bind']);
        settings.routes.cors = Hoek.applyToDefaults(root._settings.connections.routes.cors || Defaults.cors, settings.routes.cors
) || false;
        settings.routes.security = Hoek.applyToDefaults(root._settings.connections.routes.security || Defaults.security, settings
.routes.security);

        settings = Schema.apply('connection', settings);        // Applies validation changes (type cast)

        const connection = new Connection(root, settings);
        root.connections.push(connection);
        root.registerPodium(connection);
        root._single();

        const registrations = Object.keys(root._registrations);
        for (let i = 0; i < registrations.length; ++i) {
            const name = registrations[i];
            connection.registrations[name] = root._registrations[name];
        }

        connections.push(connection);
    });

    return this._clone(connections);                            // Use this for active realm
}
```
- example usage
```shell
...

exports = module.exports = internals.Connection = function (server, options) {

const now = Date.now();

Podium.call(this, internals.Connection._events);

this.settings = options;                                                        // options cloned in server.connection()
this.server = server;

// Normalize settings

this.settings.labels = Hoek.unique(this.settings.labels || []);                 // Remove duplicates
if (this.settings.port === undefined) {
    this.settings.port = 0;
...
```

#### <a name="apidoc.element.hapi.Server.prototype.initialize"></a>[function <span class="apidocSignatureSpan">hapi.Server.prototype.</span>initialize (callback)](#apidoc.element.hapi.Server.prototype.initialize)
- description and source-code
```javascript
initialize = function (callback) {

    if (!callback) {
        return Promises.wrap(this, this.initialize);
    }

    Hoek.assert(typeof callback === 'function', 'Missing required start callback function');
    const nextTickCallback = Hoek.nextTick(callback);

    if (this._registring) {
        return nextTickCallback(new Error('Cannot start server before plugins finished registration'));
    }

    if (this._state === 'initialized') {
        return nextTickCallback();
    }

    if (this._state !== 'stopped') {
        return nextTickCallback(new Error('Cannot initialize server while it is in ' + this._state + ' state'));
    }

    const error = this._validateDeps();
    if (error) {
        return nextTickCallback(error);
    }

    this._state = 'initializing';

    // Start cache

    const caches = Object.keys(this._caches);
    const each = (cache, next) => this._caches[cache].client.start(next);
    Items.parallel(caches, each, (err) => {

        if (err) {
            this._state = 'invalid';
            return callback(err);
        }

        // After hooks

        this._invoke('onPreStart', (err) => {

            if (err) {
                this._state = 'invalid';
                return callback(err);
            }

            // Load measurements

            this._heavy.start();

            // Listen to connections

            this._state = 'initialized';
            return callback();
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.prototype.start"></a>[function <span class="apidocSignatureSpan">hapi.Server.prototype.</span>start (callback)](#apidoc.element.hapi.Server.prototype.start)
- description and source-code
```javascript
start = function (callback) {

    if (!callback) {
        return Promises.wrap(this, this.start);
    }

    Hoek.assert(typeof callback === 'function', 'Missing required start callback function');
    const nextTickCallback = Hoek.nextTick(callback);

    if (!this.connections.length) {
        return nextTickCallback(new Error('No connections to start'));
    }

    if (this._state === 'initialized' ||
        this._state === 'started') {

        const error = this._validateDeps();
        if (error) {
            return nextTickCallback(error);
        }
    }

    if (this._state === 'initialized') {
        return this._start(callback);
    }

    if (this._state === 'started') {
        const each = (connection, next) => connection._start(next);
        return Items.parallel(this.connections, each, nextTickCallback);
    }

    if (this._state !== 'stopped') {
        return nextTickCallback(new Error('Cannot start server while it is in ' + this._state + ' state'));
    }

    this.initialize((err) => {

        if (err) {
            return callback(err);
        }

        this._start(callback);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.prototype.stop"></a>[function <span class="apidocSignatureSpan">hapi.Server.prototype.</span>stop ()](#apidoc.element.hapi.Server.prototype.stop)
- description and source-code
```javascript
stop = function () {

    const args = arguments.length;
    const lastArg = arguments[args - 1];
    const callback = (!args ? null : (typeof lastArg === 'function' ? lastArg : null));
    const options = (!args ? {} : (args === 1 ? (callback ? {} : arguments[0]) : arguments[0]));

    if (!callback) {
        return Promises.wrap(this, this.stop, [options]);
    }

    options.timeout = options.timeout || 5000;                                              // Default timeout to 5 seconds

    if (['stopped', 'initialized', 'started', 'invalid'].indexOf(this._state) === -1) {
        return Hoek.nextTick(callback)(new Error('Cannot stop server while in ' + this._state + ' state'));
    }

    this._state = 'stopping';

    this._invoke('onPreStop', (err) => {

        if (err) {
            this._state = 'invalid';
            return callback(err);
        }

        const each = (connection, next) => connection._stop(options, next);
        Items.parallel(this.connections, each, (err) => {

            if (err) {
                this._state = 'invalid';
                return callback(err);
            }

            const caches = Object.keys(this._caches);
            for (let i = 0; i < caches.length; ++i) {
                this._caches[caches[i]].client.stop();
            }

            this._events.emit('stop', null, () => {

                this._heavy.stop();
                this._invoke('onPostStop', (err) => {

                    if (err) {
                        this._state = 'invalid';
                        return callback(err);
                    }

                    this._state = 'stopped';
                    return callback();
                });
            });
        });
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.hapi.Server.super_"></a>[module hapi.Server.super_](#apidoc.module.hapi.Server.super_)

#### <a name="apidoc.element.hapi.Server.super_.super_"></a>[function <span class="apidocSignatureSpan">hapi.Server.</span>super_ (events)](#apidoc.element.hapi.Server.super_.super_)
- description and source-code
```javascript
super_ = function (events) {

    // Use descriptive names to avoid conflict when inherited

    this._eventListeners = Object.create(null);
    this._notificationsQueue = [];
    this._eventsProcessing = false;
    this._sourcePodiums = [];

    if (events) {
        this.registerEvent(events);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.hapi.Server.super_.prototype"></a>[module hapi.Server.super_.prototype](#apidoc.module.hapi.Server.super_.prototype)

#### <a name="apidoc.element.hapi.Server.super_.prototype._apply"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>_apply (type, func, args)](#apidoc.element.hapi.Server.super_.prototype._apply)
- description and source-code
```javascript
_apply = function (type, func, args) {

    Hoek.assert(this.connections, 'Cannot add ' + type + ' from a connectionless plugin');
    Hoek.assert(this.connections.length, 'Cannot add ' + type + ' without a connection');

    for (let i = 0; i < this.connections.length; ++i) {
        func.apply(this.connections[i], args);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_.prototype._applyChild"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>_applyChild (type, child, func, args)](#apidoc.element.hapi.Server.super_.prototype._applyChild)
- description and source-code
```javascript
_applyChild = function (type, child, func, args) {

    Hoek.assert(this.connections, 'Cannot add ' + type + ' from a connectionless plugin');
    Hoek.assert(this.connections.length, 'Cannot add ' + type + ' without a connection');

    for (let i = 0; i < this.connections.length; ++i) {
        const obj = this.connections[i][child];
        obj[func].apply(obj, args);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_.prototype._clone"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>_clone (connections, plugin)](#apidoc.element.hapi.Server.super_.prototype._clone)
- description and source-code
```javascript
_clone = function (connections, plugin) {

    const env = (plugin !== undefined ? plugin : this.realm);                     // Allow empty string
    return new internals.Plugin(this.root, connections, env, this);
}
```
- example usage
```shell
...

Hoek.assert(name, 'Authentication strategy must have a name');
Hoek.assert(name !== 'bypass', 'Cannot use reserved strategy name: bypass');
Hoek.assert(!this._strategies[name], 'Authentication strategy name already exists');
Hoek.assert(scheme, 'Authentication strategy', name, 'missing scheme');
Hoek.assert(this._schemes[scheme], 'Authentication strategy', name, 'uses unknown scheme:', scheme);

const server = this.connection.server._clone([this.connection], '');
const strategy = this._schemes[scheme](server, options);

Hoek.assert(strategy.authenticate, 'Invalid scheme:', name, 'missing authenticate() method');
Hoek.assert(typeof strategy.authenticate === 'function', 'Invalid scheme:', name, 'invalid authenticate() method');
Hoek.assert(!strategy.payload || typeof strategy.payload === 'function', 'Invalid scheme:', name, 'invalid payload() method');
Hoek.assert(!strategy.response || typeof strategy.response === 'function', 'Invalid scheme:', name, 'invalid response() method');
strategy.options = strategy.options || {};
...
```

#### <a name="apidoc.element.hapi.Server.super_.prototype._ext"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>_ext (event)](#apidoc.element.hapi.Server.super_.prototype._ext)
- description and source-code
```javascript
_ext = function (event) {

    event = Hoek.shallow(event);
    event.plugin = this;
    const type = event.type;

    if (!this.root._extensions[type]) {

        // Realm route extensions

        if (event.options.sandbox === 'plugin') {
            Hoek.assert(this.realm._extensions[type], 'Unknown event type', type);
            return this.realm._extensions[type].add(event);
        }

        // Connection route extensions

        return this._apply('ext', Connection.prototype._ext, [event]);
    }

    // Server extensions

    Hoek.assert(!event.options.sandbox, 'Cannot specify sandbox option for server extension');
    Hoek.assert(type !== 'onPreStart' || this.root._state === 'stopped', 'Cannot add onPreStart (after) extension after the server
 was initialized');
    this.root._extensions[type].add(event);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_.prototype._log"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>_log (tags, data)](#apidoc.element.hapi.Server.super_.prototype._log)
- description and source-code
```javascript
_log = function (tags, data) {

    return this.log(tags, data, null, true);
}
```
- example usage
```shell
...

    if (config.mode === 'optional' ||
        config.mode === 'try') {

        request.auth.isAuthenticated = false;
        request.auth.credentials = null;
        request.auth.error = err;
        request._log(['auth', 'unauthenticated']);
        return next();
    }

    return next(err);
}

validate(err, result, next) {                 // err can be Boom, Error, or a valid response object
...
```

#### <a name="apidoc.element.hapi.Server.super_.prototype._select"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>_select (labels, plugin)](#apidoc.element.hapi.Server.super_.prototype._select)
- description and source-code
```javascript
_select = function (labels, plugin) {

    let connections = this.connections;

    if (labels &&
        labels.length) {            // Captures both empty arrays and empty strings

        Hoek.assert(this.connections, 'Cannot select inside a connectionless plugin');

        connections = [];
        for (let i = 0; i < this.connections.length; ++i) {
            const connection = this.connections[i];
            if (Hoek.intersect(connection.settings.labels, labels).length) {
                connections.push(connection);
            }
        }

        if (!plugin &&
            connections.length === this.connections.length) {

            return this;
        }
    }

    const env = (plugin !== undefined ? plugin : this.realm);                     // Allow empty string
    return new internals.Plugin(this.root, connections, env, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_.prototype._single"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>_single ()](#apidoc.element.hapi.Server.super_.prototype._single)
- description and source-code
```javascript
_single = function () {

    if (this.connections &&
        this.connections.length === 1) {

        this.info = this.connections[0].info;
        this.listener = this.connections[0].listener;
        this.registrations = this.connections[0].registrations;
        this.auth.api = this.connections[0].auth.api;
    }
    else {
        this.info = null;
        this.listener = null;
        this.registrations = null;
        this.auth.api = null;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.bind"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>bind (context)](#apidoc.element.hapi.Server.super_.prototype.bind)
- description and source-code
```javascript
bind = function (context) {

    Hoek.assert(typeof context === 'object', 'bind must be an object');
    this.realm.settings.bind = context;
}
```
- example usage
```shell
...

    Items.serial(request._route._prerequisites, each, (err) => {

        if (err) {
            return callback(err);
        }

        const wrapped = domain ? domain.bind(internals.handler) : internals.handler;
        return wrapped(request, callback);
    });
};


internals.handler = function (request, callback) {
...
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.cache"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>cache (options, _segment)](#apidoc.element.hapi.Server.super_.prototype.cache)
- description and source-code
```javascript
cache = function (options, _segment) {

    options = Schema.apply('cachePolicy', options);

    const segment = options.segment || _segment || (this.realm.plugin ? '!' + this.realm.plugin : '');
    Hoek.assert(segment, 'Missing cache segment name');

    const cacheName = options.cache || '_default';
    const cache = this.root._caches[cacheName];
    Hoek.assert(cache, 'Unknown cache', cacheName);
    Hoek.assert(!cache.segments[segment] || cache.shared || options.shared, 'Cannot provision the same cache segment more than once
');
    cache.segments[segment] = true;

    return new Catbox.Policy(options, cache.client, segment);
}
```
- example usage
```shell
...

    settings.cache.generateFunc = (id, next) => {

id.args.push(next);                     // function (err, result, ttl)
normalized.apply(bind, id.args);
    };

    const cache = this.server.cache(settings.cache, '#' + name);

    const func = function (/* arguments, methodNext */) {

const args = [];
for (let i = 0; i < arguments.length - 1; ++i) {
    args.push(arguments[i]);
}
...
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.decoder"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>decoder (encoding, decoder)](#apidoc.element.hapi.Server.super_.prototype.decoder)
- description and source-code
```javascript
decoder = function (encoding, decoder) {

    this._apply('decoder', Connection.prototype.decoder, [encoding, decoder]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.decorate"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>decorate (type, property, method, options)](#apidoc.element.hapi.Server.super_.prototype.decorate)
- description and source-code
```javascript
decorate = function (type, property, method, options) {

    Hoek.assert(['reply', 'request', 'server'].indexOf(type) !== -1, 'Unknown decoration type:', type);
    Hoek.assert(property, 'Missing decoration property name');
    Hoek.assert(typeof property === 'string', 'Decoration property must be a string');
    Hoek.assert(property[0] !== '_', 'Property name cannot begin with an underscore:', property);

    // Request

    if (type === 'request') {
        return this.root._requestor.decorate(property, method, options);
    }

    Hoek.assert(!options, 'Cannot specify options for non-request decoration');

    // Reply

    if (type === 'reply') {
        return this.root._replier.decorate(property, method);
    }

    // Server

    Hoek.assert(!this.root._decorations[property], 'Server decoration already defined:', property);
    Hoek.assert(this[property] === undefined && this.root[property] === undefined, 'Cannot override the built-in server interface
 method:', property);

    this.root._decorations[property] = method;

    this[property] = method;
    let parent = this._parent;
    while (parent) {
        parent[property] = method;
        parent = parent._parent;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.dependency"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>dependency (dependencies, after)](#apidoc.element.hapi.Server.super_.prototype.dependency)
- description and source-code
```javascript
dependency = function (dependencies, after) {

    Hoek.assert(this.realm.plugin, 'Cannot call dependency() outside of a plugin');
    Hoek.assert(!after || typeof after === 'function', 'Invalid after method');

    dependencies = [].concat(dependencies);
    this.root._dependencies.push({ plugin: this.realm.plugin, connections: this.connections, deps: dependencies });

    if (after) {
        this.ext('onPreStart', after, { after: dependencies });
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.emit"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>emit (criteria, data, callback)](#apidoc.element.hapi.Server.super_.prototype.emit)
- description and source-code
```javascript
emit = function (criteria, data, callback) {

    this.root._events.emit(criteria, data, callback);
}
```
- example usage
```shell
...
for (let i = 0; i < vhosts.length; ++i) {
    const vhost = vhosts[i];
    const record = this._router.add({ method: route.method, path: route.path, vhost, analysis: route._analysis, id: route.settings
.id }, route);
    route.fingerprint = record.fingerprint;
    route.params = record.params;
}

this.emit('route', [route.public, this, plugin]);
};


internals.Connection.prototype._defaultRoutes = function () {

this._router.special('notFound', new Route({ method: '_special', path: '/{p*}', handler: internals.notFound }, this, this.server
, { special: true }));
this._router.special('badRequest', new Route({ method: '_special', path: '/{p*}', handler: internals.badRequest }, this, this.server
, { special: true }));
...
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.encoder"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>encoder (encoding, encoder)](#apidoc.element.hapi.Server.super_.prototype.encoder)
- description and source-code
```javascript
encoder = function (encoding, encoder) {

    this._apply('encoder', Connection.prototype.encoder, [encoding, encoder]);
}
```
- example usage
```shell
...
length !== 0 &&
response.statusCode !== 206 &&
response._isPayloadSupported()) {

delete response.headers['content-length'];
response._header('content-encoding', encoding);

compressor = request.connection._compression.encoder(request, encoding);
    }

    if ((response.headers['content-encoding'] || encoding) &&
response.headers.etag &&
response.settings.varyEtag) {

response.headers.etag = response.headers.etag.slice(0, -1) + '-' + (response.headers['content-encoding'] || encoding) + '"';
...
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.event"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>event (event)](#apidoc.element.hapi.Server.super_.prototype.event)
- description and source-code
```javascript
event = function (event) {

    this.root._events.registerEvent(event);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.expose"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>expose (key, value)](#apidoc.element.hapi.Server.super_.prototype.expose)
- description and source-code
```javascript
expose = function (key, value) {

    Hoek.assert(this.realm.plugin, 'Cannot call expose() outside of a plugin');

    const plugin = this.realm.plugin;
    this.root.plugins[plugin] = this.root.plugins[plugin] || {};

    if (typeof key === 'string') {
        this.root.plugins[plugin][key] = value;
    }
    else {
        Hoek.merge(this.root.plugins[plugin], key);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.ext"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>ext (events)](#apidoc.element.hapi.Server.super_.prototype.ext)
- description and source-code
```javascript
ext = function (events) {        // (event, method, options) -OR- (events)

    if (typeof events === 'string') {
        events = { type: arguments[0], method: arguments[1], options: arguments[2] };
    }

    events = Schema.apply('exts', events);

    for (let i = 0; i < events.length; ++i) {
        this._ext(events[i]);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.handler"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>handler (name, method)](#apidoc.element.hapi.Server.super_.prototype.handler)
- description and source-code
```javascript
handler = function (name, method) {

    Hoek.assert(typeof name === 'string', 'Invalid handler name');
    Hoek.assert(!this.root._handlers[name], 'Handler name already exists:', name);
    Hoek.assert(typeof method === 'function', 'Handler must be a function:', name);
    Hoek.assert(!method.defaults || typeof method.defaults === 'object' || typeof method.defaults === 'function', 'Handler defaults
 property must be an object or function');
    this.root._handlers[name] = method;
}
```
- example usage
```shell
...

internals.Connection.prototype._defaultRoutes = function () {

this._router.special('notFound', new Route({ method: '_special', path: '/{p*}', handler: internals.notFound }, this, this.server
, { special: true }));
this._router.special('badRequest', new Route({ method: '_special', path: '/{p*}', handler: internals.badRequest }, this, this.server
, { special: true }));

if (this.settings.routes.cors) {
    Cors.handler(this);
}
};


internals.notFound = function (request, reply) {

return reply(Boom.notFound());
...
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.inject"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>inject (options, callback)](#apidoc.element.hapi.Server.super_.prototype.inject)
- description and source-code
```javascript
inject = function (options, callback) {

    Hoek.assert(this.connections.length === 1, 'Method not available when the selection has more than one connection or none');
    return this.connections[0].inject(options, callback);
}
```
- example usage
```shell
...
};
};


internals.Connection.prototype.inject = function (options, callback) {

if (!callback) {
    return new Promise((resolve, reject) => this.inject(options, (res) => resolve(res)));
}

let settings = options;
if (typeof settings === 'string') {
    settings = { url: settings };
}
...
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.log"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>log (tags, data, timestamp, _internal)](#apidoc.element.hapi.Server.super_.prototype.log)
- description and source-code
```javascript
log = function (tags, data, timestamp, _internal) {

    tags = [].concat(tags);
    timestamp = (timestamp ? (timestamp instanceof Date ? timestamp.getTime() : timestamp) : Date.now());
    const internal = !!_internal;

    const update = (typeof data !== 'function' ? { timestamp, tags, data, internal } : () => {

        return { timestamp, tags, data: data(), internal };
    });

    this.root._events.emit({ name: 'log', tags }, update);
}
```
- example usage
```shell
...

this.connection.emit({ name: internal ? 'request-internal' : 'request', tags }, update);
};


internals.Request.prototype._log = function (tags, data) {

return this.log(tags, data, null, true);
};


internals.Request.prototype.getLog = function (tags, internal) {

Hoek.assert(this.route.settings.log, 'Request logging is disabled');
...
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.lookup"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>lookup (id)](#apidoc.element.hapi.Server.super_.prototype.lookup)
- description and source-code
```javascript
lookup = function (id) {

    Hoek.assert(this.connections.length === 1, 'Method not available when the selection has more than one connection or none');
    return this.connections[0].lookup(id);
}
```
- example usage
```shell
...
return auth._authenticate(request, next);
};


internals.Auth.access = function (request, route) {

const auth = request.connection.auth;
const config = auth.lookup(route);
if (!config) {
    return true;
}

const credentials = request.auth.credentials;
if (!credentials) {
    return false;
...
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.match"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>match (method, path, host)](#apidoc.element.hapi.Server.super_.prototype.match)
- description and source-code
```javascript
match = function (method, path, host) {

    Hoek.assert(this.connections.length === 1, 'Method not available when the selection has more than one connection or none');
    return this.connections[0].match(method, path, host);
}
```
- example usage
```shell
...
const method = request.headers['access-control-request-method'];
if (!method) {
    return reply(Boom.notFound('CORS error: Missing Access-Control-Request-Method header'));
}

// Lookup route

const route = request.connection.match(method, request.path, request.info.hostname);
if (!route) {
    return reply(Boom.notFound());
}

const settings = route.settings.cors;
if (!settings) {
    return reply({ message: 'CORS is disabled for this route' });
...
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.method"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>method (name, method, options)](#apidoc.element.hapi.Server.super_.prototype.method)
- description and source-code
```javascript
method = function (name, method, options) {

    return this.root._methods.add(name, method, options, this.realm);
}
```
- example usage
```shell
...
    // Decorate

    if (this._decorations) {
        const properties = Object.keys(this._decorations);
        for (let i = 0; i < properties.length; ++i) {
            const property = properties[i];
            const assignment = this._decorations[property];
            request[property] = (assignment.apply ? assignment.method(request) : assignment.method);
        }
    }

    return request;
};
...
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.path"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>path (relativeTo)](#apidoc.element.hapi.Server.super_.prototype.path)
- description and source-code
```javascript
path = function (relativeTo) {

    Hoek.assert(relativeTo && typeof relativeTo === 'string', 'relativeTo must be a non-empty string');
    this.realm.settings.files.relativeTo = relativeTo;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.register"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>register (plugins)](#apidoc.element.hapi.Server.super_.prototype.register)
- description and source-code
```javascript
register = function (plugins) {

    let options = (typeof arguments[1] === 'object' ? arguments[1] : {});
    const callback = (typeof arguments[1] === 'object' ? arguments[2] : arguments[1]);

    if (!callback) {
        return Promises.wrap(this, this.register, [plugins, options]);
    }

    if (this.realm.modifiers.route.prefix ||
        this.realm.modifiers.route.vhost) {

        options = Hoek.clone(options);
        options.routes = options.routes || {};

        options.routes.prefix = (this.realm.modifiers.route.prefix || '') + (options.routes.prefix || '') || undefined;
        options.routes.vhost = this.realm.modifiers.route.vhost || options.routes.vhost;
    }

    options = Schema.apply('register', options);

<span class="apidocCodeCommentSpan">    /*
        const register = function (server, options, next) { return next(); };
        register.attributes = {
            pkg: require('../package.json'),
            name: 'plugin',
            version: '1.1.1',
            multiple: false,
            dependencies: [],
            connections: false,
            once: true
        };

        const item = {
            register: register,
            options: options        // -optional--
        };

        - OR -

        const item = function () {}
        item.register = register;
        item.options = options;

        const plugins = register, items, [register, item]
    */
</span>
    const registrations = [];
    plugins = [].concat(plugins);
    for (let i = 0; i < plugins.length; ++i) {
        let plugin = plugins[i];

        if (typeof plugin === 'function') {
            if (!plugin.register) {                                 // plugin is register() function
                plugin = { register: plugin };
            }
            else {
                plugin = Hoek.shallow(plugin);                      // Convert function to object
            }
        }

        if (plugin.register.register) {                             // Required plugin
            plugin.register = plugin.register.register;
        }

        plugin = Schema.apply('plugin', plugin);

        const attributes = plugin.register.attributes;
        const registration = {
            register: plugin.register,
            name: attributes.name || attributes.pkg.name,
            version: attributes.version || attributes.pkg.version,
            multiple: attributes.multiple,
            pluginOptions: plugin.options,
            dependencies: attributes.dependencies,
            connections: attributes.connections,
            options: {
                once: attributes.once || (plugin.once !== undefined ? plugin.once : options.once),
                routes: {
                    prefix: plugin.routes.prefix || options.routes.prefix,
                    vhost: plugin.routes.vhost || options.routes.vhost
                },
                select: plugin.select || options.select
            }
        };

        registrations.push(registration);
    }

    this.root._registring = true;

    const each = (item, next) => {

        const selection = this._select(item.options.select, item.name);
        selection.realm.modifiers.route.prefix = item.options.routes.prefix;
        selection.realm.modifiers.route.vhost = item.options.routes.vhost;
        selection.realm.pluginOptions = item.pluginOptions || {};

        const registrationData = {
            version: item.version,
            name: item.name,
            options: item.pluginOptions,
            attributes: item.register.attributes
        };

        // Protect against multiple registrations

        const connectionless = (item.connections === 'conditional' ? selection.connections.length === 0 : !item.connections);
        if (connectionless) {
            if (this.root._registrations[item.name]) {
                if (item.options.once) {
                    return next();
                }

                Hoek.assert(item.multiple, 'Plugin', item.name, 'already registered');
            }
            else {
                this.root._registrations[item.name] = registrationData; ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.route"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>route (options)](#apidoc.element.hapi.Server.super_.prototype.route)
- description and source-code
```javascript
route = function (options) {

    Hoek.assert(arguments.length === 1, 'Method requires a single object argument or a single array of objects');
    Hoek.assert(typeof options === 'object', 'Invalid route options');
    Hoek.assert(this.connections, 'Cannot add route from a connectionless plugin');
    Hoek.assert(this.connections.length, 'Cannot add a route without any connections');

    this._apply('route', Connection.prototype._route, [options, this]);
}
```
- example usage
```shell
...

internals.Connection.prototype.match = function (method, path, host) {

    Hoek.assert(method && typeof method === 'string', 'Invalid method:', method);
    Hoek.assert(path && typeof path === 'string' && path[0] === '/', 'Invalid path:', path);
    Hoek.assert(!host || typeof host === 'string', 'Invalid host:', host);

    const match = this._router.route(method.toLowerCase(), path, host);
    Hoek.assert(match !== this._router.specials.badRequest, 'Invalid path:', path);
    if (match === this._router.specials.notFound) {
        return null;
    }

    return match.route.public;
};
...
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.select"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>select ()](#apidoc.element.hapi.Server.super_.prototype.select)
- description and source-code
```javascript
select = function () {

    let labels = [];
    for (let i = 0; i < arguments.length; ++i) {
        labels.push(arguments[i]);
    }

    labels = Hoek.flatten(labels);
    return this._select(labels);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.state"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>state (name, options)](#apidoc.element.hapi.Server.super_.prototype.state)
- description and source-code
```javascript
state = function (name, options) {

    this._applyChild('state', 'states', 'add', [name, options]);
}
```
- example usage
```shell
...
    const response = request.response;

    Cors.headers(response);
    internals.content(response, false);
    internals.security(response);
    internals.unmodified(response);

    internals.state(response, (err) => {

if (err) {
    request._log(['state', 'response', 'error'], err);
    request._states = {};                                           // Clear broken state
    return next(err);
}
...
```

#### <a name="apidoc.element.hapi.Server.super_.prototype.table"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.prototype.</span>table (host)](#apidoc.element.hapi.Server.super_.prototype.table)
- description and source-code
```javascript
table = function (host) {

    Hoek.assert(this.connections, 'Cannot request routing table from a connectionless plugin');

    const table = [];
    for (let i = 0; i < this.connections.length; ++i) {
        const connection = this.connections[i];
        table.push({ info: connection.info, labels: connection.settings.labels, table: connection.table(host) });
    }

    return table;
}
```
- example usage
```shell
...
    return callback(res);
});
};


internals.Connection.prototype.table = function (host) {

return this._router.table(host);
};


internals.Connection.prototype.lookup = function (id) {

Hoek.assert(id && typeof id === 'string', 'Invalid route id:', id);
...
```



# <a name="apidoc.module.hapi.Server.super_.super_.prototype"></a>[module hapi.Server.super_.super_.prototype](#apidoc.module.hapi.Server.super_.super_.prototype)

#### <a name="apidoc.element.hapi.Server.super_.super_.prototype._emit"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>_emit (criteria, data, generated, callback)](#apidoc.element.hapi.Server.super_.super_.prototype._emit)
- description and source-code
```javascript
_emit = function (criteria, data, generated, callback) {

    criteria = internals.criteria(criteria);

    const name = criteria.name;
    Hoek.assert(name, 'Criteria missing event name');

    const event = this._eventListeners[name];
    Hoek.assert(event, 'Unknown event ${name}');
    Hoek.assert(!event.flags.spread || Array.isArray(data) || typeof data === 'function', 'Data must be an array for spread event
');
    Hoek.assert(!criteria.channel || typeof criteria.channel === 'string', 'Invalid channel name');
    Hoek.assert(!criteria.channel || !event.flags.channels || event.flags.channels.indexOf(criteria.channel) !== -1, 'Unknown ${
criteria.channel} channel');

    if (typeof criteria.tags === 'string') {
        criteria.tags = [criteria.tags];
    }

    if (criteria.tags &&
        Array.isArray(criteria.tags)) {

        criteria.tags = Hoek.mapToObject(criteria.tags);
    }

    internals.emit(this, { criteria, data, callback, generated });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_.super_.prototype.addListener"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>addListener (criteria, listener)](#apidoc.element.hapi.Server.super_.super_.prototype.addListener)
- description and source-code
```javascript
addListener = function (criteria, listener) {

    criteria = internals.criteria(criteria);
    criteria.listener = listener;

    if (criteria.filter &&
        (typeof criteria.filter === 'string' || Array.isArray(criteria.filter))) {

        criteria.filter = { tags: criteria.filter };
    }

    criteria = Joi.attempt(criteria, internals.schema.listener, 'Invalid event listener options');

    const name = criteria.name;
    const event = this._eventListeners[name];
    Hoek.assert(event, 'Unknown event ${name}');
    Hoek.assert(!criteria.channels || !event.flags.channels || Hoek.intersect(event.flags.channels, criteria.channels).length ===
criteria.channels.length, 'Unknown event channels ${criteria.channels && criteria.channels.join(', ')}');

    this._eventListeners[name].handlers = this._eventListeners[name].handlers || [];
    this._eventListeners[name].handlers.push(criteria);

    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_.super_.prototype.emit"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>emit (criteria, data, callback)](#apidoc.element.hapi.Server.super_.super_.prototype.emit)
- description and source-code
```javascript
emit = function (criteria, data, callback) {

    return this._emit(criteria, data, false, callback);
}
```
- example usage
```shell
...
for (let i = 0; i < vhosts.length; ++i) {
    const vhost = vhosts[i];
    const record = this._router.add({ method: route.method, path: route.path, vhost, analysis: route._analysis, id: route.settings
.id }, route);
    route.fingerprint = record.fingerprint;
    route.params = record.params;
}

this.emit('route', [route.public, this, plugin]);
};


internals.Connection.prototype._defaultRoutes = function () {

this._router.special('notFound', new Route({ method: '_special', path: '/{p*}', handler: internals.notFound }, this, this.server
, { special: true }));
this._router.special('badRequest', new Route({ method: '_special', path: '/{p*}', handler: internals.badRequest }, this, this.server
, { special: true }));
...
```

#### <a name="apidoc.element.hapi.Server.super_.super_.prototype.hasListeners"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>hasListeners (name)](#apidoc.element.hapi.Server.super_.super_.prototype.hasListeners)
- description and source-code
```javascript
hasListeners = function (name) {

    Hoek.assert(this._eventListeners[name], 'Unknown event ${name}');
    return !!this._eventListeners[name].handlers;
}
```
- example usage
```shell
...

    this._states[name] = state;
};


internals.Request.prototype._tap = function () {

    return (this.hasListeners('finish') || this.hasListeners('peek') ? new Response.Peek(this) : null);
};


internals.Request.prototype.generateResponse = function (source, options) {

    return new Response(source, this, options);
};
...
```

#### <a name="apidoc.element.hapi.Server.super_.super_.prototype.on"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>on (criteria, listener)](#apidoc.element.hapi.Server.super_.super_.prototype.on)
- description and source-code
```javascript
on = function (criteria, listener) {

    criteria = internals.criteria(criteria);
    criteria.listener = listener;

    if (criteria.filter &&
        (typeof criteria.filter === 'string' || Array.isArray(criteria.filter))) {

        criteria.filter = { tags: criteria.filter };
    }

    criteria = Joi.attempt(criteria, internals.schema.listener, 'Invalid event listener options');

    const name = criteria.name;
    const event = this._eventListeners[name];
    Hoek.assert(event, 'Unknown event ${name}');
    Hoek.assert(!criteria.channels || !event.flags.channels || Hoek.intersect(event.flags.channels, criteria.channels).length ===
criteria.channels.length, 'Unknown event channels ${criteria.channels && criteria.channels.join(', ')}');

    this._eventListeners[name].handlers = this._eventListeners[name].handlers || [];
    this._eventListeners[name].handlers.push(criteria);

    return this;
}
```
- example usage
```shell
...

this.plugins = {};                  // Registered plugin APIs by plugin name
this.app = {};                      // Place for application-specific state without conflicts with hapi, should not be used by plugins

// Create listener

this.listener = this.settings.listener || (this.settings.tls ? Https.createServer(this.settings.tls) : Http.createServer());
this.listener.on('request', this._dispatch());
this._init();

this.listener.on('clientError', (err, socket) => {

    this.server._log(['connection', 'client', 'error'], err);
});
...
```

#### <a name="apidoc.element.hapi.Server.super_.super_.prototype.once"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>once (criteria, listener)](#apidoc.element.hapi.Server.super_.super_.prototype.once)
- description and source-code
```javascript
once = function (criteria, listener) {

    criteria = internals.criteria(criteria);
    return this.on(Object.assign(criteria, { count: 1 }), listener);
}
```
- example usage
```shell
...



internals.Connection.prototype._init = function () {

    // Setup listener

    this.listener.once('listening', () => {

// Update the address, port, and uri with active values

if (this.type === 'tcp') {
    const address = this.listener.address();
    this.info.address = address.address;
    this.info.port = address.port;
...
```

#### <a name="apidoc.element.hapi.Server.super_.super_.prototype.registerEvent"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>registerEvent (events)](#apidoc.element.hapi.Server.super_.super_.prototype.registerEvent)
- description and source-code
```javascript
registerEvent = function (events) {

    events = Hoek.flatten([].concat(events));
    events.forEach((event) => {

        if (!event) {
            return;
        }

        if (event instanceof internals.Podium) {
            return this.registerPodium(event);
        }

        if (typeof event === 'string') {
            event = { name: event };
        }

        event = Joi.attempt(event, internals.schema.event, 'Invalid event options');

        const name = event.name;
        if (this._eventListeners[name]) {
            Hoek.assert(event.shared, 'Event ${name} exists');
            return;
        }

        this._eventListeners[name] = { handlers: null, flags: event };
        this._sourcePodiums.forEach((podium) => {

            if (!podium._eventListeners[name]) {
                podium._eventListeners[name] = { handlers: null, flags: event };
            }
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_.super_.prototype.registerPodium"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>registerPodium (podiums)](#apidoc.element.hapi.Server.super_.super_.prototype.registerPodium)
- description and source-code
```javascript
registerPodium = function (podiums) {

    [].concat(podiums).forEach((podium) => {

        if (podium._sourcePodiums.indexOf(this) !== -1) {
            return;
        }

        podium._sourcePodiums.push(this);
        Object.keys(podium._eventListeners).forEach((name) => {

            if (!this._eventListeners[name]) {
                this._eventListeners[name] = { handlers: null, flags: podium._eventListeners[name].flags };
            }
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_.super_.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>removeAllListeners (name)](#apidoc.element.hapi.Server.super_.super_.prototype.removeAllListeners)
- description and source-code
```javascript
removeAllListeners = function (name) {

    Hoek.assert(this._eventListeners[name], 'Unknown event ${name}');
    this._eventListeners[name].handlers = null;
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.Server.super_.super_.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">hapi.Server.super_.super_.prototype.</span>removeListener (name, listener)](#apidoc.element.hapi.Server.super_.super_.prototype.removeListener)
- description and source-code
```javascript
removeListener = function (name, listener) {

    Hoek.assert(this._eventListeners[name], 'Unknown event ${name}');
    Hoek.assert(typeof listener === 'function', 'Listener must be a function');

    const handlers = this._eventListeners[name].handlers;
    if (!handlers) {
        return this;
    }

    const filtered = handlers.filter((handler) => handler.listener !== listener);
    this._eventListeners[name].handlers = (filtered.length ? filtered : null);
    return this;
}
```
- example usage
```shell
...
    return callback(err);
};

this.listener.once('error', onError);

const finalize = () => {

    this.listener.removeListener('error', onError);
    callback();
};

if (this.type !== 'tcp') {
    this.listener.listen(this.settings.port, finalize);
}
else {
...
```



# <a name="apidoc.module.hapi.auth"></a>[module hapi.auth](#apidoc.module.hapi.auth)

#### <a name="apidoc.element.hapi.auth.auth"></a>[function <span class="apidocSignatureSpan">hapi.</span>auth (connection)](#apidoc.element.hapi.auth.auth)
- description and source-code
```javascript
auth = function (connection) {

    this.connection = connection;
    this._schemes = {};
    this._strategies = {};
    this.settings = {
        default: null           // Strategy used as default if route has no auth settings
    };

    this.api = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.auth.access"></a>[function <span class="apidocSignatureSpan">hapi.auth.</span>access (request, route)](#apidoc.element.hapi.auth.access)
- description and source-code
```javascript
access = function (request, route) {

    const auth = request.connection.auth;
    const config = auth.lookup(route);
    if (!config) {
        return true;
    }

    const credentials = request.auth.credentials;
    if (!credentials) {
        return false;
    }

    return !internals.access(request, config, credentials, 'bypass');
}
```
- example usage
```shell
...
}

const credentials = request.auth.credentials;
if (!credentials) {
    return false;
}

return !internals.access(request, config, credentials, 'bypass');
};


internals.Auth.prototype._authenticate = function (request, next) {

const config = this.lookup(request.route);
if (!config) {
...
```

#### <a name="apidoc.element.hapi.auth.authenticate"></a>[function <span class="apidocSignatureSpan">hapi.auth.</span>authenticate (request, next)](#apidoc.element.hapi.auth.authenticate)
- description and source-code
```javascript
authenticate = function (request, next) {

    const auth = request.connection.auth;
    return auth._authenticate(request, next);
}
```
- example usage
```shell
...
internals.Auth.prototype.test = function (name, request, next) {

Hoek.assert(name, 'Missing authentication strategy name');
const strategy = this._strategies[name];
Hoek.assert(strategy, 'Unknown authentication strategy:', name);

const reply = request.server._replier.interface(request, strategy.realm, { data: true }, (response) => next(response, reply._data
 && reply._data.credentials));
strategy.methods.authenticate(request, reply);
};


internals.Auth.prototype._setupRoute = function (options, path) {

if (!options) {
    return options;         // Preserve the difference between undefined and false
...
```

#### <a name="apidoc.element.hapi.auth.payload"></a>[function <span class="apidocSignatureSpan">hapi.auth.</span>payload (request, next)](#apidoc.element.hapi.auth.payload)
- description and source-code
```javascript
payload = function (request, next) {

    if (!request.auth.isAuthenticated ||
        request.auth.strategy === 'bypass') {

        return next();
    }

    const auth = request.connection.auth;
    const strategy = auth._strategies[request.auth.strategy];

    if (!strategy.methods.payload) {
        return next();
    }

    const config = auth.lookup(request.route);
    const setting = config.payload || (strategy.methods.options.payload ? 'required' : false);
    if (!setting) {
        return next();
    }

    const finalize = (response) => {

        if (response &&
            response.isBoom &&
            response.isMissing) {

            return next(setting === 'optional' ? null : Boom.unauthorized('Missing payload authentication'));
        }

        return next(response);
    };

    request._protect.run(finalize, (exit) => {

        const reply = request.server._replier.interface(request, strategy.realm, {}, exit);
        strategy.methods.payload(request, reply);
    });
}
```
- example usage
```shell
...

    return next(response);
};

request._protect.run(finalize, (exit) => {

    const reply = request.server._replier.interface(request, strategy.realm, {}, exit);
    strategy.methods.payload(request, reply);
});
};


internals.Auth.response = function (request, next) {

const auth = request.connection.auth;
...
```

#### <a name="apidoc.element.hapi.auth.response"></a>[function <span class="apidocSignatureSpan">hapi.auth.</span>response (request, next)](#apidoc.element.hapi.auth.response)
- description and source-code
```javascript
response = function (request, next) {

    const auth = request.connection.auth;
    const config = auth.lookup(request.route);
    if (!config ||
        !request.auth.isAuthenticated ||
        request.auth.strategy === 'bypass') {

        return next();
    }

    const strategy = auth._strategies[request.auth.strategy];
    if (!strategy.methods.response) {
        return next();
    }

    request._protect.run(next, (exit) => {

        const reply = request.server._replier.interface(request, strategy.realm, {}, exit);
        strategy.methods.response(request, reply);
    });
}
```
- example usage
```shell
...
if (!strategy.methods.response) {
    return next();
}

request._protect.run(next, (exit) => {

    const reply = request.server._replier.interface(request, strategy.realm, {}, exit);
    strategy.methods.response(request, reply);
});
};


internals.Authenticator = class {
constructor(config, request, manager) {
...
```



# <a name="apidoc.module.hapi.auth.prototype"></a>[module hapi.auth.prototype](#apidoc.module.hapi.auth.prototype)

#### <a name="apidoc.element.hapi.auth.prototype._authenticate"></a>[function <span class="apidocSignatureSpan">hapi.auth.prototype.</span>_authenticate (request, next)](#apidoc.element.hapi.auth.prototype._authenticate)
- description and source-code
```javascript
_authenticate = function (request, next) {

    const config = this.lookup(request.route);
    if (!config) {
        return next();
    }

    const authenticator = new internals.Authenticator(config, request, this);
    authenticator.authenticate(next);
}
```
- example usage
```shell
...
return route.settings.auth || this.settings.default;
};


internals.Auth.authenticate = function (request, next) {

const auth = request.connection.auth;
return auth._authenticate(request, next);
};


internals.Auth.access = function (request, route) {

const auth = request.connection.auth;
const config = auth.lookup(route);
...
```

#### <a name="apidoc.element.hapi.auth.prototype._setupRoute"></a>[function <span class="apidocSignatureSpan">hapi.auth.prototype.</span>_setupRoute (options, path)](#apidoc.element.hapi.auth.prototype._setupRoute)
- description and source-code
```javascript
_setupRoute = function (options, path) {

    if (!options) {
        return options;         // Preserve the difference between undefined and false
    }

    if (typeof options === 'string') {
        options = { strategies: [options] };
    }
    else if (options.strategy) {
        options.strategies = [options.strategy];
        delete options.strategy;
    }

    if (path &&
        !options.strategies) {

        Hoek.assert(this.settings.default, 'Route missing authentication strategy and no default defined:', path);
        options = Hoek.applyToDefaults(this.settings.default, options);
    }

    path = path || 'default strategy';
    Hoek.assert(options.strategies && options.strategies.length, 'Missing authentication strategy:', path);

    options.mode = options.mode || 'required';

    if (options.entity !== undefined ||                                             // Backwards compatibility with <= 11.x.x
        options.scope !== undefined) {

        options.access = [{ entity: options.entity, scope: options.scope }];
        delete options.entity;
        delete options.scope;
    }

    if (options.access) {
        for (let i = 0; i < options.access.length; ++i) {
            const access = options.access[i];
            access.scope = internals.setupScope(access);
        }
    }

    if (options.payload === true) {
        options.payload = 'required';
    }

    let hasAuthenticatePayload = false;
    for (let i = 0; i < options.strategies.length; ++i) {
        const name = options.strategies[i];
        const strategy = this._strategies[name];
        Hoek.assert(strategy, 'Unknown authentication strategy', name, 'in', path);

        Hoek.assert(strategy.methods.payload || options.payload !== 'required', 'Payload validation can only be required when all
 strategies support it in', path);
        hasAuthenticatePayload = hasAuthenticatePayload || strategy.methods.payload;
        Hoek.assert(!strategy.methods.options.payload || options.payload === undefined || options.payload === 'required', 'Cannot
 set authentication payload to', options.payload, 'when a strategy requires payload validation in', path);
    }

    Hoek.assert(!options.payload || hasAuthenticatePayload, 'Payload authentication requires at least one strategy with payload
support in', path);

    return options;
}
```
- example usage
```shell
...


internals.Auth.prototype.default = function (options) {

Hoek.assert(!this.settings.default, 'Cannot set default strategy more than once');
options = Schema.apply('auth', options, 'default strategy');

this.settings.default = this._setupRoute(Hoek.clone(options));      // Can change options
};


internals.Auth.prototype.test = function (name, request, next) {

Hoek.assert(name, 'Missing authentication strategy name');
const strategy = this._strategies[name];
...
```

#### <a name="apidoc.element.hapi.auth.prototype.default"></a>[function <span class="apidocSignatureSpan">hapi.auth.prototype.</span>default (options)](#apidoc.element.hapi.auth.prototype.default)
- description and source-code
```javascript
default = function (options) {

    Hoek.assert(!this.settings.default, 'Cannot set default strategy more than once');
    options = Schema.apply('auth', options, 'default strategy');

    this.settings.default = this._setupRoute(Hoek.clone(options));      // Can change options
}
```
- example usage
```shell
...
};

if (strategy.api) {
    this.api[name] = strategy.api;
}

if (mode) {
    this.default({ strategies: [name], mode: mode === true ? 'required' : mode });
}
};


internals.Auth.prototype.default = function (options) {

Hoek.assert(!this.settings.default, 'Cannot set default strategy more than once');
...
```

#### <a name="apidoc.element.hapi.auth.prototype.lookup"></a>[function <span class="apidocSignatureSpan">hapi.auth.prototype.</span>lookup (route)](#apidoc.element.hapi.auth.prototype.lookup)
- description and source-code
```javascript
lookup = function (route) {

    if (route.settings.auth === false) {
        return false;
    }

    return route.settings.auth || this.settings.default;
}
```
- example usage
```shell
...
return auth._authenticate(request, next);
};


internals.Auth.access = function (request, route) {

const auth = request.connection.auth;
const config = auth.lookup(route);
if (!config) {
    return true;
}

const credentials = request.auth.credentials;
if (!credentials) {
    return false;
...
```

#### <a name="apidoc.element.hapi.auth.prototype.scheme"></a>[function <span class="apidocSignatureSpan">hapi.auth.prototype.</span>scheme (name, scheme)](#apidoc.element.hapi.auth.prototype.scheme)
- description and source-code
```javascript
scheme = function (name, scheme) {

    Hoek.assert(name, 'Authentication scheme must have a name');
    Hoek.assert(!this._schemes[name], 'Authentication scheme name already exists:', name);
    Hoek.assert(typeof scheme === 'function', 'scheme must be a function:', name);

    this._schemes[name] = scheme;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.auth.prototype.strategy"></a>[function <span class="apidocSignatureSpan">hapi.auth.prototype.</span>strategy (name, scheme)](#apidoc.element.hapi.auth.prototype.strategy)
- description and source-code
```javascript
strategy = function (name, scheme) {

    const hasMode = (typeof arguments[2] === 'string' || typeof arguments[2] === 'boolean');
    const mode = (hasMode ? arguments[2] : false);
    const options = (hasMode ? arguments[3] : arguments[2]) || null;

    Hoek.assert(name, 'Authentication strategy must have a name');
    Hoek.assert(name !== 'bypass', 'Cannot use reserved strategy name: bypass');
    Hoek.assert(!this._strategies[name], 'Authentication strategy name already exists');
    Hoek.assert(scheme, 'Authentication strategy', name, 'missing scheme');
    Hoek.assert(this._schemes[scheme], 'Authentication strategy', name, 'uses unknown scheme:', scheme);

    const server = this.connection.server._clone([this.connection], '');
    const strategy = this._schemes[scheme](server, options);

    Hoek.assert(strategy.authenticate, 'Invalid scheme:', name, 'missing authenticate() method');
    Hoek.assert(typeof strategy.authenticate === 'function', 'Invalid scheme:', name, 'invalid authenticate() method');
    Hoek.assert(!strategy.payload || typeof strategy.payload === 'function', 'Invalid scheme:', name, 'invalid payload() method');
    Hoek.assert(!strategy.response || typeof strategy.response === 'function', 'Invalid scheme:', name, 'invalid response() method
');
    strategy.options = strategy.options || {};
    Hoek.assert(strategy.payload || !strategy.options.payload, 'Cannot require payload validation without a payload method');

    this._strategies[name] = {
        methods: strategy,
        realm: server.realm
    };

    if (strategy.api) {
        this.api[name] = strategy.api;
    }

    if (mode) {
        this.default({ strategies: [name], mode: mode === true ? 'required' : mode });
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.auth.prototype.test"></a>[function <span class="apidocSignatureSpan">hapi.auth.prototype.</span>test (name, request, next)](#apidoc.element.hapi.auth.prototype.test)
- description and source-code
```javascript
test = function (name, request, next) {

    Hoek.assert(name, 'Missing authentication strategy name');
    const strategy = this._strategies[name];
    Hoek.assert(strategy, 'Unknown authentication strategy:', name);

    const reply = request.server._replier.interface(request, strategy.realm, { data: true }, (response) => next(response, reply.
_data && reply._data.credentials));
    strategy.methods.authenticate(request, reply);
}
```
- example usage
```shell
...
    const prefix = value[0];
    const type = (prefix === '+' ? 'required' : (prefix === '!' ? 'forbidden' : 'selection'));
    const clean = (type === 'selection' ? value : value.slice(1));
    scope[type] = scope[type] || [];
    scope[type].push(clean);

    if ((!scope._parameters || !scope._parameters[type]) &&
        /{([^}]+)}/.test(clean)) {

        scope._parameters = scope._parameters || {};
        scope._parameters[type] = true;
    }
}

return scope;
...
```



# <a name="apidoc.module.hapi.compression"></a>[module hapi.compression](#apidoc.module.hapi.compression)

#### <a name="apidoc.element.hapi.compression.compression"></a>[function <span class="apidocSignatureSpan">hapi.</span>compression ()](#apidoc.element.hapi.compression.compression)
- description and source-code
```javascript
compression = function () {

    this.encodings = ['identity', 'gzip', 'deflate'];
    this._encoders = {
        identity: null,
        gzip: (options) => Zlib.createGzip(options),
        deflate: (options) => Zlib.createDeflate(options)
    };

    this._decoders = {
        gzip: (options) => Zlib.createGunzip(options),
        deflate: (options) => Zlib.createInflate(options)
    };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.hapi.compression.prototype"></a>[module hapi.compression.prototype](#apidoc.module.hapi.compression.prototype)

#### <a name="apidoc.element.hapi.compression.prototype.accept"></a>[function <span class="apidocSignatureSpan">hapi.compression.prototype.</span>accept (request)](#apidoc.element.hapi.compression.prototype.accept)
- description and source-code
```javascript
accept = function (request) {

    return Accept.encoding(request.headers['accept-encoding'], this.encodings);
}
```
- example usage
```shell
...
this.info = {
    received: now,
    responded: 0,
    remoteAddress: req.connection.remoteAddress,
    remotePort: req.connection.remotePort || '',
    referrer: req.headers.referrer || req.headers.referer || '',
    host: req.headers.host ? req.headers.host.replace(/\s/g, '') : '',
    acceptEncoding: this.connection._compression.accept(this)
};

this.info.hostname = this.info.host.split(':')[0];

// Assigned elsewhere:

this.orig = {};
...
```

#### <a name="apidoc.element.hapi.compression.prototype.addDecoder"></a>[function <span class="apidocSignatureSpan">hapi.compression.prototype.</span>addDecoder (encoding, decoder)](#apidoc.element.hapi.compression.prototype.addDecoder)
- description and source-code
```javascript
addDecoder = function (encoding, decoder) {

    Hoek.assert(this._decoders[encoding] === undefined, 'Cannot override existing decoder for ${encoding}');
    Hoek.assert(typeof decoder === 'function', 'Invalid decoder function for ${encoding}');
    this._decoders[encoding] = decoder;
}
```
- example usage
```shell
...

    return match.route.public;
};


internals.Connection.prototype.decoder = function (encoding, decoder) {

    return this._compression.addDecoder(encoding, decoder);
};


internals.Connection.prototype.encoder = function (encoding, encoder) {

    return this._compression.addEncoder(encoding, encoder);
};
...
```

#### <a name="apidoc.element.hapi.compression.prototype.addEncoder"></a>[function <span class="apidocSignatureSpan">hapi.compression.prototype.</span>addEncoder (encoding, encoder)](#apidoc.element.hapi.compression.prototype.addEncoder)
- description and source-code
```javascript
addEncoder = function (encoding, encoder) {

    Hoek.assert(this._encoders[encoding] === undefined, 'Cannot override existing encoder for ${encoding}');
    Hoek.assert(typeof encoder === 'function', 'Invalid encoder function for ${encoding}');
    this._encoders[encoding] = encoder;
    this.encodings.push(encoding);
}
```
- example usage
```shell
...

return this._compression.addDecoder(encoding, decoder);
};


internals.Connection.prototype.encoder = function (encoding, encoder) {

return this._compression.addEncoder(encoding, encoder);
};


internals.Connection.prototype._ext = function (event) {

const type = event.type;
Hoek.assert(this._extensions[type], 'Unknown event type', type);
...
```

#### <a name="apidoc.element.hapi.compression.prototype.encoder"></a>[function <span class="apidocSignatureSpan">hapi.compression.prototype.</span>encoder (request, encoding)](#apidoc.element.hapi.compression.prototype.encoder)
- description and source-code
```javascript
encoder = function (request, encoding) {

    const encoder = this._encoders[encoding];
    Hoek.assert(encoder !== undefined, 'Unknown encoding ${encoding}');
    return encoder(request.route.settings.compression[encoding]);
}
```
- example usage
```shell
...
length !== 0 &&
response.statusCode !== 206 &&
response._isPayloadSupported()) {

delete response.headers['content-length'];
response._header('content-encoding', encoding);

compressor = request.connection._compression.encoder(request, encoding);
    }

    if ((response.headers['content-encoding'] || encoding) &&
response.headers.etag &&
response.settings.varyEtag) {

response.headers.etag = response.headers.etag.slice(0, -1) + '-' + (response.headers['content-encoding'] || encoding) + '"';
...
```

#### <a name="apidoc.element.hapi.compression.prototype.encoding"></a>[function <span class="apidocSignatureSpan">hapi.compression.prototype.</span>encoding (response)](#apidoc.element.hapi.compression.prototype.encoding)
- description and source-code
```javascript
encoding = function (response) {

    const request = response.request;
    if (!request.connection.settings.compression) {
        return null;
    }

    const mime = request.server.mime.type(response.headers['content-type'] || 'application/octet-stream');
    if (!mime.compressible) {
        return null;
    }

    response.vary('accept-encoding');

    if (response.headers['content-encoding']) {
        return null;
    }

    return (request.info.acceptEncoding === 'identity' ? null : request.info.acceptEncoding);
}
```
- example usage
```shell
...
Hoek.assert(typeof decoder === 'function', 'Invalid decoder function for ${encoding}');
this._decoders[encoding] = decoder;
};


internals.Compression.prototype.accept = function (request) {

return Accept.encoding(request.headers['accept-encoding'], this.encodings);
};


internals.Compression.prototype.encoding = function (response) {

const request = response.request;
if (!request.connection.settings.compression) {
...
```



# <a name="apidoc.module.hapi.connection"></a>[module hapi.connection](#apidoc.module.hapi.connection)

#### <a name="apidoc.element.hapi.connection.connection"></a>[function <span class="apidocSignatureSpan">hapi.</span>connection (server, options)](#apidoc.element.hapi.connection.connection)
- description and source-code
```javascript
connection = function (server, options) {

    const now = Date.now();

    Podium.call(this, internals.Connection._events);

    this.settings = options;                                                        // options cloned in server.connection()
    this.server = server;

    // Normalize settings

    this.settings.labels = Hoek.unique(this.settings.labels || []);                 // Remove duplicates
    if (this.settings.port === undefined) {
        this.settings.port = 0;
    }

    this.type = (typeof this.settings.port === 'string' ? 'socket' : 'tcp');
    if (this.type === 'socket') {
        this.settings.port = (this.settings.port.indexOf('/') !== -1 ? Path.resolve(this.settings.port) : this.settings.port.toLowerCase
());
    }

    if (this.settings.autoListen === undefined) {
        this.settings.autoListen = true;
    }

    Hoek.assert(this.settings.autoListen || !this.settings.port, 'Cannot specify port when autoListen is false');
    Hoek.assert(this.settings.autoListen || !this.settings.address, 'Cannot specify address when autoListen is false');

    // Connection facilities

    this._started = false;
    this._connections = {};
    this._onConnection = null;          // Used to remove event listener on stop
    this.registrations = {};            // Tracks plugin for dependency validation { name -> { version } }

    this._extensions = {
        onRequest: new Ext('onRequest', this.server),
        onPreAuth: new Ext('onPreAuth', this.server),
        onPostAuth: new Ext('onPostAuth', this.server),
        onPreHandler: new Ext('onPreHandler', this.server),
        onPostHandler: new Ext('onPostHandler', this.server),
        onPreResponse: new Ext('onPreResponse', this.server)
    };

    this._requestCounter = { value: internals.counter.min, min: internals.counter.min, max: internals.counter.max };
    this._load = server._heavy.policy(this.settings.load);
    this._compression = new Compression();
    this.states = new Statehood.Definitions(this.settings.state);
    this.auth = new Auth(this);
    this._router = new Call.Router(this.settings.router);
    this._defaultRoutes();

    this.plugins = {};                  // Registered plugin APIs by plugin name
    this.app = {};                      // Place for application-specific state without conflicts with hapi, should not be used
by plugins

    // Create listener

    this.listener = this.settings.listener || (this.settings.tls ? Https.createServer(this.settings.tls) : Http.createServer());
    this.listener.on('request', this._dispatch());
    this._init();

    this.listener.on('clientError', (err, socket) => {

        this.server._log(['connection', 'client', 'error'], err);
    });

    // Connection information

    this.info = {
        created: now,
        started: 0,
        host: this.settings.host || Os.hostname() || 'localhost',
        port: this.settings.port,
        protocol: this.type === 'tcp' ? (this.settings.tls ? 'https' : 'http') : this.type,
        id: Os.hostname() + ':' + process.pid + ':' + now.toString(36)
    };

    this.info.uri = (this.settings.uri || (this.info.protocol + ':' + (this.type === 'tcp' ? '//' + this.info.host + (this.info.
port ? ':' + this.info.port : '') : this.info.port)));

    this.on('route', Cors.options);
}
```
- example usage
```shell
...

exports = module.exports = internals.Connection = function (server, options) {

const now = Date.now();

Podium.call(this, internals.Connection._events);

this.settings = options;                                                        // options cloned in server.connection()
this.server = server;

// Normalize settings

this.settings.labels = Hoek.unique(this.settings.labels || []);                 // Remove duplicates
if (this.settings.port === undefined) {
    this.settings.port = 0;
...
```

#### <a name="apidoc.element.hapi.connection.super_"></a>[function <span class="apidocSignatureSpan">hapi.connection.</span>super_ (events)](#apidoc.element.hapi.connection.super_)
- description and source-code
```javascript
super_ = function (events) {

    // Use descriptive names to avoid conflict when inherited

    this._eventListeners = Object.create(null);
    this._notificationsQueue = [];
    this._eventsProcessing = false;
    this._sourcePodiums = [];

    if (events) {
        this.registerEvent(events);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.hapi.connection.prototype"></a>[module hapi.connection.prototype](#apidoc.module.hapi.connection.prototype)

#### <a name="apidoc.element.hapi.connection.prototype._addRoute"></a>[function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>_addRoute (config, plugin)](#apidoc.element.hapi.connection.prototype._addRoute)
- description and source-code
```javascript
_addRoute = function (config, plugin) {

    const route = new Route(config, this, plugin);                // Do no use config beyond this point, use route members
    const vhosts = [].concat(route.settings.vhost || '*');

    for (let i = 0; i < vhosts.length; ++i) {
        const vhost = vhosts[i];
        const record = this._router.add({ method: route.method, path: route.path, vhost, analysis: route._analysis, id: route.settings
.id }, route);
        route.fingerprint = record.fingerprint;
        route.params = record.params;
    }

    this.emit('route', [route.public, this, plugin]);
}
```
- example usage
```shell
...

        if (Array.isArray(config.method)) {
            for (let j = 0; j < config.method.length; ++j) {
                const method = config.method[j];

                const settings = Hoek.shallow(config);
                settings.method = method;
                this._addRoute(settings, plugin);
            }
        }
        else {
            this._addRoute(config, plugin);
        }
    }
};
...
```

#### <a name="apidoc.element.hapi.connection.prototype._defaultRoutes"></a>[function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>_defaultRoutes ()](#apidoc.element.hapi.connection.prototype._defaultRoutes)
- description and source-code
```javascript
_defaultRoutes = function () {

    this._router.special('notFound', new Route({ method: '_special', path: '/{p*}', handler: internals.notFound }, this, this.server
, { special: true }));
    this._router.special('badRequest', new Route({ method: '_special', path: '/{p*}', handler: internals.badRequest }, this, this
.server, { special: true }));

    if (this.settings.routes.cors) {
        Cors.handler(this);
    }
}
```
- example usage
```shell
...

this._requestCounter = { value: internals.counter.min, min: internals.counter.min, max: internals.counter.max };
this._load = server._heavy.policy(this.settings.load);
this._compression = new Compression();
this.states = new Statehood.Definitions(this.settings.state);
this.auth = new Auth(this);
this._router = new Call.Router(this.settings.router);
this._defaultRoutes();

this.plugins = {};                  // Registered plugin APIs by plugin name
this.app = {};                      // Place for application-specific state without conflicts with hapi, should not be used by plugins

// Create listener

this.listener = this.settings.listener || (this.settings.tls ? Https.createServer(this.settings.tls) : Http.createServer());
...
```

#### <a name="apidoc.element.hapi.connection.prototype._dispatch"></a>[function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>_dispatch (options)](#apidoc.element.hapi.connection.prototype._dispatch)
- description and source-code
```javascript
_dispatch = function (options) {

    options = options || {};

    return (req, res) => {

        // Track socket request processing state

        if (req.socket) {
            req.socket._isHapiProcessing = true;
            res.on('finish', () => {

                req.socket._isHapiProcessing = false;
                if (!this._started) {
                    req.socket.end();
                }
            });
        }

        // Create request

        const request = this.server._requestor.request(this, req, res, options);

        // Check load

        const overload = this._load.check();
        if (overload) {
            this.server._log(['load'], this.server.load);
            request._reply(overload);
        }
        else {

            // Execute request lifecycle

            request._protect.enter(() => {

                request._execute();
            });
        }
    };
}
```
- example usage
```shell
...

this.plugins = {};                  // Registered plugin APIs by plugin name
this.app = {};                      // Place for application-specific state without conflicts with hapi, should not be used by plugins

// Create listener

this.listener = this.settings.listener || (this.settings.tls ? Https.createServer(this.settings.tls) : Http.createServer());
this.listener.on('request', this._dispatch());
this._init();

this.listener.on('clientError', (err, socket) => {

    this.server._log(['connection', 'client', 'error'], err);
});
...
```

#### <a name="apidoc.element.hapi.connection.prototype._ext"></a>[function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>_ext (event)](#apidoc.element.hapi.connection.prototype._ext)
- description and source-code
```javascript
_ext = function (event) {

    const type = event.type;
    Hoek.assert(this._extensions[type], 'Unknown event type', type);
    this._extensions[type].add(event);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.connection.prototype._init"></a>[function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>_init ()](#apidoc.element.hapi.connection.prototype._init)
- description and source-code
```javascript
_init = function () {

    // Setup listener

    this.listener.once('listening', () => {

        // Update the address, port, and uri with active values

        if (this.type === 'tcp') {
            const address = this.listener.address();
            this.info.address = address.address;
            this.info.port = address.port;
            this.info.uri = (this.settings.uri || (this.info.protocol + '://' + this.info.host + ':' + this.info.port));
        }

        this._onConnection = (connection) => {

            const key = connection.remoteAddress + ':' + connection.remotePort;
            this._connections[key] = connection;

            connection.once('close', () => {

                delete this._connections[key];
            });
        };

        this.listener.on(this.settings.tls ? 'secureConnection' : 'connection', this._onConnection);
    });
}
```
- example usage
```shell
...
this.plugins = {};                  // Registered plugin APIs by plugin name
this.app = {};                      // Place for application-specific state without conflicts with hapi, should not be used by plugins

// Create listener

this.listener = this.settings.listener || (this.settings.tls ? Https.createServer(this.settings.tls) : Http.createServer());
this.listener.on('request', this._dispatch());
this._init();

this.listener.on('clientError', (err, socket) => {

    this.server._log(['connection', 'client', 'error'], err);
});

// Connection information
...
```

#### <a name="apidoc.element.hapi.connection.prototype._route"></a>[function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>_route (configs, plugin)](#apidoc.element.hapi.connection.prototype._route)
- description and source-code
```javascript
_route = function (configs, plugin) {

    configs = [].concat(configs);
    for (let i = 0; i < configs.length; ++i) {
        const config = configs[i];

        if (Array.isArray(config.method)) {
            for (let j = 0; j < config.method.length; ++j) {
                const method = config.method[j];

                const settings = Hoek.shallow(config);
                settings.method = method;
                this._addRoute(settings, plugin);
            }
        }
        else {
            this._addRoute(config, plugin);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.connection.prototype._start"></a>[function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>_start (callback)](#apidoc.element.hapi.connection.prototype._start)
- description and source-code
```javascript
_start = function (callback) {

    if (this._started) {
        return process.nextTick(callback);
    }

    this._started = true;
    this.info.started = Date.now();

    if (!this.settings.autoListen) {
        return process.nextTick(callback);
    }

    const onError = (err) => {

        this._started = false;
        return callback(err);
    };

    this.listener.once('error', onError);

    const finalize = () => {

        this.listener.removeListener('error', onError);
        callback();
    };

    if (this.type !== 'tcp') {
        this.listener.listen(this.settings.port, finalize);
    }
    else {
        const address = this.settings.address || this.settings.host || '0.0.0.0';
        this.listener.listen(this.settings.port, address, finalize);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.connection.prototype._stop"></a>[function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>_stop (options, callback)](#apidoc.element.hapi.connection.prototype._stop)
- description and source-code
```javascript
_stop = function (options, callback) {

    if (!this._started) {
        return process.nextTick(callback);
    }

    this._started = false;
    this.info.started = 0;

    const timeoutId = setTimeout(() => {

        Object.keys(this._connections).forEach((key) => {

            this._connections[key].destroy();
        });


        this._connections = {};
    }, options.timeout);

    this.listener.close(() => {

        this.listener.removeListener(this.settings.tls ? 'secureConnection' : 'connection', this._onConnection);
        clearTimeout(timeoutId);

        this._init();
        return callback();
    });

    // Tell idle keep-alive connections to close

    Object.keys(this._connections).forEach((key) => {

        const connection = this._connections[key];
        if (!connection._isHapiProcessing) {
            connection.end();
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.connection.prototype.decoder"></a>[function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>decoder (encoding, decoder)](#apidoc.element.hapi.connection.prototype.decoder)
- description and source-code
```javascript
decoder = function (encoding, decoder) {

    return this._compression.addDecoder(encoding, decoder);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.connection.prototype.encoder"></a>[function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>encoder (encoding, encoder)](#apidoc.element.hapi.connection.prototype.encoder)
- description and source-code
```javascript
encoder = function (encoding, encoder) {

    return this._compression.addEncoder(encoding, encoder);
}
```
- example usage
```shell
...
length !== 0 &&
response.statusCode !== 206 &&
response._isPayloadSupported()) {

delete response.headers['content-length'];
response._header('content-encoding', encoding);

compressor = request.connection._compression.encoder(request, encoding);
    }

    if ((response.headers['content-encoding'] || encoding) &&
response.headers.etag &&
response.settings.varyEtag) {

response.headers.etag = response.headers.etag.slice(0, -1) + '-' + (response.headers['content-encoding'] || encoding) + '"';
...
```

#### <a name="apidoc.element.hapi.connection.prototype.inject"></a>[function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>inject (options, callback)](#apidoc.element.hapi.connection.prototype.inject)
- description and source-code
```javascript
inject = function (options, callback) {

    if (!callback) {
        return new Promise((resolve, reject) => this.inject(options, (res) => resolve(res)));
    }

    let settings = options;
    if (typeof settings === 'string') {
        settings = { url: settings };
    }

    if (!settings.authority ||
        settings.credentials ||
        settings.app ||
        settings.plugins ||
        settings.allowInternals !== undefined) {        // Can be false

        settings = Hoek.shallow(settings);              // options can be reused
        delete settings.credentials;
        delete settings.artifacts;                      // Cannot appear without credentials
        delete settings.app;
        delete settings.plugins;
        delete settings.allowInternals;

        settings.authority = settings.authority || (this.info.host + ':' + this.info.port);
    }

    const needle = this._dispatch({
        credentials: options.credentials,
        artifacts: options.artifacts,
        allowInternals: options.allowInternals,
        app: options.app,
        plugins: options.plugins
    });

    Shot.inject(needle, settings, (res) => {

        if (res.raw.res._hapi) {
            res.result = res.raw.res._hapi.result;
            res.request = res.raw.res._hapi.request;
            delete res.raw.res._hapi;
        }

        if (res.result === undefined) {
            res.result = res.payload;
        }

        return callback(res);
    });
}
```
- example usage
```shell
...
};
};


internals.Connection.prototype.inject = function (options, callback) {

if (!callback) {
    return new Promise((resolve, reject) => this.inject(options, (res) => resolve(res)));
}

let settings = options;
if (typeof settings === 'string') {
    settings = { url: settings };
}
...
```

#### <a name="apidoc.element.hapi.connection.prototype.lookup"></a>[function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>lookup (id)](#apidoc.element.hapi.connection.prototype.lookup)
- description and source-code
```javascript
lookup = function (id) {

    Hoek.assert(id && typeof id === 'string', 'Invalid route id:', id);

    const record = this._router.ids[id];
    if (!record) {
        return null;
    }

    return record.route.public;
}
```
- example usage
```shell
...
return auth._authenticate(request, next);
};


internals.Auth.access = function (request, route) {

const auth = request.connection.auth;
const config = auth.lookup(route);
if (!config) {
    return true;
}

const credentials = request.auth.credentials;
if (!credentials) {
    return false;
...
```

#### <a name="apidoc.element.hapi.connection.prototype.match"></a>[function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>match (method, path, host)](#apidoc.element.hapi.connection.prototype.match)
- description and source-code
```javascript
match = function (method, path, host) {

    Hoek.assert(method && typeof method === 'string', 'Invalid method:', method);
    Hoek.assert(path && typeof path === 'string' && path[0] === '/', 'Invalid path:', path);
    Hoek.assert(!host || typeof host === 'string', 'Invalid host:', host);

    const match = this._router.route(method.toLowerCase(), path, host);
    Hoek.assert(match !== this._router.specials.badRequest, 'Invalid path:', path);
    if (match === this._router.specials.notFound) {
        return null;
    }

    return match.route.public;
}
```
- example usage
```shell
...
const method = request.headers['access-control-request-method'];
if (!method) {
    return reply(Boom.notFound('CORS error: Missing Access-Control-Request-Method header'));
}

// Lookup route

const route = request.connection.match(method, request.path, request.info.hostname);
if (!route) {
    return reply(Boom.notFound());
}

const settings = route.settings.cors;
if (!settings) {
    return reply({ message: 'CORS is disabled for this route' });
...
```

#### <a name="apidoc.element.hapi.connection.prototype.table"></a>[function <span class="apidocSignatureSpan">hapi.connection.prototype.</span>table (host)](#apidoc.element.hapi.connection.prototype.table)
- description and source-code
```javascript
table = function (host) {

    return this._router.table(host);
}
```
- example usage
```shell
...
    return callback(res);
});
};


internals.Connection.prototype.table = function (host) {

return this._router.table(host);
};


internals.Connection.prototype.lookup = function (id) {

Hoek.assert(id && typeof id === 'string', 'Invalid route id:', id);
...
```



# <a name="apidoc.module.hapi.cors"></a>[module hapi.cors](#apidoc.module.hapi.cors)

#### <a name="apidoc.element.hapi.cors.handler"></a>[function <span class="apidocSignatureSpan">hapi.cors.</span>handler (connection)](#apidoc.element.hapi.cors.handler)
- description and source-code
```javascript
handler = function (connection) {

    Route = Route || require('./route');

    if (connection._router.specials.options) {
        return;
    }

    const route = new Route({ method: '_special', path: '/{p*}', handler: internals.handler }, connection, connection.server, {
special: true });
    connection._router.special('options', route);
}
```
- example usage
```shell
...

internals.Connection.prototype._defaultRoutes = function () {

this._router.special('notFound', new Route({ method: '_special', path: '/{p*}', handler: internals.notFound }, this, this.server
, { special: true }));
this._router.special('badRequest', new Route({ method: '_special', path: '/{p*}', handler: internals.badRequest }, this, this.server
, { special: true }));

if (this.settings.routes.cors) {
    Cors.handler(this);
}
};


internals.notFound = function (request, reply) {

return reply(Boom.notFound());
...
```

#### <a name="apidoc.element.hapi.cors.headers"></a>[function <span class="apidocSignatureSpan">hapi.cors.</span>headers (response)](#apidoc.element.hapi.cors.headers)
- description and source-code
```javascript
headers = function (response) {

    const request = response.request;
    if (request._route._special) {
        return;
    }

    const settings = request.route.settings.cors;
    if (!settings) {
        return;
    }

    response.vary('origin');

    if (!request.info.cors.isOriginMatch) {
        return;
    }

    response._header('access-control-allow-origin', request.headers.origin);

    if (settings.credentials) {
        response._header('access-control-allow-credentials', 'true');
    }

    if (settings._exposedHeaders) {
        response._header('access-control-expose-headers', settings._exposedHeaders, { append: true });
    }
}
```
- example usage
```shell
...
};


internals.marshal = function (request, next) {

    const response = request.response;

    Cors.headers(response);
    internals.content(response, false);
    internals.security(response);
    internals.unmodified(response);

    internals.state(response, (err) => {

if (err) {
...
```

#### <a name="apidoc.element.hapi.cors.matchOrigin"></a>[function <span class="apidocSignatureSpan">hapi.cors.</span>matchOrigin (origin, settings)](#apidoc.element.hapi.cors.matchOrigin)
- description and source-code
```javascript
matchOrigin = function (origin, settings) {

    if (!origin) {
        return false;
    }

    if (settings._origin === true) {
        return true;
    }

    if (settings._origin.qualified.indexOf(origin) !== -1) {
        return true;
    }

    for (let i = 0; i < settings._origin.wildcards.length; ++i) {
        if (origin.match(settings._origin.wildcards[i])) {
            return true;
        }
    }

    return false;
}
```
- example usage
```shell
...
const settings = route.settings.cors;
if (!settings) {
    return reply({ message: 'CORS is disabled for this route' });
}

// Validate Origin header

if (!exports.matchOrigin(origin, settings)) {
    return reply({ message: 'CORS error: Origin not allowed' });
}

// Validate allowed headers

let headers = request.headers['access-control-request-headers'];
if (headers) {
...
```

#### <a name="apidoc.element.hapi.cors.options"></a>[function <span class="apidocSignatureSpan">hapi.cors.</span>options (route, connection, server)](#apidoc.element.hapi.cors.options)
- description and source-code
```javascript
options = function (route, connection, server) {

    if (route.method === 'options' ||
        !route.settings.cors) {

        return;
    }

    exports.handler(connection);
}
```
- example usage
```shell
...


internals.cachePolicy = Joi.object({
cache: Joi.string().allow(null).allow(''),
segment: Joi.string(),
shared: Joi.boolean()
})
.options({ allowUnknown: true });               // Catbox validates other keys


internals.method = Joi.object({
bind: Joi.object().allow(null),
generateKey: Joi.func(),
cache: internals.cachePolicy,
callback: Joi.boolean()
...
```

#### <a name="apidoc.element.hapi.cors.route"></a>[function <span class="apidocSignatureSpan">hapi.cors.</span>route (options)](#apidoc.element.hapi.cors.route)
- description and source-code
```javascript
route = function (options) {

    const settings = Hoek.applyToDefaults(Defaults.cors, options);
    if (!settings) {
        return false;
    }

    settings._headers = settings.headers.concat(settings.additionalHeaders);
    settings._headersString = settings._headers.join(',');
    for (let i = 0; i < settings._headers.length; ++i) {
        settings._headers[i] = settings._headers[i].toLowerCase();
    }

    if (settings._headers.indexOf('origin') === -1) {
        settings._headers.push('origin');
    }

    settings._exposedHeaders = settings.exposedHeaders.concat(settings.additionalExposedHeaders).join(',');

    if (settings.origin.indexOf('*') !== -1) {
        Hoek.assert(settings.origin.length === 1, 'Cannot specify cors.origin * together with other values');
        settings._origin = true;
    }
    else {
        settings._origin = {
            qualified: [],
            wildcards: []
        };

        for (let i = 0; i < settings.origin.length; ++i) {
            const origin = settings.origin[i];
            if (origin.indexOf('*') !== -1) {
                settings._origin.wildcards.push(new RegExp('^' + Hoek.escapeRegex(origin).replace(/\\\*/g, '.*').replace(/\\\?/g
, '.') + '$'));
            }
            else {
                settings._origin.qualified.push(origin);
            }
        }
    }

    return settings;
}
```
- example usage
```shell
...

internals.Connection.prototype.match = function (method, path, host) {

    Hoek.assert(method && typeof method === 'string', 'Invalid method:', method);
    Hoek.assert(path && typeof path === 'string' && path[0] === '/', 'Invalid path:', path);
    Hoek.assert(!host || typeof host === 'string', 'Invalid host:', host);

    const match = this._router.route(method.toLowerCase(), path, host);
    Hoek.assert(match !== this._router.specials.badRequest, 'Invalid path:', path);
    if (match === this._router.specials.notFound) {
        return null;
    }

    return match.route.public;
};
...
```



# <a name="apidoc.module.hapi.ext"></a>[module hapi.ext](#apidoc.module.hapi.ext)

#### <a name="apidoc.element.hapi.ext.ext"></a>[function <span class="apidocSignatureSpan">hapi.</span>ext (type, server)](#apidoc.element.hapi.ext.ext)
- description and source-code
```javascript
ext = function (type, server) {

    this._topo = new Topo();
    this._server = server;
    this._routes = [];

    this.type = type;
    this.nodes = null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.hapi.ext.prototype"></a>[module hapi.ext.prototype](#apidoc.module.hapi.ext.prototype)

#### <a name="apidoc.element.hapi.ext.prototype.add"></a>[function <span class="apidocSignatureSpan">hapi.ext.prototype.</span>add (event)](#apidoc.element.hapi.ext.prototype.add)
- description and source-code
```javascript
add = function (event) {

    const methods = [].concat(event.method);
    const options = event.options;

    for (let i = 0; i < methods.length; ++i) {
        const settings = {
            before: options.before,
            after: options.after,
            group: event.plugin.realm.plugin,
            sort: this._server._extensionsSeq++
        };

        const node = {
            func: methods[i],                 // Connection: function (request, next), Server: function (server, next)
            bind: options.bind,
            plugin: event.plugin
        };

        this._topo.add(node, settings);
    }

    this.nodes = this._topo.nodes;

    // Notify routes

    for (let i = 0; i < this._routes.length; ++i) {
        this._routes[i].rebuild(event);
    }
}
```
- example usage
```shell
...
};


internals.Connection.prototype._ext = function (event) {

const type = event.type;
Hoek.assert(this._extensions[type], 'Unknown event type', type);
this._extensions[type].add(event);
};


internals.Connection.prototype._route = function (configs, plugin) {

configs = [].concat(configs);
for (let i = 0; i < configs.length; ++i) {
...
```

#### <a name="apidoc.element.hapi.ext.prototype.merge"></a>[function <span class="apidocSignatureSpan">hapi.ext.prototype.</span>merge (others)](#apidoc.element.hapi.ext.prototype.merge)
- description and source-code
```javascript
merge = function (others) {

    const merge = [];
    for (let i = 0; i < others.length; ++i) {
        merge.push(others[i]._topo);
    }

    this._topo.merge(merge);
    this.nodes = (this._topo.nodes.length ? this._topo.nodes : null);
}
```
- example usage
```shell
...
internals.Ext.prototype.merge = function (others) {

const merge = [];
for (let i = 0; i < others.length; ++i) {
    merge.push(others[i]._topo);
}

this._topo.merge(merge);
this.nodes = (this._topo.nodes.length ? this._topo.nodes : null);
};


internals.Ext.prototype.subscribe = function (route) {

this._routes.push(route);
...
```

#### <a name="apidoc.element.hapi.ext.prototype.subscribe"></a>[function <span class="apidocSignatureSpan">hapi.ext.prototype.</span>subscribe (route)](#apidoc.element.hapi.ext.prototype.subscribe)
- description and source-code
```javascript
subscribe = function (route) {

    this._routes.push(route);
}
```
- example usage
```shell
...
    }

    const connection = this.connection._extensions[type];
    const realm = this.plugin.realm._extensions[type];

    ext.merge([connection, realm]);

    connection.subscribe(this);
    realm.subscribe(this);

    return ext;
};


internals.Route.prototype.rebuild = function (event) {
...
```



# <a name="apidoc.module.hapi.handler"></a>[module hapi.handler](#apidoc.module.hapi.handler)

#### <a name="apidoc.element.hapi.handler.configure"></a>[function <span class="apidocSignatureSpan">hapi.handler.</span>configure (handler, route)](#apidoc.element.hapi.handler.configure)
- description and source-code
```javascript
configure = function (handler, route) {

    if (typeof handler === 'object') {
        const type = Object.keys(handler)[0];
        const serverHandler = route.server._handlers[type];

        Hoek.assert(serverHandler, 'Unknown handler:', type);

        return serverHandler(route.public, handler[type]);
    }

    if (typeof handler === 'string') {
        const parsed = internals.fromString('handler', handler, route.server);
        return parsed.method;
    }

    return handler;
}
```
- example usage
```shell
...
            security._xframe = security.xframe.rule.toUpperCase();
        }
    }
}

// Handler

this.settings.handler = Handler.configure(this.settings.handler, this);
this._prerequisites = Handler.prerequisitesConfig(this.settings.pre, this.server);

// Route lifecycle

this._extensions = {
    onPreResponse: this._combineExtensions('onPreResponse')
};
...
```

#### <a name="apidoc.element.hapi.handler.defaults"></a>[function <span class="apidocSignatureSpan">hapi.handler.</span>defaults (method, handler, server)](#apidoc.element.hapi.handler.defaults)
- description and source-code
```javascript
defaults = function (method, handler, server) {

    let defaults = null;

    if (typeof handler === 'object') {
        const type = Object.keys(handler)[0];
        const serverHandler = server._handlers[type];

        Hoek.assert(serverHandler, 'Unknown handler:', type);

        if (serverHandler.defaults) {
            defaults = (typeof serverHandler.defaults === 'function' ? serverHandler.defaults(method) : serverHandler.defaults);
        }
    }

    return defaults || {};
}
```
- example usage
```shell
...
    if (typeof handler === 'object') {
        const type = Object.keys(handler)[0];
        const serverHandler = server._handlers[type];

        Hoek.assert(serverHandler, 'Unknown handler:', type);

        if (serverHandler.defaults) {
            defaults = (typeof serverHandler.defaults === 'function' ? serverHandler.defaults(method) : serverHandler.defaults);
        }
    }

    return defaults || {};
};
...
```

#### <a name="apidoc.element.hapi.handler.execute"></a>[function <span class="apidocSignatureSpan">hapi.handler.</span>execute (request, next)](#apidoc.element.hapi.handler.execute)
- description and source-code
```javascript
execute = function (request, next) {

    const finalize = (err, result) => {

        request._setResponse(err || result);
        return next();                              // Must not include an argument
    };

    request._protect.run(finalize, (exit) => {

        if (request._route._prerequisites) {
            internals.prerequisites(request, Hoek.once(exit));
        }
        else {
            internals.handler(request, exit);
        }
    });
}
```
- example usage
```shell
...

if (this.request.auth.credentials) {
    return this.validate(null, { credentials: this.request.auth.credentials, artifacts: this.request.auth.artifacts }, next);
}

// Authenticate

return this.execute(next);
    }

    execute(next) {

const config = this.config;
const request = this.request;
...
```

#### <a name="apidoc.element.hapi.handler.prerequisitesConfig"></a>[function <span class="apidocSignatureSpan">hapi.handler.</span>prerequisitesConfig (config, server)](#apidoc.element.hapi.handler.prerequisitesConfig)
- description and source-code
```javascript
prerequisitesConfig = function (config, server) {

    if (!config) {
        return null;
    }

<span class="apidocCodeCommentSpan">    /*
        [
            [
                function (request, reply) { },
                {
                    method: function (request, reply) { }
                    assign: key1
                },
                {
                    method: function (request, reply) { },
                    assign: key2
                }
            ],
            'user(params.id)'
        ]
    */
</span>
    const prerequisites = [];

    for (let i = 0; i < config.length; ++i) {
        const pres = [].concat(config[i]);

        const set = [];
        for (let j = 0; j < pres.length; ++j) {
            let pre = pres[j];
            if (typeof pre !== 'object') {
                pre = { method: pre };
            }

            const item = {
                method: pre.method,
                assign: pre.assign,
                failAction: pre.failAction || 'error'
            };

            if (typeof item.method === 'string') {
                const parsed = internals.fromString('pre', item.method, server);
                item.method = parsed.method;
                item.assign = item.assign || parsed.name;
            }

            set.push(internals.pre(item));
        }

        prerequisites.push(set);
    }

    return prerequisites.length ? prerequisites : null;
}
```
- example usage
```shell
...
        }
    }
}

// Handler

this.settings.handler = Handler.configure(this.settings.handler, this);
this._prerequisites = Handler.prerequisitesConfig(this.settings.pre, this.server);

// Route lifecycle

this._extensions = {
    onPreResponse: this._combineExtensions('onPreResponse')
};
...
```



# <a name="apidoc.module.hapi.methods"></a>[module hapi.methods](#apidoc.module.hapi.methods)

#### <a name="apidoc.element.hapi.methods.methods"></a>[function <span class="apidocSignatureSpan">hapi.</span>methods (server)](#apidoc.element.hapi.methods.methods)
- description and source-code
```javascript
methods = function (server) {

    this.server = server;
    this.methods = {};
    this._normalized = {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.hapi.methods.prototype"></a>[module hapi.methods.prototype](#apidoc.module.hapi.methods.prototype)

#### <a name="apidoc.element.hapi.methods.prototype._add"></a>[function <span class="apidocSignatureSpan">hapi.methods.prototype.</span>_add (name, method, options, realm)](#apidoc.element.hapi.methods.prototype._add)
- description and source-code
```javascript
_add = function (name, method, options, realm) {

    Hoek.assert(typeof method === 'function', 'method must be a function');
    Hoek.assert(typeof name === 'string', 'name must be a string');
    Hoek.assert(name.match(exports.methodNameRx), 'Invalid name:', name);
    Hoek.assert(!Hoek.reach(this.methods, name, { functions: false }), 'Server method function name already exists:', name);

    options = Schema.apply('method', options || {}, name);

    const settings = Hoek.cloneWithShallow(options, ['bind']);
    settings.generateKey = settings.generateKey || internals.generateKey;
    const bind = settings.bind || realm.settings.bind || null;

    const apply = function () {

        return method.apply(bind, arguments);
    };

    const bound = bind ? apply : method;

    // Normalize methods

    let normalized = bound;
    if (settings.callback === false) {                                          // Defaults to true
        normalized = function (/* arg1, arg2, ..., argn, methodNext */) {

            const args = [];
            for (let i = 0; i < arguments.length - 1; ++i) {
                args.push(arguments[i]);
            }

            const methodNext = arguments[arguments.length - 1];

            let result = null;
            let error = null;

            try {
                result = method.apply(bind, args);
            }
            catch (err) {
                error = err;
            }

            if (result instanceof Error) {
                error = result;
                result = null;
            }

            if (error ||
                typeof result !== 'object' ||
                typeof result.then !== 'function') {

                return methodNext(error, result);
            }

            // Promise object

            const onFulfilled = (outcome) => methodNext(null, outcome);
            const onRejected = (err) => methodNext(err);
            result.then(onFulfilled, onRejected);
        };
    }

    // Not cached

    if (!settings.cache) {
        return this._assign(name, bound, normalized);
    }

    // Cached

    Hoek.assert(!settings.cache.generateFunc, 'Cannot set generateFunc with method caching:', name);
    Hoek.assert(settings.cache.generateTimeout !== undefined, 'Method caching requires a timeout value in generateTimeout:', name
);

    settings.cache.generateFunc = (id, next) => {

        id.args.push(next);                     // function (err, result, ttl)
        normalized.apply(bind, id.args);
    };

    const cache = this.server.cache(settings.cache, '#' + name);

    const func = function (/* arguments, methodNext */) {

        const args = [];
        for (let i = 0; i < arguments.length - 1; ++i) {
            args.push(arguments[i]);
        }

        const methodNext = arguments[arguments.length - 1];

        const key = settings.generateKey.apply(bind, args);
        if (key === null ||                                 // Value can be ''
            typeof key !== 'string') {                      // When using custom generateKey

            return Hoek.nextTick(methodNext)(Boom.badImplementation('Invalid method key when invoking: ' + name, { name, args }));
        }

        cache.get({ id: key, args }, methodNext);
    };

    func.cache = {
        drop: function (/* arguments, callback */) {

            const args = [];
            for (let i = 0; i < arguments.length - 1; ++i) {
                args.push(arguments[i]);
            }

            const methodNext = arguments[arguments.length - 1];

            const key = settings.generateKey.apply(null, args);
            if (key === null) {                             // Value can be ''
                return Hoek.nextTick(methodNext)(Boom.badImplementation('Invalid method key'));
            }

            return cache.drop(key, methodNext);
        },
        stats: cache.stats
    };

    this._assign(name, func, func);
}
```
- example usage
```shell
...
this._normalized = {};
};


internals.Methods.prototype.add = function (name, method, options, realm) {

if (typeof name !== 'object') {
    return this._add(name, method, options, realm);
}

// {} or [{}, {}]

const items = [].concat(name);
for (let i = 0; i < items.length; ++i) {
    const item = Schema.apply('methodObject', items[i]);
...
```

#### <a name="apidoc.element.hapi.methods.prototype._assign"></a>[function <span class="apidocSignatureSpan">hapi.methods.prototype.</span>_assign (name, method, normalized)](#apidoc.element.hapi.methods.prototype._assign)
- description and source-code
```javascript
_assign = function (name, method, normalized) {

    const path = name.split('.');
    let ref = this.methods;
    for (let i = 0; i < path.length; ++i) {
        if (!ref[path[i]]) {
            ref[path[i]] = (i + 1 === path.length ? method : {});
        }

        ref = ref[path[i]];
    }

    this._normalized[name] = normalized;
}
```
- example usage
```shell
...
        result.then(onFulfilled, onRejected);
    };
}

// Not cached

if (!settings.cache) {
    return this._assign(name, bound, normalized);
}

// Cached

Hoek.assert(!settings.cache.generateFunc, 'Cannot set generateFunc with method caching:', name);
Hoek.assert(settings.cache.generateTimeout !== undefined, 'Method caching requires a timeout value in generateTimeout:', name);
...
```

#### <a name="apidoc.element.hapi.methods.prototype.add"></a>[function <span class="apidocSignatureSpan">hapi.methods.prototype.</span>add (name, method, options, realm)](#apidoc.element.hapi.methods.prototype.add)
- description and source-code
```javascript
add = function (name, method, options, realm) {

    if (typeof name !== 'object') {
        return this._add(name, method, options, realm);
    }

    // {} or [{}, {}]

    const items = [].concat(name);
    for (let i = 0; i < items.length; ++i) {
        const item = Schema.apply('methodObject', items[i]);
        this._add(item.name, item.method, item.options, realm);
    }
}
```
- example usage
```shell
...
};


internals.Connection.prototype._ext = function (event) {

const type = event.type;
Hoek.assert(this._extensions[type], 'Unknown event type', type);
this._extensions[type].add(event);
};


internals.Connection.prototype._route = function (configs, plugin) {

configs = [].concat(configs);
for (let i = 0; i < configs.length; ++i) {
...
```



# <a name="apidoc.module.hapi.promises"></a>[module hapi.promises](#apidoc.module.hapi.promises)

#### <a name="apidoc.element.hapi.promises.wrap"></a>[function <span class="apidocSignatureSpan">hapi.promises.</span>wrap (bind, method, args)](#apidoc.element.hapi.promises.wrap)
- description and source-code
```javascript
wrap = function (bind, method, args) {

    return new Promise((resolve, reject) => {

        const callback = (err, result) => {

            if (err) {
                return reject(err);
            }

            return resolve(result);
        };

        method.apply(bind, args ? args.concat(callback) : [callback]);
    });
}
```
- example usage
```shell
...

internals.handler = function (request, callback) {

    const timer = new Hoek.Bench();
    const finalize = (response) => {

if (response === null) {                            // reply.continue()
    response = Response.wrap(null, request);
    return response._prepare(finalize);
}

// Check for Error result

if (response.isBoom) {
    request._log(['handler', 'error'], { msec: timer.elapsed(), error: response.message, data: response });
...
```



# <a name="apidoc.module.hapi.protect"></a>[module hapi.protect](#apidoc.module.hapi.protect)

#### <a name="apidoc.element.hapi.protect.protect"></a>[function <span class="apidocSignatureSpan">hapi.</span>protect (request)](#apidoc.element.hapi.protect.protect)
- description and source-code
```javascript
protect = function (request) {

    this._error = null;
    this.logger = request;                          // Replaced with server when request completes

    if (!request.server.settings.useDomains) {
        this.domain = null;
        return;
    }

    Domain = Domain || require('domain');

    this.domain = Domain.create();
    this.domain.on('error', (err) => {

        return this._onError(err);
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.hapi.protect.prototype"></a>[module hapi.protect.prototype](#apidoc.module.hapi.protect.prototype)

#### <a name="apidoc.element.hapi.protect.prototype._onError"></a>[function <span class="apidocSignatureSpan">hapi.protect.prototype.</span>_onError (err)](#apidoc.element.hapi.protect.prototype._onError)
- description and source-code
```javascript
_onError = function (err) {

    const handler = this._error;
    if (handler) {
        this._error = null;
        return handler(err);
    }

    this.logger._log(['internal', 'implementation', 'error'], err);
}
```
- example usage
```shell
...
}

Domain = Domain || require('domain');

this.domain = Domain.create();
this.domain.on('error', (err) => {

    return this._onError(err);
});
};


internals.Protect.prototype._onError = function (err) {

const handler = this._error;
...
```

#### <a name="apidoc.element.hapi.protect.prototype.enter"></a>[function <span class="apidocSignatureSpan">hapi.protect.prototype.</span>enter (func)](#apidoc.element.hapi.protect.prototype.enter)
- description and source-code
```javascript
enter = function (func) {

    if (!this.domain) {
        return func();
    }

    this.domain.run(func);
}
```
- example usage
```shell
...
            this.server._log(['load'], this.server.load);
            request._reply(overload);
        }
        else {

            // Execute request lifecycle

            request._protect.enter(() => {

                request._execute();
            });
        }
    };
};
...
```

#### <a name="apidoc.element.hapi.protect.prototype.reset"></a>[function <span class="apidocSignatureSpan">hapi.protect.prototype.</span>reset ()](#apidoc.element.hapi.protect.prototype.reset)
- description and source-code
```javascript
reset = function () {

    this._error = null;
}
```
- example usage
```shell
...
return this._finalize();
    }

    if (exit) {                                             // Can be a valid response or error (if returned from an ext, already
 handled because this.response is also set)
this._setResponse(Response.wrap(exit, this));
    }

    this._protect.reset();

    const transmit = (err) => {

if (err) {                                          // Can be valid response or error
    this._setResponse(Response.wrap(err, this));
}
...
```

#### <a name="apidoc.element.hapi.protect.prototype.run"></a>[function <span class="apidocSignatureSpan">hapi.protect.prototype.</span>run (next, enter)](#apidoc.element.hapi.protect.prototype.run)
- description and source-code
```javascript
run = function (next, enter) {              // enter: function (exit)

    const finish = Hoek.once((arg0, arg1, arg2) => {

        this._error = null;
        return next(arg0, arg1, arg2);
    });

    if (this.domain) {
        this._error = (err) => {

            return finish(Boom.badImplementation('Uncaught error', err));
        };
    }

    return enter(finish);
}
```
- example usage
```shell
...

            return next(setting === 'optional' ? null : Boom.unauthorized('Missing payload authentication'));
        }

        return next(response);
    };

    request._protect.run(finalize, (exit) => {

        const reply = request.server._replier.interface(request, strategy.realm, {}, exit);
        strategy.methods.payload(request, reply);
    });
};
...
```



# <a name="apidoc.module.hapi.reply"></a>[module hapi.reply](#apidoc.module.hapi.reply)

#### <a name="apidoc.element.hapi.reply.reply"></a>[function <span class="apidocSignatureSpan">hapi.</span>reply ()](#apidoc.element.hapi.reply.reply)
- description and source-code
```javascript
reply = function () {

    this._decorations = null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.hapi.reply.prototype"></a>[module hapi.reply.prototype](#apidoc.module.hapi.reply.prototype)

#### <a name="apidoc.element.hapi.reply.prototype.decorate"></a>[function <span class="apidocSignatureSpan">hapi.reply.prototype.</span>decorate (property, method)](#apidoc.element.hapi.reply.prototype.decorate)
- description and source-code
```javascript
decorate = function (property, method) {

    Hoek.assert(!this._decorations || !this._decorations[property], 'Reply interface decoration already defined:', property);
    Hoek.assert(['request', 'response', 'close', 'state', 'unstate', 'redirect', 'continue'].indexOf(property) === -1, 'Cannot override
 built-in reply interface decoration:', property);

    this._decorations = this._decorations || {};
    this._decorations[property] = method;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.reply.prototype.interface"></a>[function <span class="apidocSignatureSpan">hapi.reply.prototype.</span>interface (request, realm, options, next)](#apidoc.element.hapi.reply.prototype.interface)
- description and source-code
```javascript
interface = function (request, realm, options, next) {        // next(err || response, data);

    const reply = (err, response, data) => {

        Hoek.assert(data === undefined || options.data, 'Reply interface does not allow a third argument');

        reply._data = data;                 // Held for later
        return reply.response(err !== null && err !== undefined ? err : response);
    };

    reply._settings = options;
    reply._replied = false;
    reply._next = Hoek.once(next);

    reply.realm = realm;
    reply.request = request;

    reply.close = internals.close;
    reply.continue = internals.continue;
    reply.state = internals.state;
    reply.unstate = internals.unstate;
    reply.redirect = internals.redirect;
    reply.response = internals.response;
    reply.entity = internals.entity;

    if (this._decorations) {
        const methods = Object.keys(this._decorations);
        for (let i = 0; i < methods.length; ++i) {
            const method = methods[i];
            reply[method] = this._decorations[method];
        }
    }

    return reply;
}
```
- example usage
```shell
...

internals.Auth.prototype.test = function (name, request, next) {

Hoek.assert(name, 'Missing authentication strategy name');
const strategy = this._strategies[name];
Hoek.assert(strategy, 'Unknown authentication strategy:', name);

const reply = request.server._replier.interface(request, strategy.realm, { data: true }, (response) => next(response, reply._data
 && reply._data.credentials));
strategy.methods.authenticate(request, reply);
};


internals.Auth.prototype._setupRoute = function (options, path) {

if (!options) {
...
```



# <a name="apidoc.module.hapi.request"></a>[module hapi.request](#apidoc.module.hapi.request)

#### <a name="apidoc.element.hapi.request.request"></a>[function <span class="apidocSignatureSpan">hapi.</span>request ()](#apidoc.element.hapi.request.request)
- description and source-code
```javascript
request = function () {

    this._decorations = null;
}
```
- example usage
```shell
...
            req.socket.end();
        }
    });
}

// Create request

const request = this.server._requestor.request(this, req, res, options);

// Check load

const overload = this._load.check();
if (overload) {
    this.server._log(['load'], this.server.load);
    request._reply(overload);
...
```



# <a name="apidoc.module.hapi.request.prototype"></a>[module hapi.request.prototype](#apidoc.module.hapi.request.prototype)

#### <a name="apidoc.element.hapi.request.prototype.decorate"></a>[function <span class="apidocSignatureSpan">hapi.request.prototype.</span>decorate (property, method, options)](#apidoc.element.hapi.request.prototype.decorate)
- description and source-code
```javascript
decorate = function (property, method, options) {

    options = options || {};

    Hoek.assert(!this._decorations || this._decorations[property] === undefined, 'Request interface decoration already defined:',
property);
    Hoek.assert(internals.properties.indexOf(property) === -1, 'Cannot override built-in request interface decoration:', property
);

    this._decorations = this._decorations || {};
    this._decorations[property] = { method, apply: options.apply };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.request.prototype.request"></a>[function <span class="apidocSignatureSpan">hapi.request.prototype.</span>request (connection, req, res, options)](#apidoc.element.hapi.request.prototype.request)
- description and source-code
```javascript
request = function (connection, req, res, options) {

    const request = new internals.Request(connection, req, res, options);

    // Decorate

    if (this._decorations) {
        const properties = Object.keys(this._decorations);
        for (let i = 0; i < properties.length; ++i) {
            const property = properties[i];
            const assignment = this._decorations[property];
            request[property] = (assignment.apply ? assignment.method(request) : assignment.method);
        }
    }

    return request;
}
```
- example usage
```shell
...
            req.socket.end();
        }
    });
}

// Create request

const request = this.server._requestor.request(this, req, res, options);

// Check load

const overload = this._load.check();
if (overload) {
    this.server._log(['load'], this.server.load);
    request._reply(overload);
...
```



# <a name="apidoc.module.hapi.response"></a>[module hapi.response](#apidoc.module.hapi.response)

#### <a name="apidoc.element.hapi.response.response"></a>[function <span class="apidocSignatureSpan">hapi.</span>response (source, request, options)](#apidoc.element.hapi.response.response)
- description and source-code
```javascript
response = function (source, request, options) {

    Podium.call(this, ['finish', { name: 'peek', spread: true }]);

    options = options || {};

    this.request = request;
    this.statusCode = null;
    this.headers = {};                          // Incomplete as some headers are stored in flags
    this.variety = null;
    this.source = null;
    this.app = {};
    this.plugins = {};
    this.send = null;                           // Set by reply()
    this.hold = null;                           // Set by reply()

    this.settings = {
        encoding: 'utf8',
        charset: 'utf-8',                       // '-' required by IANA
        ttl: null,
        stringify: null,                        // JSON.stringify options
        passThrough: true,
        varyEtag: false,
        message: null
    };

    this._payload = null;                       // Readable stream
    this._takeover = false;
    this._contentEncoding = null;               // Set during transmit
    this._contentType = null;                   // Used if no explicit content-type is set and type is known
    this._error = null;                         // The boom object when created from an error

    this._processors = {
        marshal: options.marshal,
        prepare: options.prepare,
        close: options.close
    };

    this._setSource(source, options.variety);
}
```
- example usage
```shell
...
if (!strategy.methods.response) {
    return next();
}

request._protect.run(next, (exit) => {

    const reply = request.server._replier.interface(request, strategy.realm, {}, exit);
    strategy.methods.response(request, reply);
});
};


internals.Authenticator = class {
constructor(config, request, manager) {
...
```

#### <a name="apidoc.element.hapi.response.Payload"></a>[function <span class="apidocSignatureSpan">hapi.response.</span>Payload (payload, options)](#apidoc.element.hapi.response.Payload)
- description and source-code
```javascript
Payload = function (payload, options) {

    Stream.Readable.call(this);
    this._data = payload;
    this._prefix = null;
    this._suffix = null;
    this._sizeOffset = 0;
    this._encoding = options.encoding;
}
```
- example usage
```shell
...
        payload = payload + suffix;
    }
}
else if (this.settings.stringify) {
    return next(Boom.badImplementation('Cannot set formatting options on non object response'));
}

this._payload = new internals.Payload(payload, this.settings);
return next();
};


internals.Response.prototype._tap = function () {

return (this.hasListeners('finish') || this.hasListeners('peek') ? new internals.Peek(this) : null);
...
```

#### <a name="apidoc.element.hapi.response.Peek"></a>[function <span class="apidocSignatureSpan">hapi.response.</span>Peek (podium)](#apidoc.element.hapi.response.Peek)
- description and source-code
```javascript
Peek = function (podium) {

    Stream.Transform.call(this);
    this._podium = podium;
    this.once('finish', () => {

        podium.emit('finish');
    });
}
```
- example usage
```shell
...

    this._states[name] = state;
};


internals.Request.prototype._tap = function () {

    return (this.hasListeners('finish') || this.hasListeners('peek') ? new Response.Peek(this) : null);
};


internals.Request.prototype.generateResponse = function (source, options) {

    return new Response(source, this, options);
};
...
```

#### <a name="apidoc.element.hapi.response.super_"></a>[function <span class="apidocSignatureSpan">hapi.response.</span>super_ (events)](#apidoc.element.hapi.response.super_)
- description and source-code
```javascript
super_ = function (events) {

    // Use descriptive names to avoid conflict when inherited

    this._eventListeners = Object.create(null);
    this._notificationsQueue = [];
    this._eventsProcessing = false;
    this._sourcePodiums = [];

    if (events) {
        this.registerEvent(events);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.response.unmodified"></a>[function <span class="apidocSignatureSpan">hapi.response.</span>unmodified (request, options)](#apidoc.element.hapi.response.unmodified)
- description and source-code
```javascript
unmodified = function (request, options) {

    if (request.method !== 'get' &&
        request.method !== 'head') {

        return false;
    }

    // Strong verifier

    if (options.etag &&
        request.headers['if-none-match']) {

        const ifNoneMatch = request.headers['if-none-match'].split(/\s*,\s*/);
        for (let i = 0; i < ifNoneMatch.length; ++i) {
            const etag = ifNoneMatch[i];
            if (etag === options.etag) {
                return true;
            }

            if (options.vary) {
                const etagBase = options.etag.slice(0, -1);
                const encoders = request.connection._compression.encodings;
                for (let j = 0; j < encoders.length; ++j) {
                    if (etag === etagBase + '-${encoders[j]}"') {
                        return true;
                    }
                }
            }
        }

        return false;
    }

    // Weak verifier

    const ifModifiedSinceHeader = request.headers['if-modified-since'];

    if (ifModifiedSinceHeader &&
        options.modified) {

        const ifModifiedSince = internals.parseDate(ifModifiedSinceHeader);
        const lastModified = internals.parseDate(options.modified);

        if (ifModifiedSince &&
            lastModified &&
            ifModifiedSince >= lastModified) {

            return true;
        }
    }

    return false;
}
```
- example usage
```shell
...
internals.entity = function (options) {

    Hoek.assert(options, 'Entity method missing required options');
    Hoek.assert(options.etag || options.modified, 'Entity methods missing require options key');

    this.request._entity = options;

    if (Response.unmodified(this.request, options)) {
        return this.response().code(304).takeover();
    }

    return null;
};
...
```

#### <a name="apidoc.element.hapi.response.wrap"></a>[function <span class="apidocSignatureSpan">hapi.response.</span>wrap (result, request)](#apidoc.element.hapi.response.wrap)
- description and source-code
```javascript
wrap = function (result, request) {

    return (result instanceof Error ? Boom.wrap(result)
                                    : (result instanceof internals.Response ? result
                                                                            : new internals.Response(result, request)));
}
```
- example usage
```shell
...

internals.handler = function (request, callback) {

    const timer = new Hoek.Bench();
    const finalize = (response) => {

if (response === null) {                            // reply.continue()
    response = Response.wrap(null, request);
    return response._prepare(finalize);
}

// Check for Error result

if (response.isBoom) {
    request._log(['handler', 'error'], { msec: timer.elapsed(), error: response.message, data: response });
...
```



# <a name="apidoc.module.hapi.response.prototype"></a>[module hapi.response.prototype](#apidoc.module.hapi.response.prototype)

#### <a name="apidoc.element.hapi.response.prototype._close"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_close ()](#apidoc.element.hapi.response.prototype._close)
- description and source-code
```javascript
_close = function () {

    if (this._processors.close) {
        this._processors.close(this);
    }

    const stream = this._payload || this.source;
    if (stream instanceof Stream) {
        if (stream.close) {
            stream.close();
        }
        else if (stream.destroy) {
            stream.destroy();
        }
        else {
            const read = () => {

                stream.read();
            };

            const end = () => {

                stream.removeListener('readable', read);
                stream.removeListener('error', end);
                stream.removeListener('end', end);
            };

            stream.on('readable', read);
            stream.once('error', end);
            stream.once('end', end);
        }
    }
}
```
- example usage
```shell
...
    this.raw.req.removeListener('end', this._onEnd);
    this.raw.req.removeListener('close', this._onClose);
    this.raw.req.removeListener('error', this._onError);

    if (this.response &&
        this.response._close) {

        this.response._close();
    }

    this._protect.logger = this.server;
};


internals.Request.prototype._setResponse = function (response) {
...
```

#### <a name="apidoc.element.hapi.response.prototype._header"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_header (key, value, options)](#apidoc.element.hapi.response.prototype._header)
- description and source-code
```javascript
_header = function (key, value, options) {

    options = options || {};
    const append = options.append || false;
    const separator = options.separator || ',';
    const override = options.override !== false;
    const duplicate = options.duplicate !== false;

    if ((!append && override) ||
        !this.headers[key]) {

        this.headers[key] = value;
    }
    else if (override) {
        if (key === 'set-cookie') {
            this.headers[key] = [].concat(this.headers[key], value);
        }
        else {
            const existing = this.headers[key];
            if (!duplicate) {
                const values = existing.split(separator);
                for (let i = 0; i < values.length; ++i) {
                    if (values[i] === value) {
                        return this;
                    }
                }
            }

            this.headers[key] = existing + separator + value;
        }
    }

    return this;
}
```
- example usage
```shell
...
        return reply({ message: 'CORS error: Some headers are not allowed' });
    }
}

// Reply with the route CORS headers

const response = reply();
response._header('access-control-allow-origin', request.headers.origin);
response._header('access-control-allow-methods', method);
response._header('access-control-allow-headers', settings._headersString);
response._header('access-control-max-age', settings.maxAge);

if (settings.credentials) {
    response._header('access-control-allow-credentials', 'true');
}
...
```

#### <a name="apidoc.element.hapi.response.prototype._isPayloadSupported"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_isPayloadSupported ()](#apidoc.element.hapi.response.prototype._isPayloadSupported)
- description and source-code
```javascript
_isPayloadSupported = function () {

    return (this.request.method !== 'head' && this.statusCode !== 304 && this.statusCode !== 204);
}
```
- example usage
```shell
...
request._log(['state', 'response', 'error'], err);
request._states = {};                                           // Clear broken state
return next(err);
        }

        internals.cache(response);

        if (!response._isPayloadSupported() &&
request.method !== 'head') {

// Set empty stream

response._close();                                  // Close unused file streams
response._payload = new internals.Empty();
delete response.headers['content-length'];
...
```

#### <a name="apidoc.element.hapi.response.prototype._isRewritable"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_isRewritable ()](#apidoc.element.hapi.response.prototype._isRewritable)
- description and source-code
```javascript
_isRewritable = function () {

    return this.statusCode === 301 || this.statusCode === 302;
}
```
- example usage
```shell
...
return this.statusCode === 301 || this.statusCode === 302;
};


internals.Response.prototype._setTemporary = function (isTemporary) {

if (isTemporary) {
    if (this._isRewritable()) {
        this.statusCode = 302;
    }
    else {
        this.statusCode = 307;
    }
}
else {
...
```

#### <a name="apidoc.element.hapi.response.prototype._isTemporary"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_isTemporary ()](#apidoc.element.hapi.response.prototype._isTemporary)
- description and source-code
```javascript
_isTemporary = function () {

    return this.statusCode === 302 || this.statusCode === 307;
}
```
- example usage
```shell
...
}
};


internals.Response.prototype._setRewritable = function (isRewritable) {

if (isRewritable) {
    if (this._isTemporary()) {
        this.statusCode = 302;
    }
    else {
        this.statusCode = 301;
    }
}
else {
...
```

#### <a name="apidoc.element.hapi.response.prototype._marshal"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_marshal (next)](#apidoc.element.hapi.response.prototype._marshal)
- description and source-code
```javascript
_marshal = function (next) {

    if (!this._processors.marshal) {
        return this._streamify(this.source, next);
    }

    this._processors.marshal(this, (err, source) => {

        if (err) {
            return next(err);
        }

        return this._streamify(source, next);
    });
}
```
- example usage
```shell
...

response._close();                                  // Close unused file streams
response._payload = new internals.Empty();
delete response.headers['content-length'];
return Auth.response(request, next);                // Must be last in case requires access to headers
        }

        response._marshal((err) => {

if (err) {
    return next(Boom.wrap(err));
}

if (request.jsonp &&
    response._payload.jsonp) {
...
```

#### <a name="apidoc.element.hapi.response.prototype._passThrough"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_passThrough ()](#apidoc.element.hapi.response.prototype._passThrough)
- description and source-code
```javascript
_passThrough = function () {

    if (this.variety === 'stream' &&
        this.settings.passThrough) {

        if (this.source.statusCode &&
            !this.statusCode) {

            this.statusCode = this.source.statusCode;                        // Stream is an HTTP response
        }

        if (this.source.headers) {
            let headerKeys = Object.keys(this.source.headers);

            if (headerKeys.length) {
                const localHeaders = this.headers;
                this.headers = {};

                for (let i = 0; i < headerKeys.length; ++i) {
                    const key = headerKeys[i];
                    this.header(key.toLowerCase(), Hoek.clone(this.source.headers[key]));     // Clone arrays
                }

                headerKeys = Object.keys(localHeaders);
                for (let i = 0; i < headerKeys.length; ++i) {
                    const key = headerKeys[i];
                    this.header(key, localHeaders[key], { append: key === 'set-cookie' });
                }
            }
        }
    }

    this.statusCode = this.statusCode || 200;
}
```
- example usage
```shell
...
this._takeover = true;
return this;
};


internals.Response.prototype._prepare = function (next) {

this._passThrough();

if (this.variety !== 'promise') {
    return this._processPrepare(next);
}

const onDone = Hoek.nextTick((source) => {
...
```

#### <a name="apidoc.element.hapi.response.prototype._permanent"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_permanent (isPermanent)](#apidoc.element.hapi.response.prototype._permanent)
- description and source-code
```javascript
_permanent = function (isPermanent) {

    this._setTemporary(isPermanent === false);           // Defaults to true
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.response.prototype._prepare"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_prepare (next)](#apidoc.element.hapi.response.prototype._prepare)
- description and source-code
```javascript
_prepare = function (next) {

    this._passThrough();

    if (this.variety !== 'promise') {
        return this._processPrepare(next);
    }

    const onDone = Hoek.nextTick((source) => {

        if (source instanceof Error) {
            return next(Boom.wrap(source));
        }

        if (source instanceof internals.Response) {
            return source._processPrepare(next);
        }

        this._setSource(source);
        this._passThrough();
        this._processPrepare(next);
    });

    const onError = (source) => {

        if (!(source instanceof Error)) {
            const err = new Error('Rejected promise');
            err.data = source;
            return next(Boom.wrap(err));
        }

        return next(Boom.wrap(source));
    };

    this.source.then(onDone, onError);
}
```
- example usage
```shell
...
internals.handler = function (request, callback) {

    const timer = new Hoek.Bench();
    const finalize = (response) => {

if (response === null) {                            // reply.continue()
    response = Response.wrap(null, request);
    return response._prepare(finalize);
}

// Check for Error result

if (response.isBoom) {
    request._log(['handler', 'error'], { msec: timer.elapsed(), error: response.message, data: response });
    return callback(response);
...
```

#### <a name="apidoc.element.hapi.response.prototype._processPrepare"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_processPrepare (next)](#apidoc.element.hapi.response.prototype._processPrepare)
- description and source-code
```javascript
_processPrepare = function (next) {

    if (!this._processors.prepare) {
        return next(this);
    }

    return this._processors.prepare(this, next);
}
```
- example usage
```shell
...


internals.Response.prototype._prepare = function (next) {

    this._passThrough();

    if (this.variety !== 'promise') {
return this._processPrepare(next);
    }

    const onDone = Hoek.nextTick((source) => {

if (source instanceof Error) {
    return next(Boom.wrap(source));
}
...
```

#### <a name="apidoc.element.hapi.response.prototype._rewritable"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_rewritable (isRewritable)](#apidoc.element.hapi.response.prototype._rewritable)
- description and source-code
```javascript
_rewritable = function (isRewritable) {

    this._setRewritable(isRewritable !== false);         // Defaults to true
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.response.prototype._setRewritable"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_setRewritable (isRewritable)](#apidoc.element.hapi.response.prototype._setRewritable)
- description and source-code
```javascript
_setRewritable = function (isRewritable) {

    if (isRewritable) {
        if (this._isTemporary()) {
            this.statusCode = 302;
        }
        else {
            this.statusCode = 301;
        }
    }
    else {
        if (this._isTemporary()) {
            this.statusCode = 307;
        }
        else {
            this.statusCode = 308;
        }
    }
}
```
- example usage
```shell
...
this._setTemporary(isPermanent === false);           // Defaults to true
return this;
};


internals.Response.prototype._rewritable = function (isRewritable) {

this._setRewritable(isRewritable !== false);         // Defaults to true
return this;
};


internals.Response.prototype._isTemporary = function () {

return this.statusCode === 302 || this.statusCode === 307;
...
```

#### <a name="apidoc.element.hapi.response.prototype._setSource"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_setSource (source, variety)](#apidoc.element.hapi.response.prototype._setSource)
- description and source-code
```javascript
_setSource = function (source, variety) {

    // Method must not set any headers or other properties as source can change later

    this.variety = variety || 'plain';

    if (source === null ||
        source === undefined ||
        source === '') {

        source = null;
    }
    else if (Buffer.isBuffer(source)) {
        this.variety = 'buffer';
        this._contentType = 'application/octet-stream';
    }
    else if (source instanceof Stream) {
        this.variety = 'stream';
    }
    else if (typeof source === 'object' &&
        typeof source.then === 'function') {                // Promise object

        this.variety = 'promise';
    }

    this.source = source;

    if (this.variety === 'plain' &&
        this.source !== null) {

        this._contentType = (typeof this.source === 'string' ? 'text/html' : 'application/json');
    }
}
```
- example usage
```shell
...

    this._processors = {
        marshal: options.marshal,
        prepare: options.prepare,
        close: options.close
    };

    this._setSource(source, options.variety);
};

Hoek.inherits(internals.Response, Podium);


internals.Response.wrap = function (result, request) {
...
```

#### <a name="apidoc.element.hapi.response.prototype._setTemporary"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_setTemporary (isTemporary)](#apidoc.element.hapi.response.prototype._setTemporary)
- description and source-code
```javascript
_setTemporary = function (isTemporary) {

    if (isTemporary) {
        if (this._isRewritable()) {
            this.statusCode = 302;
        }
        else {
            this.statusCode = 307;
        }
    }
    else {
        if (this._isRewritable()) {
            this.statusCode = 301;
        }
        else {
            this.statusCode = 308;
        }
    }
}
```
- example usage
```shell
...
this.rewritable = this._rewritable;
return this;
};


internals.Response.prototype._temporary = function (isTemporary) {

this._setTemporary(isTemporary !== false);           // Defaults to true
return this;
};


internals.Response.prototype._permanent = function (isPermanent) {

this._setTemporary(isPermanent === false);           // Defaults to true
...
```

#### <a name="apidoc.element.hapi.response.prototype._streamify"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_streamify (source, next)](#apidoc.element.hapi.response.prototype._streamify)
- description and source-code
```javascript
_streamify = function (source, next) {

    if (source instanceof Stream) {
        if (typeof source._read !== 'function' || typeof source._readableState !== 'object') {
            return next(Boom.badImplementation('Stream must have a streams2 readable interface'));
        }

        if (source._readableState.objectMode) {
            return next(Boom.badImplementation('Cannot reply with stream in object mode'));
        }

        this._payload = source;
        return next();
    }

    let payload = source;
    if (this.variety === 'plain' &&
        source !== null &&
        typeof source !== 'string') {

        const options = this.settings.stringify || {};
        const space = options.space || this.request.route.settings.json.space;
        const replacer = options.replacer || this.request.route.settings.json.replacer;
        const suffix = options.suffix || this.request.route.settings.json.suffix || '';
        try {
            if (replacer || space) {
                payload = JSON.stringify(payload, replacer, space);
            }
            else {
                payload = JSON.stringify(payload);
            }
        }
        catch (err) {
            return next(err);
        }

        if (suffix) {
            payload = payload + suffix;
        }
    }
    else if (this.settings.stringify) {
        return next(Boom.badImplementation('Cannot set formatting options on non object response'));
    }

    this._payload = new internals.Payload(payload, this.settings);
    return next();
}
```
- example usage
```shell
...
    return this._processors.prepare(this, next);
};


internals.Response.prototype._marshal = function (next) {

    if (!this._processors.marshal) {
return this._streamify(this.source, next);
    }

    this._processors.marshal(this, (err, source) => {

if (err) {
    return next(err);
}
...
```

#### <a name="apidoc.element.hapi.response.prototype._tap"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_tap ()](#apidoc.element.hapi.response.prototype._tap)
- description and source-code
```javascript
_tap = function () {

    return (this.hasListeners('finish') || this.hasListeners('peek') ? new internals.Peek(this) : null);
}
```
- example usage
```shell
...
if (failAction === 'error') {
    return next(err);
}

return next();
    };

    Subtext.parse(request.raw.req, request._tap(), request.route.settings.payload, (err, parsed) => {

if (!err ||
    !request._isPayloadPending) {

    request._isPayloadPending = false;
    return onParsed(err, parsed);
}
...
```

#### <a name="apidoc.element.hapi.response.prototype._temporary"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>_temporary (isTemporary)](#apidoc.element.hapi.response.prototype._temporary)
- description and source-code
```javascript
_temporary = function (isTemporary) {

    this._setTemporary(isTemporary !== false);           // Defaults to true
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.response.prototype.bytes"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>bytes (bytes)](#apidoc.element.hapi.response.prototype.bytes)
- description and source-code
```javascript
bytes = function (bytes) {

    this._header('content-length', bytes);
    return this;
}
```
- example usage
```shell
...

            // Prepare transform

            if (ranges.length === 1) {                                          // Ignore requests for multiple ranges
                const range = ranges[0];
                ranger = new Ammo.Stream(range);
                response.code(206);
                response.bytes(range.to - range.from + 1);
                response._header('content-range', 'bytes ' + range.from + '-' + range.to + '/' + length);
            }
        }
    }

    response._header('accept-ranges', 'bytes');
}
...
```

#### <a name="apidoc.element.hapi.response.prototype.charset"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>charset (charset)](#apidoc.element.hapi.response.prototype.charset)
- description and source-code
```javascript
charset = function (charset) {

    this.settings.charset = charset || null;
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.response.prototype.code"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>code (statusCode)](#apidoc.element.hapi.response.prototype.code)
- description and source-code
```javascript
code = function (statusCode) {

    Hoek.assert(Hoek.isInteger(statusCode), 'Status code must be an integer');

    this.statusCode = statusCode;
    return this;
}
```
- example usage
```shell
...

    Hoek.assert(options, 'Entity method missing required options');
    Hoek.assert(options.etag || options.modified, 'Entity methods missing require options key');

    this.request._entity = options;

    if (Response.unmodified(this.request, options)) {
        return this.response().code(304).takeover();
    }

    return null;
};
...
```

#### <a name="apidoc.element.hapi.response.prototype.created"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>created (location)](#apidoc.element.hapi.response.prototype.created)
- description and source-code
```javascript
created = function (location) {

    Hoek.assert(this.request.method === 'post' || this.request.method === 'put', 'Cannot create resource on GET');

    this.statusCode = 201;
    this.location(location);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.response.prototype.encoding"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>encoding (encoding)](#apidoc.element.hapi.response.prototype.encoding)
- description and source-code
```javascript
encoding = function (encoding) {

    this.settings.encoding = encoding;
    return this;
}
```
- example usage
```shell
...
Hoek.assert(typeof decoder === 'function', 'Invalid decoder function for ${encoding}');
this._decoders[encoding] = decoder;
};


internals.Compression.prototype.accept = function (request) {

return Accept.encoding(request.headers['accept-encoding'], this.encodings);
};


internals.Compression.prototype.encoding = function (response) {

const request = response.request;
if (!request.connection.settings.compression) {
...
```

#### <a name="apidoc.element.hapi.response.prototype.etag"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>etag (tag, options)](#apidoc.element.hapi.response.prototype.etag)
- description and source-code
```javascript
etag = function (tag, options) {

    Hoek.assert(tag !== '*', 'ETag cannot be *');

    options = options || {};
    this._header('etag', (options.weak ? 'W/' : '') + '"' + tag + '"');
    this.settings.varyEtag = options.vary !== false && !options.weak;       // vary defaults to true
    return this;
}
```
- example usage
```shell
...
const request = response.request;

// Set headers from reply.entity()

if (request._entity.etag &&
    !response.headers.etag) {

    response.etag(request._entity.etag, { vary: request._entity.vary });
}

if (request._entity.modified &&
    !response.headers['last-modified']) {

    response.header('last-modified', request._entity.modified);
}
...
```

#### <a name="apidoc.element.hapi.response.prototype.header"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>header (key, value, options)](#apidoc.element.hapi.response.prototype.header)
- description and source-code
```javascript
header = function (key, value, options) {

    key = key.toLowerCase();
    if (key === 'vary') {
        return this.vary(value);
    }

    return this._header(key, value, options);
}
```
- example usage
```shell
...

            if (headerKeys.length) {
const localHeaders = this.headers;
this.headers = {};

for (let i = 0; i < headerKeys.length; ++i) {
    const key = headerKeys[i];
    this.header(key.toLowerCase(), Hoek.clone(this.source.headers[key]));     // Clone arrays
}

headerKeys = Object.keys(localHeaders);
for (let i = 0; i < headerKeys.length; ++i) {
    const key = headerKeys[i];
    this.header(key, localHeaders[key], { append: key === 'set-cookie' });
}
...
```

#### <a name="apidoc.element.hapi.response.prototype.location"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>location (uri)](#apidoc.element.hapi.response.prototype.location)
- description and source-code
```javascript
location = function (uri) {

    this._header('location', uri);
    return this;
}
```
- example usage
```shell
...


internals.Response.prototype.created = function (location) {

Hoek.assert(this.request.method === 'post' || this.request.method === 'put', 'Cannot create resource on GET');

this.statusCode = 201;
this.location(location);
return this;
};


internals.Response.prototype.replacer = function (method) {

this.settings.stringify = this.settings.stringify || {};
...
```

#### <a name="apidoc.element.hapi.response.prototype.message"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>message (httpMessage)](#apidoc.element.hapi.response.prototype.message)
- description and source-code
```javascript
message = function (httpMessage) {

    this.settings.message = httpMessage;
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.response.prototype.passThrough"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>passThrough (enabled)](#apidoc.element.hapi.response.prototype.passThrough)
- description and source-code
```javascript
passThrough = function (enabled) {

    this.settings.passThrough = (enabled !== false);    // Defaults to true
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.response.prototype.redirect"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>redirect (location)](#apidoc.element.hapi.response.prototype.redirect)
- description and source-code
```javascript
redirect = function (location) {

    this.statusCode = 302;
    this.location(location);
    this.temporary = this._temporary;
    this.permanent = this._permanent;
    this.rewritable = this._rewritable;
    return this;
}
```
- example usage
```shell
...

this.request._clearState(name, options);
};


internals.redirect = function (location) {

return this.response('').redirect(location);
};


internals.response = function (result) {

Hoek.assert(!this._replied, 'reply interface called twice');
this._replied = true;
...
```

#### <a name="apidoc.element.hapi.response.prototype.replacer"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>replacer (method)](#apidoc.element.hapi.response.prototype.replacer)
- description and source-code
```javascript
replacer = function (method) {

    this.settings.stringify = this.settings.stringify || {};
    this.settings.stringify.replacer = method;
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.response.prototype.spaces"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>spaces (count)](#apidoc.element.hapi.response.prototype.spaces)
- description and source-code
```javascript
spaces = function (count) {

    this.settings.stringify = this.settings.stringify || {};
    this.settings.stringify.space = count;
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.response.prototype.state"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>state (name, value, options)](#apidoc.element.hapi.response.prototype.state)
- description and source-code
```javascript
state = function (name, value, options) {          // options: see Defaults.state

    this.request._setState(name, value, options);
    return this;
}
```
- example usage
```shell
...
    const response = request.response;

    Cors.headers(response);
    internals.content(response, false);
    internals.security(response);
    internals.unmodified(response);

    internals.state(response, (err) => {

if (err) {
    request._log(['state', 'response', 'error'], err);
    request._states = {};                                           // Clear broken state
    return next(err);
}
...
```

#### <a name="apidoc.element.hapi.response.prototype.suffix"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>suffix (suffix)](#apidoc.element.hapi.response.prototype.suffix)
- description and source-code
```javascript
suffix = function (suffix) {

    this.settings.stringify = this.settings.stringify || {};
    this.settings.stringify.suffix = suffix;
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.response.prototype.takeover"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>takeover ()](#apidoc.element.hapi.response.prototype.takeover)
- description and source-code
```javascript
takeover = function () {

    this._takeover = true;
    return this;
}
```
- example usage
```shell
...
};


/*
    const handler = function (request, reply) {

reply(error, result, ignore);   -> error || result (continue)
reply(...).takeover();          -> ... (continue)

reply.continue(ignore);         -> null (continue)
    };

    const ext = function (request, reply) {

reply(error, result, ignore);   -> error || result (respond)
...
```

#### <a name="apidoc.element.hapi.response.prototype.ttl"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>ttl (ttl)](#apidoc.element.hapi.response.prototype.ttl)
- description and source-code
```javascript
ttl = function (ttl) {

    this.settings.ttl = ttl;
    return this;
}
```
- example usage
```shell
...
    const policy = request.route.settings.cache &&
                   request._route._cache &&
                   (request.route.settings.cache._statuses[response.statusCode] || (response.statusCode === 304 && request.route
.settings.cache._statuses['200']));

    if (policy ||
        response.settings.ttl) {

        const ttl = (response.settings.ttl !== null ? response.settings.ttl : request._route._cache.ttl());
        const privacy = (request.auth.isAuthenticated || response.headers['set-cookie'] ? 'private' : request.route.settings.cache
.privacy || 'default');
        response._header('cache-control', 'max-age=' + Math.floor(ttl / 1000) + ', must-revalidate' + (privacy !== 'default' ? ', ' +
privacy : ''));
    }
    else if (request.route.settings.cache) {
        response._header('cache-control', request.route.settings.cache.otherwise);
    }
};
...
```

#### <a name="apidoc.element.hapi.response.prototype.type"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>type (type)](#apidoc.element.hapi.response.prototype.type)
- description and source-code
```javascript
type = function (type) {

    this._header('content-type', type);
    return this;
}
```
- example usage
```shell
...
internals.Compression.prototype.encoding = function (response) {

const request = response.request;
if (!request.connection.settings.compression) {
    return null;
}

const mime = request.server.mime.type(response.headers['content-type'] || 'application/octet-stream');
if (!mime.compressible) {
    return null;
}

response.vary('accept-encoding');

if (response.headers['content-encoding']) {
...
```

#### <a name="apidoc.element.hapi.response.prototype.unstate"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>unstate (name, options)](#apidoc.element.hapi.response.prototype.unstate)
- description and source-code
```javascript
unstate = function (name, options) {

    this.request._clearState(name, options);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.response.prototype.vary"></a>[function <span class="apidocSignatureSpan">hapi.response.prototype.</span>vary (value)](#apidoc.element.hapi.response.prototype.vary)
- description and source-code
```javascript
vary = function (value) {

    if (value === '*') {
        this.headers.vary = '*';
    }
    else if (!this.headers.vary) {
        this.headers.vary = value;
    }
    else if (this.headers.vary !== '*') {
        this._header('vary', value, { append: true, duplicate: false });
    }

    return this;
}
```
- example usage
```shell
...
    }

    const mime = request.server.mime.type(response.headers['content-type'] || 'application/octet-stream');
    if (!mime.compressible) {
        return null;
    }

    response.vary('accept-encoding');

    if (response.headers['content-encoding']) {
        return null;
    }

    return (request.info.acceptEncoding === 'identity' ? null : request.info.acceptEncoding);
};
...
```



# <a name="apidoc.module.hapi.route"></a>[module hapi.route](#apidoc.module.hapi.route)

#### <a name="apidoc.element.hapi.route.route"></a>[function <span class="apidocSignatureSpan">hapi.</span>route (route, connection, plugin, options)](#apidoc.element.hapi.route.route)
- description and source-code
```javascript
route = function (route, connection, plugin, options) {

    options = options || {};

    // Apply plugin environment (before schema validation)

    const realm = plugin.realm;
    if (realm.modifiers.route.vhost ||
        realm.modifiers.route.prefix) {

        route = Hoek.cloneWithShallow(route, ['config']);       // config is left unchanged
        route.path = (realm.modifiers.route.prefix ? realm.modifiers.route.prefix + (route.path !== '/' ? route.path : '') : route
.path);
        route.vhost = realm.modifiers.route.vhost || route.vhost;
    }

    // Setup and validate route configuration

    Hoek.assert(route.path, 'Route missing path');
    const routeDisplay = route.method + ' ' + route.path;

    let config = route.config;
    if (typeof config === 'function') {
        config = config.call(realm.settings.bind, connection.server);
    }

    Hoek.assert(route.handler || (config && config.handler), 'Missing or undefined handler:', routeDisplay);
    Hoek.assert(!!route.handler ^ !!(config && config.handler), 'Handler must only appear once:', routeDisplay);            // XOR
    Hoek.assert(route.path === '/' || route.path[route.path.length - 1] !== '/' || !connection.settings.router.stripTrailingSlash
, 'Path cannot end with a trailing slash when connection configured to strip:', routeDisplay);

    route = Schema.apply('route', route, routeDisplay);

    const handler = route.handler || config.handler;
    const method = route.method.toLowerCase();
    Hoek.assert(method !== 'head', 'Method name not allowed:', routeDisplay);

    // Apply settings in order: {connection} <- {handler} <- {realm} <- {route}

    const handlerDefaults = Handler.defaults(method, handler, connection.server);
    let base = Hoek.applyToDefaultsWithShallow(connection.settings.routes, handlerDefaults, ['bind']);
    base = Hoek.applyToDefaultsWithShallow(base, realm.settings, ['bind']);
    this.settings = Hoek.applyToDefaultsWithShallow(base, config || {}, ['bind', 'validate.headers', 'validate.payload', 'validate
.params', 'validate.query']);
    this.settings.handler = handler;
    this.settings = Schema.apply('routeConfig', this.settings, routeDisplay);

    const socketTimeout = (this.settings.timeout.socket === undefined ? 2 * 60 * 1000 : this.settings.timeout.socket);
    Hoek.assert(!this.settings.timeout.server || !socketTimeout || this.settings.timeout.server < socketTimeout, 'Server timeout
 must be shorter than socket timeout:', routeDisplay);
    Hoek.assert(!this.settings.payload.timeout || !socketTimeout || this.settings.payload.timeout < socketTimeout, 'Payload timeout
 must be shorter than socket timeout:', routeDisplay);

    this.connection = connection;
    this.server = connection.server;
    this.path = route.path;
    this.method = method;
    this.plugin = plugin;

    this.settings.vhost = route.vhost;
    this.settings.plugins = this.settings.plugins || {};            // Route-specific plugins settings, namespaced using plugin
name
    this.settings.app = this.settings.app || {};                    // Route-specific application settings

    // Path parsing

    this._special = !!options.special;
    this._analysis = this.connection._router.analyze(this.path);
    this.params = this._analysis.params;
    this.fingerprint = this._analysis.fingerprint;

    this.public = {
        method: this.method,
        path: this.path,
        vhost: this.vhost,
        realm: this.plugin.realm,
        settings: this.settings,
        fingerprint: this.fingerprint,
        auth: {
            access: (request) => Auth.access(request, this.public)
        }
    };

    // Validation

    const validation = this.settings.validate;
    if (this.method === 'get') {

        // Assert on config, not on merged settings

        Hoek.assert(!config || !config.payload, 'Cannot set payload settings on HEAD or GET request:', routeDisplay);
        Hoek.assert(!config || !config.validate || !config.validate.payload, 'Cannot validate HEAD or GET requests:', routeDisplay
);

        validation.payload = null;
    }

    ['headers', ' ...
```
- example usage
```shell
...

internals.Connection.prototype.match = function (method, path, host) {

    Hoek.assert(method && typeof method === 'string', 'Invalid method:', method);
    Hoek.assert(path && typeof path === 'string' && path[0] === '/', 'Invalid path:', path);
    Hoek.assert(!host || typeof host === 'string', 'Invalid host:', host);

    const match = this._router.route(method.toLowerCase(), path, host);
    Hoek.assert(match !== this._router.specials.badRequest, 'Invalid path:', path);
    if (match === this._router.specials.notFound) {
        return null;
    }

    return match.route.public;
};
...
```



# <a name="apidoc.module.hapi.route.prototype"></a>[module hapi.route.prototype](#apidoc.module.hapi.route.prototype)

#### <a name="apidoc.element.hapi.route.prototype._combineExtensions"></a>[function <span class="apidocSignatureSpan">hapi.route.prototype.</span>_combineExtensions (type, subscribe)](#apidoc.element.hapi.route.prototype._combineExtensions)
- description and source-code
```javascript
_combineExtensions = function (type, subscribe) {

    const ext = new Ext(type, this.server);

    const events = this.settings.ext[type];
    if (events) {
        for (let i = 0; i < events.length; ++i) {
            const event = Hoek.shallow(events[i]);
            Hoek.assert(!event.options.sandbox, 'Cannot specify sandbox option for route extension');
            event.plugin = this.plugin;
            ext.add(event);
        }
    }

    const connection = this.connection._extensions[type];
    const realm = this.plugin.realm._extensions[type];

    ext.merge([connection, realm]);

    connection.subscribe(this);
    realm.subscribe(this);

    return ext;
}
```
- example usage
```shell
...

this.settings.handler = Handler.configure(this.settings.handler, this);
this._prerequisites = Handler.prerequisitesConfig(this.settings.pre, this.server);

// Route lifecycle

this._extensions = {
    onPreResponse: this._combineExtensions('onPreResponse')
};

if (this._special) {
    this._cycle = [Handler.execute];
    return;
}
...
```

#### <a name="apidoc.element.hapi.route.prototype.rebuild"></a>[function <span class="apidocSignatureSpan">hapi.route.prototype.</span>rebuild (event)](#apidoc.element.hapi.route.prototype.rebuild)
- description and source-code
```javascript
rebuild = function (event) {

    if (event) {
        this._extensions[event.type].add(event);
        if (event.type === 'onPreResponse') {
            return;
        }
    }

    // Build lifecycle array

    const cycle = [];

    // 'onRequest'

    if (this.settings.jsonp) {
        cycle.push(internals.parseJSONP);
    }

    if (this.settings.state.parse) {
        cycle.push(internals.state);
    }

    if (this._extensions.onPreAuth.nodes) {
        cycle.push(this._extensions.onPreAuth);
    }

    const authenticate = (this.settings.auth !== false);                          // Anything other than 'false' can still require
 authentication
    if (authenticate) {
        cycle.push(Auth.authenticate);
    }

    if (this.method !== 'get') {
        cycle.push(internals.payload);

        if (authenticate) {
            cycle.push(Auth.payload);
        }
    }

    if (this._extensions.onPostAuth.nodes) {
        cycle.push(this._extensions.onPostAuth);
    }

    if (this.settings.validate.headers) {
        cycle.push(Validation.headers);
    }

    if (this.settings.validate.params) {
        cycle.push(Validation.params);
    }

    if (this.settings.jsonp) {
        cycle.push(internals.cleanupJSONP);
    }

    if (this.settings.validate.query) {
        cycle.push(Validation.query);
    }

    if (this.settings.validate.payload) {
        cycle.push(Validation.payload);
    }

    if (this._extensions.onPreHandler.nodes) {
        cycle.push(this._extensions.onPreHandler);
    }

    cycle.push(Handler.execute);                                     // Must not call next() with an Error

    if (this._extensions.onPostHandler.nodes) {
        cycle.push(this._extensions.onPostHandler);                 // An error from here on will override any result set in handler
()
    }

    if (this.settings.response._validate &&
        this.settings.response.sample !== 0) {

        cycle.push(Validation.response);
    }

    this._cycle = cycle;
}
```
- example usage
```shell
...
}

this.nodes = this._topo.nodes;

// Notify routes

for (let i = 0; i < this._routes.length; ++i) {
    this._routes[i].rebuild(event);
}
};


internals.Ext.prototype.merge = function (others) {

const merge = [];
...
```



# <a name="apidoc.module.hapi.schema"></a>[module hapi.schema](#apidoc.module.hapi.schema)

#### <a name="apidoc.element.hapi.schema.apply"></a>[function <span class="apidocSignatureSpan">hapi.schema.</span>apply (type, options, message)](#apidoc.element.hapi.schema.apply)
- description and source-code
```javascript
apply = function (type, options, message) {

    const result = Joi.validate(options, internals[type]);
    Hoek.assert(!result.error, 'Invalid', type, 'options', message ? '(' + message + ')' : '', result.error && result.error.annotate
());
    return result.value;
}
```
- example usage
```shell
...
    }
};


internals.Auth.prototype.default = function (options) {

    Hoek.assert(!this.settings.default, 'Cannot set default strategy more than once');
    options = Schema.apply('auth', options, 'default strategy');

    this.settings.default = this._setupRoute(Hoek.clone(options));      // Can change options
};


internals.Auth.prototype.test = function (name, request, next) {
...
```



# <a name="apidoc.module.hapi.transmit"></a>[module hapi.transmit](#apidoc.module.hapi.transmit)

#### <a name="apidoc.element.hapi.transmit.send"></a>[function <span class="apidocSignatureSpan">hapi.transmit.</span>send (request, callback)](#apidoc.element.hapi.transmit.send)
- description and source-code
```javascript
send = function (request, callback) {

    const response = request.response;
    if (response.isBoom) {
        return internals.fail(request, response, callback);
    }

    internals.marshal(request, (err) => {

        if (err) {
            request._setResponse(err);
            return internals.fail(request, err, callback);
        }

        return internals.transmit(response, (err) => {

            if (err) {
                request._setResponse(err);
                return internals.fail(request, err, callback);
            }

            return callback();
        });
    });
}
```
- example usage
```shell
...

const transmit = (err) => {

    if (err) {                                          // Can be valid response or error
        this._setResponse(Response.wrap(err, this));
    }

    return Transmit.send(this, () => this._finalize());
};

if (!this._route._extensions.onPreResponse.nodes) {
    return transmit();
}

return this._invoke(this._route._extensions.onPreResponse, transmit);
...
```



# <a name="apidoc.module.hapi.validation"></a>[module hapi.validation](#apidoc.module.hapi.validation)

#### <a name="apidoc.element.hapi.validation.compile"></a>[function <span class="apidocSignatureSpan">hapi.validation.</span>compile (rule)](#apidoc.element.hapi.validation.compile)
- description and source-code
```javascript
compile = function (rule) {

    // null, undefined, true - anything allowed
    // false - nothing allowed
    // {...} - ... allowed

    return (rule === false ? Joi.object({}).allow(null)
                           : typeof rule === 'function' ? rule
                                                        : !rule || rule === true ? null                     // false tested earlier
                                                                                 : Joi.compile(rule));
}
```
- example usage
```shell
...
Hoek.assert(!config || !config.validate || !config.validate.payload, 'Cannot validate HEAD or GET requests:', routeDisplay);

validation.payload = null;
    }

    ['headers', 'params', 'query', 'payload'].forEach((type) => {

validation[type] = Validation.compile(validation[type]);
    });

    if (this.settings.response.schema !== undefined ||
this.settings.response.status) {

this.settings.response._validate = true;
...
```

#### <a name="apidoc.element.hapi.validation.headers"></a>[function <span class="apidocSignatureSpan">hapi.validation.</span>headers (request, next)](#apidoc.element.hapi.validation.headers)
- description and source-code
```javascript
headers = function (request, next) {

    return internals.input('headers', request, next);
}
```
- example usage
```shell
...
};


internals.marshal = function (request, next) {

    const response = request.response;

    Cors.headers(response);
    internals.content(response, false);
    internals.security(response);
    internals.unmodified(response);

    internals.state(response, (err) => {

if (err) {
...
```

#### <a name="apidoc.element.hapi.validation.params"></a>[function <span class="apidocSignatureSpan">hapi.validation.</span>params (request, next)](#apidoc.element.hapi.validation.params)
- description and source-code
```javascript
params = function (request, next) {

    return internals.input('params', request, next);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.validation.payload"></a>[function <span class="apidocSignatureSpan">hapi.validation.</span>payload (request, next)](#apidoc.element.hapi.validation.payload)
- description and source-code
```javascript
payload = function (request, next) {

    if (request.method === 'get' ||
        request.method === 'head') {                // When route.method is '*'

        return next();
    }

    return internals.input('payload', request, next);
}
```
- example usage
```shell
...

    return next(response);
};

request._protect.run(finalize, (exit) => {

    const reply = request.server._replier.interface(request, strategy.realm, {}, exit);
    strategy.methods.payload(request, reply);
});
};


internals.Auth.response = function (request, next) {

const auth = request.connection.auth;
...
```

#### <a name="apidoc.element.hapi.validation.query"></a>[function <span class="apidocSignatureSpan">hapi.validation.</span>query (request, next)](#apidoc.element.hapi.validation.query)
- description and source-code
```javascript
query = function (request, next) {

    return internals.input('query', request, next);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.hapi.validation.response"></a>[function <span class="apidocSignatureSpan">hapi.validation.</span>response (request, next)](#apidoc.element.hapi.validation.response)
- description and source-code
```javascript
response = function (request, next) {

    if (request.route.settings.response.sample) {
        const currentSample = Math.ceil((Math.random() * 100));
        if (currentSample > request.route.settings.response.sample) {
            return next();
        }
    }

    const response = request.response;
    const statusCode = response.isBoom ? response.output.statusCode : response.statusCode;

    const statusSchema = request.route.settings.response.status[statusCode];
    if (statusCode >= 400 &&
        !statusSchema) {

        return next();          // Do not validate errors by default
    }

    const schema = statusSchema || request.route.settings.response.schema;
    if (schema === null) {
        return next();          // No rules
    }

    if (!response.isBoom &&
        request.response.variety !== 'plain') {

        return next(Boom.badImplementation('Cannot validate non-object response'));
    }

    const postValidate = (err, value) => {

        if (!err) {
            if (value !== undefined &&
                request.route.settings.response.modify) {

                if (response.isBoom) {
                    response.output.payload = value;
                }
                else {
                    response.source = value;
                }
            }

            return next();
        }

        // failAction: 'error', 'log'

        if (request.route.settings.response.failAction === 'log') {
            request._log(['validation', 'response', 'error'], err.message);
            return next();
        }

        // Return error

        if (typeof request.route.settings.response.failAction !== 'function') {
            return next(Boom.badImplementation(err.message));
        }

        // Custom handler

        request._protect.run(next, (exit) => {

            const reply = request.server._replier.interface(request, request.route.realm, {}, exit);
            request.route.settings.response.failAction(request, reply, err);
        });
    };

    const localOptions = {
        context: {
            headers: request.headers,
            params: request.params,
            query: request.query,
            payload: request.payload,
            auth: {
                isAuthenticated: request.auth.isAuthenticated,
                credentials: request.auth.credentials
            }
        }
    };

    const source = response.isBoom ? response.output.payload : response.source;
    Hoek.merge(localOptions, request.route.settings.response.options);

    if (typeof schema !== 'function') {
        return Joi.validate(source, schema, localOptions, postValidate);
    }

    request._protect.run(postValidate, (exit) => {

        return schema(source, localOptions, exit);
    });
}
```
- example usage
```shell
...
if (!strategy.methods.response) {
    return next();
}

request._protect.run(next, (exit) => {

    const reply = request.server._replier.interface(request, strategy.realm, {}, exit);
    strategy.methods.response(request, reply);
});
};


internals.Authenticator = class {
constructor(config, request, manager) {
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
