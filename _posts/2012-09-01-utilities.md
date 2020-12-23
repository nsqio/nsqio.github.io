--- 
title: utilities
layout: post
category: components
permalink: /components/utilities.html
---

These are utilities that facilitate common functionality and introspection into data streams.

 * [nsq_stat](#nsq_stat)
 * [nsq_tail](#nsq_tail)
 * [nsq_to_file](#nsq_to_file)
 * [nsq_to_http](#nsq_to_http)
 * [nsq_to_nsq](#nsq_to_nsq)
 * [to_nsq](#to_nsq)


## nsq_stat

Polls `/stats` for all the producers of the specified topic/channel and displays aggregate stats

    ---------------depth---------------+--------------metadata---------------
      total    mem    disk inflt   def |     req     t-o         msgs clients
      24660  24660       0     0    20 |  102688       0    132492418       1
      25001  25001       0     0    20 |  102688       0    132493086       1
      21132  21132       0     0    21 |  102688       0    132493729       1

#### Command Line Options

    -channel string
        NSQ channel
    -count value
        number of reports
    -http-client-connect-timeout duration
        timeout for HTTP connect (default 2s)
    -http-client-request-timeout duration
        timeout for HTTP request (default 5s)
    -interval duration
        duration of time between polling/printing output (default 2s)
    -lookupd-http-address value
        lookupd HTTP address (may be given multiple times)
    -nsqd-http-address value
        nsqd HTTP address (may be given multiple times)
    -topic string
        NSQ topic
    -version
        print version

-----

## nsq_tail

Consumes the specified topic/channel and writes to stdout (in the spirit of tail(1))

#### Command Line Options

    -channel string
        NSQ channel
    -consumer-opt value
        option to passthrough to nsq.Consumer (may be given multiple times, http://godoc.org/github.com/nsqio/go-nsq#Config)
    -lookupd-http-address value
        lookupd HTTP address (may be given multiple times)
    -max-in-flight int
        max number of messages to allow in flight (default 200)
    -n int
        total messages to show (will wait if starved)
    -nsqd-tcp-address value
        nsqd TCP address (may be given multiple times)
    -print-topic
        print topic name where message was received
    -topic value
        NSQ topic (may be given multiple times)
    -version
        print version string

-----

## nsq\_to_file

Consumes the specified topic/channel and writes out to a newline delimited file, optionally
rolling and/or compressing the file.

#### Command Line Options

    -channel string
        nsq channel (default "nsq_to_file")
    -consumer-opt value
        option to passthrough to nsq.Consumer (may be given multiple times, http://godoc.org/github.com/nsqio/go-nsq#Config)
    -datetime-format string
        strftime compatible format for <DATETIME> in filename format (default "%Y-%m-%d_%H")
    -filename-format string
        output filename format (<TOPIC>, <HOST>, <PID>, <DATETIME>, <REV> are replaced. <REV> is increased when file already exists) (default "<TOPIC>.<HOST><REV>.<DATETIME>.log")
    -gzip
        gzip output files.
    -gzip-level int
        gzip compression level (1-9, 1=BestSpeed, 9=BestCompression) (default 6)
    -host-identifier string
        value to output in log filename in place of hostname. <SHORT_HOST> and <HOSTNAME> are valid replacement tokens
    -http-client-connect-timeout duration
        timeout for HTTP connect (default 2s)
    -http-client-request-timeout duration
        timeout for HTTP request (default 5s)
    -log-level string
        set log verbosity: debug, info, warn, error, or fatal (default "info")
    -log-prefix string
        log message prefix (default "[nsq_to_file] ")
    -lookupd-http-address value
        lookupd HTTP address (may be given multiple times)
    -max-in-flight int
        max number of messages to allow in flight (default 200)
    -nsqd-tcp-address value
        nsqd TCP address (may be given multiple times)
    -output-dir string
        directory to write output files to (default "/tmp")
    -rotate-interval duration
        rotate the file every duration
    -rotate-size rotate-size
        rotate the file when it grows bigger than rotate-size bytes
    -skip-empty-files
        skip writing empty files
    -sync-interval duration
        sync file to disk every duration (default 30s)
    -topic value
        nsq topic (may be given multiple times)
    -topic-pattern string
        only log topics matching the following pattern
    -topic-refresh duration
        how frequently the topic list should be refreshed (default 1m0s)
    -version
        print version string
    -work-dir string
        directory for in-progress files before moving to output-dir

-----

## nsq\_to_http

Consumes the specified topic/channel and performs HTTP requests (GET/POST) to the specified
endpoints.

#### Command Line Options

    -channel string
        nsq channel (default "nsq_to_http")
    -consumer-opt value
        option to passthrough to nsq.Consumer (may be given multiple times, http://godoc.org/github.com/nsqio/go-nsq#Config)
    -content-type string
        the Content-Type used for POST requests (default "application/octet-stream")
    -get value
        HTTP address to make a GET request to. '%s' will be printf replaced with data (may be given multiple times)
    -header value
        Custom header for HTTP requests (may be given multiple times)
    -http-client-connect-timeout duration
        timeout for HTTP connect (default 2s)
    -http-client-request-timeout duration
        timeout for HTTP request (default 20s)
    -lookupd-http-address value
        lookupd HTTP address (may be given multiple times)
    -max-in-flight int
        max number of messages to allow in flight (default 200)
    -mode string
        the upstream request mode options: round-robin, hostpool (default), epsilon-greedy (default "hostpool")
    -n int
        number of concurrent publishers (default 100)
    -nsqd-tcp-address value
        nsqd TCP address (may be given multiple times)
    -post value
        HTTP address to make a POST request to.  data will be in the body (may be given multiple times)
    -sample float
        % of messages to publish (float b/w 0 -> 1) (default 1)
    -status-every int
        the # of requests between logging status (per handler), 0 disables (default 250)
    -topic string
        nsq topic
    -version
        print version string

-----

## nsq\_to_nsq

Consumes the specified topic/channel and re-publishes the messages to destination `nsqd` via TCP.

#### Command Line Options

    -channel string
        nsq channel (default "nsq_to_nsq")
    -consumer-opt value
        option to passthrough to nsq.Consumer (may be given multiple times, see http://godoc.org/github.com/nsqio/go-nsq#Config)
    -destination-nsqd-tcp-address value
        destination nsqd TCP address (may be given multiple times)
    -destination-topic string
        use this destination topic for all consumed topics (default is consumed topic name)
    -lookupd-http-address value
        lookupd HTTP address (may be given multiple times)
    -max-in-flight int
        max number of messages to allow in flight (default 200)
    -mode string
        the upstream request mode options: round-robin, hostpool (default), epsilon-greedy (default "hostpool")
    -nsqd-tcp-address value
        nsqd TCP address (may be given multiple times)
    -producer-opt value
        option to passthrough to nsq.Producer (may be given multiple times, see http://godoc.org/github.com/nsqio/go-nsq#Config)
    -require-json-field string
        for JSON messages: only pass messages that contain this field
    -require-json-value string
        for JSON messages: only pass messages in which the required field has this value
    -status-every int
        the # of requests between logging status (per destination), 0 disables (default 250)
    -topic value
        nsq topic (may be given multiple times)
    -version
        print version string
    -whitelist-json-field value
        for JSON messages: pass this field (may be given multiple times)

-----

## to_nsq

Takes a stdin stream and splits on newlines (default) for re-publishing to destination `nsqd` via
TCP.

#### Command Line Options

    -delimiter string
        character to split input from stdin (default "\n")
    -nsqd-tcp-address value
        destination nsqd TCP address (may be given multiple times)
    -producer-opt value
        option to passthrough to nsq.Producer (may be given multiple times, http://godoc.org/github.com/nsqio/go-nsq#Config)
    -rate int
        Throttle messages to n/second. 0 to disable
    -topic string
        NSQ topic to publish to
