# Summary

* [前言](README.md)
* [Java基础](base/README.md)
    * Java基础
        * [Java基础](base/object/Java基础.md)
        * [ final,static,this,super 关键字总结](base/object/关键字总结.md)
        * [Java异常处理](base/error/Java异常处理.md)
        * [Java反射](base/error/Java反射.md)
        * [Java注解](base/annotation/Java反射.md)
        * [Java基础面试提问](base/interview/Java基础面试提问.md)
    * 容器
        * [Java容器基础](base/collection/Java容器基础.md)
        * [HashMap相关问题](base/collection/HashMap相关问题.md)
        * [ArrayList 的扩容机制](base/collection/ArrayList 的扩容机制.md)
        * [Comparable和Comparator](base/collection/Comparable和Comparator.md)
    * 多线程
        * [多线程](base/thread/README.md)
        * [线程生命周期](base/thread/线程生命周期.md)
        * [线程通信(等待通知wait/notify机制)](base/thread/线程通信.md)
        * 死锁
            * [死锁](base/thread/死锁.md)
            * [如何发现、预防、解决死锁](base/thread/如何发现、预防、解决死锁.md)
    * 并发
        * [synchronized关键字](base/concurrent/synchronized关键字.md)
        * [ReentrantLock(补充)](base/concurrent/ReentrantLock.md)
        * [volatile关键字](base/concurrent/volatile关键字.md)
        * 线程池
            * [线程池](base/concurrent/线程池.md)
            * [ThreadPoolExecutor类](base/concurrent/ThreadPoolExecutor类.md)
            * [线程池的具体实现原理](base/concurrent/线程池的具体实现原理.md)
            * [线程池的处理流程](base/concurrent/线程池的处理流程.md)
            * [线程池使用示例](base/concurrent/线程池使用示例.md)
            * [Executors创建线程池](base/concurrent/Executors创建线程池.md)
            * [如何合理配置线程池的大小](base/concurrent/如何合理配置线程池的大小.md)
        * ThreadLocal
            * [ThreadLocal](base/concurrent/ThreadLocal.md)
            * [ThreadLocal使用不当导致内存泄漏](base/concurrent/ThreadLocal/ThreadLocal使用不当导致内存泄漏.md)
        * java锁
            * [乐观锁和悲观锁](base/concurrent/乐观锁和悲观锁.md)
            * [java锁分类](https://tech.meituan.com/2018/11/15/java-lock.html)
        * [Callable和Future](base/concurrent/Callable和Future.md)
        * [Atomic原子类](base/concurrent/Atomic原子类.md)
        * [CAS（比较并替换）](base/concurrent/cas.md)
        * [AQS构建锁和同步器](base/concurrent/AQS构建锁和同步器.md)
    * IO
        * [IO总结](base/io/IO总结.md)
        * [100个http连接，BIO和NIO所需线程问题](base/io/question/100个http连接BIO和NIO所需线程问题.md)
        * IO流入门
            * [IO流入门](./base/io/README.md)
            * [File类](./base/io/File类.md)
            * 文件流
                * [FileInputStream](./base/io/file/FileInputStream.md)
                * [FileOutputStream](./base/io/file/FileOutputStream.md)
                * [FileReader](./base/io/file/FileReader.md)
                * [FileWriter](./base/io/file/FileWriter.md)
            * [缓冲流](./base/io/buffered/README.md)
            * [IO转换流](./base/io/IO转换流/README.md)
            * [对象流](./base/io/对象流/README.md)
    * Jvm
        * Java内存区域
            * [Java内存区域](base/jvm/Java内存区域.md)
            * [HotSpot 虚拟机对象创建](base/jvm/HotSpot虚拟机对象创建.md)
        * JVM垃圾回收
            * [JVM垃圾回收](base/jvm/JVM垃圾回收.md)
            * [ JVM 内存分配与回收](base/jvm/JVM内存分配与回收.md)
            * [对象已经死亡？](base/jvm/对象已经死亡.md)
            * [垃圾收集算法](base/jvm/垃圾收集算法.md)
            * [垃圾收集器](base/jvm/垃圾收集器.md)
            * [GC中对象自救](base/jvm/GC中对象自救.md)
        * JVM性能调优
            * [如何合理的规划 JVM 性能调优](base/jvm/如何合理的规划 JVM 性能调优.md)
            * [常见的JVM设置](base/jvm/常见的JVM设置.md)
            * [内存溢出时打印内存信息](base/jvm/内存溢出时打印内存信息.md)
            * [线上如何排查FullGC(系统 CPU 突然飙升且 GC 频繁，你该如何排查)](base/jvm/线上如何排查FullGC.md)
            * [jstack等命令的实现原理](base/jvm/jstack等命令的实现原理.md)
        * 类加载过程
            * [类加载过程](base/jvm/类加载过程.md)
            * [类加载过程(精简版)](base/jvm/类加载过程精简版.md)
        * 类加载器
            * [类加载器](base/jvm/类加载器.md)
            * [类加载器（常见面试）](base/jvm/类加载器常见面试.md)
            * [tomcat类加载器](base/jvm/tomcat类加载器.md)
        * JDK问题排查
            * [JDK监控和故障处理工具汇总](base/jvm/JDK监控和故障处理工具汇总.md)
            * MAT
                * [MAT安装](base/jvm/mat安装.md)
                * [MAT使用](base/jvm/mat使用.md)
                * [Shallow heap和Retained heap](base/jvm/mat/Shallow和Retained.md)
                * [记一次MAT分析线上项目过程](base/jvm/mat/记一次MAT分析线上项目过程.md)
        * [JVM面试提问](base/jvm/JVM面试提问.md)
* [J2EE](J2EE/README.md)
    * [Servlet](J2EE/Servlet/README.md)
    * [转发和重定向](J2EE/转发和重定向.md)
    * 会话跟踪
        * [会话跟踪](J2EE/会话/README.md)
        * [会话机制](J2EE/会话/会话机制.md)
        * [Cookie](J2EE/会话/Cookie.md)
        * [Session](J2EE/会话/Session.md)
        * [Cookie和Session总结](J2EE/会话/Cookie和Session总结.md)
        * [黏性session和非黏性session](J2EE/会话/黏性session和非黏性session.md)
    * Tomcat
        * [Tomcat系统架构](J2EE/tomcat/Tomcat系统架构.md)
* [Spring](./spring/README.md)
    * [Spring常见知识点](spring/interview/README.md)
    * [Spring整体架构](spring/Framework/Spring整体架构.md)
    * Spring IoC
        * [Spring IoC常见问题](spring/ioc/SpringIoC常见问题.md)
        * [Spring Bean常见问题](spring/ioc/SpringBean常见问题.md)
        * [Spring 装配Bean的3种方式](spring/ioc/Spring 装配Bean的3种方式.md)
        * [循环依赖问题](spring/ioc/循环依赖问题.md)
    * SpringAOP
        * [SpringAOP概述](spring/aop/README.md)
        * [Spring AOP实现原理](spring/aop/SpringAOP实现原理.md)
        * AOP实战
            * [AOP实现打印日志](spring/aop/AOP打印日志.md)
            * [AOP实现Limit限流](spring/aop/Limit限流.md)
    * Spring事务
        * [Spring事务](spring/transaction/README.md)
    * Spring MVC
        * [SpringMVC常见知识点](spring/springmvc/SpringMVC常见知识点.md)
        * [SpringMVC拦截器](spring/springmvc/SpringMVC拦截器.md)
        * [RESTful](spring/springmvc/RESTful.md)
    * Spring Boot
        * [Spring Boot常见知识点](spring/SpringBoot/README.md)
        * [Spring Boot 自动配置之@Enable*与@Import注解](spring/SpringBoot/SpringBoot自动配置之@Enable*与@Import注解.md)
        * [自定义SpringBoot Starter实现自动化配置](spring/SpringBoot/自定义SpringBootStarter实现自动化配置.md)
        * [SpringBoot启动过程](spring/SpringBoot/SpringBoot启动过程.md)
    * [Spring发展提升](spring/development/Spring发展提升.md)
    * 《Spring实战(第四版)》读书笔记
        * [Spring概述](./spring/spring-in-action/Spring概述.md)
            * [面向切面](./spring/spring-in-action/面向切面.md)
            * [Spring容器](./spring/spring-in-action/summary/Spring容器.md)
            * [bean的生命周期](./spring/spring-in-action/summary/bean的生命周期.md)
                * [bean的生命周期实例](./spring/spring-in-action/summary/bean的生命周期实例.md)
        * [依赖注入](./spring/spring-in-action/DI/README.md)
            * [装配Bean](./spring/spring-in-action/DI/装配Bean.md)
            * [高级装配](./spring/spring-in-action/DI/高级装配.md)
                * [环境与profile](./spring/spring-in-action/DI/高级装配/环境与profile.md)
                * [条件化的bean](./spring/spring-in-action/DI/高级装配/条件化的bean.md)
                * [处理自动装配的歧义性](./spring/spring-in-action/DI/高级装配/处理自动装配的歧义性.md)
                * [bean的作用域](./spring/spring-in-action/DI/高级装配/bean的作用域.md)
                * [运行时值的注入](./spring/spring-in-action/DI/高级装配/运行时值的注入.md)
        * [Spring MVC](./spring/spring-in-action/SpringMVC/README.md)
            * [SpringMVC请求流程](./spring/spring-in-action/SpringMVC/SpringMVC请求流程.md)
            * [RequestMapping处理请求](./spring/spring-in-action/SpringMVC/RequestMapping处理请求.md)
            * [接收请求参数](./spring/spring-in-action/SpringMVC/接收请求参数.md)
            * [校验数据](./spring/spring-in-action/SpringMVC/校验数据.md)
            * [重定向与转发](./spring/spring-in-action/SpringMVC/重定向与转发.md)
            * [测试控制器](./spring/spring-in-action/SpringMVC/测试控制器.md)
        * [渲染Web视图](./spring/spring-in-action/viewResolver/README.md)
        * [REST API](./spring/spring-in-action/RESTAPI/README.md)
            * [表达性](./spring/spring-in-action/RESTAPI/表达性.md)
            * [异常处理并更改状态码](./spring/spring-in-action/RESTAPI/异常处理并更改状态码.md)
            * [在响应中设置头部信息](./spring/spring-in-action/RESTAPI/在响应中设置头部信息.md)
        * [NoSql](./spring/spring-in-action/NoSql/README.md)
            * [redis](./spring/spring-in-action/NoSql/redis/README.md)
    * [Spring面试提问](spring/interview/Spring面试提问.md)
* [MyBatis](./Mybatis/README.md)
    * [Mybatis常见面试题](Mybatis/interview/Mybatis常见面试题.md)
    * 《MyBatis入门到精通》读书笔记
        * [MyBatis简介](./Mybatis/book/README.md)
        * [集成与使用](./Mybatis/集成与使用.md)
        * [XML方式基本用法](./Mybatis/xml/README.md)
            * [select用法](./Mybatis/xml/select.md)
        * [Mapper接口动态代理实现原理](./Mybatis/Mapper接口动态代理实现原理.md)
        * [动态sql](./Mybatis/dynamicsql/README.md)
            * [if用法](./Mybatis/dynamicsql/if.md)
* [Redis](redis/README.md)
    * [redis面试考点](./redis/interview/README.md)
    * [redis事务](./redis/interview/redis事务.md)
    * redis使用场景
        * [Redis缓存场景](redis/scene/redis使用场景.md)
        * hash场景
            * [Redis修改局部信息场景，如用户信息（hash,）](redis/scene/Redis修改局部信息场景.md)
        * list场景
            * [Redis用作消息队列(list)](redis/scene/Redis用作消息队列.md)
            * [Redis最新内容 （list）](redis/scene/Redis最新内容.md)
        * set场景
            * [共同好友列表 (set)](redis/scene/共同好友列表.md)
        * zset场景
            * [Redis排行榜场景（zset）](redis/scene/Redis排行榜场景.md)
            * [Redis热门服务场景(zset)](redis/scene/Redis热门服务场景.md)
            * [Redis在线人数场景（zset）](redis/scene/Redis在线人数场景.md)
    * Redis可能出现的问题
        * [Redis缓存雪崩](redis/question/Redis缓存雪崩.md)
        * [Redis缓存穿透](redis/question/Redis缓存穿透.md)
        * [如何解决 Redis 的并发竞争 Key 问题](redis/question/如何解决 Redis 的并发竞争 Key 问题.md)
        * [Redis缓存预热](redis/question/Redis缓存预热.md)
        * [Redis保证缓存与数据库双写时的数据一致性](redis/question/Redis保证缓存与数据库双写时的数据一致性.md)
    * [redis分布式锁](redis/lock/README.md)
        * [一步步实现单机redis的分布式锁（setnx）](redis/lock/一步步实现单机redis的分布式锁.md)
        * [Redlock分布式锁](redis/lock/Redlock分布式锁.md)
    * [redis面试问题](redis/interview/redis面试问题.md)
    * [Redist禁用危险命令](redis/interview/Redist禁用危险命令.md)
    * 读书笔记
        * [Redis简介](./redis/book/README.md)
        * [5种数据结构](./redis/5种数据结构.md)
            * [String字符串](./redis/string/README.md)
            * [List列表](./redis/list/README.md)
            * [Set集合](./redis/set/README.md)
            * [Hash散列](./redis/hash/README.md)
            * [Zset有序集合](./redis/zset/README.md)
        * [发布与订阅(pub/sub)](./redis/发布与订阅.md)
        * [排序SORT](./redis/排序.md)
        * [事务](./redis/事务.md)
        * [键的过期时间](./redis/键的过期时间.md)
        * [持久化](./redis/persistence/README.md)
            * [快照(snapshotting)](./redis/persistence/快照.md)
            * [只追加文件(append-only file,AOF)](./redis/persistence/只追加文件.md)
    * 安装
        * [Redis安装](./redis/install/README.md)
        * [开启远程访问](./redis/install/开启远程访问.md)
    * Redis使用
        * [Spring Boot集成redis使用](./redis/use/SpringBoot集成redis使用.md)
        * [redis连接客户端选择：Jedis,Redisson,Lettuce](redis/use/redis连接客户端选择.md)
        * [JedisPool资源池优化](redis/use/JedisPool资源池优化.md)
        * [RedisUtil工具类的使用(仅供参考)](redis/use/RedisUtil工具类的使用.md)
* [数据库](./db/README.md)
    * [MySql](./db/mysql/README.md)
        * [CentosMySQL安装](db/mysql/CentosMySQL安装.md)
        * [存储引擎](./db/mysql/存储引擎.md)
        * [字符集与排序规则](db/mysql/字符集与排序规则.md)
        * [索引](db/mysql/index/README.md)
            * [索引常见的数据结构](db/mysql/index/索引常见的数据结构.md)
            * [B+TREE索引的优势](db/mysql/index/B+TREE索引的优势.md)
            * [索引实现](db/mysql/index/索引实现.md)
            * [联合索引](db/mysql/index/联合索引.md)
        * [事务](db/mysql/transaction/README.md)
        * 锁
            * [锁](db/mysql/lock/README.md)
            * [锁机制](db/mysql/lock/锁机制.md)
        * [常用操作](./db/mysql/常用操作.md)
            * [MySQL配置文件](./db/mysql/MySQL配置文件.md)
            * [MySql分页查询](./db/mysql/operation/MySql分页查询.md)
        * 性能优化
            * [大表优化](db/mysql/bigtable/README.md)
            * [大表优化过程](db/mysql/optimize/大表优化过程.md)
            * [like模糊查询优化](db/mysql/optimize/like模糊查询优化.md)
            * [Explain使用分析](db/mysql/optimize/Explain使用分析.md)
            * [一条SQL语句在MySQL中如何执行的](db/mysql/optimize/一条SQL语句在MySQL中如何执行的.md)
        * 备份
            * [热备份和冷备份概念](db/mysql/backup/热备份和冷备份概念.md)
        * 问题集锦
            * [无法连接远端Mysql](db/mysql/problem/无法连接远端Mysql.md)
        * [MySql面试提问](db/mysql/interview/MySql面试提问.md)
    * [Oracle](./db/Oracle/README.md)
        * [序列](db/Oracle/序列.md)
* [SQL](./sql/README.md)
    * SELECT
        * [SELECT检索数据](./sql/SELECT.md)
        * [ORDER BY排序检索数据](./sql/orderby.md)
        * [WHERE过滤数据](./sql/WHERE.md)
        * [LIKE等通配符过滤](./sql/LIKE等通配符过滤.md)
        * [创建计算字段](./sql/创建计算字段.md)
        * [使用函数处理数据](sql/使用函数处理数据.md)
        * [汇总数据（聚集函数）](sql/汇总数据.md)
        * [GROUP BY/HAVING分组数据](sql/分组数据.md)
        * [子查询](sql/子查询.md)
        * [JOIN联结表](sql/联结表.md)
        * [UNION组合查询](sql/UNION组合查询.md)
    * INSERT
        * [INSERT插入数据](sql/insert/INSERT插入数据.md)
    * UPDATE
        * [UPDATE更新数据](sql/insert/UPDATE更新数据.md)
    * DELETE
        * [DELETE删除数据](sql/insert/DELETE删除数据.md)
    * 创建和操纵表
        * [CREATE TABLE 创建表](sql/table/创建表.md)
        * [ALTER TABLE更新表](sql/table/更新表.md)
        * [DROP TABLE 删除表](sql/table/删除表.md)
        * [RENAME TABLE 重命名表](sql/table/重命名表.md)
    * [VIEW视图](sql/view/README.md)
    * [存储过程](sql/存储过程/README.md)
    * [事务](sql/transaction/README.md)
    * [索引](sql/索引.md)
* 消息中间件
    * RabbitMQ
        * [RabbitMQ基础](mq/RabbitMQ/RabbitMQ基础.md)
        * 实战
            * [RabbitMQ安装](mq/RabbitMQ/action/RabbitMQ安装.md)
            * [SpringBoot整合RabbitMQ](mq/RabbitMQ/action/SpringBoot整合RabbitMQ.md)
* 微服务
    * 服务发现(注册中心）
        * Eureka
            * [Eureka基础](microservice/ServiceDiscovery/eureka/eureka基础.md)
            * [SpringBoot整合Eureka](microservice/ServiceDiscovery/eureka/SpringBoot整合Eureka.md)
        * nacos
            * [nacos基础](microservice/ServiceDiscovery/nacos/nacos概念.md)
            * [nacos安装与使用](microservice/ServiceDiscovery/nacos/nacos安装与使用.md)
    * 网关
        * [为什么微服务需要API网关？](microservice/gateway/为什么微服务需要API网关.md)
        * zuul
            * [zuul基础](microservice/gateway/zuul/zuul基础.md)
            * [zuul实战](microservice/gateway/zuul/zuul实战.md)
            * [微服务保护](microservice/gateway/zuul/微服务保护.md)
        * Spring Cloud GateWay
            * [服务网关Spring Cloud GateWay基础](microservice/gateway/SpringCloudGateWay/服务网关SpringCloudGateWay基础.md)
            * [Spring Cloud GateWay网关功能](microservice/gateway/SpringCloudGateWay/SpringCloudGateWay网关功能.md)
            * [Spring Cloud GateWay实战](microservice/gateway/SpringCloudGateWay/SpringCloudGateWay实战.md)
            * [Spring Cloud GateWay之Filter](microservice/gateway/SpringCloudGateWay/SpringCloudGateWay之Filter.md)
            * [Spring Cloud GateWay负载均衡](microservice/gateway/SpringCloudGateWay/SpringCloudGateWay负载均衡.md)
            * [Spring Cloud GateWay之Hystrix断路器](microservice/gateway/SpringCloudGateWay/SpringCloudGateWay之Hystrix断路器.md)
            * [Spring Cloud GateWay跨域设置](microservice/gateway/SpringCloudGateWay/SpringCloudGateWay跨域设置.md)
        * 网关功能
            * [限流的算法](microservice/gateway/function/限流的算法.md)
    * 授权认证
        * spring-cloud-starter-oauth2
            * [使用spring-cloud-starter-oauth2搭建授权服务](microservice/auth/spring-cloud-starter-oauth2/使用spring-cloud-starter-oauth2搭建授权服务.md)
            * [Spring security OAuth2 深入解析](microservice/auth/spring-cloud-starter-oauth2/SpringsecurityOAuth2深入解析.md)
            * [Spring security OAuth2  端点（endpoints）授权url](microservice/auth/spring-cloud-starter-oauth2/SpringsecurityOAuth2授权url].md)
    * 分布式跟踪系统
        * zipkin
            * [ZinKin基础](microservice/track/zipkin/ZinKin基础.md)
            * [Sleuth Zipkin链路追踪](microservice/track/zipkin/Sleuth Zipkin链路追踪.md)
            * [Zipkin下载](microservice/track/zipkin/Zipkin下载.md)
            * [SpringBoot整合Zipkin](microservice/track/zipkin/SpringBoot整合Zipkin.md)
        * skywalking
            * [skywalking分布式追踪](microservice/track/skywalking/skywalking分布式追踪.md)
            * [Spring Cloud应用整合Skywalking](microservice/track/skywalking/SpringCloud应用整合Skywalking.md)
            * [SkyWalking收集之gRPC代理](microservice/track/skywalking/SkyWalking收集之gRPC代理.md)
    * 服务调用
        * Feign
            * [Feign基础](microservice/callservice/Feign/Feign基础.md)
    * 日志
        * logback
            * [logback日志打印](microservice/log/logback/logback日志打印.md)
        * ELK日志收集
            * [ELK日志收集](microservice/log/elk/ELK日志收集.md)
            * [微服务ELK日志配置](microservice/log/elk/微服务ELK日志配置.md)
        * P6Spy记录数据库日志
            * [P6Spy记录数据库日志](microservice/log/p6spy/P6Spy记录数据库日志.md)
    * 微服务部署
        * Docker
            * [Centos安装Docker](microservice/deploy/docker/Centos安装Docker.md)
            * [Docker 镜像与容器](microservice/deploy/docker/Docker镜像与容器.md)
            * [使用Dockerfile定制镜像](microservice/deploy/docker/使用Dockerfile定制镜像.md)
            * [Docker停止、删除所有的docker容器和镜像](microservice/deploy/docker/删除所有的docker容器和镜像.md)
            * Dockerfile 指令
                * [Dockerfile之COPY复制文件](microservice/deploy/docker/Instruction/Dockerfile之COPY复制文件.md)
            * [Docker参考文章](https://yeasy.gitbooks.io/docker_practice/)
        * Docker Compose
            * [Docker Compose入门](microservice/deploy/dockerCompose/DockerCompose入门.md)
        * Kubernetes容器编排管理平台
            * [Kubernetes基本概念](microservice/deploy/Kubernetes/Kubernetes基本概念.md)
            * [Kubernetes架构](microservice/deploy/Kubernetes/Kubernetes架构.md)
            * [Kubeadm安装Kubernetes](microservice/deploy/Kubernetes/Kubeadm安装Kubernetes.md)
        * Rancher
            * [安装Rancher](microservice/deploy/rancher/安装Rancher.md)
            * Rancher部署服务
                * [Rancher部署服务简单示例](microservice/deploy/rancher/Rancher部署服务简单示例.md)
            * [Rancher集群启动失败Failed to bring up Etcd Plane](microservice/deploy/rancher/Rancher集群启动失败FailedtobringupEtcdPlane.md)
            * [Rancher中文文档](https://docs.rancher.cn/rancher2x/)
        * Docker镜像仓库
            * Harbor
                * [Docker镜像仓库Harbor](microservice/deploy/repository/harbor/Docker镜像仓库Harbor.md)
    * 微服务监控
        * Spring Boot Actuator
            * [Spring Boot Actuator监控应用](microservice/monitor/SpringBootAdmin/SpringBootActuator监控应用.md)
        * Spring Boot Admin
            * [Spring Boot Admin入门指南](microservice/monitor/SpringBootAdmin/SpringBootAdmin入门.md)
    * 网络共享存储
        * NFS服务器
            * [NFS服务器搭建](microservice/网络文件系统/NFS服务器/NFS服务器搭建.md)
    * 常见问题
        * [分布式事务](microservice/question/分布式事务.md)
        * [单点登录SSO](microservice/question/单点登录SSO.md)
        * [分dan布式id生成方案](microservice/question/分布式id生成方案.md)
        * [限流的算法](microservice/gateway/function/限流的算法.md)
    * 项目实践
        * [chinahrss微服务实践](microservice/action/中国人社微服务实践.md)
        * [chinahrss微服务Docker化](microservice/action/chinahrss微服务Docker化.md)
        * [chinahrss使用Docker Compose部署](microservice/action/chinahrss使用DockerCompose部署.md)
        * [项目部署后调优](microservice/action/项目部署后调优.md)
    * [微服务面试提问](microservice/interview/微服务面试提问.md)
* 大型网站技术架构
    * [大型网站技术架构思维导图](framework/大型网站技术架构思维导图.md)
    * 高性能架构
        * [高并发](framework/highConcurrent/高并发.md)
    * 高可用架构
        * [可用性度量（系统可用性几个9）](framework/highAvailable/系统可用性几个9.md)
* [权限管理系统](./rbac/README.md)
    * [RBAC权限管理](./rbac/RBAC权限管理.md)
    * [创建数据库](./rbac/db/README.md)
    * [权限认证基础](rbac/base/权限认证基础.md)
    * shiro
        * [shiro基础](rbac/shiro/shiro基础.md)
        * [SpringBoot整合shiro](rbac/shiro/SpringBoot整合shiro.md)
        * [Shiro与JWT整合](rbac/shiro/Shiro与JWT整合.md)
    * Spring Security
        * [SpringBoot整合Spring Security](rbac/SpringSecurity/SpringBoot整合SpringSecurity.md)
        * [Spring Security入门](rbac/SpringSecurity/SpringSecurity入门.md)
    * OAuth2
        * [OAuth2基础](rbac/oauth2/OAuth2基础.md)
    * jwt
        * [JWT详解](rbac/jwt/JWT详解.md)
* [测试](test/README.md)
    * [单元测试](test/单元测试.md)
        * [Junit](./test/junit/README.md)
            * [Junit常见注解和执行顺序](./test/junit/Junit常见注解和执行顺序.md)
        * [Mock](./test/mock/README.md)
            * [Mockito](./test/mock/mockito/README.md)
                * [Mockito基本功能](./test/mock/mockito/Mockito基本功能.md)
                * [Mockito使用案例](./test/mock/mockito/Mockito使用案例.md)
                * [Mockito原理](./test/mock/mockito/Mockito原理.md)
                * [Mockito单测service](test/mock/Mockito单测service.md)
    * 压力测试
        * siege
            * [Mac压测Siege](test/PressureTest/siege/Mac压测Siege.md)
            * [Siege压测POST实例](test/PressureTest/siege/Siege压测POST实例.md)
        * JMeter
            * [mac下JMeter的安装](test/PressureTest/JMeter/JMeter的安装.md)
            * [JMeter的基本使用](test/PressureTest/JMeter/JMeter的基本使用.md)
            * 遇到的问题
                * [JMeter测试连接超时](test/PressureTest/JMeter/question/JMeter测试连接超时.md)
* [linux](linux/README.md)
    * [操作命令](linux/operation/README.md)
        * [linux查看哪些进程占用CPU内存资源多](linux/operation/linux查看哪些进程占用CPU内存资源多.md)
        * [Linux清除缓存buff/cache](linux/operation/Linux清除缓存buffcache.md)
        * [用户管理](linux/operation/用户管理.md)
        * [查找文件](linux/operation/查找文件.md)
        * [根据端口号/进程号查项目位置](linux/operation/根据端口号/进程号查项目位置.md)
        * [Linux文件大小和磁盘使用情况](linux/operation/Linux文件大小.md)
    * [sshd](linux/sshd/README.md)
        * [ssh一段时间就断掉](linux/sshd/ssh一段时间就断掉.md)
    * 挖矿
        * [清除挖矿程序（sysupdate, networkservice进程）](linux/error/清除挖矿程序.md)
        * [清除挖矿程序（kdevtmpfsi进程）](linux/error/清除挖矿程序kdevtmpfsi.md)
        * [清除挖矿程序（docker中Ubuntu容器）](linux/error/清除挖矿程序docker中Ubuntu容器.md)
    * Swap交换分区
        * [Linux Swap交换分区](linux/swap/LinuxSwap交换分区.md)
    * [nginx](linux/nginx/README.md)
        * [安装nginx](linux/nginx/安装nginx.md)
        * [nginx设置开机自启动](linux/nginx/nginx设置开机自启动.md)
        * 问题集锦
            * [nginx设置请求body大小](linux/nginx/problem/nginx设置请求body大小.md)
            * [403 Forbidden](linux/nginx/problem/403Forbidden.md)
            * [支持websocket](linux/nginx/problem/支持websocket.md)
        * [nginx的root和alias的区别](linux/nginx/nginx的root和alias的区别.md)
    * 软件安装
        * [Java安装](linux/insatll/java.md)
        * [FTP](linux/ftp/README.md)
            * [安装FTP服务](linux/ftp/安装FTP服务.md)
        * [unzip](linux/unzip/README.md)
        * [kafka](linux/kafka/README.md)
    * [云服务器ECS](aliyun/ecs/README.md)
        * [安装/重装系统](aliyun/ecs/安装系统.md)
* [计算机基础](./cs/README.md)
    * 计算机网络
        * [计算机网络常见知识点](net/计算机网络常见知识点.md)
        * [计算机网络面试问题](net/计算机网络面试问题.md)
    * [UML类图](cs/uml/README.md)
    * [磁盘存取](cs/disk/README.md)
    * [DNS域名解析](cs/dns/README.md)
    * [CDN](./cdn/README.md)
        * 相关概念
            * [DNS域名解析](cs/dns/README.md)
        * [阿里云CDN使用](cdn/阿里云CDN使用.md)
        * [阿里云带宽价格](cdn/阿里云带宽价格.md)
* [第三方库](library/README.md)
    * Sentinel
        * [Sentinel限流](library/Sentinel/Sentinel限流.md)
        * [Sentinel与Spring Cloud Gateway限流实例](library/Sentinel/Sentinel限流实例.md)
    * Spring Boot Admin
        * [整合Spring Boot Admin](library/SpringBootAdmin/整合SpringBootAdmin.md)
* [工具](tools/README.md)
    * maven
        * [Maven核心知识](tools/maven/Maven核心知识.md)
    * [jrebel热加载](./tools/Jrebel/README.MD)
    * [p3c插件检测代码规范](./tools/p3c/README.MD)
    * Swagger
        * [Swagger的使用](tools/swagger/Swagger的使用.md)
    * [抓包](./tools/grabbag/README.MD)
        * [fiddler(windows推荐)](./tools/grabbag/fiddler.MD)
    * [gitlab](./tools/gitlab/README.md)
        * [gitlab搭建](tools/gitlab/gitlab搭建.md)
        * Gitlab-CI
            * [Gitlab-Runner的安装与使用](tools/gitlab/ci/Gitlab-Runner的安装与使用.md)
            * [Gitlab-Runner实践](tools/gitlab/ci/Gitlab-Runner实践.md)
        * [gitlab配置custom hook](tools/gitlab/custom-hook.md)
        * [gitlab内存占用过大](tools/gitlab/gitlab内存占用过大.md)
        * [问题集锦](tools/gitlab/问题集锦.md)
    * [数据库连接池Druid](druid/README.md)
        * [Druid多数据源配置](druid/Druid多数据源配置.md)
    * [快捷键](keymap/README.md)
        * [IDEA上阅读源码快捷键](keymap/idea/IDEA上阅读源码快捷键.md)
    * [版本控制](./tools/vcs/README.md)
        * [git](./tools/vcs/git/README.md)
            * [gitignore文件屏蔽规则](./tools/vcs/git/gitignore文件屏蔽规则.md)
            * [android gitignore 模板](./tools/vcs/git/androidGitignore模板.md)
    * [运行脚本](tools/script/运行脚本.md)
    * gitbook
        * [gitbook插件使用](https://juejin.im/post/5ce51e126fb9a07ed440d7d0)
    * IDE
        * IDEA
            * [IDEA maven下载jar包太慢](tools/ide/idea/IDEAmaven下载jar包太慢.md)
* Java相关技术原理
    * [JavaAgent探针原理JVMTI](principle/agent/JavaAgent探针原理JVMTI.md)
* 常用工具类
    * 跨域支持
        * [CorsConfig](utils/跨域支持/CorsConfig.md)
* 面经
    * [盒马鲜生20200316](myinterview/2020/盒马鲜生20200316.md)
* 面试提问
    * [Java基础面试提问](base/interview/Java基础面试提问.md)
    * [JVM面试提问](base/jvm/JVM面试提问.md)
    * [Spring面试提问](spring/interview/Spring面试提问.md)
    * [MySql面试提问](db/mysql/interview/MySql面试提问.md)
    * [redis面试提问](redis/interview/redis面试问题.md)
    * [微服务面试提问](microservice/interview/微服务面试提问.md)
    * [计算机网络面试问题](net/计算机网络面试问题.md)
* 部门管理/项目管理
    * [关于亲力亲为的思考](manager/关于亲力亲为的思考.md)
    * [如何进行工作分配](manager/如何进行工作分配.md)
    * [如何做职场规划](manager/如何做职场规划.md)
* 工作日常思考
    * [APP更新方案选择](work/APP更新方案选择.md)

