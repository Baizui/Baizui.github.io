---
layout: article
title:  "tableau、初学者"
date:   2017-11-30 22:07:50 +0800
categories: infovis
image:
  teaser: t.jpg
  feature: t.jpg

---


## 发布与发放
* tableau中的图像和 PDF 不包含底层数据，无论是交互性还是数据更新度都是静态的，因为它们只是在特定时刻获取的快照
* tableau中的工作簿，无论是否打包来包含数据，都可与使用 Tableau Reader 或 Tableau Desktop 的其他人共享。其中Tableau Reader可以查看工作簿并与之交互，而Tableau Desktop可以查看和编辑工作簿。
* tableau中的仪表板图像将为最新状态的仪表板，而故事图像将包含最新状态的最新故事点
* Tableau Desktop中的工作簿可另存为 .twb 文件或 .twbx 文件。其中 .twb 工作簿未打包数据本身 – 它们只包含连接数据和构造视图所需要的信息。 打开 .twb 文件需要有权访问用来创建该文件的同一数据源。而.twbx 工作簿是打包的 – 它们包含与 .twb 相同的信息，以及任何数据和本地文件。.twbx 文件不加密，因此没有数据安全性 – 打开 .twbx 将显示所有底层数据。

## Tableau 入门
* Tableau Desktop是自动创建默认联接。
* tableau可以选择让数据是实时连接到数据还是提取数据。
* 维度是类别字段，这些字段是我们对数值数据进行切片和切块时的依据。维度常常是离散的。离散的字段在图表中形成标签，在数据窗格和视图中以蓝色进行颜色编码。
* 度量则是我们的指标。这是我们希望分析的数字。度量常常是连续的。连续的字段在图表中形成轴，其胶囊以绿色进行颜色编码。
* Tableau Desktop 会以年度汇集日期。可以使用“加号 (+)”将其展开。
* 在 Tableau Desktop 中，我们只需要在“数据”窗格中，通过拖放操作叠放字段，就能创建分层结构。
* 最有效的工作簿分享方式是将其发布到 Tableau Server 或 Tableau Online 中。已发布的工作簿仍然具有完整的交互性，随时保持最新版本。 

## 连接数据源
* 有实时和提取两种方式连接数据源。实时：适合数据量较小，数据实时更新的情况。提取：将数据抽到内存中，生成.tde文件，要更新数据，当报表publish到server上可以设置数据源的刷新Schedule。数据源右上角有一个筛选器，点击“添加”对数据进行筛选，类似自定义SQL中的where条件。数据源是可以多表关联的，默认内联。

## 使用多个维度
- 每个度量创建单个轴。将度量拖到“行”和“列”功能区来为每个度量添加单个轴。
- 两个度量共用一个轴。拖动一个度量或轴并将其放在现有轴上。
- 双轴，其中有两个在同一个区中分层的独立轴。双轴是相互层叠的独立轴。若要添加度量作为双轴，只需将字段拖到视图右侧并在看到黑色虚线时放置，也可以在该度量的字段菜单中选择“双轴”。使用双轴时，可以通过右键单击“双轴”并选择“同步轴”来使得两个轴对齐。
 
## 参考来源
* [tableau视频--发布与发放](https://www.tableau.com/zh-cn/learn/tutorials/on-demand/distributing-and-publishing?product=&version=10.0&topic=getting_started)
* [tableau视频--入门](https://www.tableau.com/zh-cn/learn/tutorials/on-demand/getting-started?product=&version=10.0&topic=getting_started)
* [tableau视频--Tableau界面](https://www.tableau.com/zh-cn/learn/tutorials/on-demand/tableau-interface?product=&version=10.0&topic=getting_started)