---
layout: commands
title: zremrangebyscore 命令 -- Redis中文资料站
permalink: commands/zremrangebyscore.html
disqusIdentifier: command_zremrangebyscore
disqusUrl: http://redis.cn/commands/zremrangebyscore.html
commandsType: sortedsets
---

Removes all elements in the sorted set stored at `key` with a score between
`min` and `max` (inclusive).

Since version 2.1.6, `min` and `max` can be exclusive, following the syntax of
`ZRANGEBYSCORE`.

## ����ֵ

@integer-reply: the number of elements removed.

##����

```cli
ZADD myzset 1 "one"
ZADD myzset 2 "two"
ZADD myzset 3 "three"
ZREMRANGEBYSCORE myzset -inf (2
ZRANGE myzset 0 -1 WITHSCORES
```
