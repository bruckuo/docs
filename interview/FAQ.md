## 重点(必读)
> [方向重点](https://mp.weixin.qq.com/s/RkMxPbm8E99-rTZKmvBy6Q)

### 每日
<font color="red">1、事物的隔离级别</font>
>未提交读(<font color="red">Read Uncommitted</font>)：允许脏读，也就是可能读取到其他会话中未提交事务修改的数据

>提交读(<font color="red">Read Committed</font>)：只能读取到已经提交的数据。Oracle等多数数据库默认都是该级别 (不重复读)

>可重复读(<font color="red">Repeated Read</font>)：可重复读。在同一个事务内的查询都是事务开始时刻一致的，InnoDB默认级别。在SQL标准中，该隔离级别消除了不可重复读，但是还存在幻象读

>串行读(<font color="red">Serializable</font>)：完全串行化的读，每次读都需要获得表级共享锁，读写相互都会阻塞

* <font color="red">脏读</font>: 脏读就是指当一个事务正在访问数据，并且对数据进行了修改，而这种修改还没有提交到数据库中，这时，另外一个事务也访问这个数据，然后使用了这个数据。
 
* <font color="red">不可重复读</font>:是指在一个事务内，多次读同一数据。在这个事务还没有结束时，另外一个事务也访问该同一数据。那么，在第一个事务中的两次读数据之间，由于第二个事务的修改，那么第一个事务两次读到的的数据可能是不一样的。这样就发生了在一个事务内两次读到的数据是不一样的，因此称为是不可重复读。

* <font color="red">幻读</font>:第一个事务对一个表中的数据进行了修改，这种修改涉及到表中的全部数据行。同时，第二个事务也修改这个表中的数据，这种修改是向表中插入一行新数据。那么，以后就会发生操作第一个事务的用户发现表中还有没有修改的数据行，就好象发生了幻觉一样。

<font color="red">事务级别越高,性能越差</font>

<font color="red">2、dubbo线上配置(这问题很扯淡)</font>  
> 答案：[精通Dubbo——Dubbo配置文件详解](https://blog.csdn.net/fuyuwei2015/article/details/72836075)  

<font color="red">3、Spring Cloud</font>  
 
<font color="red">4、MySQL优化</font>     
> [MySQL数据库优化的八种方式(经典必看)](https://www.jianshu.com/p/dac715a88b44)  
> [mysql优化,不用怕面试题了](https://blog.csdn.net/samjustin1/article/details/52314813)
   
### 滴
<font color="red">1、@Autowired和@Resource的区别</font>
>答案：[参考](https://www.zhihu.com/question/39356740) 
  
2、Executors.newFixedThreadPool(1)和Executors.newSingleThreadExecutor()区别

3、tomcat启动时候加载大量数据导致页面抖动问题处理  
 
### MySQL知识点
> [MySQL 面试之必会知识点](https://www.jianshu.com/p/5052f6a454ef)  
> [MySQL 高性能优化实战总结](https://mp.weixin.qq.com/s/sRsJzFO9dPtKhovJNWN3Dg)  
> [DB主从一致性架构优化4种方法](https://mp.weixin.qq.com/s/vcvlFQywsdGzsUYVWn17Gw)

### SpringCloud知识点
> [SpringCloud实现原理图](https://www.imooc.com/article/23679)  
> [微服务架构-Spring Cloud](https://www.jfox.info/2017/%E5%BE%AE%E6%9C%8D%E5%8A%A1%E6%9E%B6%E6%9E%84springcloud.html)
### Java知识点
> [CompletableFuture 详解](https://www.jianshu.com/p/6f3ee90ab7d3)  
> [Java线程池创建方式详解](https://blog.csdn.net/u011630575/article/details/51037423)   
> [HashMap和ConcurrentHashMap详解](https://mp.weixin.qq.com/s/QhRWDFgpjQ83Yz66V_6scQ) 
> [sleep()和wait()的区别](https://mp.weixin.qq.com/s/gvaksKy2ss90bsybCnajpQ)  
> [Thread Local的原理与适用场景](https://mp.weixin.qq.com/s/2Gfk9IjIMakk3DspRYxZdQ)  
> [如何合理的规划一次jvm性能调优](https://juejin.im/post/59f02f406fb9a0451869f01c)  


  

