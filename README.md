# Tolerance-SnowDB
### 一个基于raft协议的高可用分布式数据库



​	该项目为一个分布式集群数据库，支持高可用和容错特性，参考了MIT分布式课程部分代码



#### 原理：

- 底层共识协议基于：raft
- 数据库：目前只是一个简单的hashmap，以后会把本人写的基于bitcask模型的snowDb融合进来（由于snowdb使用c++编写，两者之间需要rpc通信，目前还没有融合进来）



#### Todo

- 扩展为一个shard分片的分布式数据库
- 支持二阶段提交事务
