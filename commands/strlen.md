---
layout: commands
title: strlen 命令 -- Redis中文资料站
permalink: commands/strlen.html
disqusIdentifier: command_strlen
disqusUrl: http://redis.cn/commands/strlen.html
commandsType: strings
---

Returns the length of the string value stored at `key`.
An error is returned when `key` holds a non-string value.

## ����ֵ

@integer-reply: the length of the string at `key`, or `0` when `key` does not
exist.

##����

```cli
SET mykey "Hello world"
STRLEN mykey
STRLEN nonexisting
```
