--- 
title: Installing
layout: post
category: deployment
permalink: /deployment/installing.html
---

### <a name="binary">Binary Releases</a>

Pre-built binaries for linux, darwin, freebsd and windows are available for download:

#### Current Stable Release: **`v1.0.0-compat`**

 * [nsq-1.0.0-compat.darwin-amd64.go1.8.tar.gz][1.0.0-compat_darwin_go18]
 * [nsq-1.0.0-compat.linux-amd64.go1.8.tar.gz][1.0.0-compat_linux_go18]
 * [nsq-1.0.0-compat.freebsd-amd64.go1.8.tar.gz][1.0.0-compat_freebsd_go18]
 * [nsq-1.0.0-compat.windows-amd64.go1.8.tar.gz][1.0.0-compat_windows_go18]

#### Older Stable Releases

 * [nsq-0.3.8.darwin-amd64.go1.6.2.tar.gz][0.3.8_darwin_go162]
 * [nsq-0.3.8.linux-amd64.go1.6.2.tar.gz][0.3.8_linux_go162]
 * [nsq-0.3.8.freebsd-amd64.go1.6.2.tar.gz][0.3.8_freebsd_go162]
 * [nsq-0.3.8.windows-amd64.go1.6.2.tar.gz][0.3.8_windows_go162]
 * [nsq-0.3.7.darwin-amd64.go1.6.tar.gz][0.3.7_darwin_go16]
 * [nsq-0.3.7.linux-amd64.go1.6.tar.gz][0.3.7_linux_go16]
 * [nsq-0.3.7.freebsd-amd64.go1.6.tar.gz][0.3.7_freebsd_go16]
 * [nsq-0.3.7.windows-amd64.go1.6.tar.gz][0.3.7_windows_go16]

### Docker

See [the docs][docker_docs] for deploying NSQ with [Docker][docker].

### OSX

     $ brew install nsq

### Building From Source

#### Pre-requisites

 * **[golang](http://golang.org/doc/install)** (version **`1.7+`** is required)
 * **[gpm](https://github.com/pote/gpm)** (dependency manager)

#### Compiling

NSQ uses **[gpm](https://github.com/pote/gpm)** to manage dependencies and produce reliable
builds.  **Using `gpm` is the preferred method when compiling from source.**

{% highlight bash %}
$ gpm install
$ go get github.com/nsqio/nsq/...
{% endhighlight %}

NSQ remains `go get` compatible but it is not recommended as it is not guaranteed to
produce reliable builds (pinned dependencies need to be satisfied manually).

#### Testing

{% highlight bash %}
$ ./test.sh
{% endhighlight %}

[1.0.0-compat_darwin_go18]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.0.0-compat.darwin-amd64.go1.8.tar.gz
[1.0.0-compat_linux_go18]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.0.0-compat.linux-amd64.go1.8.tar.gz
[1.0.0-compat_freebsd_go18]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.0.0-compat.freebsd-amd64.go1.8.tar.gz
[1.0.0-compat_windows_go18]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.0.0-compat.windows-amd64.go1.8.tar.gz

[0.3.8_darwin_go162]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-0.3.8.darwin-amd64.go1.6.2.tar.gz
[0.3.8_linux_go162]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-0.3.8.linux-amd64.go1.6.2.tar.gz
[0.3.8_freebsd_go162]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-0.3.8.freebsd-amd64.go1.6.2.tar.gz
[0.3.8_windows_go162]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-0.3.8.windows-amd64.go1.6.2.tar.gz

[0.3.7_darwin_go16]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-0.3.7.darwin-amd64.go1.6.tar.gz
[0.3.7_linux_go16]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-0.3.7.linux-amd64.go1.6.tar.gz
[0.3.7_freebsd_go16]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-0.3.7.freebsd-amd64.go1.6.tar.gz
[0.3.7_windows_go16]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-0.3.7.windows-amd64.go1.6.tar.gz

[docker]: https://docker.io/
[docker_docs]: {{ site.baseurl }}/deployment/docker.html
