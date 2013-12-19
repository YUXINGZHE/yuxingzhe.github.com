---
layout: post
title: "OnTrak Sensor Sub Components/Services"
tags: [OnTrak, Sensor Sub]
author_name: YUXINGZHE
author_uri: http://twitter.com/yuxingzhe
---

<span class="dropcap">所</span>有的OnTrak传感器接头的电气结构都基本相似，只有4-3/4" OnTrak略有区别。下面的功能框图(OnTrak Communication Functional Block Diagram)显示了前面介绍的各控制模块，传感器和其他的电子模块(boards, sensors and other electronic elements)之间是如何进行通讯和连接的。

<a target="_blank" href="https://ldcvgg.blu.livefilestore.com/y2p7e9hv_Vx2j4HBa0o4KYhuM5aFEW5rGmPoGzTU8bPVhsVut8RIAdOG3axDce6jnG_3HnlgimsV3I3DDY7JM7EYS2gFL_Evh9Dv0GWaQ0oan0/OnTrakCFBD.png?psid=1">
<img class="aligncenter" title="OnTrak Communication Functional Block Diagram" style="width:600px;height:400px;" src="https://ldcvgg.blu.livefilestore.com/y2p7e9hv_Vx2j4HBa0o4KYhuM5aFEW5rGmPoGzTU8bPVhsVut8RIAdOG3axDce6jnG_3HnlgimsV3I3DDY7JM7EYS2gFL_Evh9Dv0GWaQ0oan0/OnTrakCFBD.png?psid=1" alt="OnTrak Communication Functional Block Diagram">

#### 主控/存储模块(Master/Memory) ####

主控/存储模块具有集中控制和数据存储两大功能，作为主控制模块它执行并控制着OnTrak接头内的各项任务。主控/存储模块中有8块存储器(Flash Memory IC)，总容量为32M，其中存储着各种数据信息，承担着OnTrak接头数据存储的任务。

<a target="_blank" href="https://ldcvgg.blu.livefilestore.com/y2psVJeIzB5gBHcg8Q5_0jPc5H00dMzdf7urpHNBdIK4WSVjafpjs27GLvKoZnk6lPfVHWaupsO16ZtsivzglrdabSQY-nzv-Tu2gXuxAeiS3U/OnTrakFBDMasterMemoryBoard.jpg?psid=1">
<img class="aligncenter" title="Functional Block Diagram OnTrak Master/Memory Board" style="width:600px;height:400px;" src="https://ldcvgg.blu.livefilestore.com/y2psVJeIzB5gBHcg8Q5_0jPc5H00dMzdf7urpHNBdIK4WSVjafpjs27GLvKoZnk6lPfVHWaupsO16ZtsivzglrdabSQY-nzv-Tu2gXuxAeiS3U/OnTrakFBDMasterMemoryBoard.jpg?psid=1" alt="Functional Block Diagram OnTrak Master/Memory Board">

从上面的功能框图(Functional Block Diagram OnTrak Master/Memory Board)可以看到，<u>I/O1039(Adam总线)主要负责OnTrak系统中各模块之间的内部通讯</u>，如主控/存储集成电路PCBA(Printed Circuit Board Assembly)，压力/伽马PCBA，多频传播电阻率(MPR)接收器PCBA，低压供电(LVPS)模块，及导向探头微控制器PCBA(Directional Sonde Microcontroller PCBA)等。高可靠性的<u>调制解调器(modem)</u>可以为内部数据通讯提供高达9600波特的传输速率。<u>实时时钟RTC(Real Time Clock)</u>电路为存储器中的每个传感器数据包都分配了一个时间戳。在泥浆停止循环的情况下，RTC电路改由备用电池供电以保证继续正常工作。

此外，<u>以太控制器(Ethernet Controller)</u>还能通过数据导出接口(Dump Port)在一分多钟时间里将32M数据全部转储出来。

#### 定向探头(Directional) ####

OnTrak定向探头的主要组件包括三个加速度计和三个磁通门传感器，核心驱动模块(core drivers)，定向微处理器(directional micro processor)，定向供电模块(directional power supply board)等。在探头两端分别有一个对中器，除了对中器(centralizers)以外，各种不同尺寸接头的定向探头结构都是一样的。上部对中器(upper centralizer)上有一个电源和通讯接口与钻铤相连。定向探头结构如下所示。

