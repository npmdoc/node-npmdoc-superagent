# api documentation for  [superagent (v3.5.2)](https://github.com/visionmedia/superagent#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-superagent.svg)](https://travis-ci.org/npmdoc/node-npmdoc-superagent)
#### elegant & feature rich browser / node HTTP with a fluent API

[![NPM](https://nodei.co/npm/superagent.png?downloads=true)](https://www.npmjs.com/package/superagent)

[![apidoc](https://npmdoc.github.io/node-npmdoc-superagent/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-superagent_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-superagent/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-superagent/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "TJ Holowaychuk",
        "email": "tj@vision-media.ca"
    },
    "browser": {
        "./lib/node/index.js": "./lib/client.js",
        "./test/support/server.js": "./test/support/blank.js"
    },
    "bugs": {
        "url": "https://github.com/visionmedia/superagent/issues"
    },
    "component": {
        "scripts": {
            "superagent": "lib/client.js"
        }
    },
    "contributors": [
        {
            "name": "Kornel Lesiński",
            "email": "kornel@geekhood.net"
        },
        {
            "name": "Peter Lyons",
            "email": "pete@peterlyons.com"
        },
        {
            "name": "Hunter Loftis",
            "email": "hunter@hunterloftis.com"
        }
    ],
    "dependencies": {
        "component-emitter": "^1.2.0",
        "cookiejar": "^2.0.6",
        "debug": "^2.2.0",
        "extend": "^3.0.0",
        "form-data": "^2.1.1",
        "formidable": "^1.1.1",
        "methods": "^1.1.1",
        "mime": "^1.3.4",
        "qs": "^6.1.0",
        "readable-stream": "^2.0.5"
    },
    "description": "elegant & feature rich browser / node HTTP with a fluent API",
    "devDependencies": {
        "Base64": "^1.0.0",
        "basic-auth-connect": "^1.0.0",
        "body-parser": "^1.15.0",
        "browserify": "^14.0.0",
        "cookie-parser": "^1.4.1",
        "express": "^4.13.4",
        "express-session": "^1.13.0",
        "marked": "^0.3.5",
        "mocha": "^3.1.2",
        "multer": "^1.2.0",
        "should": "^11.1.1",
        "should-http": "^0.0.4",
        "zuul": "^3.11.1"
    },
    "directories": {},
    "dist": {
        "shasum": "3361a3971567504c351063abeaae0faa23dbf3f8",
        "tarball": "https://registry.npmjs.org/superagent/-/superagent-3.5.2.tgz"
    },
    "engines": {
        "node": ">= 0.12"
    },
    "gitHead": "ef9af6c85b2b1a0cf5f350bece2f7e33d89b888a",
    "homepage": "https://github.com/visionmedia/superagent#readme",
    "keywords": [
        "http",
        "ajax",
        "request",
        "agent"
    ],
    "license": "MIT",
    "main": "./lib/node/index.js",
    "maintainers": [
        {
            "name": "defunctzombie",
            "email": "shtylman@gmail.com"
        },
        {
            "name": "kof",
            "email": "oleg008@gmail.com"
        },
        {
            "name": "kornel",
            "email": "pornel@pornel.net"
        },
        {
            "name": "naman34",
            "email": "naman34@gmail.com"
        },
        {
            "name": "nw",
            "email": "nw@nwhite.net"
        },
        {
            "name": "rauchg",
            "email": "rauchg@gmail.com"
        },
        {
            "name": "superjoe",
            "email": "superjoe30@gmail.com"
        },
        {
            "name": "tjholowaychuk",
            "email": "tj@vision-media.ca"
        },
        {
            "name": "travisjeffery",
            "email": "tj@travisjeffery.com"
        },
        {
            "name": "yields",
            "email": "yields@icloud.com"
        }
    ],
    "name": "superagent",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/visionmedia/superagent.git"
    },
    "scripts": {
        "prepublish": "make all",
        "test": "make test"
    },
    "version": "3.5.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module superagent](#apidoc.module.superagent)
1.  [function <span class="apidocSignatureSpan">superagent.</span>Request (method, url)](#apidoc.element.superagent.Request)
1.  [function <span class="apidocSignatureSpan">superagent.</span>Response (req)](#apidoc.element.superagent.Response)
1.  [function <span class="apidocSignatureSpan">superagent.</span>acl (url, data, fn)](#apidoc.element.superagent.acl)
1.  [function <span class="apidocSignatureSpan">superagent.</span>agent (options)](#apidoc.element.superagent.agent)
1.  [function <span class="apidocSignatureSpan">superagent.</span>bind (url, data, fn)](#apidoc.element.superagent.bind)
1.  [function <span class="apidocSignatureSpan">superagent.</span>checkout (url, data, fn)](#apidoc.element.superagent.checkout)
1.  [function <span class="apidocSignatureSpan">superagent.</span>client (method, url)](#apidoc.element.superagent.client)
1.  [function <span class="apidocSignatureSpan">superagent.</span>connect (url, data, fn)](#apidoc.element.superagent.connect)
1.  [function <span class="apidocSignatureSpan">superagent.</span>copy (url, data, fn)](#apidoc.element.superagent.copy)
1.  [function <span class="apidocSignatureSpan">superagent.</span>del (url, data, fn)](#apidoc.element.superagent.del)
1.  [function <span class="apidocSignatureSpan">superagent.</span>delete (url, data, fn)](#apidoc.element.superagent.delete)
1.  [function <span class="apidocSignatureSpan">superagent.</span>get (url, data, fn)](#apidoc.element.superagent.get)
1.  [function <span class="apidocSignatureSpan">superagent.</span>head (url, data, fn)](#apidoc.element.superagent.head)
1.  [function <span class="apidocSignatureSpan">superagent.</span>link (url, data, fn)](#apidoc.element.superagent.link)
1.  [function <span class="apidocSignatureSpan">superagent.</span>lock (url, data, fn)](#apidoc.element.superagent.lock)
1.  [function <span class="apidocSignatureSpan">superagent.</span>m-search (url, data, fn)](#apidoc.element.superagent.m-search)
1.  [function <span class="apidocSignatureSpan">superagent.</span>merge (url, data, fn)](#apidoc.element.superagent.merge)
1.  [function <span class="apidocSignatureSpan">superagent.</span>mkactivity (url, data, fn)](#apidoc.element.superagent.mkactivity)
1.  [function <span class="apidocSignatureSpan">superagent.</span>mkcalendar (url, data, fn)](#apidoc.element.superagent.mkcalendar)
1.  [function <span class="apidocSignatureSpan">superagent.</span>mkcol (url, data, fn)](#apidoc.element.superagent.mkcol)
1.  [function <span class="apidocSignatureSpan">superagent.</span>move (url, data, fn)](#apidoc.element.superagent.move)
1.  [function <span class="apidocSignatureSpan">superagent.</span>notify (url, data, fn)](#apidoc.element.superagent.notify)
1.  [function <span class="apidocSignatureSpan">superagent.</span>options (url, data, fn)](#apidoc.element.superagent.options)
1.  [function <span class="apidocSignatureSpan">superagent.</span>patch (url, data, fn)](#apidoc.element.superagent.patch)
1.  [function <span class="apidocSignatureSpan">superagent.</span>post (url, data, fn)](#apidoc.element.superagent.post)
1.  [function <span class="apidocSignatureSpan">superagent.</span>propfind (url, data, fn)](#apidoc.element.superagent.propfind)
1.  [function <span class="apidocSignatureSpan">superagent.</span>proppatch (url, data, fn)](#apidoc.element.superagent.proppatch)
1.  [function <span class="apidocSignatureSpan">superagent.</span>purge (url, data, fn)](#apidoc.element.superagent.purge)
1.  [function <span class="apidocSignatureSpan">superagent.</span>put (url, data, fn)](#apidoc.element.superagent.put)
1.  [function <span class="apidocSignatureSpan">superagent.</span>rebind (url, data, fn)](#apidoc.element.superagent.rebind)
1.  [function <span class="apidocSignatureSpan">superagent.</span>report (url, data, fn)](#apidoc.element.superagent.report)
1.  [function <span class="apidocSignatureSpan">superagent.</span>request_base (obj)](#apidoc.element.superagent.request_base)
1.  [function <span class="apidocSignatureSpan">superagent.</span>response_base (obj)](#apidoc.element.superagent.response_base)
1.  [function <span class="apidocSignatureSpan">superagent.</span>search (url, data, fn)](#apidoc.element.superagent.search)
1.  [function <span class="apidocSignatureSpan">superagent.</span>subscribe (url, data, fn)](#apidoc.element.superagent.subscribe)
1.  [function <span class="apidocSignatureSpan">superagent.</span>trace (url, data, fn)](#apidoc.element.superagent.trace)
1.  [function <span class="apidocSignatureSpan">superagent.</span>unbind (url, data, fn)](#apidoc.element.superagent.unbind)
1.  [function <span class="apidocSignatureSpan">superagent.</span>unlink (url, data, fn)](#apidoc.element.superagent.unlink)
1.  [function <span class="apidocSignatureSpan">superagent.</span>unlock (url, data, fn)](#apidoc.element.superagent.unlock)
1.  [function <span class="apidocSignatureSpan">superagent.</span>unsubscribe (url, data, fn)](#apidoc.element.superagent.unsubscribe)
1.  object <span class="apidocSignatureSpan">superagent.</span>Request.prototype
1.  object <span class="apidocSignatureSpan">superagent.</span>Response.prototype
1.  object <span class="apidocSignatureSpan">superagent.</span>agent.prototype
1.  object <span class="apidocSignatureSpan">superagent.</span>parse
1.  object <span class="apidocSignatureSpan">superagent.</span>protocols
1.  object <span class="apidocSignatureSpan">superagent.</span>request_base.prototype
1.  object <span class="apidocSignatureSpan">superagent.</span>response_base.prototype
1.  object <span class="apidocSignatureSpan">superagent.</span>serialize
1.  object <span class="apidocSignatureSpan">superagent.</span>utils

#### [module superagent.Request](#apidoc.module.superagent.Request)
1.  [function <span class="apidocSignatureSpan">superagent.</span>Request (method, url)](#apidoc.element.superagent.Request.Request)
1.  [function <span class="apidocSignatureSpan">superagent.Request.</span>super_ ()](#apidoc.element.superagent.Request.super_)

#### [module superagent.Request.prototype](#apidoc.module.superagent.Request.prototype)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_appendQueryString (req)](#apidoc.element.superagent.Request.prototype._appendQueryString)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_emitResponse (body, files)](#apidoc.element.superagent.Request.prototype._emitResponse)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_end ()](#apidoc.element.superagent.Request.prototype._end)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_getFormData ()](#apidoc.element.superagent.Request.prototype._getFormData)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_isHost (obj)](#apidoc.element.superagent.Request.prototype._isHost)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_isResponseOK (res)](#apidoc.element.superagent.Request.prototype._isResponseOK)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_pipeContinue (stream, options)](#apidoc.element.superagent.Request.prototype._pipeContinue)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_redirect (res)](#apidoc.element.superagent.Request.prototype._redirect)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_retry ()](#apidoc.element.superagent.Request.prototype._retry)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_setTimeouts ()](#apidoc.element.superagent.Request.prototype._setTimeouts)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_shouldUnzip (res)](#apidoc.element.superagent.Request.prototype._shouldUnzip)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_timeoutError (reason, timeout, errno)](#apidoc.element.superagent.Request.prototype._timeoutError)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>abort ()](#apidoc.element.superagent.Request.prototype.abort)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>accept (type)](#apidoc.element.superagent.Request.prototype.accept)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>agent (agent)](#apidoc.element.superagent.Request.prototype.agent)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>attach (field, file, options)](#apidoc.element.superagent.Request.prototype.attach)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>auth (user, pass, options)](#apidoc.element.superagent.Request.prototype.auth)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>buffer (val)](#apidoc.element.superagent.Request.prototype.buffer)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>ca (cert)](#apidoc.element.superagent.Request.prototype.ca)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>callback (err, res)](#apidoc.element.superagent.Request.prototype.callback)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>catch (cb)](#apidoc.element.superagent.Request.prototype.catch)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>cert (cert)](#apidoc.element.superagent.Request.prototype.cert)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>clearTimeout ()](#apidoc.element.superagent.Request.prototype.clearTimeout)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>end (fn)](#apidoc.element.superagent.Request.prototype.end)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>field (name, val)](#apidoc.element.superagent.Request.prototype.field)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>get (field)](#apidoc.element.superagent.Request.prototype.get)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>getHeader (field)](#apidoc.element.superagent.Request.prototype.getHeader)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>key (cert)](#apidoc.element.superagent.Request.prototype.key)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>ok (cb)](#apidoc.element.superagent.Request.prototype.ok)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>parse (fn)](#apidoc.element.superagent.Request.prototype.parse)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>pfx (cert)](#apidoc.element.superagent.Request.prototype.pfx)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>pipe (stream, options)](#apidoc.element.superagent.Request.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>query (val)](#apidoc.element.superagent.Request.prototype.query)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>redirects (n)](#apidoc.element.superagent.Request.prototype.redirects)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>request ()](#apidoc.element.superagent.Request.prototype.request)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>responseType (val)](#apidoc.element.superagent.Request.prototype.responseType)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>retry (count)](#apidoc.element.superagent.Request.prototype.retry)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>send (data)](#apidoc.element.superagent.Request.prototype.send)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>serialize (fn)](#apidoc.element.superagent.Request.prototype.serialize)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>set (field, val)](#apidoc.element.superagent.Request.prototype.set)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>sortQuery (sort)](#apidoc.element.superagent.Request.prototype.sortQuery)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>then (resolve, reject)](#apidoc.element.superagent.Request.prototype.then)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>timeout (options)](#apidoc.element.superagent.Request.prototype.timeout)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>toJSON ()](#apidoc.element.superagent.Request.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>type (type)](#apidoc.element.superagent.Request.prototype.type)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>unset (field)](#apidoc.element.superagent.Request.prototype.unset)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>use (fn)](#apidoc.element.superagent.Request.prototype.use)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>withCredentials (on)](#apidoc.element.superagent.Request.prototype.withCredentials)
1.  [function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>write (data, encoding)](#apidoc.element.superagent.Request.prototype.write)

#### [module superagent.Response](#apidoc.module.superagent.Response)
1.  [function <span class="apidocSignatureSpan">superagent.</span>Response (req)](#apidoc.element.superagent.Response.Response)
1.  [function <span class="apidocSignatureSpan">superagent.Response.</span>super_ ()](#apidoc.element.superagent.Response.super_)

#### [module superagent.Response.prototype](#apidoc.module.superagent.Response.prototype)
1.  [function <span class="apidocSignatureSpan">superagent.Response.prototype.</span>_setHeaderProperties (header)](#apidoc.element.superagent.Response.prototype._setHeaderProperties)
1.  [function <span class="apidocSignatureSpan">superagent.Response.prototype.</span>_setStatusProperties (status)](#apidoc.element.superagent.Response.prototype._setStatusProperties)
1.  [function <span class="apidocSignatureSpan">superagent.Response.prototype.</span>destroy (err)](#apidoc.element.superagent.Response.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">superagent.Response.prototype.</span>get (field)](#apidoc.element.superagent.Response.prototype.get)
1.  [function <span class="apidocSignatureSpan">superagent.Response.prototype.</span>pause ()](#apidoc.element.superagent.Response.prototype.pause)
1.  [function <span class="apidocSignatureSpan">superagent.Response.prototype.</span>resume ()](#apidoc.element.superagent.Response.prototype.resume)
1.  [function <span class="apidocSignatureSpan">superagent.Response.prototype.</span>setStatusProperties (status)](#apidoc.element.superagent.Response.prototype.setStatusProperties)
1.  [function <span class="apidocSignatureSpan">superagent.Response.prototype.</span>toError ()](#apidoc.element.superagent.Response.prototype.toError)
1.  [function <span class="apidocSignatureSpan">superagent.Response.prototype.</span>toJSON ()](#apidoc.element.superagent.Response.prototype.toJSON)

#### [module superagent.agent](#apidoc.module.superagent.agent)
1.  [function <span class="apidocSignatureSpan">superagent.</span>agent (options)](#apidoc.element.superagent.agent.agent)

#### [module superagent.agent.prototype](#apidoc.module.superagent.agent.prototype)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>_attachCookies (req)](#apidoc.element.superagent.agent.prototype._attachCookies)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>_saveCookies (res)](#apidoc.element.superagent.agent.prototype._saveCookies)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>acl (url, fn)](#apidoc.element.superagent.agent.prototype.acl)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>bind (url, fn)](#apidoc.element.superagent.agent.prototype.bind)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>checkout (url, fn)](#apidoc.element.superagent.agent.prototype.checkout)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>connect (url, fn)](#apidoc.element.superagent.agent.prototype.connect)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>copy (url, fn)](#apidoc.element.superagent.agent.prototype.copy)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>del (url, fn)](#apidoc.element.superagent.agent.prototype.del)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>delete (url, fn)](#apidoc.element.superagent.agent.prototype.delete)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>get (url, fn)](#apidoc.element.superagent.agent.prototype.get)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>head (url, fn)](#apidoc.element.superagent.agent.prototype.head)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>link (url, fn)](#apidoc.element.superagent.agent.prototype.link)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>lock (url, fn)](#apidoc.element.superagent.agent.prototype.lock)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>m-search (url, fn)](#apidoc.element.superagent.agent.prototype.m-search)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>merge (url, fn)](#apidoc.element.superagent.agent.prototype.merge)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>mkactivity (url, fn)](#apidoc.element.superagent.agent.prototype.mkactivity)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>mkcalendar (url, fn)](#apidoc.element.superagent.agent.prototype.mkcalendar)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>mkcol (url, fn)](#apidoc.element.superagent.agent.prototype.mkcol)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>move (url, fn)](#apidoc.element.superagent.agent.prototype.move)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>notify (url, fn)](#apidoc.element.superagent.agent.prototype.notify)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>options (url, fn)](#apidoc.element.superagent.agent.prototype.options)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>patch (url, fn)](#apidoc.element.superagent.agent.prototype.patch)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>post (url, fn)](#apidoc.element.superagent.agent.prototype.post)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>propfind (url, fn)](#apidoc.element.superagent.agent.prototype.propfind)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>proppatch (url, fn)](#apidoc.element.superagent.agent.prototype.proppatch)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>purge (url, fn)](#apidoc.element.superagent.agent.prototype.purge)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>put (url, fn)](#apidoc.element.superagent.agent.prototype.put)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>rebind (url, fn)](#apidoc.element.superagent.agent.prototype.rebind)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>report (url, fn)](#apidoc.element.superagent.agent.prototype.report)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>search (url, fn)](#apidoc.element.superagent.agent.prototype.search)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>subscribe (url, fn)](#apidoc.element.superagent.agent.prototype.subscribe)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>trace (url, fn)](#apidoc.element.superagent.agent.prototype.trace)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>unbind (url, fn)](#apidoc.element.superagent.agent.prototype.unbind)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>unlink (url, fn)](#apidoc.element.superagent.agent.prototype.unlink)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>unlock (url, fn)](#apidoc.element.superagent.agent.prototype.unlock)
1.  [function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>unsubscribe (url, fn)](#apidoc.element.superagent.agent.prototype.unsubscribe)

#### [module superagent.client](#apidoc.module.superagent.client)
1.  [function <span class="apidocSignatureSpan">superagent.</span>client (method, url)](#apidoc.element.superagent.client.client)
1.  [function <span class="apidocSignatureSpan">superagent.client.</span>Request (method, url)](#apidoc.element.superagent.client.Request)
1.  [function <span class="apidocSignatureSpan">superagent.client.</span>Response (req)](#apidoc.element.superagent.client.Response)
1.  [function <span class="apidocSignatureSpan">superagent.client.</span>del (url, data, fn)](#apidoc.element.superagent.client.del)
1.  [function <span class="apidocSignatureSpan">superagent.client.</span>delete (url, data, fn)](#apidoc.element.superagent.client.delete)
1.  [function <span class="apidocSignatureSpan">superagent.client.</span>get (url, data, fn)](#apidoc.element.superagent.client.get)
1.  [function <span class="apidocSignatureSpan">superagent.client.</span>getXHR ()](#apidoc.element.superagent.client.getXHR)
1.  [function <span class="apidocSignatureSpan">superagent.client.</span>head (url, data, fn)](#apidoc.element.superagent.client.head)
1.  [function <span class="apidocSignatureSpan">superagent.client.</span>options (url, data, fn)](#apidoc.element.superagent.client.options)
1.  [function <span class="apidocSignatureSpan">superagent.client.</span>parseString (str)](#apidoc.element.superagent.client.parseString)
1.  [function <span class="apidocSignatureSpan">superagent.client.</span>patch (url, data, fn)](#apidoc.element.superagent.client.patch)
1.  [function <span class="apidocSignatureSpan">superagent.client.</span>post (url, data, fn)](#apidoc.element.superagent.client.post)
1.  [function <span class="apidocSignatureSpan">superagent.client.</span>put (url, data, fn)](#apidoc.element.superagent.client.put)
1.  [function <span class="apidocSignatureSpan">superagent.client.</span>serializeObject (obj)](#apidoc.element.superagent.client.serializeObject)
1.  object <span class="apidocSignatureSpan">superagent.client.</span>parse
1.  object <span class="apidocSignatureSpan">superagent.client.</span>serialize
1.  object <span class="apidocSignatureSpan">superagent.client.</span>types

#### [module superagent.parse](#apidoc.module.superagent.parse)
1.  [function <span class="apidocSignatureSpan">superagent.parse.</span>image (res, fn)](#apidoc.element.superagent.parse.image)
1.  [function <span class="apidocSignatureSpan">superagent.parse.</span>text (res, fn)](#apidoc.element.superagent.parse.text)

#### [module superagent.request_base](#apidoc.module.superagent.request_base)
1.  [function <span class="apidocSignatureSpan">superagent.</span>request_base (obj)](#apidoc.element.superagent.request_base.request_base)

#### [module superagent.request_base.prototype](#apidoc.module.superagent.request_base.prototype)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>_isResponseOK (res)](#apidoc.element.superagent.request_base.prototype._isResponseOK)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>_retry ()](#apidoc.element.superagent.request_base.prototype._retry)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>_setTimeouts ()](#apidoc.element.superagent.request_base.prototype._setTimeouts)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>_timeoutError (reason, timeout, errno)](#apidoc.element.superagent.request_base.prototype._timeoutError)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>abort ()](#apidoc.element.superagent.request_base.prototype.abort)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>catch (cb)](#apidoc.element.superagent.request_base.prototype.catch)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>clearTimeout ()](#apidoc.element.superagent.request_base.prototype.clearTimeout)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>field (name, val)](#apidoc.element.superagent.request_base.prototype.field)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>get (field)](#apidoc.element.superagent.request_base.prototype.get)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>getHeader (field)](#apidoc.element.superagent.request_base.prototype.getHeader)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>ok (cb)](#apidoc.element.superagent.request_base.prototype.ok)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>parse (fn)](#apidoc.element.superagent.request_base.prototype.parse)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>redirects (n)](#apidoc.element.superagent.request_base.prototype.redirects)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>responseType (val)](#apidoc.element.superagent.request_base.prototype.responseType)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>retry (count)](#apidoc.element.superagent.request_base.prototype.retry)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>send (data)](#apidoc.element.superagent.request_base.prototype.send)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>serialize (fn)](#apidoc.element.superagent.request_base.prototype.serialize)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>set (field, val)](#apidoc.element.superagent.request_base.prototype.set)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>sortQuery (sort)](#apidoc.element.superagent.request_base.prototype.sortQuery)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>then (resolve, reject)](#apidoc.element.superagent.request_base.prototype.then)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>timeout (options)](#apidoc.element.superagent.request_base.prototype.timeout)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>toJSON ()](#apidoc.element.superagent.request_base.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>unset (field)](#apidoc.element.superagent.request_base.prototype.unset)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>use (fn)](#apidoc.element.superagent.request_base.prototype.use)
1.  [function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>withCredentials (on)](#apidoc.element.superagent.request_base.prototype.withCredentials)

#### [module superagent.response_base](#apidoc.module.superagent.response_base)
1.  [function <span class="apidocSignatureSpan">superagent.</span>response_base (obj)](#apidoc.element.superagent.response_base.response_base)

#### [module superagent.response_base.prototype](#apidoc.module.superagent.response_base.prototype)
1.  [function <span class="apidocSignatureSpan">superagent.response_base.prototype.</span>_setHeaderProperties (header)](#apidoc.element.superagent.response_base.prototype._setHeaderProperties)
1.  [function <span class="apidocSignatureSpan">superagent.response_base.prototype.</span>_setStatusProperties (status)](#apidoc.element.superagent.response_base.prototype._setStatusProperties)
1.  [function <span class="apidocSignatureSpan">superagent.response_base.prototype.</span>get (field)](#apidoc.element.superagent.response_base.prototype.get)

#### [module superagent.serialize](#apidoc.module.superagent.serialize)

#### [module superagent.utils](#apidoc.module.superagent.utils)
1.  [function <span class="apidocSignatureSpan">superagent.utils.</span>cleanHeader (header, shouldStripCookie)](#apidoc.element.superagent.utils.cleanHeader)
1.  [function <span class="apidocSignatureSpan">superagent.utils.</span>params (str)](#apidoc.element.superagent.utils.params)
1.  [function <span class="apidocSignatureSpan">superagent.utils.</span>parseLinks (str)](#apidoc.element.superagent.utils.parseLinks)
1.  [function <span class="apidocSignatureSpan">superagent.utils.</span>type (str)](#apidoc.element.superagent.utils.type)



# <a name="apidoc.module.superagent"></a>[module superagent](#apidoc.module.superagent)

#### <a name="apidoc.element.superagent.Request"></a>[function <span class="apidocSignatureSpan">superagent.</span>Request (method, url)](#apidoc.element.superagent.Request)
- description and source-code
```javascript
function Request(method, url) {
  Stream.call(this);
  if ('string' != typeof url) url = format(url);
  this._agent = false;
  this._formData = null;
  this.method = method;
  this.url = url;
  _initHeaders(this);
  this.writable = true;
  this._redirects = 0;
  this.redirects(method === 'HEAD' ? 0 : 5);
  this.cookies = '';
  this.qs = {};
  this.qsRaw = [];
  this._redirectList = [];
  this._streamRequest = false;
  this.once('end', this.clearTimeout.bind(this));
}
```
- example usage
```shell
...
/**
 * Expose 'request'.
 */

var request = exports = module.exports = function(method, url) {
// callback
if ('function' == typeof url) {
  return new exports.Request('GET', method).end(url);
}

// url first
if (1 == arguments.length) {
  return new exports.Request('GET', method);
}
...
```

#### <a name="apidoc.element.superagent.Response"></a>[function <span class="apidocSignatureSpan">superagent.</span>Response (req)](#apidoc.element.superagent.Response)
- description and source-code
```javascript
function Response(req) {
  Stream.call(this);
  var res = this.res = req.res;
  this.request = req;
  this.req = req.req;
  this.text = res.text;
  this.body = res.body !== undefined ? res.body : {};
  this.files = res.files || {};
  this.buffered = 'string' == typeof this.text;
  this.header = this.headers = res.headers;
  this._setStatusProperties(res.statusCode);
  this._setHeaderProperties(this.header);
  this.setEncoding = res.setEncoding.bind(res);
  res.on('data', this.emit.bind(this, 'data'));
  res.on('end', this.emit.bind(this, 'end'));
  res.on('close', this.emit.bind(this, 'close'));
  res.on('error', this.emit.bind(this, 'error'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.acl"></a>[function <span class="apidocSignatureSpan">superagent.</span>acl (url, data, fn)](#apidoc.element.superagent.acl)
- description and source-code
```javascript
acl = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent"></a>[function <span class="apidocSignatureSpan">superagent.</span>agent (options)](#apidoc.element.superagent.agent)
- description and source-code
```javascript
function Agent(options) {
  if (!(this instanceof Agent)) return new Agent(options);
  if (options) {
    this._ca = options.ca;
    this._key = options.key;
    this._pfx = options.pfx;
    this._cert = options.cert;
  }
  this.jar = new CookieJar;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.bind"></a>[function <span class="apidocSignatureSpan">superagent.</span>bind (url, data, fn)](#apidoc.element.superagent.bind)
- description and source-code
```javascript
bind = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
...
    e.percent = e.loaded / e.total * 100;
  }
  e.direction = direction;
  self.emit('progress', e);
}
if (this.hasListeners('progress')) {
  try {
    xhr.onprogress = handleProgress.bind(null, 'download');
    if (xhr.upload) {
      xhr.upload.onprogress = handleProgress.bind(null, 'upload');
    }
  } catch(e) {
    // Accessing xhr.upload fails in IE from a web worker, so just pretend it doesn't exist.
    // Reported here:
    // https://connect.microsoft.com/IE/feedback/details/837245/xmlhttprequest-upload-throws-invalid-argument-when-used-from-web
-worker-context
...
```

#### <a name="apidoc.element.superagent.checkout"></a>[function <span class="apidocSignatureSpan">superagent.</span>checkout (url, data, fn)](#apidoc.element.superagent.checkout)
- description and source-code
```javascript
checkout = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.client"></a>[function <span class="apidocSignatureSpan">superagent.</span>client (method, url)](#apidoc.element.superagent.client)
- description and source-code
```javascript
client = function (method, url) {
  // callback
  if ('function' == typeof url) {
    return new exports.Request('GET', method).end(url);
  }

  // url first
  if (1 == arguments.length) {
    return new exports.Request('GET', method);
  }

  return new exports.Request(method, url);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.connect"></a>[function <span class="apidocSignatureSpan">superagent.</span>connect (url, data, fn)](#apidoc.element.superagent.connect)
- description and source-code
```javascript
connect = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.copy"></a>[function <span class="apidocSignatureSpan">superagent.</span>copy (url, data, fn)](#apidoc.element.superagent.copy)
- description and source-code
```javascript
copy = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.del"></a>[function <span class="apidocSignatureSpan">superagent.</span>del (url, data, fn)](#apidoc.element.superagent.del)
- description and source-code
```javascript
del = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.delete"></a>[function <span class="apidocSignatureSpan">superagent.</span>delete (url, data, fn)](#apidoc.element.superagent.delete)
- description and source-code
```javascript
delete = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.get"></a>[function <span class="apidocSignatureSpan">superagent.</span>get (url, data, fn)](#apidoc.element.superagent.get)
- description and source-code
```javascript
get = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
...

'''js
var nocache = require('superagent-no-cache');
var request = require('superagent');
var prefix = require('superagent-prefix')('/static');

request
  .get('/some-url')
  .query({ action: 'edit', city: 'London' }) // query string
  .use(prefix) // Prefixes *only* this request
  .use(nocache) // Prevents caching of *only* this request
  .end(function(err, res){
    // Do something
  });
'''
...
```

#### <a name="apidoc.element.superagent.head"></a>[function <span class="apidocSignatureSpan">superagent.</span>head (url, data, fn)](#apidoc.element.superagent.head)
- description and source-code
```javascript
head = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.link"></a>[function <span class="apidocSignatureSpan">superagent.</span>link (url, data, fn)](#apidoc.element.superagent.link)
- description and source-code
```javascript
link = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.lock"></a>[function <span class="apidocSignatureSpan">superagent.</span>lock (url, data, fn)](#apidoc.element.superagent.lock)
- description and source-code
```javascript
lock = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.m-search"></a>[function <span class="apidocSignatureSpan">superagent.</span>m-search (url, data, fn)](#apidoc.element.superagent.m-search)
- description and source-code
```javascript
m-search = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.merge"></a>[function <span class="apidocSignatureSpan">superagent.</span>merge (url, data, fn)](#apidoc.element.superagent.merge)
- description and source-code
```javascript
merge = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.mkactivity"></a>[function <span class="apidocSignatureSpan">superagent.</span>mkactivity (url, data, fn)](#apidoc.element.superagent.mkactivity)
- description and source-code
```javascript
mkactivity = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.mkcalendar"></a>[function <span class="apidocSignatureSpan">superagent.</span>mkcalendar (url, data, fn)](#apidoc.element.superagent.mkcalendar)
- description and source-code
```javascript
mkcalendar = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.mkcol"></a>[function <span class="apidocSignatureSpan">superagent.</span>mkcol (url, data, fn)](#apidoc.element.superagent.mkcol)
- description and source-code
```javascript
mkcol = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.move"></a>[function <span class="apidocSignatureSpan">superagent.</span>move (url, data, fn)](#apidoc.element.superagent.move)
- description and source-code
```javascript
move = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.notify"></a>[function <span class="apidocSignatureSpan">superagent.</span>notify (url, data, fn)](#apidoc.element.superagent.notify)
- description and source-code
```javascript
notify = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.options"></a>[function <span class="apidocSignatureSpan">superagent.</span>options (url, data, fn)](#apidoc.element.superagent.options)
- description and source-code
```javascript
options = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.patch"></a>[function <span class="apidocSignatureSpan">superagent.</span>patch (url, data, fn)](#apidoc.element.superagent.patch)
- description and source-code
```javascript
patch = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.post"></a>[function <span class="apidocSignatureSpan">superagent.</span>post (url, data, fn)](#apidoc.element.superagent.post)
- description and source-code
```javascript
post = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
...
$ npm install superagent
'''

Works with [browserify](https://github.com/substack/node-browserify) and should work with [webpack](https://github.com/visionmedia
/superagent/wiki/SuperAgent-for-Webpack)

'''js
request
  .post('/api/pet')
  .send({ name: 'Manny', species: 'cat' })
  .set('X-API-Key', 'foobar')
  .set('Accept', 'application/json')
  .end(function(err, res){
    // Calling the end function will send the request
  });
'''
...
```

#### <a name="apidoc.element.superagent.propfind"></a>[function <span class="apidocSignatureSpan">superagent.</span>propfind (url, data, fn)](#apidoc.element.superagent.propfind)
- description and source-code
```javascript
propfind = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.proppatch"></a>[function <span class="apidocSignatureSpan">superagent.</span>proppatch (url, data, fn)](#apidoc.element.superagent.proppatch)
- description and source-code
```javascript
proppatch = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.purge"></a>[function <span class="apidocSignatureSpan">superagent.</span>purge (url, data, fn)](#apidoc.element.superagent.purge)
- description and source-code
```javascript
purge = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.put"></a>[function <span class="apidocSignatureSpan">superagent.</span>put (url, data, fn)](#apidoc.element.superagent.put)
- description and source-code
```javascript
put = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.rebind"></a>[function <span class="apidocSignatureSpan">superagent.</span>rebind (url, data, fn)](#apidoc.element.superagent.rebind)
- description and source-code
```javascript
rebind = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.report"></a>[function <span class="apidocSignatureSpan">superagent.</span>report (url, data, fn)](#apidoc.element.superagent.report)
- description and source-code
```javascript
report = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.request_base"></a>[function <span class="apidocSignatureSpan">superagent.</span>request_base (obj)](#apidoc.element.superagent.request_base)
- description and source-code
```javascript
function RequestBase(obj) {
  if (obj) return mixin(obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.response_base"></a>[function <span class="apidocSignatureSpan">superagent.</span>response_base (obj)](#apidoc.element.superagent.response_base)
- description and source-code
```javascript
function ResponseBase(obj) {
  if (obj) return mixin(obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.search"></a>[function <span class="apidocSignatureSpan">superagent.</span>search (url, data, fn)](#apidoc.element.superagent.search)
- description and source-code
```javascript
search = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.subscribe"></a>[function <span class="apidocSignatureSpan">superagent.</span>subscribe (url, data, fn)](#apidoc.element.superagent.subscribe)
- description and source-code
```javascript
subscribe = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.trace"></a>[function <span class="apidocSignatureSpan">superagent.</span>trace (url, data, fn)](#apidoc.element.superagent.trace)
- description and source-code
```javascript
trace = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.unbind"></a>[function <span class="apidocSignatureSpan">superagent.</span>unbind (url, data, fn)](#apidoc.element.superagent.unbind)
- description and source-code
```javascript
unbind = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.unlink"></a>[function <span class="apidocSignatureSpan">superagent.</span>unlink (url, data, fn)](#apidoc.element.superagent.unlink)
- description and source-code
```javascript
unlink = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.unlock"></a>[function <span class="apidocSignatureSpan">superagent.</span>unlock (url, data, fn)](#apidoc.element.superagent.unlock)
- description and source-code
```javascript
unlock = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.unsubscribe"></a>[function <span class="apidocSignatureSpan">superagent.</span>unsubscribe (url, data, fn)](#apidoc.element.superagent.unsubscribe)
- description and source-code
```javascript
unsubscribe = function (url, data, fn){
  var req = request(method, url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.superagent.Request"></a>[module superagent.Request](#apidoc.module.superagent.Request)

#### <a name="apidoc.element.superagent.Request.Request"></a>[function <span class="apidocSignatureSpan">superagent.</span>Request (method, url)](#apidoc.element.superagent.Request.Request)
- description and source-code
```javascript
function Request(method, url) {
  Stream.call(this);
  if ('string' != typeof url) url = format(url);
  this._agent = false;
  this._formData = null;
  this.method = method;
  this.url = url;
  _initHeaders(this);
  this.writable = true;
  this._redirects = 0;
  this.redirects(method === 'HEAD' ? 0 : 5);
  this.cookies = '';
  this.qs = {};
  this.qsRaw = [];
  this._redirectList = [];
  this._streamRequest = false;
  this.once('end', this.clearTimeout.bind(this));
}
```
- example usage
```shell
...
/**
 * Expose 'request'.
 */

var request = exports = module.exports = function(method, url) {
// callback
if ('function' == typeof url) {
  return new exports.Request('GET', method).end(url);
}

// url first
if (1 == arguments.length) {
  return new exports.Request('GET', method);
}
...
```

#### <a name="apidoc.element.superagent.Request.super_"></a>[function <span class="apidocSignatureSpan">superagent.Request.</span>super_ ()](#apidoc.element.superagent.Request.super_)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.superagent.Request.prototype"></a>[module superagent.Request.prototype](#apidoc.module.superagent.Request.prototype)

#### <a name="apidoc.element.superagent.Request.prototype._appendQueryString"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_appendQueryString (req)](#apidoc.element.superagent.Request.prototype._appendQueryString)
- description and source-code
```javascript
_appendQueryString = function (req){
  var query = qs.stringify(this.qs, { indices: false, strictNullHandling: true });
  query += ((query.length && this.qsRaw.length) ? '&' : '') + this.qsRaw.join('&');
  req.path += query.length ? (~req.path.indexOf('?') ? '&' : '?') + query : '';

  if (this._sort) {
    var index = req.path.indexOf('?');
    if (index >= 0) {
      var queryArr = req.path.substring(index + 1).split('&');
      if (isFunction(this._sort)) {
        queryArr.sort(this._sort);
      } else {
        queryArr.sort();
      }
      req.path = req.path.substring(0, index) + '?' + queryArr.join('&');
    }
  }
}
```
- example usage
```shell
...
}
this._endCalled = true;

// store callback
this._callback = fn || noop;

// querystring
this._appendQueryString();

return this._end();
};

Request.prototype._end = function() {
var self = this;
var xhr = this.xhr = request.getXHR();
...
```

#### <a name="apidoc.element.superagent.Request.prototype._emitResponse"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_emitResponse (body, files)](#apidoc.element.superagent.Request.prototype._emitResponse)
- description and source-code
```javascript
_emitResponse = function (body, files){
    var response = new Response(this);
    this.response = response;
    response.redirects = this._redirectList;
    if (undefined !== body) {
      response.body = body;
    }
    response.files = files;
    this.emit('response', response);
    return response;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype._end"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_end ()](#apidoc.element.superagent.Request.prototype._end)
- description and source-code
```javascript
_end = function () {
  var self = this;
  var data = this._data;
  var req = this.req;
  var buffer = this._buffer;
  var method = this.method;

  this._setTimeouts();

  // body
  if ('HEAD' != method && !req._headerSent) {
    // serialize stuff
    if ('string' != typeof data) {
      var contentType = req.getHeader('Content-Type')
      // Parse out just the content type from the header (ignore the charset)
      if (contentType) contentType = contentType.split(';')[0]
      var serialize = exports.serialize[contentType];
      if (!serialize && isJSON(contentType)) {
        serialize = exports.serialize['application/json'];
      }
      if (serialize) data = serialize(data);
    }

    // content-length
    if (data && !req.getHeader('Content-Length')) {
      req.setHeader('Content-Length', Buffer.isBuffer(data) ? data.length : Buffer.byteLength(data));
    }
  }

  // response
  req.once('response', function(res){
    debug('%s %s -> %s', self.method, self.url, res.statusCode);

    if (self._responseTimeoutTimer) {
      clearTimeout(self._responseTimeoutTimer);
    }

    if (self.piped) {
      return;
    }

    var max = self._maxRedirects;
    var mime = utils.type(res.headers['content-type'] || '') || 'text/plain';
    var type = mime.split('/')[0];
    var multipart = 'multipart' == type;
    var redirect = isRedirect(res.statusCode);
    var parser = self._parser;
    var responseType = self._responseType;

    self.res = res;

    // redirect
    if (redirect && self._redirects++ != max) {
      return self._redirect(res);
    }

    if ('HEAD' == self.method) {
      self.emit('end');
      self.callback(null, self._emitResponse());
      return;
    }

    // zlib support
    if (self._shouldUnzip(res)) {
      unzip(req, res);
    }

    if (!parser) {
      if (responseType) {
        parser = exports.parse.image; // It's actually a generic Buffer
        buffer = true;
      } else if (multipart) {
        var form = new formidable.IncomingForm();
        parser = form.parse.bind(form);
        buffer = true;
      } else if (isImageOrVideo(mime)) {
        parser = exports.parse.image;
        buffer = true; // For backwards-compatibility buffering default is ad-hoc MIME-dependent
      } else if (exports.parse[mime]) {
        parser = exports.parse[mime];
      } else if ('text' == type) {
        parser = exports.parse.text;
        buffer = (buffer !== false);

        // everyone wants their own white-labeled json
      } else if (isJSON(mime)) {
        parser = exports.parse['application/json'];
        buffer = (buffer !== false);
      } else if (buffer) {
        parser = exports.parse.text;
      }
    }

    // by default only buffer text/*, json and messed up thing from hell
    if (undefined === buffer && isText(mime) || isJSON(mime)) {
      buffer = true;
    }

    var parserHandlesEnd = false;
    if (parser) {
      try {
        // Unbuffered parsers are supposed to emit response early,
        // which is weird BTW, because response.body won't be there.
        parserHandlesEnd = buffer;

        parser(res, function(err, obj, files) {
          if (self.timedout) {
            // Timeout has already handled all callbacks
            return;
          }

          // Intentional (non-timeout) abort is supposed to preserve partial response,
          // even if it doesn't parse.
          if (err && !self._aborted) {
            return self.callback(err);
          }

          if (parserHandlesEnd) {
            self.emit('end');
            self.callback(null, self._emitResponse(obj, files));
          }
        });
      } catch (err) {
        self.callback(err);
        return;
      }
    }

    self.res = res;

    // unbuffered
    if (!buffer) {
      debug('unbuffered %s %s', self.method, self.url);
      self.callback(null, self._emitResponse());
      if (multipart) return // allow multipart to handle end event
      res.once('end', function(){
        debug('end %s %s', self.method, self.url);
        self.emit('end');
      })
      return;
    }

    // terminating eve ...
```
- example usage
```shell
...

// store callback
this._callback = fn || noop;

// querystring
this._appendQueryString();

return this._end();
};

Request.prototype._end = function() {
var self = this;
var xhr = this.xhr = request.getXHR();
var data = this._formData || this._data;
...
```

#### <a name="apidoc.element.superagent.Request.prototype._getFormData"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_getFormData ()](#apidoc.element.superagent.Request.prototype._getFormData)
- description and source-code
```javascript
_getFormData = function () {
  if (!this._formData) {
    this._formData = new FormData();
    var that = this;
    this._formData.on('error', function(err) {
      that.emit('error', err);
      that.abort();
    });
  }
  return this._formData;
}
```
- example usage
```shell
...

Request.prototype.attach = function(field, file, options){
if (file) {
  if (this._data) {
    throw Error("superagent can't mix .send() and .attach()");
  }

  this._getFormData().append(field, file, options || file.name);
}
return this;
};

Request.prototype._getFormData = function(){
if (!this._formData) {
  this._formData = new root.FormData();
...
```

#### <a name="apidoc.element.superagent.Request.prototype._isHost"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_isHost (obj)](#apidoc.element.superagent.Request.prototype._isHost)
- description and source-code
```javascript
function _isHost(obj) {
  return Buffer.isBuffer(obj) || obj instanceof Stream || obj instanceof FormData;
}
```
- example usage
```shell
...
  return this.callback(err);
}

// CORS
if (this._withCredentials) xhr.withCredentials = true;

// body
if (!this._formData && 'GET' != this.method && 'HEAD' != this.method && 'string' != typeof data && !this._isHost(data)) {
  // serialize stuff
  var contentType = this._header['content-type'];
  var serialize = this._serializer || request.serialize[contentType ? contentType.split(';')[0] : ''];
  if (!serialize && isJSON(contentType)) {
    serialize = request.serialize['application/json'];
  }
  if (serialize) data = serialize(data);
...
```

#### <a name="apidoc.element.superagent.Request.prototype._isResponseOK"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_isResponseOK (res)](#apidoc.element.superagent.Request.prototype._isResponseOK)
- description and source-code
```javascript
_isResponseOK = function (res) {
  if (!res) {
    return false;
  }

  if (this._okCallback) {
    return this._okCallback(res);
  }

  return res.status >= 200 && res.status < 300;
}
```
- example usage
```shell
...
  return self.callback(err);
}

self.emit('response', res);

var new_err;
try {
  if (!self._isResponseOK(res)) {
    new_err = new Error(res.statusText || 'Unsuccessful HTTP response');
    new_err.original = err;
    new_err.response = res;
    new_err.status = res.status;
  }
} catch(e) {
  new_err = e; // #985 touching res may cause INVALID_STATE_ERR on old Android
...
```

#### <a name="apidoc.element.superagent.Request.prototype._pipeContinue"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_pipeContinue (stream, options)](#apidoc.element.superagent.Request.prototype._pipeContinue)
- description and source-code
```javascript
_pipeContinue = function (stream, options){
  var self = this;
  this.req.once('response', function(res){
    // redirect
    var redirect = isRedirect(res.statusCode);
    if (redirect && self._redirects++ != self._maxRedirects) {
      return self._redirect(res)._pipeContinue(stream, options);
    }

    self.res = res;
    self._emitResponse();
    if (self._aborted) return;

    if (self._shouldUnzip(res)) {
      res.pipe(zlib.createUnzip()).pipe(stream, options);
    } else {
      res.pipe(stream, options);
    }
    res.once('end', function(){
      self.emit('end');
    });
  });
  return stream;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype._redirect"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_redirect (res)](#apidoc.element.superagent.Request.prototype._redirect)
- description and source-code
```javascript
_redirect = function (res){
  var url = res.headers.location;
  if (!url) {
    return this.callback(new Error('No location header for redirect'), res);
  }

  debug('redirect %s -> %s', this.url, url);

  // location
  url = resolve(this.url, url);

  // ensure the response is being consumed
  // this is required for Node v0.10+
  res.resume();

  var headers = this.req._headers;

  var shouldStripCookie = parse(url).host !== parse(this.url).host;

  // implementation of 302 following defacto standard
  if (res.statusCode == 301 || res.statusCode == 302){
    // strip Content-* related fields
    // in case of POST etc
    headers = utils.cleanHeader(this.req._headers, shouldStripCookie);

    // force GET
    this.method = 'HEAD' == this.method
      ? 'HEAD'
      : 'GET';

    // clear data
    this._data = null;
  }
  // 303 is always GET
  if (res.statusCode == 303) {
    // strip Content-* related fields
    // in case of POST etc
    headers = utils.cleanHeader(this.req._headers, shouldStripCookie);

    // force method
    this.method = 'GET';

    // clear data
    this._data = null;
  }
  // 307 preserves method
  // 308 preserves method
  delete headers.host;

  delete this.req;
  delete this._formData;

  // remove all add header except User-Agent
  _initHeaders(this)

  // redirect
  this._endCalled = false;
  this.url = url;
  this.qs = {};
  this.qsRaw = [];
  this.set(headers);
  this.emit('redirect', res);
  this._redirectList.push(this.url);
  this.end(this._callback);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype._retry"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_retry ()](#apidoc.element.superagent.Request.prototype._retry)
- description and source-code
```javascript
_retry = function () {
  this.clearTimeout();

  // node
  if (this.req) {
    this.req = null;
    this.req = this.request();
  }

  this._aborted = false;
  this.timedout = false;

  return this._end();
}
```
- example usage
```shell
...
 * @param {Response} res
 * @api private
 */

Request.prototype.callback = function(err, res){
// console.log(this._retries, this._maxRetries)
if (this._maxRetries && this._retries++ < this._maxRetries && shouldRetry(err, res)) {
  return this._retry();
}

var fn = this._callback;
this.clearTimeout();

if (err) {
  if (this._maxRetries) err.retries = this._retries - 1;
...
```

#### <a name="apidoc.element.superagent.Request.prototype._setTimeouts"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_setTimeouts ()](#apidoc.element.superagent.Request.prototype._setTimeouts)
- description and source-code
```javascript
_setTimeouts = function () {
  var self = this;

  // deadline
  if (this._timeout && !this._timer) {
    this._timer = setTimeout(function(){
      self._timeoutError('Timeout of ', self._timeout, 'ETIME');
    }, this._timeout);
  }
  // response timeout
  if (this._responseTimeout && !this._responseTimeoutTimer) {
    this._responseTimeoutTimer = setTimeout(function(){
      self._timeoutError('Response timeout of ', self._responseTimeout, 'ETIMEDOUT');
    }, this._responseTimeout);
  }
}
```
- example usage
```shell
...
};

Request.prototype._end = function() {
var self = this;
var xhr = this.xhr = request.getXHR();
var data = this._formData || this._data;

this._setTimeouts();

// state change
xhr.onreadystatechange = function(){
  var readyState = xhr.readyState;
  if (readyState >= 2 && self._responseTimeoutTimer) {
    clearTimeout(self._responseTimeoutTimer);
  }
...
```

#### <a name="apidoc.element.superagent.Request.prototype._shouldUnzip"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_shouldUnzip (res)](#apidoc.element.superagent.Request.prototype._shouldUnzip)
- description and source-code
```javascript
_shouldUnzip = function (res){
  if (res.statusCode === 204 || res.statusCode === 304) {
    // These aren't supposed to have any body
    return false;
  }

  // header content is a string, and distinction between 0 and no information is crucial
  if ('0' === res.headers['content-length']) {
    // We know that the body is empty (unfortunately, this check does not cover chunked encoding)
    return false;
  }

  // console.log(res);
  return /^\s*(?:deflate|gzip)\s*$/.test(res.headers['content-encoding']);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype._timeoutError"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>_timeoutError (reason, timeout, errno)](#apidoc.element.superagent.Request.prototype._timeoutError)
- description and source-code
```javascript
_timeoutError = function (reason, timeout, errno){
  if (this._aborted) {
    return;
  }
  var err = new Error(reason + timeout + 'ms exceeded');
  err.timeout = timeout;
  err.code = 'ECONNABORTED';
  err.errno = errno;
  this.timedout = true;
  this.abort();
  this.callback(err);
}
```
- example usage
```shell
...

RequestBase.prototype._setTimeouts = function() {
var self = this;

// deadline
if (this._timeout && !this._timer) {
  this._timer = setTimeout(function(){
    self._timeoutError('Timeout of ', self._timeout, 'ETIME');
  }, this._timeout);
}
// response timeout
if (this._responseTimeout && !this._responseTimeoutTimer) {
  this._responseTimeoutTimer = setTimeout(function(){
    self._timeoutError('Response timeout of ', self._responseTimeout, 'ETIMEDOUT');
  }, this._responseTimeout);
...
```

#### <a name="apidoc.element.superagent.Request.prototype.abort"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>abort ()](#apidoc.element.superagent.Request.prototype.abort)
- description and source-code
```javascript
abort = function (){
  if (this._aborted) {
    return this;
  }
  this._aborted = true;
  this.xhr && this.xhr.abort(); // browser
  this.req && this.req.abort(); // node
  this.clearTimeout();
  this.emit('abort');
  return this;
}
```
- example usage
```shell
...
 * @api public
 */
RequestBase.prototype.abort = function(){
  if (this._aborted) {
    return this;
  }
  this._aborted = true;
  this.xhr && this.xhr.abort(); // browser
  this.req && this.req.abort(); // node
  this.clearTimeout();
  this.emit('abort');
  return this;
};

/**
...
```

#### <a name="apidoc.element.superagent.Request.prototype.accept"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>accept (type)](#apidoc.element.superagent.Request.prototype.accept)
- description and source-code
```javascript
accept = function (type){
  return this.set('Accept', ~type.indexOf('/')
    ? type
    : mime.lookup(type));
}
```
- example usage
```shell
...
* Set Accept to 'type', mapping values from 'request.types'.
*
* Examples:
*
*      superagent.types.json = 'application/json';
*
*      request.get('/agent')
*        .accept('json')
*        .end(callback);
*
*      request.get('/agent')
*        .accept('application/json')
*        .end(callback);
*
* @param {String} accept
...
```

#### <a name="apidoc.element.superagent.Request.prototype.agent"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>agent (agent)](#apidoc.element.superagent.Request.prototype.agent)
- description and source-code
```javascript
agent = function (agent){
  if (!arguments.length) return this._agent;
  this._agent = agent;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype.attach"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>attach (field, file, options)](#apidoc.element.superagent.Request.prototype.attach)
- description and source-code
```javascript
attach = function (field, file, options){
  if (file) {
    if (this._data) {
      throw Error("superagent can't mix .send() and .attach()");
    }

    var o = options || {};
    if ('string' == typeof options) {
      o = { filename: options };
    }

    if ('string' == typeof file) {
      if (!o.filename) o.filename = file;
      debug('creating 'fs.ReadStream' instance for file: %s', file);
      file = fs.createReadStream(file);
    } else if (!o.filename && file.path) {
      o.filename = file.path;
    }

    this._getFormData().append(field, file, o);
  }
  return this;
}
```
- example usage
```shell
...

/**
* Queue the given 'file' as an attachment to the specified 'field',
* with optional 'options' (or filename).
*
* ''' js
* request.post('/upload')
*   .attach('content', new Blob(['<a id="a"><b id="b">hey!</b></a>'], { type: "text/html"}))
*   .end(callback);
* '''
*
* @param {String} field
* @param {Blob|File} file
* @param {String|Object} options
* @return {Request} for chaining
...
```

#### <a name="apidoc.element.superagent.Request.prototype.auth"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>auth (user, pass, options)](#apidoc.element.superagent.Request.prototype.auth)
- description and source-code
```javascript
auth = function (user, pass, options){
  if (1 === arguments.length) pass = '';
  if (2 === arguments.length && typeof pass === 'object') options = pass;
  if (!options) {
    options = { type: 'basic' };
  }
  switch (options.type) {
    case 'bearer':
      return this.set('Authorization', 'Bearer ' + user);

    default: // 'basic'
      if (!~user.indexOf(':')) user = user + ':';
      var str = new Buffer(user + pass).toString('base64');
      return this.set('Authorization', 'Basic ' + str);
  }
}
```
- example usage
```shell
...
    break;

    case 'auto':
      this.username = user;
      this.password = pass;
    break;

    case 'bearer': // usage would be .auth(accessToken, { type: 'bearer' })
      this.set('Authorization', 'Bearer ' + user);
    break;
  }
  return this;
};

/**
...
```

#### <a name="apidoc.element.superagent.Request.prototype.buffer"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>buffer (val)](#apidoc.element.superagent.Request.prototype.buffer)
- description and source-code
```javascript
buffer = function (val){
  this._buffer = (false !== val);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype.ca"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>ca (cert)](#apidoc.element.superagent.Request.prototype.ca)
- description and source-code
```javascript
ca = function (cert){
  this._ca = cert;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype.callback"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>callback (err, res)](#apidoc.element.superagent.Request.prototype.callback)
- description and source-code
```javascript
callback = function (err, res){
  // console.log(this._retries, this._maxRetries)
  if (this._maxRetries && this._retries++ < this._maxRetries && shouldRetry(err, res)) {
    return this._retry();
  }

  // Avoid the error which is emitted from 'socket hang up' to cause the fn undefined error on JS runtime.
  var fn = this._callback || noop;
  this.clearTimeout();
  if (this.called) return console.warn('superagent: double callback bug');
  this.called = true;

  if (!err) {
    if (this._isResponseOK(res)) {
      return fn(err, res);
    }

    var msg = 'Unsuccessful HTTP response';
    if (res) {
      msg = http.STATUS_CODES[res.status] || msg;
    }
    err = new Error(msg);
    err.status = res ? res.status : undefined;
  }

  err.response = res;
  if (this._maxRetries) err.retries = this._retries - 1;

  // only emit error event if there is a listener
  // otherwise we assume the callback to '.end()' will get the error
  if (err && this.listeners('error').length > 0) {
    this.emit('error', err);
  }

  fn(err, res);
}
```
- example usage
```shell
...
    err.status = self.xhr.status ? self.xhr.status : null;
    err.statusCode = err.status; // backwards-compat only
  } else {
    err.rawResponse = null;
    err.status = null;
  }

  return self.callback(err);
}

self.emit('response', res);

var new_err;
try {
  if (!self._isResponseOK(res)) {
...
```

#### <a name="apidoc.element.superagent.Request.prototype.catch"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>catch (cb)](#apidoc.element.superagent.Request.prototype.catch)
- description and source-code
```javascript
catch = function (cb) {
  return this.then(undefined, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype.cert"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>cert (cert)](#apidoc.element.superagent.Request.prototype.cert)
- description and source-code
```javascript
cert = function (cert){
  this._cert = cert;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype.clearTimeout"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>clearTimeout ()](#apidoc.element.superagent.Request.prototype.clearTimeout)
- description and source-code
```javascript
function _clearTimeout(){
  clearTimeout(this._timer);
  clearTimeout(this._responseTimeoutTimer);
  delete this._timer;
  delete this._responseTimeoutTimer;
  return this;
}
```
- example usage
```shell
...
Request.prototype.callback = function(err, res){
// console.log(this._retries, this._maxRetries)
if (this._maxRetries && this._retries++ < this._maxRetries && shouldRetry(err, res)) {
  return this._retry();
}

var fn = this._callback;
this.clearTimeout();

if (err) {
  if (this._maxRetries) err.retries = this._retries - 1;
  this.emit('error', err);
}

fn(err, res);
...
```

#### <a name="apidoc.element.superagent.Request.prototype.end"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>end (fn)](#apidoc.element.superagent.Request.prototype.end)
- description and source-code
```javascript
end = function (fn){
  this.request();
  debug('%s %s', this.method, this.url);

  if (this._endCalled) {
    console.warn("Warning: .end() was called twice. This is not supported in superagent");
  }
  this._endCalled = true;

  // store callback
  this._callback = fn || noop;

  return this._end();
}
```
- example usage
```shell
...

'''js
request
  .post('/api/pet')
  .send({ name: 'Manny', species: 'cat' })
  .set('X-API-Key', 'foobar')
  .set('Accept', 'application/json')
  .end(function(err, res){
    // Calling the end function will send the request
  });
'''

## Supported browsers and Node versions

Tested browsers:
...
```

#### <a name="apidoc.element.superagent.Request.prototype.field"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>field (name, val)](#apidoc.element.superagent.Request.prototype.field)
- description and source-code
```javascript
field = function (name, val) {

  // name should be either a string or an object.
  if (null === name ||  undefined === name) {
    throw new Error('.field(name, val) name can not be empty');
  }

  if (this._data) {
    console.error(".field() can't be used if .send() is used. Please use only .send() or only .field() & .attach()");
  }

  if (isObject(name)) {
    for (var key in name) {
      this.field(key, name[key]);
    }
    return this;
  }

  if (Array.isArray(val)) {
    for (var i in val) {
      this.field(name, val[i]);
    }
    return this;
  }

  // val should be defined now
  if (null === val || undefined === val) {
    throw new Error('.field(name, val) val can not be empty');
  }
  if ('boolean' === typeof val) {
    val = '' + val;
  }
  this._getFormData().append(name, val);
  return this;
}
```
- example usage
```shell
...

Tested browsers:

- Latest Firefox, Chrome, Safari
- Latest Android, iPhone
- IE10 through latest. IE9 with polyfills.

Even though IE9 is supported, a polyfill for 'window.FormData' is required for '.field()'.

Node 4 or later is required.

# Plugins

SuperAgent is easily extended via plugins.
...
```

#### <a name="apidoc.element.superagent.Request.prototype.get"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>get (field)](#apidoc.element.superagent.Request.prototype.get)
- description and source-code
```javascript
get = function (field){
  return this._header[field.toLowerCase()];
}
```
- example usage
```shell
...

'''js
var nocache = require('superagent-no-cache');
var request = require('superagent');
var prefix = require('superagent-prefix')('/static');

request
  .get('/some-url')
  .query({ action: 'edit', city: 'London' }) // query string
  .use(prefix) // Prefixes *only* this request
  .use(nocache) // Prevents caching of *only* this request
  .end(function(err, res){
    // Do something
  });
'''
...
```

#### <a name="apidoc.element.superagent.Request.prototype.getHeader"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>getHeader (field)](#apidoc.element.superagent.Request.prototype.getHeader)
- description and source-code
```javascript
getHeader = function (field){
  return this._header[field.toLowerCase()];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype.key"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>key (cert)](#apidoc.element.superagent.Request.prototype.key)
- description and source-code
```javascript
key = function (cert){
  this._key = cert;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype.ok"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>ok (cb)](#apidoc.element.superagent.Request.prototype.ok)
- description and source-code
```javascript
ok = function (cb) {
  if ('function' !== typeof cb) throw Error("Callback required");
  this._okCallback = cb;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype.parse"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>parse (fn)](#apidoc.element.superagent.Request.prototype.parse)
- description and source-code
```javascript
function parse(fn){
  this._parser = fn;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype.pfx"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>pfx (cert)](#apidoc.element.superagent.Request.prototype.pfx)
- description and source-code
```javascript
pfx = function (cert){
  this._pfx = cert;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype.pipe"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>pipe (stream, options)](#apidoc.element.superagent.Request.prototype.pipe)
- description and source-code
```javascript
pipe = function (stream, options){
  this.piped = true; // HACK...
  this.buffer(false);
  this.end();
  return this._pipeContinue(stream, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype.query"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>query (val)](#apidoc.element.superagent.Request.prototype.query)
- description and source-code
```javascript
query = function (val){
  if ('string' == typeof val) {
    this.qsRaw.push(val);
    return this;
  }

  extend(this.qs, val);
  return this;
}
```
- example usage
```shell
...
'''js
var nocache = require('superagent-no-cache');
var request = require('superagent');
var prefix = require('superagent-prefix')('/static');

request
  .get('/some-url')
  .query({ action: 'edit', city: 'London' }) // query string
  .use(prefix) // Prefixes *only* this request
  .use(nocache) // Prevents caching of *only* this request
  .end(function(err, res){
    // Do something
  });
'''
...
```

#### <a name="apidoc.element.superagent.Request.prototype.redirects"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>redirects (n)](#apidoc.element.superagent.Request.prototype.redirects)
- description and source-code
```javascript
redirects = function (n){
  this._maxRedirects = n;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype.request"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>request ()](#apidoc.element.superagent.Request.prototype.request)
- description and source-code
```javascript
request = function (){
  if (this.req) return this.req;

  var self = this;
  var options = {};
  var url = this.url;
  var retries = this._retries;

  // default to http://
  if (0 != url.indexOf('http')) url = 'http://' + url;
  url = parse(url);

  // support unix sockets
  if (/^https?\+unix:/.test(url.protocol) === true) {
    // get the protocol
    url.protocol = url.protocol.split('+')[0] + ':';

    // get the socket, path
    var unixParts = url.path.match(/^([^/]+)(.+)$/);
    options.socketPath = unixParts[1].replace(/%2F/g, '/');
    url.pathname = unixParts[2];
  }

  // options
  options.method = this.method;
  options.port = url.port;
  options.path = url.pathname;
  options.host = url.hostname;
  options.ca = this._ca;
  options.key = this._key;
  options.pfx = this._pfx;
  options.cert = this._cert;
  options.agent = this._agent;

  // initiate request
  var mod = exports.protocols[url.protocol];

  // request
  var req = this.req = mod.request(options);
  if ('HEAD' != options.method) {
    req.setHeader('Accept-Encoding', 'gzip, deflate');
  }
  this.protocol = url.protocol;
  this.host = url.host;

  // expose events
  req.once('drain', function(){ self.emit('drain'); });

  req.once('error', function(err){
    // flag abortion here for out timeouts
    // because node will emit a faux-error "socket hang up"
    // when request is aborted before a connection is made
    if (self._aborted) return;
    // if not the same, we are in the **old** (cancelled) request,
    // so need to continue (same as for above)
    if (self._retries !== retries) return;
    // if we've received a response then we don't want to let
    // an error in the request blow up the response
    if (self.response) return;
    self.callback(err);
  });

  // auth
  if (url.auth) {
    var auth = url.auth.split(':');
    this.auth(auth[0], auth[1]);
  }

  // query
  if (url.search)
    this.query(url.search.substr(1));

  // add cookies
  if (this.cookies) req.setHeader('Cookie', this.cookies);

  for (var key in this.header) {
    if (this.header.hasOwnProperty(key))
      req.setHeader(key, this.header[key]);
  }

  try {
    this._appendQueryString(req);
  } catch (e) {
    return this.emit('error', e);
  }

  return req;
}
```
- example usage
```shell
...

RequestBase.prototype._retry = function() {
  this.clearTimeout();

  // node
  if (this.req) {
    this.req = null;
    this.req = this.request();
  }

  this._aborted = false;
  this.timedout = false;

  return this._end();
};
...
```

#### <a name="apidoc.element.superagent.Request.prototype.responseType"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>responseType (val)](#apidoc.element.superagent.Request.prototype.responseType)
- description and source-code
```javascript
responseType = function (val){
  this._responseType = val;
  return this;
}
```
- example usage
```shell
...
* which return Blob and ArrayBuffer, respectively.
*
* In Node all values result in Buffer.
*
* Examples:
*
*      req.get('/')
*        .responseType('blob')
*        .end(callback);
*
* @param {String} val
* @return {Request} for chaining
* @api public
*/
...
```

#### <a name="apidoc.element.superagent.Request.prototype.retry"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>retry (count)](#apidoc.element.superagent.Request.prototype.retry)
- description and source-code
```javascript
function retry(count){
  // Default to 1 if no count passed or true
  if (arguments.length === 0 || count === true) count = 1;
  if (count <= 0) count = 0;
  this._maxRetries = count;
  this._retries = 0;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype.send"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>send (data)](#apidoc.element.superagent.Request.prototype.send)
- description and source-code
```javascript
send = function (data){
  var isObj = isObject(data);
  var type = this._header['content-type'];

  if (this._formData) {
    console.error(".send() can't be used if .attach() or .field() is used. Please use only .send() or only .field() & .attach()");
  }

  if (isObj && !this._data) {
    if (Array.isArray(data)) {
      this._data = [];
    } else if (!this._isHost(data)) {
      this._data = {};
    }
  } else if (data && this._data && this._isHost(this._data)) {
    throw Error("Can't merge these send calls");
  }

  // merge
  if (isObj && isObject(this._data)) {
    for (var key in data) {
      this._data[key] = data[key];
    }
  } else if ('string' == typeof data) {
    // default to x-www-form-urlencoded
    if (!type) this.type('form');
    type = this._header['content-type'];
    if ('application/x-www-form-urlencoded' == type) {
      this._data = this._data
        ? this._data + '&' + data
        : data;
    } else {
      this._data = (this._data || '') + data;
    }
  } else {
    this._data = data;
  }

  if (!isObj || this._isHost(data)) {
    return this;
  }

  // default to json
  if (!type) this.type('json');
  return this;
}
```
- example usage
```shell
...
'''

Works with [browserify](https://github.com/substack/node-browserify) and should work with [webpack](https://github.com/visionmedia
/superagent/wiki/SuperAgent-for-Webpack)

'''js
request
  .post('/api/pet')
  .send({ name: 'Manny', species: 'cat' })
  .set('X-API-Key', 'foobar')
  .set('Accept', 'application/json')
  .end(function(err, res){
    // Calling the end function will send the request
  });
'''
...
```

#### <a name="apidoc.element.superagent.Request.prototype.serialize"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>serialize (fn)](#apidoc.element.superagent.Request.prototype.serialize)
- description and source-code
```javascript
function serialize(fn){
  this._serializer = fn;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype.set"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>set (field, val)](#apidoc.element.superagent.Request.prototype.set)
- description and source-code
```javascript
set = function (field, val){
  if (isObject(field)) {
    for (var key in field) {
      this.set(key, field[key]);
    }
    return this;
  }
  this._header[field.toLowerCase()] = val;
  this.header[field] = val;
  return this;
}
```
- example usage
```shell
...

Works with [browserify](https://github.com/substack/node-browserify) and should work with [webpack](https://github.com/visionmedia
/superagent/wiki/SuperAgent-for-Webpack)

'''js
request
  .post('/api/pet')
  .send({ name: 'Manny', species: 'cat' })
  .set('X-API-Key', 'foobar')
  .set('Accept', 'application/json')
  .end(function(err, res){
    // Calling the end function will send the request
  });
'''

## Supported browsers and Node versions
...
```

#### <a name="apidoc.element.superagent.Request.prototype.sortQuery"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>sortQuery (sort)](#apidoc.element.superagent.Request.prototype.sortQuery)
- description and source-code
```javascript
sortQuery = function (sort) {
  // _sort default to true but otherwise can be a function or boolean
  this._sort = typeof sort === 'undefined' ? true : sort;
  return this;
}
```
- example usage
```shell
...
*
* Examples:
*
*       // default order
*       request.get('/user')
*         .query('name=Nick')
*         .query('search=Manny')
*         .sortQuery()
*         .end(callback)
*
*       // customized sort function
*       request.get('/user')
*         .query('name=Nick')
*         .query('search=Manny')
*         .sortQuery(function(a, b){
...
```

#### <a name="apidoc.element.superagent.Request.prototype.then"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>then (resolve, reject)](#apidoc.element.superagent.Request.prototype.then)
- description and source-code
```javascript
function then(resolve, reject) {
  if (!this._fullfilledPromise) {
    var self = this;
    if (this._endCalled) {
      console.warn("Warning: superagent request was sent twice, because both .end() and .then() were called. Never call .end() if
 you use promises");
    }
    this._fullfilledPromise = new Promise(function(innerResolve, innerReject){
      self.end(function(err, res){
        if (err) innerReject(err); else innerResolve(res);
      });
    });
  }
  return this._fullfilledPromise.then(resolve, reject);
}
```
- example usage
```shell
...
 * @return {Request}
 */

RequestBase.prototype.then = function then(resolve, reject) {
if (!this._fullfilledPromise) {
  var self = this;
  if (this._endCalled) {
    console.warn("Warning: superagent request was sent twice, because both .end() and .then() were called. Never call .end() if
you use promises");
  }
  this._fullfilledPromise = new Promise(function(innerResolve, innerReject){
    self.end(function(err, res){
      if (err) innerReject(err); else innerResolve(res);
    });
  });
}
...
```

#### <a name="apidoc.element.superagent.Request.prototype.timeout"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>timeout (options)](#apidoc.element.superagent.Request.prototype.timeout)
- description and source-code
```javascript
function timeout(options){
  if (!options || 'object' !== typeof options) {
    this._timeout = options;
    this._responseTimeout = 0;
    return this;
  }

  for(var option in options) {
    switch(option) {
      case 'deadline':
        this._timeout = options.deadline;
        break;
      case 'response':
        this._responseTimeout = options.response;
        break;
      default:
        console.warn("Unknown timeout option", option);
    }
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>toJSON ()](#apidoc.element.superagent.Request.prototype.toJSON)
- description and source-code
```javascript
toJSON = function (){
  return {
    method: this.method,
    url: this.url,
    data: this._data,
    headers: this._header
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype.type"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>type (type)](#apidoc.element.superagent.Request.prototype.type)
- description and source-code
```javascript
type = function (type){
  return this.set('Content-Type', ~type.indexOf('/')
    ? type
    : mime.lookup(type));
}
```
- example usage
```shell
...
* Set Content-Type to 'type', mapping values from 'request.types'.
*
* Examples:
*
*      superagent.types.xml = 'application/xml';
*
*      request.post('/')
*        .type('xml')
*        .send(xmlstring)
*        .end(callback);
*
*      request.post('/')
*        .type('application/xml')
*        .send(xmlstring)
*        .end(callback);
...
```

#### <a name="apidoc.element.superagent.Request.prototype.unset"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>unset (field)](#apidoc.element.superagent.Request.prototype.unset)
- description and source-code
```javascript
unset = function (field){
  delete this._header[field.toLowerCase()];
  delete this.header[field];
  return this;
}
```
- example usage
```shell
...
/**
 * Remove header 'field'.
 * Case-insensitive.
 *
 * Example:
 *
 *      req.get('/')
 *        .unset('User-Agent')
 *        .end(callback);
 *
 * @param {String} field
 */
RequestBase.prototype.unset = function(field){
delete this._header[field.toLowerCase()];
delete this.header[field];
...
```

#### <a name="apidoc.element.superagent.Request.prototype.use"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>use (fn)](#apidoc.element.superagent.Request.prototype.use)
- description and source-code
```javascript
function use(fn) {
  fn(this);
  return this;
}
```
- example usage
```shell
...
var nocache = require('superagent-no-cache');
var request = require('superagent');
var prefix = require('superagent-prefix')('/static');

request
  .get('/some-url')
  .query({ action: 'edit', city: 'London' }) // query string
  .use(prefix) // Prefixes *only* this request
  .use(nocache) // Prevents caching of *only* this request
  .end(function(err, res){
    // Do something
  });
'''

Existing plugins:
...
```

#### <a name="apidoc.element.superagent.Request.prototype.withCredentials"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>withCredentials (on)](#apidoc.element.superagent.Request.prototype.withCredentials)
- description and source-code
```javascript
withCredentials = function (on){
  // This is browser-only functionality. Node side is no-op.
  if(on==undefined) on = true;
  this._withCredentials = on;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Request.prototype.write"></a>[function <span class="apidocSignatureSpan">superagent.Request.prototype.</span>write (data, encoding)](#apidoc.element.superagent.Request.prototype.write)
- description and source-code
```javascript
write = function (data, encoding){
  var req = this.request();
  if (!this._streamRequest) {
    this._streamRequest = true;
  }
  return req.write(data, encoding);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.superagent.Response"></a>[module superagent.Response](#apidoc.module.superagent.Response)

#### <a name="apidoc.element.superagent.Response.Response"></a>[function <span class="apidocSignatureSpan">superagent.</span>Response (req)](#apidoc.element.superagent.Response.Response)
- description and source-code
```javascript
function Response(req) {
  Stream.call(this);
  var res = this.res = req.res;
  this.request = req;
  this.req = req.req;
  this.text = res.text;
  this.body = res.body !== undefined ? res.body : {};
  this.files = res.files || {};
  this.buffered = 'string' == typeof this.text;
  this.header = this.headers = res.headers;
  this._setStatusProperties(res.statusCode);
  this._setHeaderProperties(this.header);
  this.setEncoding = res.setEncoding.bind(res);
  res.on('data', this.emit.bind(this, 'data'));
  res.on('end', this.emit.bind(this, 'end'));
  res.on('close', this.emit.bind(this, 'close'));
  res.on('error', this.emit.bind(this, 'error'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Response.super_"></a>[function <span class="apidocSignatureSpan">superagent.Response.</span>super_ ()](#apidoc.element.superagent.Response.super_)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.superagent.Response.prototype"></a>[module superagent.Response.prototype](#apidoc.module.superagent.Response.prototype)

#### <a name="apidoc.element.superagent.Response.prototype._setHeaderProperties"></a>[function <span class="apidocSignatureSpan">superagent.Response.prototype.</span>_setHeaderProperties (header)](#apidoc.element.superagent.Response.prototype._setHeaderProperties)
- description and source-code
```javascript
_setHeaderProperties = function (header){
    // TODO: moar!
    // TODO: make this a util

    // content-type
    var ct = header['content-type'] || '';
    this.type = utils.type(ct);

    // params
    var params = utils.params(ct);
    for (var key in params) this[key] = params[key];

    this.links = {};

    // links
    try {
        if (header.link) {
            this.links = utils.parseLinks(header.link);
        }
    } catch (err) {
        // ignore
    }
}
```
- example usage
```shell
...
}
this._setStatusProperties(status);
this.header = this.headers = parseHeader(this.xhr.getAllResponseHeaders());
// getAllResponseHeaders sometimes falsely returns "" for CORS requests, but
// getResponseHeader still works. so we get content-type even if getting
// other headers fails.
this.header['content-type'] = this.xhr.getResponseHeader('content-type');
this._setHeaderProperties(this.header);

if (null === this.text && req._responseType) {
  this.body = this.xhr.response;
} else {
  this.body = this.req.method != 'HEAD'
    ? this._parseBody(this.text ? this.text : this.xhr.response)
    : null;
...
```

#### <a name="apidoc.element.superagent.Response.prototype._setStatusProperties"></a>[function <span class="apidocSignatureSpan">superagent.Response.prototype.</span>_setStatusProperties (status)](#apidoc.element.superagent.Response.prototype._setStatusProperties)
- description and source-code
```javascript
_setStatusProperties = function (status){
    var type = status / 100 | 0;

    // status / class
    this.status = this.statusCode = status;
    this.statusType = type;

    // basics
    this.info = 1 == type;
    this.ok = 2 == type;
    this.redirect = 3 == type;
    this.clientError = 4 == type;
    this.serverError = 5 == type;
    this.error = (4 == type || 5 == type)
        ? this.toError()
        : false;

    // sugar
    this.accepted = 202 == status;
    this.noContent = 204 == status;
    this.badRequest = 400 == status;
    this.unauthorized = 401 == status;
    this.notAcceptable = 406 == status;
    this.forbidden = 403 == status;
    this.notFound = 404 == status;
}
```
- example usage
```shell
...
   : null;
this.statusText = this.req.xhr.statusText;
var status = this.xhr.status;
// handle IE9 bug: http://stackoverflow.com/questions/10046972/msie-returns-status-code-of-1223-for-ajax-request
if (status === 1223) {
    status = 204;
}
this._setStatusProperties(status);
this.header = this.headers = parseHeader(this.xhr.getAllResponseHeaders());
// getAllResponseHeaders sometimes falsely returns "" for CORS requests, but
// getResponseHeader still works. so we get content-type even if getting
// other headers fails.
this.header['content-type'] = this.xhr.getResponseHeader('content-type');
this._setHeaderProperties(this.header);
...
```

#### <a name="apidoc.element.superagent.Response.prototype.destroy"></a>[function <span class="apidocSignatureSpan">superagent.Response.prototype.</span>destroy (err)](#apidoc.element.superagent.Response.prototype.destroy)
- description and source-code
```javascript
destroy = function (err){
  this.res.destroy(err);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Response.prototype.get"></a>[function <span class="apidocSignatureSpan">superagent.Response.prototype.</span>get (field)](#apidoc.element.superagent.Response.prototype.get)
- description and source-code
```javascript
get = function (field){
    return this.header[field.toLowerCase()];
}
```
- example usage
```shell
...

'''js
var nocache = require('superagent-no-cache');
var request = require('superagent');
var prefix = require('superagent-prefix')('/static');

request
  .get('/some-url')
  .query({ action: 'edit', city: 'London' }) // query string
  .use(prefix) // Prefixes *only* this request
  .use(nocache) // Prevents caching of *only* this request
  .end(function(err, res){
    // Do something
  });
'''
...
```

#### <a name="apidoc.element.superagent.Response.prototype.pause"></a>[function <span class="apidocSignatureSpan">superagent.Response.prototype.</span>pause ()](#apidoc.element.superagent.Response.prototype.pause)
- description and source-code
```javascript
pause = function (){
  this.res.pause();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Response.prototype.resume"></a>[function <span class="apidocSignatureSpan">superagent.Response.prototype.</span>resume ()](#apidoc.element.superagent.Response.prototype.resume)
- description and source-code
```javascript
resume = function (){
  this.res.resume();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Response.prototype.setStatusProperties"></a>[function <span class="apidocSignatureSpan">superagent.Response.prototype.</span>setStatusProperties (status)](#apidoc.element.superagent.Response.prototype.setStatusProperties)
- description and source-code
```javascript
setStatusProperties = function (status){
  console.warn("In superagent 2.x setStatusProperties is a private method");
  return this._setStatusProperties(status);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.Response.prototype.toError"></a>[function <span class="apidocSignatureSpan">superagent.Response.prototype.</span>toError ()](#apidoc.element.superagent.Response.prototype.toError)
- description and source-code
```javascript
toError = function (){
  var req = this.req;
  var method = req.method;
  var path = req.path;

  var msg = 'cannot ' + method + ' ' + path + ' (' + this.status + ')';
  var err = new Error(msg);
  err.status = this.status;
  err.text = this.text;
  err.method = method;
  err.path = path;

  return err;
}
```
- example usage
```shell
...
// basics
this.info = 1 == type;
this.ok = 2 == type;
this.redirect = 3 == type;
this.clientError = 4 == type;
this.serverError = 5 == type;
this.error = (4 == type || 5 == type)
    ? this.toError()
    : false;

// sugar
this.accepted = 202 == status;
this.noContent = 204 == status;
this.badRequest = 400 == status;
this.unauthorized = 401 == status;
...
```

#### <a name="apidoc.element.superagent.Response.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">superagent.Response.prototype.</span>toJSON ()](#apidoc.element.superagent.Response.prototype.toJSON)
- description and source-code
```javascript
toJSON = function (){
  return {
    req: this.request.toJSON(),
    header: this.header,
    status: this.status,
    text: this.text
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.superagent.agent"></a>[module superagent.agent](#apidoc.module.superagent.agent)

#### <a name="apidoc.element.superagent.agent.agent"></a>[function <span class="apidocSignatureSpan">superagent.</span>agent (options)](#apidoc.element.superagent.agent.agent)
- description and source-code
```javascript
function Agent(options) {
  if (!(this instanceof Agent)) return new Agent(options);
  if (options) {
    this._ca = options.ca;
    this._key = options.key;
    this._pfx = options.pfx;
    this._cert = options.cert;
  }
  this.jar = new CookieJar;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.superagent.agent.prototype"></a>[module superagent.agent.prototype](#apidoc.module.superagent.agent.prototype)

#### <a name="apidoc.element.superagent.agent.prototype._attachCookies"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>_attachCookies (req)](#apidoc.element.superagent.agent.prototype._attachCookies)
- description and source-code
```javascript
_attachCookies = function (req){
  var url = parse(req.url);
  var access = CookieAccess(url.hostname, url.pathname, 'https:' == url.protocol);
  var cookies = this.jar.getCookies(access).toValueString();
  req.cookies = cookies;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype._saveCookies"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>_saveCookies (res)](#apidoc.element.superagent.agent.prototype._saveCookies)
- description and source-code
```javascript
_saveCookies = function (res){
  var cookies = res.headers['set-cookie'];
  if (cookies) this.jar.setCookies(cookies);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.acl"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>acl (url, fn)](#apidoc.element.superagent.agent.prototype.acl)
- description and source-code
```javascript
acl = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.bind"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>bind (url, fn)](#apidoc.element.superagent.agent.prototype.bind)
- description and source-code
```javascript
bind = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
...
    e.percent = e.loaded / e.total * 100;
  }
  e.direction = direction;
  self.emit('progress', e);
}
if (this.hasListeners('progress')) {
  try {
    xhr.onprogress = handleProgress.bind(null, 'download');
    if (xhr.upload) {
      xhr.upload.onprogress = handleProgress.bind(null, 'upload');
    }
  } catch(e) {
    // Accessing xhr.upload fails in IE from a web worker, so just pretend it doesn't exist.
    // Reported here:
    // https://connect.microsoft.com/IE/feedback/details/837245/xmlhttprequest-upload-throws-invalid-argument-when-used-from-web
-worker-context
...
```

#### <a name="apidoc.element.superagent.agent.prototype.checkout"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>checkout (url, fn)](#apidoc.element.superagent.agent.prototype.checkout)
- description and source-code
```javascript
checkout = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.connect"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>connect (url, fn)](#apidoc.element.superagent.agent.prototype.connect)
- description and source-code
```javascript
connect = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.copy"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>copy (url, fn)](#apidoc.element.superagent.agent.prototype.copy)
- description and source-code
```javascript
copy = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.del"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>del (url, fn)](#apidoc.element.superagent.agent.prototype.del)
- description and source-code
```javascript
del = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.delete"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>delete (url, fn)](#apidoc.element.superagent.agent.prototype.delete)
- description and source-code
```javascript
delete = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.get"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>get (url, fn)](#apidoc.element.superagent.agent.prototype.get)
- description and source-code
```javascript
get = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
...

'''js
var nocache = require('superagent-no-cache');
var request = require('superagent');
var prefix = require('superagent-prefix')('/static');

request
  .get('/some-url')
  .query({ action: 'edit', city: 'London' }) // query string
  .use(prefix) // Prefixes *only* this request
  .use(nocache) // Prevents caching of *only* this request
  .end(function(err, res){
    // Do something
  });
'''
...
```

#### <a name="apidoc.element.superagent.agent.prototype.head"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>head (url, fn)](#apidoc.element.superagent.agent.prototype.head)
- description and source-code
```javascript
head = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.link"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>link (url, fn)](#apidoc.element.superagent.agent.prototype.link)
- description and source-code
```javascript
link = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.lock"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>lock (url, fn)](#apidoc.element.superagent.agent.prototype.lock)
- description and source-code
```javascript
lock = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.m-search"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>m-search (url, fn)](#apidoc.element.superagent.agent.prototype.m-search)
- description and source-code
```javascript
m-search = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.merge"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>merge (url, fn)](#apidoc.element.superagent.agent.prototype.merge)
- description and source-code
```javascript
merge = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.mkactivity"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>mkactivity (url, fn)](#apidoc.element.superagent.agent.prototype.mkactivity)
- description and source-code
```javascript
mkactivity = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.mkcalendar"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>mkcalendar (url, fn)](#apidoc.element.superagent.agent.prototype.mkcalendar)
- description and source-code
```javascript
mkcalendar = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.mkcol"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>mkcol (url, fn)](#apidoc.element.superagent.agent.prototype.mkcol)
- description and source-code
```javascript
mkcol = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.move"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>move (url, fn)](#apidoc.element.superagent.agent.prototype.move)
- description and source-code
```javascript
move = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.notify"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>notify (url, fn)](#apidoc.element.superagent.agent.prototype.notify)
- description and source-code
```javascript
notify = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.options"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>options (url, fn)](#apidoc.element.superagent.agent.prototype.options)
- description and source-code
```javascript
options = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.patch"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>patch (url, fn)](#apidoc.element.superagent.agent.prototype.patch)
- description and source-code
```javascript
patch = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.post"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>post (url, fn)](#apidoc.element.superagent.agent.prototype.post)
- description and source-code
```javascript
post = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
...
$ npm install superagent
'''

Works with [browserify](https://github.com/substack/node-browserify) and should work with [webpack](https://github.com/visionmedia
/superagent/wiki/SuperAgent-for-Webpack)

'''js
request
  .post('/api/pet')
  .send({ name: 'Manny', species: 'cat' })
  .set('X-API-Key', 'foobar')
  .set('Accept', 'application/json')
  .end(function(err, res){
    // Calling the end function will send the request
  });
'''
...
```

#### <a name="apidoc.element.superagent.agent.prototype.propfind"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>propfind (url, fn)](#apidoc.element.superagent.agent.prototype.propfind)
- description and source-code
```javascript
propfind = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.proppatch"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>proppatch (url, fn)](#apidoc.element.superagent.agent.prototype.proppatch)
- description and source-code
```javascript
proppatch = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.purge"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>purge (url, fn)](#apidoc.element.superagent.agent.prototype.purge)
- description and source-code
```javascript
purge = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.put"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>put (url, fn)](#apidoc.element.superagent.agent.prototype.put)
- description and source-code
```javascript
put = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.rebind"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>rebind (url, fn)](#apidoc.element.superagent.agent.prototype.rebind)
- description and source-code
```javascript
rebind = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.report"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>report (url, fn)](#apidoc.element.superagent.agent.prototype.report)
- description and source-code
```javascript
report = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.search"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>search (url, fn)](#apidoc.element.superagent.agent.prototype.search)
- description and source-code
```javascript
search = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.subscribe"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>subscribe (url, fn)](#apidoc.element.superagent.agent.prototype.subscribe)
- description and source-code
```javascript
subscribe = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.trace"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>trace (url, fn)](#apidoc.element.superagent.agent.prototype.trace)
- description and source-code
```javascript
trace = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.unbind"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>unbind (url, fn)](#apidoc.element.superagent.agent.prototype.unbind)
- description and source-code
```javascript
unbind = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.unlink"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>unlink (url, fn)](#apidoc.element.superagent.agent.prototype.unlink)
- description and source-code
```javascript
unlink = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.unlock"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>unlock (url, fn)](#apidoc.element.superagent.agent.prototype.unlock)
- description and source-code
```javascript
unlock = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.agent.prototype.unsubscribe"></a>[function <span class="apidocSignatureSpan">superagent.agent.prototype.</span>unsubscribe (url, fn)](#apidoc.element.superagent.agent.prototype.unsubscribe)
- description and source-code
```javascript
unsubscribe = function (url, fn){
  var req = new request.Request(method, url);
  req.ca(this._ca);
  req.key(this._key);
  req.pfx(this._pfx);
  req.cert(this._cert);

  req.on('response', this._saveCookies.bind(this));
  req.on('redirect', this._saveCookies.bind(this));
  req.on('redirect', this._attachCookies.bind(this, req));
  this._attachCookies(req);

  fn && req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.superagent.client"></a>[module superagent.client](#apidoc.module.superagent.client)

#### <a name="apidoc.element.superagent.client.client"></a>[function <span class="apidocSignatureSpan">superagent.</span>client (method, url)](#apidoc.element.superagent.client.client)
- description and source-code
```javascript
client = function (method, url) {
  // callback
  if ('function' == typeof url) {
    return new exports.Request('GET', method).end(url);
  }

  // url first
  if (1 == arguments.length) {
    return new exports.Request('GET', method);
  }

  return new exports.Request(method, url);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.client.Request"></a>[function <span class="apidocSignatureSpan">superagent.client.</span>Request (method, url)](#apidoc.element.superagent.client.Request)
- description and source-code
```javascript
function Request(method, url) {
  var self = this;
  this._query = this._query || [];
  this.method = method;
  this.url = url;
  this.header = {}; // preserves header name case
  this._header = {}; // coerces header names to lowercase
  this.on('end', function(){
    var err = null;
    var res = null;

    try {
      res = new Response(self);
    } catch(e) {
      err = new Error('Parser is unable to parse the response');
      err.parse = true;
      err.original = e;
      // issue #675: return the raw response if the response parsing fails
      if (self.xhr) {
        // ie9 doesn't have 'response' property
        err.rawResponse = typeof self.xhr.responseType == 'undefined' ? self.xhr.responseText : self.xhr.response;
        // issue #876: return the http status code if the response parsing fails
        err.status = self.xhr.status ? self.xhr.status : null;
        err.statusCode = err.status; // backwards-compat only
      } else {
        err.rawResponse = null;
        err.status = null;
      }

      return self.callback(err);
    }

    self.emit('response', res);

    var new_err;
    try {
      if (!self._isResponseOK(res)) {
        new_err = new Error(res.statusText || 'Unsuccessful HTTP response');
        new_err.original = err;
        new_err.response = res;
        new_err.status = res.status;
      }
    } catch(e) {
      new_err = e; // #985 touching res may cause INVALID_STATE_ERR on old Android
    }

    // #1000 don't catch errors from the callback to avoid double calling it
    if (new_err) {
      self.callback(new_err, res);
    } else {
      self.callback(null, res);
    }
  });
}
```
- example usage
```shell
...
/**
 * Expose 'request'.
 */

var request = exports = module.exports = function(method, url) {
// callback
if ('function' == typeof url) {
  return new exports.Request('GET', method).end(url);
}

// url first
if (1 == arguments.length) {
  return new exports.Request('GET', method);
}
...
```

#### <a name="apidoc.element.superagent.client.Response"></a>[function <span class="apidocSignatureSpan">superagent.client.</span>Response (req)](#apidoc.element.superagent.client.Response)
- description and source-code
```javascript
function Response(req) {
  this.req = req;
  this.xhr = this.req.xhr;
  // responseText is accessible only if responseType is '' or 'text' and on older browsers
  this.text = ((this.req.method !='HEAD' && (this.xhr.responseType === '' || this.xhr.responseType === 'text')) || typeof this.xhr
.responseType === 'undefined')
     ? this.xhr.responseText
     : null;
  this.statusText = this.req.xhr.statusText;
  var status = this.xhr.status;
  // handle IE9 bug: http://stackoverflow.com/questions/10046972/msie-returns-status-code-of-1223-for-ajax-request
  if (status === 1223) {
      status = 204;
  }
  this._setStatusProperties(status);
  this.header = this.headers = parseHeader(this.xhr.getAllResponseHeaders());
  // getAllResponseHeaders sometimes falsely returns "" for CORS requests, but
  // getResponseHeader still works. so we get content-type even if getting
  // other headers fails.
  this.header['content-type'] = this.xhr.getResponseHeader('content-type');
  this._setHeaderProperties(this.header);

  if (null === this.text && req._responseType) {
    this.body = this.xhr.response;
  } else {
    this.body = this.req.method != 'HEAD'
      ? this._parseBody(this.text ? this.text : this.xhr.response)
      : null;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.client.del"></a>[function <span class="apidocSignatureSpan">superagent.client.</span>del (url, data, fn)](#apidoc.element.superagent.client.del)
- description and source-code
```javascript
function del(url, data, fn){
  var req = request('DELETE', url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  if (fn) req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.client.delete"></a>[function <span class="apidocSignatureSpan">superagent.client.</span>delete (url, data, fn)](#apidoc.element.superagent.client.delete)
- description and source-code
```javascript
function del(url, data, fn){
  var req = request('DELETE', url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  if (fn) req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.client.get"></a>[function <span class="apidocSignatureSpan">superagent.client.</span>get (url, data, fn)](#apidoc.element.superagent.client.get)
- description and source-code
```javascript
get = function (url, data, fn){
  var req = request('GET', url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.query(data);
  if (fn) req.end(fn);
  return req;
}
```
- example usage
```shell
...

'''js
var nocache = require('superagent-no-cache');
var request = require('superagent');
var prefix = require('superagent-prefix')('/static');

request
  .get('/some-url')
  .query({ action: 'edit', city: 'London' }) // query string
  .use(prefix) // Prefixes *only* this request
  .use(nocache) // Prevents caching of *only* this request
  .end(function(err, res){
    // Do something
  });
'''
...
```

#### <a name="apidoc.element.superagent.client.getXHR"></a>[function <span class="apidocSignatureSpan">superagent.client.</span>getXHR ()](#apidoc.element.superagent.client.getXHR)
- description and source-code
```javascript
getXHR = function () {
  if (root.XMLHttpRequest
      && (!root.location || 'file:' != root.location.protocol
          || !root.ActiveXObject)) {
    return new XMLHttpRequest;
  } else {
    try { return new ActiveXObject('Microsoft.XMLHTTP'); } catch(e) {}
    try { return new ActiveXObject('Msxml2.XMLHTTP.6.0'); } catch(e) {}
    try { return new ActiveXObject('Msxml2.XMLHTTP.3.0'); } catch(e) {}
    try { return new ActiveXObject('Msxml2.XMLHTTP'); } catch(e) {}
  }
  throw Error("Browser-only verison of superagent could not find XHR");
}
```
- example usage
```shell
...
this._appendQueryString();

return this._end();
};

Request.prototype._end = function() {
var self = this;
var xhr = this.xhr = request.getXHR();
var data = this._formData || this._data;

this._setTimeouts();

// state change
xhr.onreadystatechange = function(){
  var readyState = xhr.readyState;
...
```

#### <a name="apidoc.element.superagent.client.head"></a>[function <span class="apidocSignatureSpan">superagent.client.</span>head (url, data, fn)](#apidoc.element.superagent.client.head)
- description and source-code
```javascript
head = function (url, data, fn){
  var req = request('HEAD', url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  if (fn) req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.client.options"></a>[function <span class="apidocSignatureSpan">superagent.client.</span>options (url, data, fn)](#apidoc.element.superagent.client.options)
- description and source-code
```javascript
options = function (url, data, fn){
  var req = request('OPTIONS', url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  if (fn) req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.client.parseString"></a>[function <span class="apidocSignatureSpan">superagent.client.</span>parseString (str)](#apidoc.element.superagent.client.parseString)
- description and source-code
```javascript
function parseString(str) {
  var obj = {};
  var pairs = str.split('&');
  var pair;
  var pos;

  for (var i = 0, len = pairs.length; i < len; ++i) {
    pair = pairs[i];
    pos = pair.indexOf('=');
    if (pos == -1) {
      obj[decodeURIComponent(pair)] = '';
    } else {
      obj[decodeURIComponent(pair.slice(0, pos))] =
        decodeURIComponent(pair.slice(pos + 1));
    }
  }

  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.client.patch"></a>[function <span class="apidocSignatureSpan">superagent.client.</span>patch (url, data, fn)](#apidoc.element.superagent.client.patch)
- description and source-code
```javascript
patch = function (url, data, fn){
  var req = request('PATCH', url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  if (fn) req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.client.post"></a>[function <span class="apidocSignatureSpan">superagent.client.</span>post (url, data, fn)](#apidoc.element.superagent.client.post)
- description and source-code
```javascript
post = function (url, data, fn){
  var req = request('POST', url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  if (fn) req.end(fn);
  return req;
}
```
- example usage
```shell
...
$ npm install superagent
'''

Works with [browserify](https://github.com/substack/node-browserify) and should work with [webpack](https://github.com/visionmedia
/superagent/wiki/SuperAgent-for-Webpack)

'''js
request
  .post('/api/pet')
  .send({ name: 'Manny', species: 'cat' })
  .set('X-API-Key', 'foobar')
  .set('Accept', 'application/json')
  .end(function(err, res){
    // Calling the end function will send the request
  });
'''
...
```

#### <a name="apidoc.element.superagent.client.put"></a>[function <span class="apidocSignatureSpan">superagent.client.</span>put (url, data, fn)](#apidoc.element.superagent.client.put)
- description and source-code
```javascript
put = function (url, data, fn){
  var req = request('PUT', url);
  if ('function' == typeof data) fn = data, data = null;
  if (data) req.send(data);
  if (fn) req.end(fn);
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.client.serializeObject"></a>[function <span class="apidocSignatureSpan">superagent.client.</span>serializeObject (obj)](#apidoc.element.superagent.client.serializeObject)
- description and source-code
```javascript
function serialize(obj) {
  if (!isObject(obj)) return obj;
  var pairs = [];
  for (var key in obj) {
    pushEncodedKeyValuePair(pairs, key, obj[key]);
  }
  return pairs.join('&');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.superagent.parse"></a>[module superagent.parse](#apidoc.module.superagent.parse)

#### <a name="apidoc.element.superagent.parse.image"></a>[function <span class="apidocSignatureSpan">superagent.parse.</span>image (res, fn)](#apidoc.element.superagent.parse.image)
- description and source-code
```javascript
image = function (res, fn){
  var data = []; // Binary data needs binary storage

  res.on('data', function(chunk){
      data.push(chunk);
  });
  res.on('end', function () {
      fn(null, Buffer.concat(data));
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.parse.text"></a>[function <span class="apidocSignatureSpan">superagent.parse.</span>text (res, fn)](#apidoc.element.superagent.parse.text)
- description and source-code
```javascript
text = function (res, fn){
  res.text = '';
  res.setEncoding('utf8');
  res.on('data', function(chunk){ res.text += chunk; });
  res.on('end', fn);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.superagent.request_base"></a>[module superagent.request_base](#apidoc.module.superagent.request_base)

#### <a name="apidoc.element.superagent.request_base.request_base"></a>[function <span class="apidocSignatureSpan">superagent.</span>request_base (obj)](#apidoc.element.superagent.request_base.request_base)
- description and source-code
```javascript
function RequestBase(obj) {
  if (obj) return mixin(obj);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.superagent.request_base.prototype"></a>[module superagent.request_base.prototype](#apidoc.module.superagent.request_base.prototype)

#### <a name="apidoc.element.superagent.request_base.prototype._isResponseOK"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>_isResponseOK (res)](#apidoc.element.superagent.request_base.prototype._isResponseOK)
- description and source-code
```javascript
_isResponseOK = function (res) {
  if (!res) {
    return false;
  }

  if (this._okCallback) {
    return this._okCallback(res);
  }

  return res.status >= 200 && res.status < 300;
}
```
- example usage
```shell
...
  return self.callback(err);
}

self.emit('response', res);

var new_err;
try {
  if (!self._isResponseOK(res)) {
    new_err = new Error(res.statusText || 'Unsuccessful HTTP response');
    new_err.original = err;
    new_err.response = res;
    new_err.status = res.status;
  }
} catch(e) {
  new_err = e; // #985 touching res may cause INVALID_STATE_ERR on old Android
...
```

#### <a name="apidoc.element.superagent.request_base.prototype._retry"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>_retry ()](#apidoc.element.superagent.request_base.prototype._retry)
- description and source-code
```javascript
_retry = function () {
  this.clearTimeout();

  // node
  if (this.req) {
    this.req = null;
    this.req = this.request();
  }

  this._aborted = false;
  this.timedout = false;

  return this._end();
}
```
- example usage
```shell
...
 * @param {Response} res
 * @api private
 */

Request.prototype.callback = function(err, res){
// console.log(this._retries, this._maxRetries)
if (this._maxRetries && this._retries++ < this._maxRetries && shouldRetry(err, res)) {
  return this._retry();
}

var fn = this._callback;
this.clearTimeout();

if (err) {
  if (this._maxRetries) err.retries = this._retries - 1;
...
```

#### <a name="apidoc.element.superagent.request_base.prototype._setTimeouts"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>_setTimeouts ()](#apidoc.element.superagent.request_base.prototype._setTimeouts)
- description and source-code
```javascript
_setTimeouts = function () {
  var self = this;

  // deadline
  if (this._timeout && !this._timer) {
    this._timer = setTimeout(function(){
      self._timeoutError('Timeout of ', self._timeout, 'ETIME');
    }, this._timeout);
  }
  // response timeout
  if (this._responseTimeout && !this._responseTimeoutTimer) {
    this._responseTimeoutTimer = setTimeout(function(){
      self._timeoutError('Response timeout of ', self._responseTimeout, 'ETIMEDOUT');
    }, this._responseTimeout);
  }
}
```
- example usage
```shell
...
};

Request.prototype._end = function() {
var self = this;
var xhr = this.xhr = request.getXHR();
var data = this._formData || this._data;

this._setTimeouts();

// state change
xhr.onreadystatechange = function(){
  var readyState = xhr.readyState;
  if (readyState >= 2 && self._responseTimeoutTimer) {
    clearTimeout(self._responseTimeoutTimer);
  }
...
```

#### <a name="apidoc.element.superagent.request_base.prototype._timeoutError"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>_timeoutError (reason, timeout, errno)](#apidoc.element.superagent.request_base.prototype._timeoutError)
- description and source-code
```javascript
_timeoutError = function (reason, timeout, errno){
  if (this._aborted) {
    return;
  }
  var err = new Error(reason + timeout + 'ms exceeded');
  err.timeout = timeout;
  err.code = 'ECONNABORTED';
  err.errno = errno;
  this.timedout = true;
  this.abort();
  this.callback(err);
}
```
- example usage
```shell
...

RequestBase.prototype._setTimeouts = function() {
var self = this;

// deadline
if (this._timeout && !this._timer) {
  this._timer = setTimeout(function(){
    self._timeoutError('Timeout of ', self._timeout, 'ETIME');
  }, this._timeout);
}
// response timeout
if (this._responseTimeout && !this._responseTimeoutTimer) {
  this._responseTimeoutTimer = setTimeout(function(){
    self._timeoutError('Response timeout of ', self._responseTimeout, 'ETIMEDOUT');
  }, this._responseTimeout);
...
```

#### <a name="apidoc.element.superagent.request_base.prototype.abort"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>abort ()](#apidoc.element.superagent.request_base.prototype.abort)
- description and source-code
```javascript
abort = function (){
  if (this._aborted) {
    return this;
  }
  this._aborted = true;
  this.xhr && this.xhr.abort(); // browser
  this.req && this.req.abort(); // node
  this.clearTimeout();
  this.emit('abort');
  return this;
}
```
- example usage
```shell
...
 * @api public
 */
RequestBase.prototype.abort = function(){
  if (this._aborted) {
    return this;
  }
  this._aborted = true;
  this.xhr && this.xhr.abort(); // browser
  this.req && this.req.abort(); // node
  this.clearTimeout();
  this.emit('abort');
  return this;
};

/**
...
```

#### <a name="apidoc.element.superagent.request_base.prototype.catch"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>catch (cb)](#apidoc.element.superagent.request_base.prototype.catch)
- description and source-code
```javascript
catch = function (cb) {
  return this.then(undefined, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.request_base.prototype.clearTimeout"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>clearTimeout ()](#apidoc.element.superagent.request_base.prototype.clearTimeout)
- description and source-code
```javascript
function _clearTimeout(){
  clearTimeout(this._timer);
  clearTimeout(this._responseTimeoutTimer);
  delete this._timer;
  delete this._responseTimeoutTimer;
  return this;
}
```
- example usage
```shell
...
Request.prototype.callback = function(err, res){
// console.log(this._retries, this._maxRetries)
if (this._maxRetries && this._retries++ < this._maxRetries && shouldRetry(err, res)) {
  return this._retry();
}

var fn = this._callback;
this.clearTimeout();

if (err) {
  if (this._maxRetries) err.retries = this._retries - 1;
  this.emit('error', err);
}

fn(err, res);
...
```

#### <a name="apidoc.element.superagent.request_base.prototype.field"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>field (name, val)](#apidoc.element.superagent.request_base.prototype.field)
- description and source-code
```javascript
field = function (name, val) {

  // name should be either a string or an object.
  if (null === name ||  undefined === name) {
    throw new Error('.field(name, val) name can not be empty');
  }

  if (this._data) {
    console.error(".field() can't be used if .send() is used. Please use only .send() or only .field() & .attach()");
  }

  if (isObject(name)) {
    for (var key in name) {
      this.field(key, name[key]);
    }
    return this;
  }

  if (Array.isArray(val)) {
    for (var i in val) {
      this.field(name, val[i]);
    }
    return this;
  }

  // val should be defined now
  if (null === val || undefined === val) {
    throw new Error('.field(name, val) val can not be empty');
  }
  if ('boolean' === typeof val) {
    val = '' + val;
  }
  this._getFormData().append(name, val);
  return this;
}
```
- example usage
```shell
...

Tested browsers:

- Latest Firefox, Chrome, Safari
- Latest Android, iPhone
- IE10 through latest. IE9 with polyfills.

Even though IE9 is supported, a polyfill for 'window.FormData' is required for '.field()'.

Node 4 or later is required.

# Plugins

SuperAgent is easily extended via plugins.
...
```

#### <a name="apidoc.element.superagent.request_base.prototype.get"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>get (field)](#apidoc.element.superagent.request_base.prototype.get)
- description and source-code
```javascript
get = function (field){
  return this._header[field.toLowerCase()];
}
```
- example usage
```shell
...

'''js
var nocache = require('superagent-no-cache');
var request = require('superagent');
var prefix = require('superagent-prefix')('/static');

request
  .get('/some-url')
  .query({ action: 'edit', city: 'London' }) // query string
  .use(prefix) // Prefixes *only* this request
  .use(nocache) // Prevents caching of *only* this request
  .end(function(err, res){
    // Do something
  });
'''
...
```

#### <a name="apidoc.element.superagent.request_base.prototype.getHeader"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>getHeader (field)](#apidoc.element.superagent.request_base.prototype.getHeader)
- description and source-code
```javascript
getHeader = function (field){
  return this._header[field.toLowerCase()];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.request_base.prototype.ok"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>ok (cb)](#apidoc.element.superagent.request_base.prototype.ok)
- description and source-code
```javascript
ok = function (cb) {
  if ('function' !== typeof cb) throw Error("Callback required");
  this._okCallback = cb;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.request_base.prototype.parse"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>parse (fn)](#apidoc.element.superagent.request_base.prototype.parse)
- description and source-code
```javascript
function parse(fn){
  this._parser = fn;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.request_base.prototype.redirects"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>redirects (n)](#apidoc.element.superagent.request_base.prototype.redirects)
- description and source-code
```javascript
redirects = function (n){
  this._maxRedirects = n;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.request_base.prototype.responseType"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>responseType (val)](#apidoc.element.superagent.request_base.prototype.responseType)
- description and source-code
```javascript
responseType = function (val){
  this._responseType = val;
  return this;
}
```
- example usage
```shell
...
* which return Blob and ArrayBuffer, respectively.
*
* In Node all values result in Buffer.
*
* Examples:
*
*      req.get('/')
*        .responseType('blob')
*        .end(callback);
*
* @param {String} val
* @return {Request} for chaining
* @api public
*/
...
```

#### <a name="apidoc.element.superagent.request_base.prototype.retry"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>retry (count)](#apidoc.element.superagent.request_base.prototype.retry)
- description and source-code
```javascript
function retry(count){
  // Default to 1 if no count passed or true
  if (arguments.length === 0 || count === true) count = 1;
  if (count <= 0) count = 0;
  this._maxRetries = count;
  this._retries = 0;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.request_base.prototype.send"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>send (data)](#apidoc.element.superagent.request_base.prototype.send)
- description and source-code
```javascript
send = function (data){
  var isObj = isObject(data);
  var type = this._header['content-type'];

  if (this._formData) {
    console.error(".send() can't be used if .attach() or .field() is used. Please use only .send() or only .field() & .attach()");
  }

  if (isObj && !this._data) {
    if (Array.isArray(data)) {
      this._data = [];
    } else if (!this._isHost(data)) {
      this._data = {};
    }
  } else if (data && this._data && this._isHost(this._data)) {
    throw Error("Can't merge these send calls");
  }

  // merge
  if (isObj && isObject(this._data)) {
    for (var key in data) {
      this._data[key] = data[key];
    }
  } else if ('string' == typeof data) {
    // default to x-www-form-urlencoded
    if (!type) this.type('form');
    type = this._header['content-type'];
    if ('application/x-www-form-urlencoded' == type) {
      this._data = this._data
        ? this._data + '&' + data
        : data;
    } else {
      this._data = (this._data || '') + data;
    }
  } else {
    this._data = data;
  }

  if (!isObj || this._isHost(data)) {
    return this;
  }

  // default to json
  if (!type) this.type('json');
  return this;
}
```
- example usage
```shell
...
'''

Works with [browserify](https://github.com/substack/node-browserify) and should work with [webpack](https://github.com/visionmedia
/superagent/wiki/SuperAgent-for-Webpack)

'''js
request
  .post('/api/pet')
  .send({ name: 'Manny', species: 'cat' })
  .set('X-API-Key', 'foobar')
  .set('Accept', 'application/json')
  .end(function(err, res){
    // Calling the end function will send the request
  });
'''
...
```

#### <a name="apidoc.element.superagent.request_base.prototype.serialize"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>serialize (fn)](#apidoc.element.superagent.request_base.prototype.serialize)
- description and source-code
```javascript
function serialize(fn){
  this._serializer = fn;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.request_base.prototype.set"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>set (field, val)](#apidoc.element.superagent.request_base.prototype.set)
- description and source-code
```javascript
set = function (field, val){
  if (isObject(field)) {
    for (var key in field) {
      this.set(key, field[key]);
    }
    return this;
  }
  this._header[field.toLowerCase()] = val;
  this.header[field] = val;
  return this;
}
```
- example usage
```shell
...

Works with [browserify](https://github.com/substack/node-browserify) and should work with [webpack](https://github.com/visionmedia
/superagent/wiki/SuperAgent-for-Webpack)

'''js
request
  .post('/api/pet')
  .send({ name: 'Manny', species: 'cat' })
  .set('X-API-Key', 'foobar')
  .set('Accept', 'application/json')
  .end(function(err, res){
    // Calling the end function will send the request
  });
'''

## Supported browsers and Node versions
...
```

#### <a name="apidoc.element.superagent.request_base.prototype.sortQuery"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>sortQuery (sort)](#apidoc.element.superagent.request_base.prototype.sortQuery)
- description and source-code
```javascript
sortQuery = function (sort) {
  // _sort default to true but otherwise can be a function or boolean
  this._sort = typeof sort === 'undefined' ? true : sort;
  return this;
}
```
- example usage
```shell
...
*
* Examples:
*
*       // default order
*       request.get('/user')
*         .query('name=Nick')
*         .query('search=Manny')
*         .sortQuery()
*         .end(callback)
*
*       // customized sort function
*       request.get('/user')
*         .query('name=Nick')
*         .query('search=Manny')
*         .sortQuery(function(a, b){
...
```

#### <a name="apidoc.element.superagent.request_base.prototype.then"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>then (resolve, reject)](#apidoc.element.superagent.request_base.prototype.then)
- description and source-code
```javascript
function then(resolve, reject) {
  if (!this._fullfilledPromise) {
    var self = this;
    if (this._endCalled) {
      console.warn("Warning: superagent request was sent twice, because both .end() and .then() were called. Never call .end() if
 you use promises");
    }
    this._fullfilledPromise = new Promise(function(innerResolve, innerReject){
      self.end(function(err, res){
        if (err) innerReject(err); else innerResolve(res);
      });
    });
  }
  return this._fullfilledPromise.then(resolve, reject);
}
```
- example usage
```shell
...
 * @return {Request}
 */

RequestBase.prototype.then = function then(resolve, reject) {
if (!this._fullfilledPromise) {
  var self = this;
  if (this._endCalled) {
    console.warn("Warning: superagent request was sent twice, because both .end() and .then() were called. Never call .end() if
you use promises");
  }
  this._fullfilledPromise = new Promise(function(innerResolve, innerReject){
    self.end(function(err, res){
      if (err) innerReject(err); else innerResolve(res);
    });
  });
}
...
```

#### <a name="apidoc.element.superagent.request_base.prototype.timeout"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>timeout (options)](#apidoc.element.superagent.request_base.prototype.timeout)
- description and source-code
```javascript
function timeout(options){
  if (!options || 'object' !== typeof options) {
    this._timeout = options;
    this._responseTimeout = 0;
    return this;
  }

  for(var option in options) {
    switch(option) {
      case 'deadline':
        this._timeout = options.deadline;
        break;
      case 'response':
        this._responseTimeout = options.response;
        break;
      default:
        console.warn("Unknown timeout option", option);
    }
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.request_base.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>toJSON ()](#apidoc.element.superagent.request_base.prototype.toJSON)
- description and source-code
```javascript
toJSON = function (){
  return {
    method: this.method,
    url: this.url,
    data: this._data,
    headers: this._header
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.request_base.prototype.unset"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>unset (field)](#apidoc.element.superagent.request_base.prototype.unset)
- description and source-code
```javascript
unset = function (field){
  delete this._header[field.toLowerCase()];
  delete this.header[field];
  return this;
}
```
- example usage
```shell
...
/**
 * Remove header 'field'.
 * Case-insensitive.
 *
 * Example:
 *
 *      req.get('/')
 *        .unset('User-Agent')
 *        .end(callback);
 *
 * @param {String} field
 */
RequestBase.prototype.unset = function(field){
delete this._header[field.toLowerCase()];
delete this.header[field];
...
```

#### <a name="apidoc.element.superagent.request_base.prototype.use"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>use (fn)](#apidoc.element.superagent.request_base.prototype.use)
- description and source-code
```javascript
function use(fn) {
  fn(this);
  return this;
}
```
- example usage
```shell
...
var nocache = require('superagent-no-cache');
var request = require('superagent');
var prefix = require('superagent-prefix')('/static');

request
  .get('/some-url')
  .query({ action: 'edit', city: 'London' }) // query string
  .use(prefix) // Prefixes *only* this request
  .use(nocache) // Prevents caching of *only* this request
  .end(function(err, res){
    // Do something
  });
'''

Existing plugins:
...
```

#### <a name="apidoc.element.superagent.request_base.prototype.withCredentials"></a>[function <span class="apidocSignatureSpan">superagent.request_base.prototype.</span>withCredentials (on)](#apidoc.element.superagent.request_base.prototype.withCredentials)
- description and source-code
```javascript
withCredentials = function (on){
  // This is browser-only functionality. Node side is no-op.
  if(on==undefined) on = true;
  this._withCredentials = on;
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.superagent.response_base"></a>[module superagent.response_base](#apidoc.module.superagent.response_base)

#### <a name="apidoc.element.superagent.response_base.response_base"></a>[function <span class="apidocSignatureSpan">superagent.</span>response_base (obj)](#apidoc.element.superagent.response_base.response_base)
- description and source-code
```javascript
function ResponseBase(obj) {
  if (obj) return mixin(obj);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.superagent.response_base.prototype"></a>[module superagent.response_base.prototype](#apidoc.module.superagent.response_base.prototype)

#### <a name="apidoc.element.superagent.response_base.prototype._setHeaderProperties"></a>[function <span class="apidocSignatureSpan">superagent.response_base.prototype.</span>_setHeaderProperties (header)](#apidoc.element.superagent.response_base.prototype._setHeaderProperties)
- description and source-code
```javascript
_setHeaderProperties = function (header){
    // TODO: moar!
    // TODO: make this a util

    // content-type
    var ct = header['content-type'] || '';
    this.type = utils.type(ct);

    // params
    var params = utils.params(ct);
    for (var key in params) this[key] = params[key];

    this.links = {};

    // links
    try {
        if (header.link) {
            this.links = utils.parseLinks(header.link);
        }
    } catch (err) {
        // ignore
    }
}
```
- example usage
```shell
...
}
this._setStatusProperties(status);
this.header = this.headers = parseHeader(this.xhr.getAllResponseHeaders());
// getAllResponseHeaders sometimes falsely returns "" for CORS requests, but
// getResponseHeader still works. so we get content-type even if getting
// other headers fails.
this.header['content-type'] = this.xhr.getResponseHeader('content-type');
this._setHeaderProperties(this.header);

if (null === this.text && req._responseType) {
  this.body = this.xhr.response;
} else {
  this.body = this.req.method != 'HEAD'
    ? this._parseBody(this.text ? this.text : this.xhr.response)
    : null;
...
```

#### <a name="apidoc.element.superagent.response_base.prototype._setStatusProperties"></a>[function <span class="apidocSignatureSpan">superagent.response_base.prototype.</span>_setStatusProperties (status)](#apidoc.element.superagent.response_base.prototype._setStatusProperties)
- description and source-code
```javascript
_setStatusProperties = function (status){
    var type = status / 100 | 0;

    // status / class
    this.status = this.statusCode = status;
    this.statusType = type;

    // basics
    this.info = 1 == type;
    this.ok = 2 == type;
    this.redirect = 3 == type;
    this.clientError = 4 == type;
    this.serverError = 5 == type;
    this.error = (4 == type || 5 == type)
        ? this.toError()
        : false;

    // sugar
    this.accepted = 202 == status;
    this.noContent = 204 == status;
    this.badRequest = 400 == status;
    this.unauthorized = 401 == status;
    this.notAcceptable = 406 == status;
    this.forbidden = 403 == status;
    this.notFound = 404 == status;
}
```
- example usage
```shell
...
   : null;
this.statusText = this.req.xhr.statusText;
var status = this.xhr.status;
// handle IE9 bug: http://stackoverflow.com/questions/10046972/msie-returns-status-code-of-1223-for-ajax-request
if (status === 1223) {
    status = 204;
}
this._setStatusProperties(status);
this.header = this.headers = parseHeader(this.xhr.getAllResponseHeaders());
// getAllResponseHeaders sometimes falsely returns "" for CORS requests, but
// getResponseHeader still works. so we get content-type even if getting
// other headers fails.
this.header['content-type'] = this.xhr.getResponseHeader('content-type');
this._setHeaderProperties(this.header);
...
```

#### <a name="apidoc.element.superagent.response_base.prototype.get"></a>[function <span class="apidocSignatureSpan">superagent.response_base.prototype.</span>get (field)](#apidoc.element.superagent.response_base.prototype.get)
- description and source-code
```javascript
get = function (field){
    return this.header[field.toLowerCase()];
}
```
- example usage
```shell
...

'''js
var nocache = require('superagent-no-cache');
var request = require('superagent');
var prefix = require('superagent-prefix')('/static');

request
  .get('/some-url')
  .query({ action: 'edit', city: 'London' }) // query string
  .use(prefix) // Prefixes *only* this request
  .use(nocache) // Prevents caching of *only* this request
  .end(function(err, res){
    // Do something
  });
'''
...
```



# <a name="apidoc.module.superagent.serialize"></a>[module superagent.serialize](#apidoc.module.superagent.serialize)



# <a name="apidoc.module.superagent.utils"></a>[module superagent.utils](#apidoc.module.superagent.utils)

#### <a name="apidoc.element.superagent.utils.cleanHeader"></a>[function <span class="apidocSignatureSpan">superagent.utils.</span>cleanHeader (header, shouldStripCookie)](#apidoc.element.superagent.utils.cleanHeader)
- description and source-code
```javascript
cleanHeader = function (header, shouldStripCookie){
  delete header['content-type'];
  delete header['content-length'];
  delete header['transfer-encoding'];
  delete header['host'];
  if (shouldStripCookie) {
    delete header['cookie'];
  }
  return header;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superagent.utils.params"></a>[function <span class="apidocSignatureSpan">superagent.utils.</span>params (str)](#apidoc.element.superagent.utils.params)
- description and source-code
```javascript
params = function (str){
  return str.split(/ *; */).reduce(function(obj, str){
    var parts = str.split(/ *= */);
    var key = parts.shift();
    var val = parts.shift();

    if (key && val) obj[key] = val;
    return obj;
  }, {});
}
```
- example usage
```shell
...
// TODO: make this a util

// content-type
var ct = header['content-type'] || '';
this.type = utils.type(ct);

// params
var params = utils.params(ct);
for (var key in params) this[key] = params[key];

this.links = {};

// links
try {
    if (header.link) {
...
```

#### <a name="apidoc.element.superagent.utils.parseLinks"></a>[function <span class="apidocSignatureSpan">superagent.utils.</span>parseLinks (str)](#apidoc.element.superagent.utils.parseLinks)
- description and source-code
```javascript
parseLinks = function (str){
  return str.split(/ *, */).reduce(function(obj, str){
    var parts = str.split(/ *; */);
    var url = parts[0].slice(1, -1);
    var rel = parts[1].split(/ *= */)[1].slice(1, -1);
    obj[rel] = url;
    return obj;
  }, {});
}
```
- example usage
```shell
...
    for (var key in params) this[key] = params[key];

    this.links = {};

    // links
    try {
        if (header.link) {
            this.links = utils.parseLinks(header.link);
        }
    } catch (err) {
        // ignore
    }
};

/**
...
```

#### <a name="apidoc.element.superagent.utils.type"></a>[function <span class="apidocSignatureSpan">superagent.utils.</span>type (str)](#apidoc.element.superagent.utils.type)
- description and source-code
```javascript
type = function (str){
  return str.split(/ *; */).shift();
}
```
- example usage
```shell
...
* Set Content-Type to 'type', mapping values from 'request.types'.
*
* Examples:
*
*      superagent.types.xml = 'application/xml';
*
*      request.post('/')
*        .type('xml')
*        .send(xmlstring)
*        .end(callback);
*
*      request.post('/')
*        .type('application/xml')
*        .send(xmlstring)
*        .end(callback);
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
