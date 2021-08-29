[volatile关键字](https://lotabout.me/2019/Java-volatile-keyword/)

　　一旦一个共享变量（类的成员变量、类的静态成员变量）被volatile修饰之后，那么就具备了两层语义：

　　1）保证了不同线程对这个变量进行操作时的可见性，即一个线程修改了某个变量的值，这新值对其他线程来说是立即可见的。

　　2）禁止进行指令重排序。

    volatile也无法保证对变量的任何操作都是原子性的

[volatile关键字解析](https://www.cnblogs.com/dolphin0520/p/3920373.html)

[深入理解可重入锁](jianshu.com/p/6e8a49121133)

[Java中volatile关键字的最全总结](https://cloud.tencent.com/developer/article/1618122)

线程封闭：Ad-hoc线程封闭，栈封闭，ThreadLocal类

ThreadLocal类：防止对可变的单实例变量或全局变量进行共享

ThreadLocal对象可以提供线程局部变量，每个线程Thread拥有一份自己的副本变量，多个线程互不干扰。

ThreadLocal的作用是提供线程内的局部变量，这种变量在多线程环境下访问时能够保证各个线程里变量的独立性。

[万字详解ThreadLocal关键字.md](https://github.com/Snailclimb/JavaGuide/blob/master/docs/java/multi-thread/%E4%B8%87%E5%AD%97%E8%AF%A6%E8%A7%A3ThreadLocal%E5%85%B3%E9%94%AE%E5%AD%97.md)

[ThreadLocal详解](https://zhuanlan.zhihu.com/p/34406557)

安全发布

Java监视器模式：一种编写代码的约定，对于任何一种锁对象，只要自始至终都使用该锁对象，都可以用来保护对象的状态。

使用私有的锁对象而非对象的内置锁（或任何其他可通过共有方式访问的锁）

[Java的值传递和引用传递](https://segmentfault.com/a/1190000016773324)