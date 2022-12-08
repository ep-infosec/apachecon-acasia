---
title: "No Topic Metadata Limitation, the Infinite Data Retention in Apache Pulsar"
date: "2022-07-30T14:50:00"
track: "messaging"
room: "A"
presenters: "Penghui Li"
speechLink: "https://www.youtube.com/embed/4qcv5TyaSRQ"
stype: "Chinese Session"
---
Abstract: The Pulsar topic data will not be limited by the storage resources of a single node anymore, even if the topic is a non-partitioned topic or a partitioned topic with a single partition. The fundamental reason is that Pulsar uses the logical storage model. Pulsar topic data will be distributed to more bookies nodes, and the partition/topic will not be 1:1 bound to any storage node. 

But the Logical Storage Model also means that we need to maintain metadata for each data segment in the metadata store, a ledger list to indicate which ledgers are the data stored. The metadata storage mode will be a bottleneck if you want infinite topic data retention. Reducing the frequency of ledger rollover can extend the time to encounter bottlenecks, but the topic unloading will also cause ledger rollover. It can be triggered but the load manager, restart broker, or manually.

The topic metadata limitation is mainly in two parts:

1. a) The large Znode size to maintain the metadata of a topic
2. b) The memory consumption to cache all the ledgers of a topic 

Penghui will share how Pulsar gets rid of the limitation to support infinite data retention of the topic.
 ### Speakers: 
 <img src="images/speaker/1185.png" width="200" /><br>Penghui Li: StreamNative Tech lead & Apache Pulsar PMC member/committer, Penghui Li is passionate about helping organizations to architect and implement messaging services. Prior to StreamNative, Penghui was a Software Engineer at Zhaopin.com, where he lead the adoption and implementation of Pulsar.

 