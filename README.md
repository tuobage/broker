# broker
消息分发系统，类似zmq库的pub/sub功能，功能但比zmq的简单，只纯粹做异步消息代理。


1.目前只支持tcp协议。

2.消息底层采用zero copy策略。

3.只负责消息流的传递，不负责包的完整性。

# 测试数据：

平均包为20字节：代理速度1270W/s，cpu：9%，内存：113m.

平均包为50字节：代理速度730W/s，cpu：11%，内存：132m.
