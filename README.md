# Test
$ go test

# publish
$ go run stdinpub.go -server tcp://localhost:1883 -topic test  -clientid xxx -username xxx -password xxx -qos 1

# subscribe
$ go run stdoutsub.go -server tcp://localhost:1883 -topic test -clientid xxx -username xxx -password xxx -qos 1




mqtt.go
=======

mqtt library in golang

Eclipse Paho MQTT Go client
===========================


This repository contains the source code for the [Eclipse Paho](http://eclipse.org/paho) MQTT Go client library. 

This code builds a library which enable applications to connect to an [MQTT](http://mqtt.org) broker to publish messages, and to subscribe to topics and receive published messages.

This library supports a fully asynchronous mode of operation.


Installation and Build
----------------------

This client is designed to work with the standard Go tools, so installation is as easy as:

```
go get git.eclipse.org/gitroot/paho/org.eclipse.paho.mqtt.golang.git
```

The client depends on Google's [websockets](http://godoc.org/code.google.com/p/go.net/websocket) package, 
also easily installed with the command:

```
go get code.google.com/p/go.net/websocket
```


Usage and API
-------------

Detailed API documentation is available by using to godoc tool, or can be browsed online
using the [godoc.org](http://godoc.org/git.eclipse.org/gitroot/paho/org.eclipse.paho.mqtt.golang.git) service.

Make use of the library by importing it in your Go client source code. For example,
```
import MQTT "git.eclipse.org/gitroot/paho/org.eclipse.paho.mqtt.golang.git"
```

Samples are available in the `/samples` directory for reference.


Runtime tracing
---------------

Tracing is enabled by using the `SetTraceLevel` option when creating a ClientOptions struct. See the ClientOptions
documentation for more details.


Reporting bugs
--------------

Please report bugs under the "MQTT-Go" Component in [Eclipse Bugzilla](http://bugs.eclipse.org/bugs/) for the Paho Technology project. This is a very new library as of Q1 2014, so there are sure to be bugs.


More information
----------------

Discussion of the Paho clients takes place on the [Eclipse paho-dev mailing list](https://dev.eclipse.org/mailman/listinfo/paho-dev).

General questions about the MQTT protocol are discussed in the [MQTT Google Group](https://groups.google.com/forum/?hl=en-US&fromgroups#!forum/mqtt).

There is much more information available via the [MQTT community site](http://mqtt.org).

