---
title: "使用Apache ECharts在Apache Superset中引入高级的下钻功能"
date: "2022-07-29T14:40:00"
track: "datavisualization"
presenters: "Ville Brofeldt"
stype: "英文演讲"
speechLink: "https://player.bilibili.com/player.html?aid=899557406&cid=805946016&page=1"
---
目前Apache Superset的功能是仪表板原生过滤器，这使得向仪表板添加交互式过滤器成为可能，从而控制图表上显示的数据。然而，到目前为止，只有精选图表类型提供了向其他图表发出过滤器的交叉过滤功能，这限制了用户交互主要局限于本地过滤器。

目前，该项目正在致力于为主要的可视化类型引入一组丰富的交互功能，使使用图表向下钻取(例如单击一个国家以显示城市分布)、钻取(钻取数据集中的任何维度，不考虑层次结构)、钻取(动态显示行级数据)和钻取到仪表板(打开一个新的仪表板，选中的维度预先作为本地过滤器填充)成为可能。这意味着用户将能够与图表交互，而不是局限于当前的本机筛选类型集。

在这次演讲中，我们将探索该特性的细节，新的上下文菜单，扩展功能的钩子，以及在构建自定义可视化插件和时间轴时使用该特性。我们还将展示该特性如何与Apache ECharts (Superset使用的主要可视化库)集成，以及未来的开发计划。
 ### Speakers:
 <img src="images/speaker/1227.png" width="200" /><br>Ville Brofeldt: 软件工程师, Ville Brofeldt是Apache Superset项目的长期提交者和PMC成员，在数据可视化、数据工程和预测分析方面拥有丰富的经验。
