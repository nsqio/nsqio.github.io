--- 
title: Installing
layout: post
category: deployment
permalink: /deployment/installing.html
---

### <a name="binary">Binary Releases</a>

Pre-built binaries for linux, darwin, freebsd and windows are available for download:

#### Current Stable Release: **`v1.2.0`**

 * [nsq-1.2.0.darwin-amd64.go1.12.9.tar.gz][1.2.0_darwin]
 * [nsq-1.2.0.linux-amd64.go1.12.9.tar.gz][1.2.0_linux]
 * [nsq-1.2.0.freebsd-amd64.go1.12.9.tar.gz][1.2.0_freebsd]
 * [nsq-1.2.0.windows-amd64.go1.12.9.tar.gz][1.2.0_windows]

#### Older Stable Releases

 * [nsq-1.1.0.darwin-amd64.go1.10.3.tar.gz][1.1.0_darwin_go1103]
 * [nsq-1.1.0.linux-amd64.go1.10.3.tar.gz][1.1.0_linux_go1103]
 * [nsq-1.1.0.freebsd-amd64.go1.10.3.tar.gz][1.1.0_freebsd_go1103]
 * [nsq-1.1.0.windows-amd64.go1.10.3.tar.gz][1.1.0_windows_go1103]

### Docker

See [the docs][docker_docs] for deploying NSQ with [Docker][docker].

### OSX

     $ brew install nsq

### Building From Source

#### Pre-requisites

 * **[golang](https://golang.org/doc/install)** (version **`1.9+`** is required)

#### Compiling

NSQ uses go modules to produce reliable builds.

{% highlight bash %}
$ git clone https://github.com/nsqio/nsq
$ cd nsq
$ make
{% endhighlight %}

#### Testing

{% highlight bash %}
$ ./test.sh
{% endhighlight %}

[1.2.0_darwin]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.2.0.darwin-amd64.go1.12.9.tar.gz
[1.2.0_linux]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.2.0.linux-amd64.go1.12.9.tar.gz
[1.2.0_freebsd]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.2.0.freebsd-amd64.go1.12.9.tar.gz
[1.2.0_windows]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.2.0.windows-amd64.go1.12.9.tar.gz

[1.1.0_darwin_go1103]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.1.0.darwin-amd64.go1.10.3.tar.gz
[1.1.0_linux_go1103]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.1.0.linux-amd64.go1.10.3.tar.gz
[1.1.0_freebsd_go1103]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.1.0.freebsd-amd64.go1.10.3.tar.gz
[1.1.0_windows_go1103]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.1.0.windows-amd64.go1.10.3.tar.gz

[docker]: https://docker.io/
[docker_docs]: {{ site.baseurl }}/deployment/docker.html
