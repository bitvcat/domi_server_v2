
## domi server 第二版

自己随便写的游戏服务器。

采用c++底层 + lua上层的结构，lua主要负责游戏业务逻辑，c++处理底层（网络、aoi、定时器、数据库等）

对比第一版本的改动：

- 不再使用libevent（太多无用的功能），移植redis的网络库；
- 未使用多线程，采用单线程（主线程一个eventloop）；
- 使用lua5.3


**ps：**

这个东西是自己工作空闲时间写的，也是想自己学点东西。比较挫。会自己慢慢优化，还有很多东西待完成。

