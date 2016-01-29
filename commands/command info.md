---
layout: commands
title: command info 命令 -- Redis中文资料站
permalink: commands/command info.html
disqusIdentifier: command_command_info
disqusUrl: http://redis.cn/commands/command info.html
commandsType: server
---

Returns @array-reply of details about multiple Redis commands.

Same result format as `COMMAND` except you can specify which commands
get returned.

If you request details about non-existing commands, their return
position will be nil.


## ����ֵ

@array-reply: nested list of command details.

##����

```cli
COMMAND INFO get set eval
COMMAND INFO foo evalsha config bar
```
