p2p的源码又下面几个包

- discover 		包含了[Kademlia协议](../references/Kademlia协议原理简介.pdf)。是基于UDP的p2p节点发现协议。
- discv5		新的节点发现协议。 还是试验属性。本次分析没有涉及。
- nat			网络地址转换的部分代码
- netutil		一些工具
- simulations	p2p网络的模拟。 本次分析没有涉及。

discover部分的源码分析

- [发现的节点的持久化存储 database.go](./database.go源码分析.md)
- [Kademlia协议的核心逻辑 tabel.go](./table.go源码分析.md)
- [UDP协议的处理逻辑udp.go](./udp.go源码分析.md)
- [网络地址转换 nat.go](./nat源码分析.md)

p2p/ 部分源码分析

- [节点之间的加密链路处理协议 rlpx.go](./rlpx节点之间的加密链路.md)
- [挑选节点然后进行连接的处理逻辑 dail.go](./dial.go源码分析.md)
- [节点和节点连接的处理以及协议的处理 peer.go](./peer.go源码分析.md)
- [p2p服务器的逻辑 server.go](./server.go源码分析.md)
