# Base
## Java Base
* 数据类型
   * 基本数据类型
      * 整数类型: byte(1\*8bit), short(2\*8bit), int(4\*8bit), long(8\*8bit)
      * 浮点型: float(4\*8bit), double(8\*8bit)
      * boolean(1bit)
      * char(2\*8bit)
   * 包装类型
      * 整数类型: Byte, Short, Integer, Long
      * 浮点型: Float, Double
      * Boolean
      * Charactor
   * 引用类型
      * Object: 所有的类都继承了Object类, 所有的类对象都是一个Object
* 循环语句/条件语句
   ```Java
      do {
         // do something
      }while()
   ```
   ```Java
      for(int i=0;i<10;i++){
         // do something
      }
   ```
   ```Java
      if(){
      
      }else if(){
      
      }else{
      
      }
   ```
* 异常
   * Throwable
   * 运行时异常: RuntimeException
   * 检查时异常: Exception
* IO
* 集合类
   * Array: `int[] nums = new int[5]`
   * List
      * ArrayList: `List<Integer> nums = new ArrayList<>();`
      * LinkedList: `List<Integer> nums = new LinkedList<>();`
   * Set
      * HashSet: `Set<Integer> nums = new HashSet<>();`
   * Map: 
      * HashMap: `Map<String, Integer> nums = new HashMap<>();`
      * ConccurrentHashMap: `Map<String, Integer> nums = new ConccurrentHashMap<>();`
   * Queue:
      * LinkedBlockingQueue
      * ArrayBlockingQueue
      * PriorityBlockingQueue
      * SynchronousQueue
* 多线程
   * Thread
   * Runable
   * Executor
   * ThreadPoolExecutor
* 锁
   * synchronized
   * ReentrantLock
   * AQS
## JVM
* 内存划分
* GC算法
* GC收集器
* 类加载机制
## Data Structure
* 数组
* 链表: 单链表, 循环双链表
* 队列
* 栈
* 树: 二叉树, 平衡二叉树, 红黑树, B树, B+树l
## Algorithm
* 贪心算法
* 分治法
* 动态规划
## Design Model
* 建造者模式
* 单例模式
* 观察者模式
* 策略模式
* 过滤器模式
## Computer Network
* 七层网络模型
* [TCP](https://tools.ietf.org/html/rfc793)
* [UDP](https://tools.ietf.org/html/rfc768)
* [HTTP](https://developer.mozilla.org/en-US/docs/Web/HTTP#:~:text=Hypertext%20Transfer%20Protocol%20(HTTP)%20is,be%20used%20for%20other%20purposes.)
* [HTTPS](https://www.ssl.com/faqs/what-is-https/)
## Linux
* Move: cd, mkdir, ls, pwd, rm, cp, mv
* Search: grep, find, where, which, locate
* Privilege: chmod, chowm, su, who
* Service: df, free, top, ps, kill, service
* Network: ssh, scp, wget, curl, netstat
* Configuration: uname, ifconfig, yum, echo, history, man, info
* Read: cat, less, more, tail, head, vim

# Advance
## Distribution
## Micro Service
## Hadoop
## Middleware
* Redis, Mysql, RocketMQ/Kafka, Zookeeper, Spring/SpringBoot/SpringCloud

# Book
* [数据结构](/book/数据结构与算法分析java语言描述原书第3版.pdf)
* [算法](/book/算法第四版.pdf)
* [设计模式](/book/HeadFirst设计模式.pdf)
* [深入理解Java虚拟机](深入理解Java虚拟机.pdf)

# Ide
* [Jet Brains Toolbox App](https://www.jetbrains.com/toolbox/app/)(在toolbox中下载各种ide)
    * [有@edu邮箱](https://www.jetbrains.com/shop/eform/students)
    * 无@edu邮箱: 破解

# Reference
* [Java菜鸟教程](https://www.runoob.com/java/java-tutorial.html)
* [设计模式菜鸟教程](https://www.runoob.com/design-pattern/design-pattern-tutorial.html)
