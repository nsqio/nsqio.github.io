--- 
title: Installing
layout: post
category: deployment
permalink: /deployment/installing.html
---

### <a name="binary">Binary Releases</a>

Pre-built binaries for linux, darwin, freebsd and windows are available for download:

#### Current Stable Release: **`v1.1.0`**

 * [nsq-1.1.0.darwin-amd64.go1.10.3.tar.gz][1.1.0_darwin_go1103]
 * [nsq-1.1.0.linux-amd64.go1.10.3.tar.gz][1.1.0_linux_go1103]
 * [nsq-1.1.0.freebsd-amd64.go1.10.3.tar.gz][1.1.0_freebsd_go1103]
 * [nsq-1.1.0.windows-amd64.go1.10.3.tar.gz][1.1.0_windows_go1103]

#### Older Stable Releases

 * [nsq-1.0.0-compat.darwin-amd64.go1.8.tar.gz][1.0.0-compat_darwin_go18]
 * [nsq-1.0.0-compat.linux-amd64.go1.8.tar.gz][1.0.0-compat_linux_go18]
 * [nsq-1.0.0-compat.freebsd-amd64.go1.8.tar.gz][1.0.0-compat_freebsd_go18]
 * [nsq-1.0.0-compat.windows-amd64.go1.8.tar.gz][1.0.0-compat_windows_go18]

### Docker

See [the docs][docker_docs] for deploying NSQ with [Docker][docker].

### OSX

     $ brew install nsq

### Building From Source

#### Pre-requisites

 * **[golang](http://golang.org/doc/install)** (version **`1.7+`** is required)
 * **[dep](https://github.com/golang/dep)** (dependency manager)

#### Compiling

NSQ uses **[dep](https://github.com/golang/dep)** to manage dependencies and produce reliable
builds.  **Using `dep` is the preferred method when compiling from source.**

{% highlight bash %}
$ git clone https://github.com/nsqio/nsq $GOPATH/src/github.com/nsqio/nsq
$ cd $GOPATH/src/github.com/nsqio/nsq
$ dep ensure
{% endhighlight %}

NSQ remains `go get` compatible but it is not recommended as it is not guaranteed to
produce reliable builds (pinned dependencies need to be satisfied manually).

#### Testing

{% highlight bash %}
$ ./test.sh
{% endhighlight %}

[1.1.0_darwin_go1103]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.1.0.darwin-amd64.go1.10.3.tar.gz
[1.1.0_linux_go1103]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.1.0.linux-amd64.go1.10.3.tar.gz
[1.1.0_freebsd_go1103]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.1.0.freebsd-amd64.go1.10.3.tar.gz
[1.1.0_windows_go1103]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.1.0.windows-amd64.go1.10.3.tar.gz

[1.0.0-compat_darwin_go18]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.0.0-compat.darwin-amd64.go1.8.tar.gz
[1.0.0-compat_linux_go18]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.0.0-compat.linux-amd64.go1.8.tar.gz
[1.0.0-compat_freebsd_go18]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.0.0-compat.freebsd-amd64.go1.8.tar.gz
[1.0.0-compat_windows_go18]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.0.0-compat.windows-amd64.go1.8.tar.gz

[docker]: https://docker.io/
[docker_docs]: {{ site.baseurl }}/deployment/docker.html
