# Python基础记录
- GIL：全局解释器锁（Global Interpreter Lock），确保任何时候只有一个python线程在执行，说明多线程的python并不能真正的并行执行。可以用进程池来解决这个问题，在每个进程上都创建一个实例，这样每个实例都有自己的GIL，从而可以利用多核CPU达到并行效果；**进程之间的开销主要来源与：主进程和子进程之间的通信，必须进行序列化和反序列化操作。**

- 