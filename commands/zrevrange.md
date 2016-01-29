---
layout: commands
title: zrevrange 命令 -- Redis中文资料站
permalink: commands/zrevrange.html
disqusIdentifier: command_zrevrange
disqusUrl: http://redis.cn/commands/zrevrange.html
commandsType: sortedsets
---

Returns the specified range of elements in the sorted set stored at `key`.
The elements are considered to be ordered from the highest to the lowest score.
Descending lexicographical order is used for elements with equal score.

Apart from the reversed ordering, `ZREVRANGE` is similar to `ZRANGE`.

## ����ֵ

@array-reply: list of elements in the specified range (optionally with
their scores).

##����

```cli
ZADD myzset 1 "one"
ZADD myzset 2 "two"
ZADD myzset 3 "three"
ZREVRANGE myzset 0 -1
ZREVRANGE myzset 2 3
ZREVRANGE myzset -2 -1
```
