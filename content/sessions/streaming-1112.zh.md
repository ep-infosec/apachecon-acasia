---
title: "基于 Apache Flink 的实时计算数据流框架在京东零售业务的实践和落地"
date: "2022-07-29T15:30:00"
track: "streaming"
presenters: "张颖，闫莉刚"
stype: "中文演讲"
speechLink: "https://player.bilibili.com/player.html?aid=899523647&cid=806318669&page=1"
---
京东零售数据与智能部基于京东业务特点，为提升特定场景下研发人员的开发效率而搭建了一套基于 Flink 的实时计算框架，致力于构建基于 Flink 的独有的数据流场景，本次主要分享京东零售数据与智能部积累的一些机器学习工程和相关数据分析的技术场景和相应的解决方案，包括但不限于：

1）榜单场景：致力于解决多流 join 场景和 TopN 场景

2）Query 动线分析场景：利用 Flink Gelly 将图分析结果数据落入多维分析 OLAP，然后启动流式分析查询 OLAP，供数据分析人员提供 QP 场景的 AB 因果分析等技术要点

3）机器学习场景：致力于构建基于Flink的独有的机器学习工作流，内部构成机器学习链路闭环，包括但不限于实时特征生成、样本拼接、特征工程、模型训练、模型预估等环节，全链路批流一体，复用算子。
 ### Speakers: 
 <img src="images/speaker/1112.png" width="200" /><br>张颖: 京东, 算法工程师, 我曾经负责搜推数据处理和轻量级训练系统和在线学习数据链路的搭建，包括Feature Dump 链路构建、label pipeline 的搭建、样本拼接、样本预处理、特征工程和小模型分布式训练，目前在负责数据分析优化部实时计算业务，并且希望在此基础之上沉淀出一套完整且能高效赋能业务的框架。比较积极参与社区，alink、dl on flink 等多个开源项目的contributor，曾经在Flink Forward Asia 2021 和 InfoQ QCon+ 案例研习社全球软件大会进行过演讲。

  <img src="images/speaker/1112_2.png" width="200" /><br>闫莉刚: 京东，资深技术专家，在数据流低代码实现有多年心得，主导了京东大数据实时平台建设、数据流框架以及组件化工具建设。


