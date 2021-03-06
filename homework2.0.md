以下附加作业是针对目前已经符合P6+/P7水平的同学，并且有时间可以挑战一下自己的。能做出来90分以上，直接联系我。

### 1. JVM

从Classloader到模块化，动态加载的插件机制。

1. 10-使用自定义Classloader机制，实现xlass的加载：xlass是作业材料。
2. 20-实现xlass打包的xar（类似class文件打包的jar）的加载：xar里是xlass。
3. 30-基于自定义Classloader实现类的动态加载和卸载：需要设计加载和卸载。
4. 30-基于自定义Classloader实现模块化机制：需要设计模块化机制。
5. 30-使用xar作为模块，实现xar动态加载和卸载：综合应用前面的内容。

### 2. NIO

实现一个http 文件服务器和一个ftp文件服务器。
1. 10-实现文件列表展示：http直接网页展示列表即可。ftp支持cd、ls命令。
2. 20-实现文件上传下载：http上传不需要支持multi-part，直接post文件内容即可。ftp只需要支持主动模式或被动模式的一种。
3. 30-支持断点续传：http下载需要实现range，上传需要自己设计服务器端的分片方式并记录。ftp需要实现retr，stor，rest命令。
4. 30-实现多线程文件上传下载：基于断点续传，需考虑客户端分片方式，多线程调度。
5. 30-实现爬虫爬取前面实现的服务器上所有文件：需要考虑html解析，记录多个文件的传输进度，位置等。

### 3. 并发

#### 3.1-侧重集合：

1. 10-基于基本类型和数组，实现ArrayList/LinkedList，支持自动扩容和迭代器
2. 20-基于基本类型和数组和List，HashMap/LinkedHashMap功能，处理hash冲突和扩容
3. 30-考虑List和Map的并发安全问题，基于读写锁改进安全问题
4. 30-考虑List和Map的并发安全问题，基于AQS改进安全问题
5. 30-编写测试代码比较它们与java-util/JUC集合类的性能和并发安全性

#### 3.2-侧重应用：

1. 10-根据课程提供的场景，实现一个订单处理Service，模拟处理100万订单：后面提供模拟数据。
2. 20-使用多线程方法优化订单处理，对比处理性能
3. 30-使用并发工具和集合类改进订单Service，对比处理性能
4. 30-使用分布式集群+分库分表方式处理拆分订单，对比处理性能：第6模块讲解分库分表。
5. 30-使用读写分离和分布式缓存优化订单的读性能：第6、8模块讲解读写分离和缓存。

### 4. 框架

#### 4.1 Spring AOP

1. 10-讲网关的frontend/backend/filter/router/线程池都改造成Spring配置方式；
2. 20-基于AOP改造Netty网关，filter和router使用AOP方式实现；
3. 30-基于前述改造，将网关请求前后端分离，中级使用JMS传递消息；
4. 30-尝试使用ByteBuddy实现一个简单的基于类的AOP；
5. 30-尝试使用ByteBuddy与Instrument实现一个简单JavaAgent实现无侵入下的AOP；

