# kafkaSummary

![kafka](https://kafka.apache.org/23/images/kafka-apis.png)
# 问题深思
* kafka节点之间如何复制备份的？
* kafka消息是否会丢失？为什么？
* kafka最合理的配置是什么？
* kafka的leader选举机制是什么？
* kafka对硬件的配置有什么要求？
* kafka的消息保证有几种方式？
* kafka为什么会丢消息？

## 1.基本概念
   * kafka的主题和分区内部是如何存储的，它有什么特点？
   * 与传统的消费系统相比，kafka的消费模型有什么特点？
   * 卡夫卡如何实现分布式的数据存储和数据读取？
   
## 2.broker 的基本模块
![broker](https://img-blog.csdn.net/20140803144704215?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbGl6aGl0YW8=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

### kafkaAPIS
   * LogManager
   ![log](http://on-img.com/chart_image/5b717077e4b067df5a071754.png?_=1534417180862)
   
   >> LogSegment: skiplist 表数据结构
   
   * ReplicaManager
   ![replica](https://img-blog.csdn.net/20180914092814878?watermark/2/text/aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzM5OTA3NzYz/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70)
   
   * Offset Manager
   
   * Kafka Sechduler
