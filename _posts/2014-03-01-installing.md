--- 
title: Installing
layout: post
category: deployment
permalink: /deployment/installing.html
---

### <a name="binary">Binary Releases</a>

Pre-built binaries for linux, darwin, freebsd and windows are available for download:

#### Current Stable Release: **`v1.2.1`**

 * [nsq-1.3.0.darwin-amd64.go1.21.5.tar.gz][1.3.0_darwin]
 * [nsq-1.3.0.darwin-arm64.go1.21.5.tar.gz][1.3.0_darwin_arm64]
 * [nsq-1.3.0.linux-amd64.go1.21.5.tar.gz][1.3.0_linux]
 * [nsq-1.3.0.linux-arm64.go1.21.5.tar.gz][1.3.0_linux_arm64]
 * [nsq-1.3.0.freebsd-amd64.go1.21.5.tar.gz][1.3.0_freebsd]
 * [nsq-1.3.0.windows-amd64.go1.21.5.tar.gz][1.3.0_windows]

#### Older Stable Releases

 * [nsq-1.2.1.darwin-amd64.go1.16.6.tar.gz][1.2.1_darwin]
 * [nsq-1.2.1.darwin-arm64.go1.16.6.tar.gz][1.2.1_darwin_arm64]
 * [nsq-1.2.1.linux-amd64.go1.16.6.tar.gz][1.2.1_linux]
 * [nsq-1.2.1.linux-arm64.go1.16.6.tar.gz][1.2.1_linux_arm64]
 * [nsq-1.2.1.freebsd-amd64.go1.16.6.tar.gz][1.2.1_freebsd]
 * [nsq-1.2.1.windows-amd64.go1.16.6.tar.gz][1.2.1_windows]

### Docker

See [the docs][docker_docs] for deploying NSQ with [Docker][docker].

### OSX

     $ brew install nsq

### Building From Source

#### Pre-requisites

 * **[golang](https://golang.org/doc/install)** (version **`1.17+`** is required)

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

[1.3.0_darwin]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.3.0.darwin-amd64.go1.21.5.tar.gz
[1.3.0_darwin_arm64]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.3.0.darwin-arm64.go1.21.5.tar.gz
[1.3.0_linux]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.3.0.linux-amd64.go1.21.5.tar.gz
[1.3.0_linux_arm64]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.3.0.linux-arm64.go1.21.5.tar.gz
[1.3.0_freebsd]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.3.0.freebsd-amd64.go1.21.5.tar.gz
[1.3.0_windows]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.3.0.windows-amd64.go1.21.5.tar.gz

[1.2.1_darwin]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.2.1.darwin-amd64.go1.16.6.tar.gz
[1.2.1_darwin_arm64]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.2.1.darwin-arm64.go1.16.6.tar.gz
[1.2.1_linux]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.2.1.linux-amd64.go1.16.6.tar.gz
[1.2.1_linux_arm64]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.2.1.linux-arm64.go1.16.6.tar.gz
[1.2.1_freebsd]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.2.1.freebsd-amd64.go1.16.6.tar.gz
[1.2.1_windows]: https://s3.amazonaws.com/bitly-downloads/nsq/nsq-1.2.1.windows-amd64.go1.16.6.tar.gz

[docker]: https://docker.io/
[docker_docs]: {{ site.baseurl }}/deployment/docker.html