<a target="_blank" href="https://ldcvgg.blu.livefilestore.com/y2pQPK2dJYOxMA1o7XhHRzn8CcDup1s_KedGZvn2Q3q05VMvFoL6nxhXYPv30-GgRJ7zuorsIXs1Z5WKAdyUmNksFbo_u7CUnIUvl_fqhmbHU4/DirectionalSonde.png?psid=1">
<img class="aligncenter" title="Directional Sonde" style="width:500px;height:300px;" src="https://ldcvgg.blu.livefilestore.com/y2pQPK2dJYOxMA1o7XhHRzn8CcDup1s_KedGZvn2Q3q05VMvFoL6nxhXYPv30-GgRJ7zuorsIXs1Z5WKAdyUmNksFbo_u7CUnIUvl_fqhmbHU4/DirectionalSonde.png?psid=1" alt="Directional Sonde">


由于M33总线需要穿过定向探头将来自BCPM的电力供应给OnTrak以及OnTrak下部的其他接头(如导向模块)，因此，在将来自加速度计，磁通门传感器，温度传感器的模拟信号以及M33总线的电流信号数字化后，还需要考虑温度、增益、信号补偿、信号失调和信号畸变的影响对上述测量信号进行校正。M33总线中的电流信号经测量，放大后转换成差分模拟电压(a differential analog voltage)；所测得的的电流信号可以用于磁通门传感器的误差校正(磁通门传感器读数会受到M33总线中电流的干扰)。

下表给出了计算导向钻井过程中各参数所需要的测量数据。

<table id="customers" align="center">
<caption>表1 定向参数计算所需测量数据</caption>
<tr>
<th>定向参数</th>
<th>测量数据</th>
</tr>

<tr>
<td>井斜</td>
<td>Gx, Gy, Gz</td>
</tr>

<tr class="alt">
<td>方位</td>
<td>Gx, Gy, Gz, Hx, Hy, Hz</td>
</tr>

<tr>
<td>磁工具面</td>
<td>Gx, Gy, Hx, Hy, Hz</td>
</tr>

<tr class="alt">
<td>重力工具面</td>
<td>Gx, Gy</td>
</tr>

<tr>
<td>磁倾角</td>
<td>Gx, Gy, Gz, Hx, Hy, Hz</td>
</tr>

<tr class="alt">
<td>总磁场强度</td>
<td>Hx, Hy, Hz</td>
</tr>

<tr>
<td>轴向磁场强度</td>
<td>Hz</td>
</tr>

<tr class="alt">
<td>旋转井斜(Rotating Inclination)</td>
<td>Gz</td>
</tr>

<tr>
<td>旋转方位(Rotating Azimuth)</td>
<td>Gx, Gy, Gz, Hx, Hy, Hz</td>
</tr>
</table>

>注意：OnTrak定向测井为动态测井方式(a Flow on survey)！

定向系统在已有技术的基础上，通过改进硬件和软件系统提升了近20%的定向测量精度。与前期产品相比，方位测量的精度更是提升了50%。

<table id="customers" align="center" style="width:90%;">
<caption>表2 定向测量范围和精度</caption>
<tr>
<th>定向参数</th>
<th>测量范围</th>
<th>测量精度(低于150℃)</th>
<th>测量精度(高于150℃)</th>
</tr>

<tr>
<td>井斜，探头(Inclination, Probe)</td>
<td>0°- 180°</td>
<td>±0.075°</td>
<td>±0.075°</td>
</tr>

<tr class="alt">
<td>井斜，系统(Inclination, System)</td>
<td>0°- 180°</td>
<td>±0.1°</td>
<td>±0.1°</td>
</tr>

<tr>
<td>方位，探头(Inclination, Probe)</td>
<td>0°- 360°</td>
<td>±0.6°</td>
<td>±0.6°</td>
</tr>

<tr class="alt">
<td>方位，系统(Inclination, System)</td>
<td>0°- 360°</td>
<td>±1.0°</td>
<td>±1.0°</td>
</tr>

