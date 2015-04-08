## node 操作 mysql 的原理是什么？ 

node-mysql 是用纯 JS 实现的 MySQL 驱动（也有其他用 C/C++ Addon 实现的），优势是兼容性好，安装时不需要编译，但可能稳定性和性能不如 libmysql 的实现（毕竟是官方的）。
至于实现细节，显然你应该去看 MySQL 的通讯协议标准 https://dev.mysql.com/doc/internals/en/client-server-protocol.html

   
node-mysql 实现了 mysql 的协议，就这么简单

https://github.com/felixge/faster-than-c


## 怎样在Node.js中实现Sleep的功能？

最近在研究用Node.js做网络爬虫，在爬一个网站的时候，通过测试发现它有一个限制，如果持续爬它超过100个网络链接的时候，它就会限制你访问，过一段时间（5分钟左右）才让你访问。我想实现一个功能，如果访问达到90个链接的时候，程序暂停一会（1分钟左右），然后继续访问，就相当于其他语言中的Sleep功能（不要告诉我用循环，这个方法CPU都被它占用了）。在Node.js这种异步环境下，有没有比较好的方法实现Sleep这样的功能？


答曰：setTimeout, 可以考虑结合 async.forever 使用