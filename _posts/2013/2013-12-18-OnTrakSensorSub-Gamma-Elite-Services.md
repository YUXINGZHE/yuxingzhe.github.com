---
layout: post
title: "Gamma Elite<sup>SM</sup> Service"
tags: [OnTrak, Sensor Sub]
author_name: YUXINGZHE
author_uri: http://twitter.com/yuxingzhe
---

<span class="dropcap">在</span>OnTrak传感器接头不断旋转时，Gamma Elite<sup>SM</sup>功能将伽马与方位的测量联系起来(correlates gamma ray measurements to azimuthal orientation)，从而对井眼轨迹实现更加精确的控制以最大化提高油气采收率，并能在使用各种不同性能钻井液的情况下取得实时的地层结构与油藏物理信息。

在未引入高级伽马功能以前，需要将接头提起并将传感器定位完毕后再进行事后测量(post drilling logging)。而高级伽马服务可以获取实钻方位数据，从而省去了定向伽马的工作，节省了钻井时间。

分区伽马测量(sectored gamma ray measurements)以及近钻头传感器的布置方式能尽早地检测到钻头何时进入和离开油藏区域，这也为油藏定位和方案决策提供了一个不可或缺的判断方法。

#### 测量原理(Principle of measurement) ####

高频工具面测量技术(High frequency tool-face determination)将伽马测量数据分入8个相互分离的工具面扇区内，这样能提供更为精确的地质倾角与方位的信息。用户可以选择上下左右四个区域来决定实时数据的传输模式。

<a target="_blank" href="https://lncvgg.blu.livefilestore.com/y2prbAZZzcOWGaeSYFxuSStYHaCCJkUAqyq5qMSBYzqD4MeYjtuJ0jD4Lo0ff7-082c35MUeoxycuqGa09I-YWmergizOWlA9kbyal_WDjxA8c/ToolfaceSectors.png?psid=1">
<img class="aligncenter" title="Sector schematic illustrating orientation of 8 tool-face sectors; color scheme indicates quadrants available for real-time data transmission" style="width:400px;height:380px;" src="https://lncvgg.blu.livefilestore.com/y2prbAZZzcOWGaeSYFxuSStYHaCCJkUAqyq5qMSBYzqD4MeYjtuJ0jD4Lo0ff7-082c35MUeoxycuqGa09I-YWmergizOWlA9kbyal_WDjxA8c/ToolfaceSectors.png?psid=1" alt="Sector schematic illustrating orientation of 8 tool-face sectors; color scheme indicates quadrants available for real-time data transmission">

当接头旋转时，<u>每个扇区会累记25s内所检测到的信号数量，定向探头测得的工具面值每16ms更新一次(60Hz)</u>。而处于扇区边界处的信号则会根据它们与各扇区边界和工具面的相对距离进行分类。每个扇区所接收到的信号总数除以探测器在各扇区停留的时间就得到了相应扇区每秒钟所接收到的信号数量(cps)。

在接头上相隔180°安装着两个相互独立的闪烁计数器，这样不但可以提高计数精度，而且还能保证在其中一个发生故障后，另外一个仍能继续完成测量任务，从而提高了系统的可靠性。当转速高达400RPM时探测器仍能十分精确地分辨出各相邻扇区的边界。

<a target="_blank" href="https://lncvgg.blu.livefilestore.com/y2pZhY1vn6RB4li6EsFwExxKPI-x7scbRr96lw5GvbBpJQ3H45sarKE9qZ0lY1q6C7XCeLgZHMJR6ejTE9Crjj5qt5PcC1WUFQFCGMvPKXVTr8/SectoringPrincipal.png?psid=1">
<img class="aligncenter" title="Schematic illustrating principle of sectoring: red marksrepresenting count events, yellow ticks representing tool face measurements" style="width:400px;height:380px;" src="https://lncvgg.blu.livefilestore.com/y2pZhY1vn6RB4li6EsFwExxKPI-x7scbRr96lw5GvbBpJQ3H45sarKE9qZ0lY1q6C7XCeLgZHMJR6ejTE9Crjj5qt5PcC1WUFQFCGMvPKXVTr8/SectoringPrincipal.png?psid=1" alt="Schematic illustrating principle of sectoring: red marks representing count events, yellow ticks representing tool face measurements">