<tr>
<td>旋转方位(Azimuth Rotating)</td>
<td>0°- 360°</td>
<td>TBD(To Be Determined)</td>
<td>TBD</td>
</tr>

<tr class="alt">
<td>参考工具面(磁)</td>
<td>0°- 360°</td>
<td>±1.5°</td>
<td>±1.5°</td>
</tr>

<tr>
<td>参考工具面(重力)</td>
<td>0°- 360°</td>
<td>±1.5°</td>
<td>±1.5°</td>
</tr>

<tr class="alt">
<td>总磁场强度</td>
<td>0-100000 gamma</td>
<td>±100</td>
<td>±100</td>
</tr>

<tr>
<td>磁倾角</td>
<td>-90°- 90°</td>
<td>±0.2°</td>
<td>±0.2°</td>
</tr>

<tr class="alt">
<td>重力场强度</td>
<td>0 - 4000 mG</td>
<td>±2.0</td>
<td>±2.0</td>
</tr>
</table>

#### 振动与粘滑(VSS) ####

定向探头还负责OnTrak中振动和粘滑的计算。定向探头首先计算出G_RMS中发生的振动，然后根据振动级别参考表(vibration criteria reference chart)对计算值进行评级。为了计算OnTrak的粘滑值，需要分别在最低，最高和平均转速工况下对OnTrak接头进行测试，然后计算出S1和S2值，这样就可以确定出OnTrak的粘滑等级。(In order to determine stick slip data a minimum, maximum and average RPM is calculated. With the calculation of S1 and S2 values the stick slip severity level is determined.)

<table id="customers" align="center">
<caption>表3 振动测量范围，精度与分辨率</caption>
<tr>
<th>测试参数</th>
<th>范围</th>
<th>精度</th>
<th>分辨率</th>
</tr>

<tr>
<td>侧向(X&Y)振动</td>
<td>-10G - 10G</td>
<td>±15%</td>
<td>24 mG</td>
</tr>

<tr class="alt">
<td>轴向(Z)振动</td>
<td>-10G - 10G</td>
<td>±15%</td>
<td>24 mG</td>
</tr>
</table>

#### 电阻率 ####

OnTrak平台使用了在MPR & USMPR接头中得到成功应用的多频传播电阻率(MPR)技术，它采用了补偿式两频谱(2 MHz & 400 KHz)四发射器两接收器结构，总共能够提供8个定量的电阻率数据。<u>每个发射器开启0.625s，使得MPR每5s更新一次。</u>其数字电路设计与USMPR接头相同，发射器和接收器PCBA均为Q-Pack设计，安装在双层盖板下方。

<a target="_blank" href="https://ldcvgg.blu.livefilestore.com/y2ple1RqVFsMv54UPogFgoGkvcz2ZmzN1Nvc8tEpz8P88qOkw3Bu4DJvbP1K9H3ftwTGKFZTCGIV6_1XFiRIcTTA4wKyIolu3w8bEubVtrtZwo/OnTrakAntenna.png?psid=1">
<img class="aligncenter" title="OnTrak Antenna Spacing" style="width:700px;height:200px;" src="https://ldcvgg.blu.livefilestore.com/y2ple1RqVFsMv54UPogFgoGkvcz2ZmzN1Nvc8tEpz8P88qOkw3Bu4DJvbP1K9H3ftwTGKFZTCGIV6_1XFiRIcTTA4wKyIolu3w8bEubVtrtZwo/OnTrakAntenna.png?psid=1" alt="OnTrak Antenna Spacing">

新型天线技术(采用单绕式而非双绕式)降低了系统噪音，并消除了接收器间的串扰，从而使得电阻率的测量精度提高了15%。

#### 伽马 ####

OnTrak伽马包将晶体(Crystal)，光电倍增管PMT(Photo-Multiplier Tube)，前置放大器(Pre-amp)及高压供电HVPS(High Voltage Power Supply)子模块都集成到了一起，这样减少了各模块之间的连接部件，提高了接头的可靠性。这种设计还降低了Crystal/PMT发生分离和失调的风险(de-bonding and alignment problems)。两个伽马传感器分别被安装在两个盖板下，相互隔开180°，这样可以同时使用这两个传感器进行双伽马测量。<u>向井下看去，1号伽马传感器在划片槽左边90°的地方。</u>

