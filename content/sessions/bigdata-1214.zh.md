---
title: "基于血缘的离线数仓数据发现方法"
date: "2022-07-29T16:50:00"
track: "bigdata"
room: "B"
presenters: "韩帅,孙科"
speechLink: "https://player.bilibili.com/player.html?aid=772071638&cid=805992133&page=1"
stype: "中文演讲"
---
在数据中台的大背景下，离线数仓领域中用户经常需要解决以下问题:
- 哪些 Hive 表包含业务 A 的数据
- Hive 表核心字段是否存在转存导致的权限放大问题
- Hive 表是否包含机密数据需要被清理
这些问题可以统一归类为数据发现问题。字节跳动针对离线数仓任务进行SQL分析，构建 Hive表的血缘关系，基于标签传播算法以自动化工程化地解决数据发现问题，规避人工标注存在的周期长、成本高、准确率低、不灵活等问题。
数据发现包括但不限于: Hive 表/列的业务分类分级和机密字段识别等。
应用场景举例:
1. 哪些 Hive 表包含业务 A 的埋点数据
通过分析 ETL SQL的执行逻辑结合各类 Filter 过滤条件判断下游表是否会包含 app='a' 的数据
2. 某ODS表中以复杂结构存储了一些机密数据，通过对下游表进行SQL分析，识别出下游表是否包含复杂结构的一部分数据, 进而识别权限放大问题。例如，是否包含map中某一个key的数据等
3. 某个机密字段是否已经完成脱敏
 ### Speakers: 
 <img src="images/speaker/1214.png" width="200" /><br>韩帅: 字节跳动-大数据计算引擎组 高级研发工程师, 拥有多年大数据研发经验。熟悉SparkSQL, Hive, Calcite, Druid等多种大数据组件。

 <img src="images/speaker/1214_2.png" width="200" /><br>孙科: 字节跳动-大数据计算引擎组 高级研发工程师, 负责统一 SQL 查询服务, Hive 元数据, 权限服务和大数据安全合规相关工作，拥有多年大数据研发经验，熟悉SparkSQL, Hive, Hudi, Parquet和Calcite等多种大数据组件。

 