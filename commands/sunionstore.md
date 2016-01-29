---
layout: commands
title: sunionstore 命令 -- Redis中文资料站
permalink: commands/sunionstore.html
disqusIdentifier: command_sunionstore
disqusUrl: http://redis.cn/commands/sunionstore.html
commandsType: sets
---

This command is equal to `SUNION`, but instead of returning the resulting set,
it is stored in `destination`.

If `destination` already exists, it is overwritten.

## ����ֵ

@integer-reply: the number of elements in the resulting set.

##����

```cli
SADD key1 "a"
SADD key1 "b"
SADD key1 "c"
SADD key2 "c"
SADD key2 "d"
SADD key2 "e"
SUNIONSTORE key key1 key2
SMEMBERS key
```
