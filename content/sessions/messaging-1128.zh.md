---
title: "鲁班RocketMQ平台消息灰度方案"
date: "2022-07-30T14:40:00"
room: "B"
track: "messaging"
presenters: "区二立"
speechLink: "https://player.bilibili.com/player.html?aid=557106751&cid=806450981&page=1"
stype: "中文演讲"
---
RocketMQ（以下简称MQ）作为消息中间件在事务管理，异步解耦，削峰填谷，数据同步等应用场景中有着广泛使用。当业务系统进行灰度发布时，Dubbo与HTTP的调用可以基于业界通用的灰度方式在vivo的微服务治理与网关平台来实现，但MQ已知的灰度方案都不能完全解决消息的隔离与切换衔接问题，为此，vivo技术架构团队在鲁班MQ平台（包含根因分析、资源管理、订阅关系校验、延时优化等等的扩展）增加了MQ灰度功能的扩展实现，该方案主要以拆分queue的目标使用方式为基础进行深度扩展封装实现。
 ### Speakers: 
 <img src="images/speaker/1128.png" width="200" /><br>区二立: vivo, 技术总监, 
 - 前阿里中间件技术架构师，阿里云云原生解决方案架构师，在不同场合从原理与实战上分享过不同的中间件。
 - 当前任职vivo平台中心总监，从0到1主导建设鲁班MQ平台，分库分表平台（支持复杂语句，定制化的策略），包括dubbo/mq/http/xxlJob的共享开发平台，全格式的全局id服务(考虑开源)；
 - 扩展封装redisson, dubbo,sentinel,seata等通用中间件。

 