伽马数据累记原则如下：

<ul style="margin-left:50px;">
<li>如果井斜小于5°，定向探头将传输磁工具面(MTF)数据</li>
<li>如果转速低于15RPM且井斜大于5°，定向探头将传输重力工具面(GTF)数据</li>
<li>如果转速高于15RPM且井斜大于5°，定向探头将传输重力工具面(GTF)数据。利用动态测井所获取的方位与井斜数据，再通过磁通门传感器可以得到以上信息。(This information is derived from the magnetometers using the azimuth and inclination determined by the "flow on" survey.)</li></ul>

#### 遥测(Telemetry) ####

遥测所需的各扇区每秒接收到的信号数量(CPS)可以通过以下两种方式得到：

<ul style="margin-left:50px;">
<li>使用更加可靠的双探测器模式("归一化方法")，或者</li>
<li>单独选择A通道或B通道(如果其中之一发生故障的话)</li></ul>

接头可以自动检测闪烁计数器的好坏，如果检测到其中一个闪烁计数器发生了故障，接头将自动切换到单通道模式下发送实时计数数据。

由于接头具有自动检测功能，因此通过下行指令指定某一个或同时指定两个探测器来进行实时数据传输并不会对方位伽马的测量精度产生任何影响。

四个区域的信号频率经过归一化后进行上行传输：

<table id="customers" align="center" style="width:80%;">
<caption>表1 伽马信号</caption>
<tr>
<th>代码</th>
<th>助记符</th>
<th>Adam节点 +CMD</th>
<th>变化趋势(Scaling)</th>
<th>位数(Bits)</th>
<th>描述</th>
</tr>

<tr>
<td>PGAM_CFG_TOPX</td>
<td>GRBUX</td>
<td>Node E4 - Cmd 40</td>
<td rowspan="4">0.168-172.463cps线性变化</td>
<td>10</td>
<td>上四分区伽马</td>
</tr>

<tr class="alt">
<td>PGAM_CFG_BTMX</td>
<td>GRBDX</td>
<td>Node E4 - Cmd 40</td>
<td>10</td>
<td>下四分区伽马</td>
</tr>

<tr>
<td>PGAM_CFG_LHX</td>
<td>GRBLX</td>
<td>Node E4 - Cmd 40</td>
<td>10</td>
<td>左四分区伽马</td>
</tr>

<tr class="alt">
<td>PGAM_CFG_RHX</td>
<td>GRBRX</td>
<td>Node E4 - Cmd 40</td>
<td>10</td>
<td>右四分区伽马</td>
</tr>
</table>

在地面系统中由RTProc根据四个分区中的信号数量(base counts)分别计算出表观和修正API值(apparent and corrected API values)：

<ul style="margin-left:50px;">
<li>GRBUX&nbsp;&rArr;&nbsp;GRAUX&nbsp;&rArr;&nbsp;GRCUX</li>
<li>GRBDX&nbsp;&rArr;&nbsp;GRADX&nbsp;&rArr;&nbsp;GRCDX</li>
<li>GRBRX&nbsp;&rArr;&nbsp;GRARX&nbsp;&rArr;&nbsp;GRCRX</li>
<li>GRBLX&nbsp;&rArr;&nbsp;GRALX&nbsp;&rArr;&nbsp;GRCLX</li></ul>

#### 存储(Memory) ####

以下参数每隔25s写入1b2cffff.m00文件一次：

<table id="customers" align="center">
<caption></caption>
<tr>
<th>通道A</th>
<th>通道B</th>
</tr>

<tr>
<td colspan="2">每个扇区接收到的信号数量</td>
</tr>

<tr class="alt">
<td>PGAM_CHA_PULSE0M</td>
<td>PGAM_CHB_PULSE0M</td>
</tr>

<tr>
<td>PGAM_CHA_PULSE1M</td>
<td>PGAM_CHB_PULSE1M</td>
</tr>

<tr class="alt">
<td>PGAM_CHA_PULSE2M</td>
<td>PGAM_CHB_PULSE2M</td>
</tr>

<tr>
<td>PGAM_CHA_PULSE3M</td>
<td>PGAM_CHB_PULSE3M</td>
</tr>

<tr class="alt">
<td>PGAM_CHA_PULSE4M</td>
<td>PGAM_CHB_PULSE4M</td>
</tr>

