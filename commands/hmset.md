---
layout: commands
title: hmset 命令 -- Redis中文资料站
permalink: commands/hmset.html
disqusIdentifier: command_hmset
disqusUrl: http://redis.cn/commands/hmset.html
commandsType: hashes
---

Sets the specified fields to their respective values in the hash stored at
`key`.
This command overwrites any existing fields in the hash.
If `key` does not exist, a new key holding a hash is created.

## ����ֵ

@simple-string-reply

##����

```cli
HMSET myhash field1 "Hello" field2 "World"
HGET myhash field1
HGET myhash field2
```
