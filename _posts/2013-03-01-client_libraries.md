---
title: Client Libraries
layout: post
category: Clients
permalink: /clients/client_libraries.html
---

Is the information in this table out-of-date? Are you using one of these client libraries in
production? Tell us about it on the [mailing list][mailing_list] or Twitter [@imsnakes][imsnakes] /
[@jehiah][jehiah].

<table class="table table-bordered client-libraries">
  <tr>
    <th>Name</th>
    <th>Language</th>
    <th>SUB</th>
    <th>PUB</th>
    <th>Discovery</th>
    <th>Backoff</th>
    <th>TLS</th>
    <th>Snappy</th>
    <th>Sampling</th>
    <th>AUTH</th>
    <th>Notes</th>
  </tr>
  <tr class="success">
    <td><a href="{{ site.baseurl }}/components/nsqd.html#post-pub">nsqd</a></td>
    <td>HTTP</td>
    <td></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><strong>built-in</strong></td>
  </tr>
  <tr class="success">
    <td><a href="https://github.com/nsqio/go-nsq">go-nsq</a></td>
    <td>Go</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><strong>official</strong></td>
  </tr>
  <tr class="success">
    <td><a href="https://github.com/nsqio/pynsq">pynsq</a></td>
    <td>Python</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><strong>official</strong></td>
  </tr>
  <tr class="success">
    <td><a href="https://github.com/dudleycarr/nsqjs">nsqjs</a></td>
    <td>JavaScript</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><strong>official</strong></td>
  </tr>
  <tr class="success">
    <td><a href="https://github.com/wistia/elixir_nsq">elixir_nsq</a></td>
    <td>Elixir</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
  </tr>
  <tr class="success">
    <td><a href="https://github.com/project-fifo/ensq">ensq</a></td>
    <td>Erlang</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="success">
    <td><a href="https://github.com/sproutsocial/nsq-j">nsq-j</a></td>
    <td>Java</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
  </tr>
  <tr class="success">
    <td><a href="https://github.com/brainlag/JavaNSQClient">JavaNSQClient</a></td>
    <td>Java</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="success">
    <td><a href="https://github.com/nsqio/TrendrrNSQClient">TrendrrNSQClient</a></td>
    <td>Java</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="success">
    <td><a href="https://github.com/domwong/nsqjava">nsqjava</a></td>
    <td>Java</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="success">
    <td><a href="https://github.com/segmentio/nsq.js">nsq.js</a></td>
    <td>JavaScript</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="success">
    <td><a href="https://github.com/brianc/node-nsqueue">node-nsqueue</a></td>
    <td>JavaScript</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="success">
    <td><a href="https://github.com/abusix/knsq">knsq</a></td>
    <td>Kotlin</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
  </tr>
  <tr class="success">
    <td><a href="https://github.com/judwhite/NsqSharp">NsqSharp</a></td>
    <td>.NET</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
  </tr>
  <tr class="success">
    <td><a href="https://github.com/yunnian/php-nsq">php-nsq</a></td>
    <td>PHP</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="success">
    <td><a href="https://github.com/wk30/phpnsq">phpnsq</a></td>
    <td>PHP</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
  </tr>
  <tr class="success">
      <td><a href="https://github.com/dlecocq/nsq-py">nsq-py</a></td>
      <td>Python</td>
      <td><i class="fa fa-check"></i></td>
      <td><i class="fa fa-check"></i></td>
      <td><i class="fa fa-check"></i></td>
      <td><i class="fa fa-check"></i></td>
      <td><i class="fa fa-check"></i></td>
      <td><i class="fa fa-check"></i></td>
      <td><i class="fa fa-check"></i></td>
      <td><i class="fa fa-check"></i></td>
      <td></td>
  </tr>
  <tr class="success">
      <td><a href="https://github.com/wtolson/gnsq">gnsq</a></td>
      <td>Python</td>
      <td><i class="fa fa-check"></i></td>
      <td><i class="fa fa-check"></i></td>
      <td><i class="fa fa-check"></i></td>
      <td><i class="fa fa-check"></i></td>
      <td><i class="fa fa-check"></i></td>
      <td><i class="fa fa-check"></i></td>
      <td><i class="fa fa-check"></i></td>
      <td><i class="fa fa-check"></i></td>
      <td></td>
  </tr>
  <tr class="success">
    <td><a href="https://github.com/chrisroberts/krakow">krakow</a></td>
    <td>Ruby</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="success">
    <td><a href="https://github.com/DaDDyE/ruby_nsq">ruby_nsq</a></td>
    <td>Ruby</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="success">
    <td><a href="https://github.com/Qihoo360/evpp/tree/master/apps/evnsq">evnsq</a></td>
    <td>C++</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
  </tr>
  <tr class="info">
    <td><a href="https://github.com/nsqio/libnsq">libnsq</a></td>
    <td>C</td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><strong>official</strong></td>
  </tr>
  <tr class="info">
    <td><a href="https://github.com/gamelost/hsnsq">hsnsq</a></td>
    <td>Haskell</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="info">
    <td><a href="https://github.com/nsqio/nsq-java">nsq-java</a></td>
    <td>Java</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="info">
    <td><a href="https://github.com/jmanero/nsq-client">nsq-client</a></td>
    <td>JavaScript</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="info">
    <td><a href="https://github.com/ClothesHorse/NSQnet">NSQnet</a></td>
    <td>.NET</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="info">
    <td><a href="https://github.com/melo/perl-anyevent-nsq">perl-anyevent-nsq</a></td>
    <td>Perl</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="info">
    <td><a href="https://github.com/dsoprea/NsqSpinner">NsqSpinner</a></td>
    <td>Python</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="info">
    <td><a href="https://github.com/wistia/nsq-ruby">nsq-ruby</a></td>
    <td>Ruby</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="info">
    <td><a href="https://github.com/wlgq2/uvnsq">uvnsq</a></td>
    <td>C++11</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="warning">
    <td><a href="https://github.com/thieman/nsq-clojure">nsq-clojure</a></td>
    <td>Clojure</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="warning">
    <td><a href="https://github.com/anvie/nsqie">nsqie</a></td>
    <td>Scala</td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="warning">
    <td><a href="https://github.com/phillro/nodensq">nodensq</a></td>
    <td>JavaScript</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="warning">
    <td><a href="https://github.com/wisespace-io/nsqueue">nsqueue</a></td>
    <td>Rust</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>  
  <tr class="warning">
    <td><a href="https://github.com/aohan237/asyncnsq">asyncnsq</a></td>
    <td>Python</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="warning">
    <td><a href="https://github.com/ryanslade/nsq-ocaml">nsq-ocaml</a></td>
    <td>OCaml</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="warning">
    <td><a href="https://github.com/adamgoose/node-red-contrib-nsq">node-red-contrib-nsq</a></td>
    <td><a href="https://nodered.org">NodeRED</a> Nodes</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="warning">
    <td><a href="https://github.com/aohan237/asyncnsq-rs">asyncnsq</a></td>
    <td>Rust</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr class="warning">
    <td><a href="https://github.com/harporoeder/tokio-nsq">tokio-nsq</a></td>
    <td>Rust</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
  </tr>
  <tr class="warning">
    <td><a href="https://github.com/list-family/ansq">ansq</a></td>
    <td>Python</td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><i class="fa fa-check"></i></td>
    <td><i class="fa fa-check"></i></td>
    <td></td>
  </tr>
</table>

[mailing_list]: https://groups.google.com/forum/#!forum/nsq-users
[imsnakes]: https://twitter.com/imsnakes
[jehiah]: https://twitter.com/jehiah