<tr>
<td>PGAM_CHA_PULSE5M</td>
<td>PGAM_CHB_PULSE5M</td>
</tr>

<tr class="alt">
<td>PGAM_CHA_PULSE6M</td>
<td>PGAM_CHB_PULSE6M</td>
</tr>

<tr>
<td>PGAM_CHA_PULSE7M</td>
<td>PGAM_CHB_PULSE7M</td>
</tr>

<tr class="alt">
<td colspan="2">每个扇区的信号采集时间</td>
</tr>

<tr>
<td>PGAM_CHA_TIME0M</td>
<td>PGAM_CHB_TIME0M</td>
</tr>

<tr class="alt">
<td>PGAM_CHA_TIME1M</td>
<td>PGAM_CHB_TIME1M</td>
</tr>

<tr>
<td>PGAM_CHA_TIME2M</td>
<td>PGAM_CHB_TIME2M</td>
</tr>

<tr class="alt">
<td>PGAM_CHA_TIME3M</td>
<td>PGAM_CHB_TIME3M</td>
</tr>

<tr>
<td>PGAM_CHA_TIME4M</td>
<td>PGAM_CHB_TIME4M</td>
</tr>

<tr class="alt">
<td>PGAM_CHA_TIME5M</td>
<td>PGAM_CHB_TIME5M</td>
</tr>

<tr>
<td>PGAM_CHA_TIME6M</td>
<td>PGAM_CHB_TIME6M</td>
</tr>

<tr class="alt">
<td>PGAM_CHA_TIME7M</td>
<td>PGAM_CHB_TIME7M</td>
</tr>
</table>

在以上32个原始测量数据的基础上，存储器处理单元将绘制出以下252条曲线：

