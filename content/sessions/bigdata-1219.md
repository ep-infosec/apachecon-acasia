---
title: "How to use the Cloud Shuffle Service in the Spark scenario of Bytedance"
date: "2022-07-30T16:10:00"
track: "bigdata"
room: "B"
presenters: "魏中佳"
speechLink: "https://www.youtube.com/embed/RBcpMorlxMk"
stype: "Chinese Session"
---
Bytedance mainly uses Spark for offline big data processing. Every day, hundreds of thousands of Spark jobs are performed online. Internal service users have specific requirements for SLA. If the SLA is breached, services will be greatly affected. Shuffle is an important operation of the Spark engine. In large-scale operations, the open-source ExternalShuffleService(ESS) implementation mechanism may cause disk IOPS bottlenecks and Fetch requests backlog caused by a large number of random reads. As a result, Stage recalculation and even job failure often occur in the calculation process, which leads to a vicious cycle of resource use and seriously affects SLA. In addition, in the offline mixed scenario inside Bytedance, the capacity of the online machine is small, and the problem of full disk is often encountered during operation.
In this context, the Spark team optimized ESS, including optimizing Shuffle parameters (reducing random read requests) and increasing Shuffle traffic limiting, greatly improving ESS stability in SSD clusters. On the other hand, we propose Cloud Shuffle Service(CSS) as a solution for the cluster of HDD/offline mixing scenarios. That is, the Map Task pushes data from a partition to the same CSS working node in push mode. The Reduce task can read data from the corresponding node in sequence, greatly improving the read performance and Shuffle stability, and effectively ensuring SLA.
The CSS has been connected to Spark, Flink, and MapReduce in ByteDance.
 ### Speakers: 
 <img src="images/speaker/1219.png" width="200" /><br>Zhongjia Wei: Graduated from the University of Electronic Science and Technology of China, he is currently a infrastructure big data development engineer of ByteDance, focusing on the field of distributed computing of big data. He is mainly responsible for Spark kernel development and ByteDance self-developed Shuffle Service development.

 
