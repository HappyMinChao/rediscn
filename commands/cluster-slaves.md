---
layout: commands
title: cluster-slaves 命令
permalink: commands/cluster-slaves.html
disqusIdentifier: command_cluster-slaves
disqusUrl: http://redis.cn/commands/cluster-slaves.html
commandsType: cluster
---

The command provides a list of slave nodes replicating from the specified
master node. The list is provided in the same format used by `CLUSTER NODES` (please refer to its documentation for the specification of the format).

The command will fail if the specified node is not known or if it is not
a master according to the node table of the node receiving the command.

Note that if a slave is added, moved, or removed from a given master node,
and we ask `CLUSTER SLAVES` to a node that has not yet received the
configuration update, it may show stale information. However eventually
(in a matter of seconds if there are no network partitions) all the nodes
will agree about the set of nodes associated with a given master.

@return

The command returns data in the same format as `CLUSTER NODES`.