<table id="customers" align="center" style="width:90%;">
<caption></caption>
<tr>
<th>标准数据(Standard)</th>
<th>网格化数据(Gridded)</th>
<th>滤波数据(Filtered)</th>
<th></th>
<th></th>
<th>曲线数量(# of curves)</th>
</tr>

<tr>
<td>GRBSA</td>
<td>GRBSAG</td>
<td>GRBSAF</td>
<td>Sector 0-7</td>
<td>Base Counts; Channel A (CPS)</td>
<td>8</td>
</tr>

<tr class="alt">
<td>GRBSB</td>
<td>GRBSBG</td>
<td>GRBSBF</td>
<td>Sector 0-7</td>
<td>Base Counts; Channel B (CPS)</td>
<td>8</td>
</tr>

<tr>
<td>GRBS</td>
<td>GRBSG</td>
<td>GRBSF</td>
<td>Sector 0-7</td>
<td>Base Counts; Channels Normalized (CPS)</td>
<td>8</td>
</tr>

<tr class="alt">
<td>GRBU</td>
<td>GRBUG</td>
<td>GRBUF</td>
<td>Upper Quadrant</td>
<td>Base Counts; Channels Normalized (CPS)</td>
<td>1</td>
</tr>

<tr>
<td>GRBD</td>
<td>GRBDG</td>
<td>GRBDF</td>
<td>Lower Quadrant</td>
<td>Base Counts; Channels Normalized (CPS)</td>
<td>1</td>
</tr>

<tr class="alt">
<td>GRBL</td>
<td>GRBLG</td>
<td>GRBLF</td>
<td>Left Quadrant</td>
<td>Base Counts; Channels Normalized (CPS)</td>
<td>1</td>
</tr>

<tr>
<td>GRBR</td>
<td>GRBRG</td>
<td>GRBRF</td>
<td>Right Quadrant</td>
<td>Base Counts; Channels Normalized (CPS)</td>
<td>1</td>
</tr>

<tr class="alt">
<td>GRASA</td>
<td>GRASAG</td>
<td>GRASAF</td>
<td>Sector 0-7</td>
<td>Apparent; Channel A (API)</td>
<td>8</td>
</tr>

<tr>
<td>GRASB</td>
<td>GRASBG</td>
<td>GRASBF</td>
<td>Sector 0-7</td>
<td>Apparent; Channel B (API)</td>
<td>8</td>
</tr>

<tr class="alt">
<td>GRAS</td>
<td>GRASG</td>
<td>GRASF</td>
<td>Sector 0-7</td>
<td>Apparent; Channels Normalized (API)</td>
<td>8</td>
</tr>

<tr>
<td>GRAU</td>
<td>GRAUG</td>
<td>GRAUF</td>
<td>Upper Quadrant</td>
<td>Apparent; Channels Normalized (API)</td>
<td>1</td>
</tr>

<tr class="alt">
<td>GRAD</td>
<td>GRADG</td>
<td>GRADF</td>
<td>Lower Quadrant</td>
<td>Apparent; Channels Normalized (API)</td>
<td>1</td>
</tr>

<tr>
<td>GRAL</td>
<td>GRALG</td>
<td>GRALF</td>
<td>Left Quadrant</td>
<td>Apparent; Channels Normalized (API)</td>
<td>1</td>
</tr>

<tr class="alt">
<td>GRAR</td>
<td>GRARG</td>
<td>GRARF</td>
<td>Right Quadrant</td>
<td>Apparent; Channels Normalized (API)</td>
<td>1</td>
</tr>

<tr>
<td>GRCSC</td>
<td>GRCSCG</td>
<td>GRCSCF</td>
<td>Sector 0-7</td>
<td>Corrected; Channel A (API)</td>
<td>8</td>
</tr>

<tr class="alt">
<td>GRCSB</td>
<td>GRCSBG</td>
<td>GRCSBF</td>
<td>Sector 0-7</td>
<td>Corrected; Channel B (API)</td>
<td>8</td>
</tr>

<tr>
<td>GRCS</td>
<td>GRCSG</td>
<td>GRCSF</td>
<td>Sector 0-7</td>
<td>Corrected; Channels Normalized (API)</td>
<td>8</td>
</tr>

<tr class="alt">
<td>GRCU</td>
<td>GRCUG</td>
<td>GRCUF</td>
<td>Upper Quadrant</td>
<td>Corrected; Channels Normalized (API)</td>
<td>1</td>
</tr>

<tr>
<td>GRCD</td>
<td>GRCDG</td>
<td>GRCDF</td>
<td>Lower Quadrant</td>
<td>Corrected; Channels Normalized (API)</td>
<td>1</td>
</tr>

<tr class="alt">
<td>GRCL</td>
<td>GRCLG</td>
<td>GRCLF</td>
<td>Left Quadrant</td>
<td>Corrected; Channels Normalized (API)</td>
<td>1</td>
</tr>

<tr>
<td>GRCR</td>
<td>GRCRG</td>
<td>GRCRF</td>
<td>Right Quadrant</td>
<td>Corrected; Channels Normalized (API)</td>
<td>1</td>
</tr>

<tr class="alt">
<td colspan="6" style="text-align:right;">Total: 3 x 84 =252</td>
</tr>
</table>

#### 数据输出(Service Deliverables) ####

##### 实时应用程序(Real-time applications) #####

用户可以选择上下左右四个区域来决定实时数据的传输模式，这些数据可以曲线或图形的方式显示出来，用户可从中直接或间接地确定钻遇地层的视倾角和真倾角值(apparent and true dip)。

下图中给出了一个经典的地质导向案例，其中两条伽马曲线分别代表上下四分区所测得的数据，从这两条曲线的变化趋势可以看出钻头正穿过泥质砂岩进入到较为干净的地层中(exit from a shaly sand into a cleaner formation)。

<a target="_blank" href="https://lncvgg.blu.livefilestore.com/y2pca8rYW52s4O-_YktIVUPF6WK86WM1jLVGflhhINHhHecnyILKR9-YPQhmIZRsYxCFBGTjdpdE5MQMax8vcclsBYocg7S6XBXZ2A4iIKVqYo/WellpathCrossingaCleanerLayer.jpg?psid=1">
<img class="aligncenter" title="Wellpath crossing into a cleaner layer: First detection at low-side and approx. 5m later by the highside real-time gamma measurement" style="width:450px;height:300px;"
src="https://lncvgg.blu.livefilestore.com/y2pca8rYW52s4O-_YktIVUPF6WK86WM1jLVGflhhINHhHecnyILKR9-YPQhmIZRsYxCFBGTjdpdE5MQMax8vcclsBYocg7S6XBXZ2A4iIKVqYo/WellpathCrossingaCleanerLayer.jpg?psid=1" alt="Wellpath crossing into a cleaner layer: First detection at low-side and approx. 5m later by the highside real-time gamma measurement">

在能获取所有4个分区的伽马数据的情况下，也可以使用RigLink 2.4 U2软件(或更高版本的应用程序)绘制出实时的变化图，如下所示。

<a target="_blank" href="https://lncvgg.blu.livefilestore.com/y2p95dz2uN-4wr9OO8iPyl7gDbGh_1b5T7STNtNyu6HT_MORTRLQk0JvlarXyur95MVOxFtFr-2ZB_F2wSqeEe45UO33lZhkpItE2zEX1de-ww/RigLink.jpg?psid=1">
<img class="aligncenter" title="User configurable RigLink display screen illustrating 4 quadrant real-time gamma data as log curves in track 1 and as an image plot in track 5" style="width:580px;height:440px;" src="https://lncvgg.blu.livefilestore.com/y2p95dz2uN-4wr9OO8iPyl7gDbGh_1b5T7STNtNyu6HT_MORTRLQk0JvlarXyur95MVOxFtFr-2ZB_F2wSqeEe45UO33lZhkpItE2zEX1de-ww/RigLink.jpg?psid=1" alt="User configurable RigLink display screen illustrating 4 quadrant real-time gamma data as log curves in track 1 and as an image plot in track 5">

##### 后处理(Post processing) #####

高级伽马存储器中的数据经过MemProc处理后可以导出到ASCII格式或xtf格式的文件中。图形包Case可如下图那样绘制静态彩色图像(从xtf文件输入原始数据)。其中纵向与横向的内插值均可由用户自行定义。

<a target="_blank" href="https://lncvgg.blu.livefilestore.com/y2pdswWcGDd3MwHXSU2jXzRpBOhS_zYC0BG8kPwbLUW6LaG695wOqOmNlCOF7iwDhZVgKWFYBmf3qO8h7K8k4Hq0FsGi817i8ZWRWuznVzTPFM/SectoredGammaData.jpg?psid=1">
<img class="aligncenter" title="Sectored gamma data: Real-time transmitted data plotted as curves (track 1) or images (track 3) allow immediate geosteering decisions; high density memory data (track 2) for enhanced structural analysis" style="width:290px;height:490px;" src="https://lncvgg.blu.livefilestore.com/y2pdswWcGDd3MwHXSU2jXzRpBOhS_zYC0BG8kPwbLUW6LaG695wOqOmNlCOF7iwDhZVgKWFYBmf3qO8h7K8k4Hq0FsGi817i8ZWRWuznVzTPFM/SectoredGammaData.jpg?psid=1" alt="Sectored gamma data: Real-time transmitted data plotted as curves (track 1) or images (track 3) allow immediate geosteering decisions; high density memory data (track 2) for enhanced structural analysis">

##### 高级后处理(Advanced post processing) #####

根据用户需求，贝克阿特拉斯地质部(Baker Atlas GeoScience department)可以提供地质构造解释以及地层倾角等高级后处理功能。

<a target="_blank" href="https://lncvgg.blu.livefilestore.com/y2pwrEDtKhkv5QDU-RDtJoCdF7IdAx-uGsHgNQZTf6J2PHLRk0GU6flUQls-sXLQcFCizeaFwhIfgRSFSkyYnyqZ0PmKhPU0iy2Qh324Zc2n7I/AdvancedPostProcessing.jpg?psid=1">
<img class="aligncenter" title="Illustration of a structural analysis based on density data and created using the Spatial plotting package of Recall. Structural features are easier identifiable on the dynamically color scaled image (track 2) than on the static color scaled image in track 1. Track 3 illustrates the true dips picked from the image plotted as tadpoles" style="width:500px;height:560px;" src="https://lncvgg.blu.livefilestore.com/y2pwrEDtKhkv5QDU-RDtJoCdF7IdAx-uGsHgNQZTf6J2PHLRk0GU6flUQls-sXLQcFCizeaFwhIfgRSFSkyYnyqZ0PmKhPU0iy2Qh324Zc2n7I/AdvancedPostProcessing.jpg?psid=1" alt="Illustration of a structural analysis based on density data and created using the Spatial plotting package of Recall. Structural features are easier identifiable on the dynamically color scaled image (track 2) than on the static color scaled image in track 1. Track 3 illustrates the true dips picked from the image plotted as tadpoles">