HVPS的输出由压力/伽马PCBA控制。

在100 API，60ft/hr (ROP)和1ft地层厚度(1 ft sample)的情况下，自然伽马的测量精度为±2.5 API。这比目前使用的其他传感器接头说明书中所标示的精度提高了17%。

>注意：在4-3/4" OnTrak中HVPS从Crystal，PMT和Pre-amp中分离了出来。

#### 压力 ####

井眼和环空压力传感器与电阻温度装置RTD(Resistance Temperature Device)一起安装在同一个盖板下，这个盖板可以在现场进行更换，先卸下盖板上的8个螺钉后更换盖板，然后把每个螺钉用50 ft-lbs的力矩打紧。需要注意的是，当每次更换新的盖板后，都需要将其标定系数(calibration coefficients)重新输入到压力/伽马PCBA(P/G PCBA)当中。

当停止循环泥浆时(此时接头内的交流发电机不工作)，P/G PCBA与压力传感器由电池驱动，此时静压(井眼及环空压力)每2s记录一次。

<a target="_blank" href="https://ldcvgg.blu.livefilestore.com/y2pMT_CEniUVmwQoVLB6hhyYU8WuegdVYuBgOve7sq5uIQPbnkehMv02RieY3F_TZMYSFbig6VLNJL1_RJ6F0EFcQ6WohA-BUsd_9ojo1enaQk/PressureGammaHatchCover.png?psid=1">
<img class="aligncenter" title="Pressure Gamma Hatch Cover" style="width:700px;height:220px;" src="https://ldcvgg.blu.livefilestore.com/y2pMT_CEniUVmwQoVLB6hhyYU8WuegdVYuBgOve7sq5uIQPbnkehMv02RieY3F_TZMYSFbig6VLNJL1_RJ6F0EFcQ6WohA-BUsd_9ojo1enaQk/PressureGammaHatchCover.png?psid=1" alt="Pressure Gamma Hatch Cover">

<table id="customers" align="center">
<caption>表4 压力传感器测量范围，精度与分辨率</caption>
<tr>
<th>测试参数</th>
<th>范围</th>
<th>精度</th>
<th>分辨率</th>
</tr>

<tr>
<td>井眼压力</td>
<td>0-25,000 psi</td>
<td>±0.25% FS (62.5 psi)</td>
<td>5psi</td>
</tr>

<tr class="alt">
<td>环空压力</td>
<td>0-25,000 psi</td>
<td>±0.25% FS (62.5 psi)</td>
<td>5psi</td>
</tr>

<tr>
<td>温度</td>
<td>0 - 200°C</td>
<td>±1.0°C</td>
<td>0.5°C</td>
</tr>
</table>

#### 电池 ####

<a target="_blank" href="https://ldcvgg.blu.livefilestore.com/y2pU0TNvx8j5cRIJe21k3z6CXYwhNSqQhjpRsZVzUtUwyfl__ldIaxD8iVKUuOSlj2OCSNN_KlYNfREI_vKe30yt2ANFQ7OwpX79BUp3uvAc0I/BatteryHatchCover.png?psid=1">
<img class="aligncenter" title="Battery Hatch Cover" style="width:650px;height:150px;" src="https://ldcvgg.blu.livefilestore.com/y2pU0TNvx8j5cRIJe21k3z6CXYwhNSqQhjpRsZVzUtUwyfl__ldIaxD8iVKUuOSlj2OCSNN_KlYNfREI_vKe30yt2ANFQ7OwpX79BUp3uvAc0I/BatteryHatchCover.png?psid=1" alt="Battery Hatch Cover">

电池盖板中有一块双C系列氯化锂/亚硫酰二氯电池(MR型，不会发生膨胀)，该电池长约103mm，直径为21mm。安装完成后，可以为P/G PCBA提供7.34V的交流电。电池盖板可根据需要在钻台现场进行更换。

当停止循环泥浆时，电池将为P/G PCBA供电以测量井眼与环空中的压力。

>注意：当停止循环泥浆时，OnTrak只测量井眼和环空的压力，不提供测井和伽马测量功能。

