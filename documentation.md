---
layout: index
title: Redis文档中心 -- Redis中文资料站
excerpt: redis文档中心，这里介绍了redis基本数据类型、完整的命令、持久化、内存优化等一系列redis基本功能和配置使用的介绍文档。
permalink: documentation.html
disqusIdentifier: documentation
disqusUrl: http://redis.cn/documentation.html
---

Documentation
===

Note: The Redis Documentation is also available in raw (computer friendly) format in the [redis-doc github repository](http://github.com/antirez/redis-doc). The Redis Documentation is released under the [Creative Commons Attribution-ShareAlike 4.0 International license](https://creativecommons.org/licenses/by-sa/4.0/).

Programming with Redis
---

* [The full list of commands](/commands.html) implemented by Redis, along with thorough documentation for each of them.
* [Pipelining](/topics/pipelining.html): Learn how to send multiple commands
at once, saving on round trip time.
* [Redis Pub/Sub](topics/pubsub.html): Redis is a fast and stable Publish/Subscribe messaging system! Check it out.
* [Redis Lua scripting](/commands/eval.html): Redis 2.6 Lua scripting feature documentation.
* [Memory optimization](/topics/memory-optimization.html): Understand how
Redis uses RAM and learn some tricks to use less of it.
* [Expires](/commands/expire.html): Redis allows to set a time to live different for every key so that the key will be automatically removed from the server when it expires.
* [Redis as an LRU cache](/topics/lru-cache.html): How to configure and use Redis as a cache with a fixed amount of memory and auto eviction of keys.
* [Redis transactions](/topics/transactions.html): It is possible to group commands together so that they are executed as a single transaction.
* [Mass insertion of data](/topics/mass-insert.html): How to add a big amount of pre existing or generated data to a Redis instance in a short time.
* [Partitioning](/topics/partitioning.html): How to distribute your data among multiple Redis instances.
* [Distributed locks](/topics/distlock.html): Implementing a distributed lock manager with Redis.
* [Redis keyspace notifications](/topics/notifications.html): Get notifications of keyspace events via Pub/Sub (Redis 2.8 or greater).

Tutorials & FAQ
---

* [Introduction to Redis data types](/topics/data-types-intro.html): This is a good starting point to learn the Redis API and data model.
* [Writing a simple Twitter clone with PHP and Redis](/topics/twitter-clone.html)
* [Auto complete with Redis](http://autocomplete.redis.io)
* [Data types short summary](/topics/data-types.html): A short summary of the different types of values that Redis supports, not as updated and info rich as the first tutorial listed in this section.
* [FAQ](/topics/faq): Some common questions about Redis.

Administration
---
* [Configuration](/topics/config.html): How to configure redis.
* [Replication](/topics/replication.html): What you need to know in order to
set up master-slave replication.
* [Persistence](/topics/persistence.html): Know your options when configuring
Redis' durability.
* [Redis Administration](/topics/admin.html): Selected administration topics.
* [Security](/topics/security.html): An overview of Redis security.
* [Encryption](/topics/encryption.html): How to encrypt Redis client-server communication.
* [Signals Handling](/topics/signals.html): How Redis handles signals.
* [Connections Handling](/topics/clients.html): How Redis handles clients connections.
* [High Availability](/topics/sentinel.html): Redis Sentinel is the official high availability solution for Redis.
* [Latency monitoring](/topics/latency-monitor.html): Redis integrated latency monitoring and reporting capabilities are helpful to tune Redis instances for low latency workloads.
* [Benchmarks](/topics/benchmarks.html): See how fast Redis is in different platforms.
* [Redis Releases](/topics/releases.html): Redis development cycle and version numbering.

Troubleshooting
---

* [Redis problems?](/topics/problems.html): Bugs? High latency? Other issues? Use [our problems troubleshooting page](/topics/problems) as a starting point to find more information.

Redis Cluster
---

* [Redis Cluster tutorial](/topics/cluster-tutorial.html): a gentle introduction and setup guide to Redis Cluster.
* [Redis Cluster specification](/topics/cluster-spec.html): the more formal description of the behavior and algorithms used in Redis Cluster.

Other distributed systems based on Redis
---

* [Roshi](https://github.com/soundcloud/roshi) is a large-scale CRDT set implementation for timestamped events based on Redis and implemented in Go. It was initially developed for [the SoundCloud stream](http://developers.soundcloud.com/blog/roshi-a-crdt-system-for-timestamped-events).

Specifications
---

* [Redis Design Drafts](/topics/rdd.html): Design drafts of new proposals.
* [Redis Protocol specification](/topics/protocol.html): if you're implementing a
client, or out of curiosity, learn how to communicate with Redis at a
low level.
* [Redis RDB format](https://github.com/sripathikrishnan/redis-rdb-tools/wiki/Redis-RDB-Dump-File-Format) specification, and [RDB version history](https://github.com/sripathikrishnan/redis-rdb-tools/blob/master/docs/RDB_Version_History.textile).
* [Internals](/topics/internals.html): Learn details about how Redis is implemented under the hood.

Resources
---

* [Redis Cheat Sheet](http://www.cheatography.com/tasjaevan/cheat-sheets/redis/): Online or printable function reference for Redis.

Use cases
---
* [Who is using Redis](/topics/whos-using-redis.html)

Books
---

The following is a list of books covering Redis that are already published. Books are ordered by release date (newer books first).

* [Redis in Action (Manning, 2013)](http://www.manning.com/carlson/) by [Josiah L. Carlson](http://twitter.com/dr_josiah) (early access edition).
* [Instant Redis Optimization How-to (Packt, 2013)](http://www.packtpub.com/redis-optimization-how-to/book) by [Arun Chinnachamy](http://twitter.com/ArunChinnachamy).
* [Instant Redis Persistence (Packt, 2013)](http://www.packtpub.com/redis-persistence/book) by Matt Palmer.
* [The Little Redis Book (Free Book, 2012)](http://openmymind.net/2012/1/23/The-Little-Redis-Book/) by [Karl Seguin](http://twitter.com/karlseguin) is a great *free* and concise book that will get you started with Redis.
* [Redis Cookbook (O'Reilly Media, 2011)](http://shop.oreilly.com/product/0636920020127.do) by [Tiago Macedo](http://twitter.com/tmacedo) and [Fred Oliveira](http://twitter.com/f).

The following books have Redis related content but are not specifically about Redis:

* [Seven databases in seven weeks (The Pragmatic Bookshelf, 2012)](http://pragprog.com/book/rwdata/seven-databases-in-seven-weeks).
* [Mining the Social Web (O'Reilly Media, 2011)](http://shop.oreilly.com/product/0636920010203.do)
* [Professional NoSQL (Wrox, 2011)](http://www.wrox.com/WileyCDA/WroxTitle/Professional-NoSQL.productCd-047094224X.html)

Credits
---

Redis is maintained and developed by [Salvatore Sanfilippo](http://twitter.com/antirez). In the past [Pieter Noordhuis](http://twitter.com/pnoordhuis) and [Matt Stancliff](https://matt.sh) provided a very significant amount of code and ideas to both the Redis core and client libraries.

The full list of Redis contributors can be found in the [Redis contributors page at Github](https://github.com/antirez/redis/graphs/contributors). However there are other forms of contributions such as ideas, testing, and bug reporting. When possible this contributions are acknowledged in the commit messages. The [mailing list archives](http://groups.google.com/group/redis-db) and the [Github issues page](https://github.com/antirez/redis/issues) are good sources to find people active in the Redis community providing ideas and helping other users.

Sponsors
---

The work [Salvatore Sanfilippo](http://antirez.com) does in order to develop Redis is sponsored by [Redis Labs](http://redislabs.com). Other sponsors and past sponsors of the Redis project are listed in the [Sponsors page](/topics/sponsors).

License, Trademark and Logo
---

* Redis is released under the three clause BSD license. You can find [additional information in our license page](/topics/license.html).
* The Redis trademark and logos are owned by Salvatore Sanfilippo, please read the [Redis trademark guidelines](/topics/trademark.html) for our policy about the use of the Redis trademarks and logo.