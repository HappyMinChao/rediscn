---
layout: commands
title: keys 命令 -- Redis中文资料站
permalink: commands/keys.html
disqusIdentifier: command_keys
disqusUrl: http://redis.cn/commands/keys.html
commandsType: keys
---

Returns all keys matching `pattern`.

While the time complexity for this operation is O(N), the constant times are
fairly low.
For example, Redis running on an entry level laptop can scan a 1 million key
database in 40 milliseconds.

**Warning**: consider `KEYS` as a command that should only be used in production
environments with extreme care.
It may ruin performance when it is executed against large databases.
This command is intended for debugging and special operations, such as changing
your keyspace layout.
Don't use `KEYS` in your regular application code.
If you're looking for a way to find keys in a subset of your keyspace, consider
using `SCAN` or [sets][tdts].

[tdts]: /topics/data-types#sets

Supported glob-style patterns:

* `h?llo` matches `hello`, `hallo` and `hxllo`
* `h*llo` matches `hllo` and `heeeello`
* `h[ae]llo` matches `hello` and `hallo,` but not `hillo`
* `h[^e]llo` matches `hallo`, `hbllo`, ... but not `hello`
* `h[a-b]llo` matches `hallo` and `hbllo`

Use `\` to escape special characters if you want to match them verbatim.

## ����ֵ

@array-reply: list of keys matching `pattern`.

##����

```cli
MSET one 1 two 2 three 3 four 4
KEYS *o*
KEYS t??
KEYS *
```
