# Responder: a Familiar Web Service Framework

Speaker: Kenneth Reitz

Link: https://www.pytennessee.org/talks/responder-a-familiar-web-service-framework
Presentation: https://github.com/kennethreitz/talks/tree/master/archive/responder

## Python web history

* Before Django
* 2005 Django
* 2006 PyLons
* 2007 Webob
* 2010 Flask - originally a joke, but they grew in popularity

Current choice - Django or Flask

## Web sockets

RE: Web socket connections - some people run a node.js or go service. You don't
get first cls

Look at Sever-Sent Events (SSE). Allows you to push down to the client, which
is what you want for web socket connections. There is no first class support.
You need a async server to do this properly.

### Newer options

* Falcon
* Django channels - allows you to do advance concurrency stuff.
* Hug

## Responder

A web framework that Reitz created

* Include Requests as a standard HTTP client
* Base the Request/Response obj very similr to Requests' own objects
* Make "the world's best web framework"

https://github.com/kennethreitz/responder

The appeal of responder is the async component.

This group of tools are asgi, not wsqi

