---
title: "RocketMQ Streams-轻流计算在云安全和边缘计算的最佳实践"
date: "2022-07-30T14:00:00"
track: "messaging"
room: "B"
presenters: "袁小栋"
speechLink: "https://player.bilibili.com/player.html?aid=472054413&cid=806352398&page=1"
stype: "中文演讲"
---
大数据越来越重要，越来越多的产品依赖大数据计算，如果你的产品是部署在用户机房，边缘端，私有云，当产品输出时，就会部署一些列大数据集群如：采集集群，流计算集群，消息队列集群，每个集群最少3台机器才能保证集群的可靠性，即使有混部，输出资源也是非常大的，尤其是流计算需要对任务提前设置资源，而且每个任务资源开销也很大，很快资源不足了，还需要扩容（采购，审批，部署）。RocketMQ Streams集成了采集能力，消息队列，流计算能力一体化，1core，1g可以部署，而且可以像web应用那样通过增加实例横向扩展，尤其对于高过滤场景做了大量优化资源不随规则增加线性增加，cpu资源是同类大数据计算的40%，cpu是4%。

在这个专题中，大家不仅可以了解rocketmq-streams的实现原理，也可以基于阿里对rocketmq-streams的应用实践，来判断自己的业务是否可以有更轻的方案，降低产品成本，提供竞争力
 ### Speakers: 
 <img src="images/speaker/1049.png" width="200" /><br>袁小栋: 阿里云, 高级技术专家, 袁小栋：Apache RocketMQ Committer, rocketmq-streams cofounder，阿里云高级技术专家，安全智能计算引擎负责人

 