# HTTP-NG

- 模块化及功能增强

- 分布式对象

- 第一层：报文传输

  > **不考虑报文的含义和目的，只关心报文的有效传输**

  - 1 对报文进行管道化和批量化传输，以降低往返耗时

  - 2 重用连接，以降低时延，提高传输宽带

  - 3 在同一条连接上并行地复用多个报文流，在防止报文流饿死的同时优化共享连接

  - 4 对报文进行有效的分段，使报文边界的确定更加容易

- 第二层：远程调用

  > `HTTP-NG` 结构的中间层提供了对远程方法调用的支持。提供了通用对请求/响应框架，客户端可通过此框架调用对服务器资源的操作。**不关心特定操作的实现及语义**

- 第三层：Web应用

  > 基本思想是提供与 `HTTP/1.1` 等价的功能和一些扩展接口，同时将其映射到一个可扩展的分布式对象框架中去

- WebMUX

- 二进制连接协议