##### 电池寿命 #####

在停止循环泥浆的状态下，对于常规的压力/伽马控制模块(10068121，conventional Pressure Gamma board)，电池的寿命为38-50h(2005年9月前所使用的电池寿命为72h)。

在停止循环泥浆的状态下，对于高级伽马压力/伽马控制模块(10068121，Gamma Elite Pressure Gamma boards)，电池的寿命为175-180h。由于电路有所差异，它们需要的电流要更小。

#### 接头通讯接口(数据导出接口)(Tool Communications Port, Data Dump Port) ####

<a target="_blank" href="https://ldcvgg.blu.livefilestore.com/y2pwngfAOP6CGYbJ9Vt0nhHPUSC3uKsRleC9a8YgCsHwyIUlSFcxrffrw4e3bfxmO_QybKZiKd53jUzbwYlNFersCqRcy5PArvVgVUEv7GBT-U/DataDumpPort.png?psid=1">
<img class="aligncenter" title="Data Dump Port / Read out Port" style="width:550px;height:200px;" src="https://ldcvgg.blu.livefilestore.com/y2pwngfAOP6CGYbJ9Vt0nhHPUSC3uKsRleC9a8YgCsHwyIUlSFcxrffrw4e3bfxmO_QybKZiKd53jUzbwYlNFersCqRcy5PArvVgVUEv7GBT-U/DataDumpPort.png?psid=1" alt="Data Dump Port / Read out Port">

这个接口允许用户进行数据导出，与接头进行通讯，并可利用接头通讯系统TCS(Tool Communication System)对接头进行诊断。

接口使用TXD & RXD线与以太系统进行通讯(Ethernet Communications，TP拓扑网络采用双绞线进行通讯，两根用于差分发送，两根用于差分接收)。

或者，也可以通过M33或I/O1039总线进行通讯。

#### OnTrak锥形滑套扶正器(TSS) ####

OnTrak TSS可以保护OnTrak传感器接头，尤其是电阻率天线在钻遇较硬研磨性地层时免受磨损和拉伤伤害。由于它只是起到防磨的作用，因此TSS比其他正规的井下扶正器的尺寸要小得多。TSS扶正器外径尺寸如下(适用于各种井眼)：

<ul style="margin-left:50px;">
<li>6-3/4" OnTrak传感器接头 8-1/4" OD</li>
<li>8-1/4" OnTrak传感器接头 10-5/8" OD</li>
<li>9-1/2" OnTrak传感器接头 11-1/2" OD</li></ul>

在TSS上有一个卡瓦和螺钉，卡瓦处外径较小，处于上部发射器的上方。当扶正器受到扭曲(torqued)时，锥形化的外形使得在扶正器上产生一个径向的力矩，这个力矩使得卡瓦越来越紧，从而维持住扶正器的位置保持不变。这是一种全新的设计方式，与泥浆马达的挤入式扶正器的设计理念截然不同。

第一次安装TSS时需要对传感器接头进行微小的加工，因此在安装TSS时需要事先进行详细的计算。R&M手册“TSS拆装”(文件编号：COMMON-10-0702-001)部分有关于TSS的更加详细的信息。该手册可通过TechPubs搜索得到。

<a target="_blank" href="https://ldcvgg.blu.livefilestore.com/y2pmvZrwSR_OeuqEnO2YRoYuWHQ28UtXHhdEbT58TuxyKU7kvlyhDg_TOLImMxjod45f-WRl-TsaQ2JYglv8QzkdV8_Y90exTjA0ihH94UNEkM/OnTrakTaperedSleeveStabilizer.png?psid=1">
<img class="aligncenter" title="Ontrak Tapered Sleeve Stabilizer" style="width:700px;height:170px;" src="https://ldcvgg.blu.livefilestore.com/y2pmvZrwSR_OeuqEnO2YRoYuWHQ28UtXHhdEbT58TuxyKU7kvlyhDg_TOLImMxjod45f-WRl-TsaQ2JYglv8QzkdV8_Y90exTjA0ihH94UNEkM/OnTrakTaperedSleeveStabilizer.png?psid=1" alt="Ontrak Tapered Sleeve Stabilizer">
