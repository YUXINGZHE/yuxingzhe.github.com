---
layout: post
title: "Operation of Bypass System"
tags: [OnTrak, Suyface System]
author_name: YUXINGZHE
author_uri: http://twitter.com/yuxingzhe
---

    本部分对旁路系统的组件以及相关操作等内容做了简要介绍，关于旁路系统的安装过程请参见[Bypass System Rigup](./_posts/2013/2013-12-20-Bypass-System-Rigup/index.html)

<span class="dropcap">M</span>WD地面系统Advantage与一套额外的旁路工具包(bypass kit)连接后，可以与井下工具进行通讯从而对AutoTrak实施操作。

<a target="_blank" href="https://kndlaw.blu.livefilestore.com/y2p2GNRN8gI3Yc9QK_OM9ur4Q4yvu1evkvcauzrsNcpaw3LXbF1VatARxyIaoTlPG5kiV4-DBKWn2fWb2F1-3DeNQe_1gf0BDZrlOwUrzuc_gw/Schematic%20Closed%20Loop%20Communication.png?psid=1">
<img class="aligncenter" title="Schematic Closed Loop Communication" style="width:500px;height:360px;" src="https://kndlaw.blu.livefilestore.com/y2p2GNRN8gI3Yc9QK_OM9ur4Q4yvu1evkvcauzrsNcpaw3LXbF1VatARxyIaoTlPG5kiV4-DBKWn2fWb2F1-3DeNQe_1gf0BDZrlOwUrzuc_gw/Schematic%20Closed%20Loop%20Communication.png?psid=1" alt="Schematic Closed Loop Communication"></a>

地面系统可以远程操控旁路系统来调节泥浆的循环流量，从而实现井下通讯。以下将对系统中各组件进行介绍。

> ##### 旁路系统安全规范 #####
>
>旁路系统与井架上的高压管汇相连，因此所有操作人员以及系统安装人员均应严格遵守以下安全操作规范。
>
> <ul style="margin-left:50px;">
><li>柔性软管(Flexible hoses)只能用于将低压回流泥浆引入到泥浆循环系统中，禁止安装在旁路执行器BPA(Bypass Actuator)或可调旁路执行器ABPA(Adjustable BPA)的入口处。</li>
><li>高压系统上的所有连接设备均应具有产品合格证书，并对其进行仔细检查以保证满足最高工作压力条件。严禁使用压力等级不明的设备。</li>
><li>未获井架工(rig operators)或相关负责人的许可，禁止在泥浆系统上连接设备。</li>
><li>与井架连接的所有设备均应具有产品测试与维护合格证书。在使用前现场人员应对设备表面进行检查，如发现任何问题，应及时提出。</li>
><li>系统连接完成后，在工作中需定期对旁路执行器及连接管路进行检查。</li></ul>

#### 旁路控制盒(Bypass Controller) ####

旁路系统通过旁路控制盒BPC(Bypass Controller Box)发出的电信号进行控制。BPC将来自Advantage或4×4键盘控制面板的指令进行编码后传送给BPA电磁阀转换成阀门的开关信号，然后将参数指令传送到井下AutoTrak工具中。阀门的每次开关动作都被称作一次"阀门启动(a valve actuation)"。

<a target="_blank" href="https://kndlaw.blu.livefilestore.com/y2pV5VFZS9rKP43DR_RC-cj7W4ISYMgRe8UoOgq2TtqUMppL4nv4EAZyj4LQznviiVgWz9XZEICVRCRq4bZEk5LR-ssV0RIHmGzIyUxlIehJc8/BPC%20Front%20and%20Back%20Panels.png?psid=1">
<img class="aligncenter" title="BPC Front and Back Panels" style="width:360px;height:240px;" src="https://kndlaw.blu.livefilestore.com/y2pV5VFZS9rKP43DR_RC-cj7W4ISYMgRe8UoOgq2TtqUMppL4nv4EAZyj4LQznviiVgWz9XZEICVRCRq4bZEk5LR-ssV0RIHmGzIyUxlIehJc8/BPC%20Front%20and%20Back%20Panels.png?psid=1" alt="BPC Front and Back Panels"></a>

旁路控制盒操作面板上有一个电源开关(power switch)，三个供电LED指示灯，一个电磁阀驱动红绿LED指示灯(red/green solenoid driver LED)，以及一个LCD显示屏(旁边还有一个复位按钮，但并不是在所有旁路控制盒上都有)。如果旁路控制盒工作异常，可尝试重新接通电源。此外，在供电面板上还有三个用于调节输出电压的微调按钮(trim pots)，但谨记绝对严禁使用这些微调按钮对电压进行调节，如有疑问，请直接更换新的电源。接通电源后，面板上的三个LED指示灯都会被点亮，如果有一个LED指示灯没有反应，那么需要更换新的电源。如果旁路控制盒启动正常，那么在LCD显示屏上将可以看到以下信息：

<b style="margin:50px;">Bypass Controllor Version 4.00</b>

几秒钟之后会变为：

<b style="margin:50px;">Ready 0 0</b>

此时旁路控制盒就可以正常工作了。

只有当发送信号时，电磁阀驱动LED指示灯才会被点亮。当有信号输出时，电磁阀驱动LED指示灯将变成绿色，如果指示灯显示为红色，那么很可能是控制盒与旁路执行器电磁阀之间的连接出现了故障。检查好电线及连接处后可尝试重新发送信号进行测试。

正常情况下旁路控制盒不需要进行任何维护工作，如果出现了故障，直接进行整体更换。如果电磁阀驱动模块无法工作，在将控制盒发回给我们之前请先拆下驱动模块并仔细检查保险丝(fuse)是否熔断(驱动模块的拆装步骤如下)。在更换熔断保险丝(blown fuses)前，请对新的保险丝的产品等级进行仔细检查。禁止使用电流承受能力为315mA(fast response，快速反应型)以外的其他等级的保险丝。电源与电磁阀驱动模块的更换步骤如下：

<ol style="margin-left:50px;">
<li>关闭旁路控制盒电源并将其与主供电电源断开连接；</li>
<li>使用合适的工具将所有支撑电磁阀驱动模块(2个)和电源(4个)的连接螺丝松开；</li>
<li>在将所有连接螺丝取下后，慢慢地将驱动模块和电源从盒子中取出来。由于电磁阀驱动模块没有外壳进行保护，因此在取出时请特别小心；</li>
<li>插入新的模块；</li>
<li>拧紧螺丝；</li>
<li>重新与主供电电源连接。打开旁路控制盒电源并检查启动信息是否正常。</li></ol>

##### 旁路控制盒(BPC)操作手册 #####

如需手动输入下行指令，请按菜单键(M)，此时LCD显示屏将显示：

<b style="margin:50px;">Enter Pulse Length</b>

请使用左右方向键来设定脉冲长度(8,12或16)，然后按下Enter键。

请使用左右方向键来选择所需的指令，在选择好指令后请按下Enter键，此时系统将提示输入与该指令相关的参数值。不同参数的输入方式不同，方位与井斜需要手动输入，而其他的参数可以通过左右方向键来直接进行选择。输入正确的参数后，按下Enter键(如果需要输入两个参数，请按上述步骤输入一个参数值后点击return按钮)。此时LCD显示屏将会显示：

<b style="margin:50px;">Transmit Yed/No</b>

如确认发送下行指令，请选中"yes"并按下Enter键。你也可以点击取消按钮"C"来取消发送。此时LCD显示屏将会显示：

<b style="margin:50px;">Abort Transmission Yes/No</b>

选中"yes"并按下Enter键。

>注意：现行使用的BCPM硬件只支持8s的脉冲长度。

#### 旁路执行器(Bypass Actuator, BPA) ####

下行信号控制器DLC(Downlink Controller)可通过地面系统对泥浆流量进行编码然后向下传输信号。为此，我们需要在立管上安装一个旁路执行器(BPA)阀将多余的泥浆导回到泥浆循环系统中。下页的旁路执行器为现在使用的两种型号之一。执行器可通过电磁阀控制空气马达驱动一个菱形阀芯(a diamond disc)旋转90°，此外还有另外一个阀芯正对着第一个阀芯安装在执行器阀体内，两个阀芯上各有一个小孔，当第一个阀芯旋转90°时，两个小孔连成一条直线，这样泥浆就可以从执行器阀内流出。(The actuator uses a solenoid controlled air motor capable of rotating a diamond disc through 90°. This disc has two holes in it, as does a second disc mounted hard up against the first. In the closed position, the holes lie at 90° to each other, however, when the first disc is rotated 90°, the holes line up and allow flow to pass from the standpipe to the outlet.)

>注意：规范规定在4-3/4"/6-3/4"工具中，BPA中所使用的三通在旁路执行器阀门连续工作3小时或者开关1000次以后必须进行更换，在8-1/2"/9-1/2"工具中，BPA中所使用的三通在旁路执行器阀门连续工作1.5小时或者开关500次后必须进行一次更换(请参考下述步骤)。对于6-3/4" ATK，BPA在连续开启工作不超过6小时后需进行一次维护；对于8-1/4" ATK，BPA在连续开启工作不超过3小时后需进行一次维护。具体要求请参考文件TA AT01/022/EB。请注意三通的维护可能还需要满足当地的特殊安全规范，例如，挪威船级社DNV规定由于现场压力测试数据不可靠，在英国BPA上所使用的三通不允许在井架现场进行更换。

<a target="_blank" href="https://kndlaw.blu.livefilestore.com/y2pDig5mfrksx3egijB-4hmXLA58QnJu8A5CsNSCVH482iaKC5MUIhx9m1GrCyYNga6QrBUeIey8I0Zl1XfdyeLO4L5Yu9di0mWtwaKO7r32Lg/Schematic%20Drawing%20of%20the%20Bypass%20System%20(BSS).png?psid=1">
<img class="aligncenter" title="Schematic Drawing of the Bypass System (BSS)" style="width:470px;height:200px;" src="https://kndlaw.blu.livefilestore.com/y2pDig5mfrksx3egijB-4hmXLA58QnJu8A5CsNSCVH482iaKC5MUIhx9m1GrCyYNga6QrBUeIey8I0Zl1XfdyeLO4L5Yu9di0mWtwaKO7r32Lg/Schematic%20Drawing%20of%20the%20Bypass%20System%20(BSS).png?psid=1" alt="Schematic Drawing of the Bypass System (BSS)"></a>

旁路系统将在整体组装完毕后或放在铁篮(basket)内被运送到钻井现场，**作为系统部件铁篮内任一组件发生故障，就需要更换一套全新的盘路系统**。同样地，如果铁篮内的组件满足不了安全使用要求，那么也必须更换一套新的旁路系统。

一体化铁篮有两种型式。如下图所示，左边为可调式旁路执行器系统ABPA(Adjustable Bypass Actuator)，右边则为装配了可调式喷嘴ANU(Adjustable Nozzle Unit)的旁路执行器系统BPA(Bypass Actuator)。

<a target="_blank" href="https://kndlaw.blu.livefilestore.com/y2pLGbHF10YLffYhYyf0VN5pl73L83Iu9lFzaXK6F5b0faa_NDlSn7YrT-0XOKMMCq63EoherbMcc0qem7XXZGD5SXgRCDDKS8QRsOsvtYTf9k/ABPA%20(left)%20and%20BPA%20(right).jpg?psid=1">
<img class="aligncenter" title="ABPA (left) and BPA (right)" style="width:360px;height:240px;" src="https://kndlaw.blu.livefilestore.com/y2pLGbHF10YLffYhYyf0VN5pl73L83Iu9lFzaXK6F5b0faa_NDlSn7YrT-0XOKMMCq63EoherbMcc0qem7XXZGD5SXgRCDDKS8QRsOsvtYTf9k/ABPA%20(left)%20and%20BPA%20(right).jpg?psid=1" alt="ABPA (left) and BPA (right)"></a>

#### 标准BPA铁篮(Standard BPA Basket) ####

标准BPA铁篮的规格如下：

<table id="customers" align="center" style="width:85%;">
<caption><b>表1</b> BPA规格</caption>
<tr class="alt">
<td><b>重量</b></td>
<td>400Kg (900lbs)</td>
</tr>

<tr>
<td><b>尺寸</b></td>
<td>1.6m × 0.6m × 0.9m / 5.2ft × 2ft × 3ft</td>
</tr>

<tr class="alt">
<td><b>最大立管承压(Maximum Standpipe Pressure)</b></td>
<td>500bar (7100psi)</td>
</tr>

<tr>
<td><b>气源</b></td>
<td>6.2-9bar @ 630l/min / 90-130psi @ 166gpm</td>
</tr>

<tr class="alt">
<td><b>高压油壬连接方式</b></td>
<td>高压输入管汇: 2" Fig 1502 Box / 低压输出管汇: 2" Fig 1502 Pin</td>
</tr>

<tr>
<td><b>合格证</b></td>
<td>挪威船级社（DNV）型式认可证书（TAC）No.D-2518，并满足美国工程师协会（ASME）锅炉与压力容器规范（Section VIII. Div. 2. 1995）</td>
</tr>
</table>

<a target="_blank" href="https://kndlaw.blu.livefilestore.com/y2pkD7uk69LH7MTue9uX3dfcqCKvs7hhsmU2OJAef7nHeiUMFQthqmcsF6a3qmOKyNAbSCYm-kDvtXMtSuACOQbyV415kOuQzQkvfECa-7nP90/Bypass%20Actuator%20(BPA).jpg?psid=1">
<img class="aligncenter" title="Bypass Actuator (BPA)" style="width:470px;height:290px;" src="https://kndlaw.blu.livefilestore.com/y2pkD7uk69LH7MTue9uX3dfcqCKvs7hhsmU2OJAef7nHeiUMFQthqmcsF6a3qmOKyNAbSCYm-kDvtXMtSuACOQbyV415kOuQzQkvfECa-7nP90/Bypass%20Actuator%20(BPA).jpg?psid=1" alt="Bypass Actuator (BPA)"></a>

安装好旁路系统后，请现场有经验的井架工人对安装情况进行仔细检查。

#### 可调式BPA系统(ABPA, Adjustable BPA Unit) ####

ABPA通过一个横置活塞来旋转伸入到阀体内的阀杆。转动手轮可以调节气动活塞的止动范围，从而能够精确控制菱形阀芯的旋转圈数。将执行器阀与喷嘴安装在一起可以精确控制两个阀芯的重合开度，调节步骤如下：

<ol style="margin-left:50px;">
<li>在ABPA初次启用时，气动活塞的调节手轮是被锁死的，使用时必须首先进行解锁并活动手轮。也可以在调节气动活塞时活动手轮以免手轮卡死。</li>

<a target="_blank" href="https://kndlaw.blu.livefilestore.com/y2pKh89zNdNfhuSaXjsIEWM6QGxq4D2WZdJqd_QMU1OMLUw3JOhpZC4TcknS9AvWKSWIiKwDwHzVmGlc9Kh2rkcZ1l5IghvqhANud-n2xfkAE0/Schematic%20Drawing%20of%20the%20ABPA%20Bypass%20System.png?psid=1">
<img class="aligncenter" title="Schematic Drawing of the ABPA Bypass System" style="width:460px;height:250px;" src="https://kndlaw.blu.livefilestore.com/y2pKh89zNdNfhuSaXjsIEWM6QGxq4D2WZdJqd_QMU1OMLUw3JOhpZC4TcknS9AvWKSWIiKwDwHzVmGlc9Kh2rkcZ1l5IghvqhANud-n2xfkAE0/Schematic%20Drawing%20of%20the%20ABPA%20Bypass%20System.png?psid=1" alt="Schematic Drawing of the ABPA Bypass System"></a>

<li>启动时将手轮逆时针旋转到底，阀杆将转动90°，此时可得到最大总过流面积(TFA)为22.0/33"；启动时将手轮顺时针转动到底，阀杆将转动30°，此时可得到最小总过流面积(TFA)为7.4/33"。</li></ol>

>注意：下行数据传输过程中不允许调整总过流面积(TFA)。

<table id="customers" align="center" style="width:85%;">
<caption><b>表2</b> ABPA规格</caption>
<tr class="alt">
<td><b>重量</b></td>
<td>200Kg (450lbs)</td>
</tr>

<tr>
<td><b>尺寸</b></td>
<td>1.5m × 0.88m × 0.43m / 5ft × 2.9ft × 1.4ft</td>
</tr>

<tr class="alt">
<td><b>最大立管承压(Maximum Standpipe Pressure)</b></td>
<td>500bar (7100psi)</td>
</tr>

<tr>
<td><b>气源</b></td>
<td>6.2-9bar @ 630l/min / 90-130psi @ 166gpm</td>
</tr>

<tr class="alt">
<td><b>高压油壬连接方式</b></td>
<td>高压输入管汇: 2" Fig 1502 Box / 低压输出管汇: 2" Fig 1502 Pin</td>
</tr>

<tr>
<td><b>合格证</b></td>
<td>挪威船级社（DNV）型式认可证书（TAC）No.D-2518，并满足美国工程师协会（ASME）锅炉与压力容器规范（Section VIII. Div. 2. 1995）</td>
</tr>
</table>

<a target="_blank" href="https://kndlaw.blu.livefilestore.com/y2pgHiVECP9MAvfC4iOJWxBaJCjHpGYHMrZxj5KdcjBXGbW6QE97ouuA-rz7XE2VLbsAu3Olg9iUqs7hEzJ5nJndYiMLtTinUbyz7YWYTs-5Kw/Adjustable%20Bypass%20Actuator%20(ABPA).jpg?psid=1">
<img class="aligncenter" title="Adjustable Bypass Actuator (ABPA)" style="width:500px;height:400px;" src="https://kndlaw.blu.livefilestore.com/y2pgHiVECP9MAvfC4iOJWxBaJCjHpGYHMrZxj5KdcjBXGbW6QE97ouuA-rz7XE2VLbsAu3Olg9iUqs7hEzJ5nJndYiMLtTinUbyz7YWYTs-5Kw/Adjustable%20Bypass%20Actuator%20(ABPA).jpg?psid=1" alt="Adjustable Bypass Actuator (ABPA)"></a>

在阀杆上从30°到90°每隔15°都标记有相应的刻度线，与阀体旋转角度相对应的喷嘴尺寸如下表所示。

<table id="customers" align="center">
<caption><b>表3</b> 阀体旋转角度与等价喷嘴尺寸转换表</caption>
<tr class="alt">
<td><b>阀体旋转角度</b></td>
<td>deg</td>
<td>30</td>
<td>40</td>
<td>50</td>
<td>60</td>
<td>70</td>
<td>80</td>
<td>90</td>
</tr>

<tr>
<td><b>等价喷嘴尺寸</b></td>
<td>/32"</td>
<td>7.4</td>
<td>11.1</td>
<td>13.9</td>
<td>16.3</td>
<td>18.4</td>
<td>20.2</td>
<td>22.0</td>
</tr>
</table>

当把ABPA安装到井架上后，将很难从阀杆上观察到阀体的旋转角度刻度线，因此设计了另外一套方法来识别总过流面积(TFA)。将阀杆从30°转到90°的过程中手轮需要转过的圈数为±26圈，由此可知手轮每转动一圈阀杆转动2.2°。下图给出了阀杆从30°位置逆时针转动时手轮转动圈数与喷嘴尺寸间的等价关系曲线。

>注意：谨记在需要调整TFA时，应先将手轮顺时针旋转到底，然后再逆时针旋转一定圈数直到所需要的角度为止。阀杆上的刻度线并不一定准确。

<a target="_blank" href="https://kndlaw.blu.livefilestore.com/y2p5rgx3U2qB2zWIouezMY1dIdTNpontRO8bm20a5NWfX1P4rjm8xd446tB0qvOgP55ANJ32XZS_g_aSYqAgi-or-3ADJnBT2oFn0gaZ63cL1o/ABPA%20Setting%20Chart.png?psid=1">
<img class="aligncenter" title="ABPA Setting Chart" style="width:490px;height:320px;" src="https://kndlaw.blu.livefilestore.com/y2p5rgx3U2qB2zWIouezMY1dIdTNpontRO8bm20a5NWfX1P4rjm8xd446tB0qvOgP55ANJ32XZS_g_aSYqAgi-or-3ADJnBT2oFn0gaZ63cL1o/ABPA%20Setting%20Chart.png?psid=1" alt="ABPA Setting Chart"></a>

##### 将TFA设置为14/32"的操作步骤 #####

<ol style="margin-left:50px;">
<li>从上图可以看出，14/32"的TFA对应手轮从30°位置逆时针旋转9圈。</li>
<li>松开手轮的锁紧螺钉(hand-wheel clamp screw)，将手柄调整到合适的操作位置。</li>
<li>顺时针旋转手轮直到旋转不动为止，此时即为30°位置。如果可以请检查阀杆上的刻度线观察是否一致。</li>
<li>逆时针旋转手轮9圈，将TFA设定为14/32"。</li>
<li>调整调节手柄并将其沿着执行器放置。拧紧锁紧螺钉的防松螺母，它在执行器正常工作时可以起到锁紧误操作的作用。</li></ol>

##### ABPA启动设置建议(Suggested ABPA Starting Settings) #####

下表列出了不同尺寸工具下ABPA的初始手轮位置设置。如果下行信号传输失败，那么需要根据具体尺寸工具的具体反应进行调节(开或关)。

请注意，下表中所给出的圈数为手轮从全关位置开始逆时针转过的圈数。

<table id="customers" align="center">
<caption><b>表4</b> ABPA手轮初始设置</caption>
<tr>
<th>工具尺寸</th>
<th>手轮旋转圈数</th>
</tr>

<tr>
<td>9-1/2"</td>
<td>18</td>
</tr>

<tr class="alt">
<td>8-1/4"</td>
<td>15</td>
</tr>

<tr>
<td>6-3/4"</td>
<td>12</td>
</tr>

<tr class="alt">
<td>4-3/4"</td>
<td>4</td>
</tr>
</table>

>注意：在使用4-3/4"工具调节其ABPA时，建议手轮以1/4圈为单元进行调节，4-3/4"尺寸的工具其下行信息传输窗口要比其他更大尺寸工具的窗口小得多(the "window" for successful downlinking with this tool is narrower than for the larger tool sizes)。

#### 现场维护与检查 ####

通常情况下ABPA不允许在钻井现场进行维护，但在每次调节手轮后都需要在调节杆上涂上一层润滑脂以防发生腐蚀。

当使用4-3/4"/6-3/4"工具时，BPA中所使用的三通在开启旁路执行器阀门时连续工作3小时后或者，当使用8-1/2"/9-1/2"工具时，BPA中所使用的三通在开启旁路执行器阀门时连续工作1.5小时后，必须进行一次更换。具体操作步骤请参见后面章节内容(更换ABPA/BPA中的三通)。

为了满足规范要求，4-3/4"/6-3/4"工具中的旁路执行器在连续开启工作6小时后或者，8-1/2"/9-1/2"工具中的旁路执行器在连续开启工作3小时后，必须送回基地进行维护和检修，并对其进行重新认证(sent to town for servicing, inspection, and recertification)。阀门开启与关闭均被视为一次启动(Valve open and then closed again is two actuations)。

#### 可调式喷嘴/接头(Adjustable Nozzle/Sub) ####

在ABPA中可通过调节两阀芯之间的孔隙重合度来控制旁通流量，而在传统的BPA中则使用可调式喷嘴(ANU)来实现这一功能 。喷嘴或与喷嘴等价的阀门开度必须根据具体的井眼水力条件加以调整。但在一般情况下14/32"喷嘴即可满足要求。在立管压力较高时需选用较小尺寸的喷嘴来限制旁路流量，而在立管压力较低时则需选用较大尺寸的喷嘴。

>注意：当在12-1/4"或更大尺寸的井眼中使用8-1/4" / 9-1/2"工具时，最大的16/32"喷嘴不需要另接喷嘴接头进行转换，因为在这种情况下所使用的喷嘴尺寸可能高达22/32"。

##### 可调式喷嘴(Adjustable Nozzle Unit) #####

可调式喷嘴可通过调节通过井眼与旁路系统的泥浆比例，在不断开工具与立管之间连接的情况下调节旁路过流面积(AFT)。

<a target="_blank" href="https://kndlaw.blu.livefilestore.com/y2poTGzTnbv9vN9Ac9BRk8o9BFk55hqU9usQGJz7qm_-Hz9CHHowGrz1aMnFH0b1CKOVkwMmZv4ix28b9grZCkI5r0HYIbYC-CTeVUbOqmZuio/Adjustable%20Nozzle%20Unit.jpg?psid=1">
<img class="aligncenter" title="Adjustable Nozzle Unit" style="width:500px;height:370px;" src="https://kndlaw.blu.livefilestore.com/y2poTGzTnbv9vN9Ac9BRk8o9BFk55hqU9usQGJz7qm_-Hz9CHHowGrz1aMnFH0b1CKOVkwMmZv4ix28b9grZCkI5r0HYIbYC-CTeVUbOqmZuio/Adjustable%20Nozzle%20Unit.jpg?psid=1" alt="Adjustable Nozzle Unit"></a>

转动喷嘴手轮可调节内部阀芯的开度，直至阀门处于全开状态。

<a target="_blank" href="https://kndlaw.blu.livefilestore.com/y2pfL_iC2LMPjY0B-8X7GKXj94c37OYCc8X6vZO4IDPM7boTU4af0sc1YtINgQYpvuGV0hdiNP3m4ZPFaa3D7wQVZI4OCObDjzpKX1DuwzsTLM/Disc%20with%20Triangular%20Shaped%20Hole%20for%20ANU.png?psid=1">
<img class="aligncenter" title="Disc with Triangular Shaped Hole for ANU" style="width:180px;height:160px;float:right;" src="https://kndlaw.blu.livefilestore.com/y2pfL_iC2LMPjY0B-8X7GKXj94c37OYCc8X6vZO4IDPM7boTU4af0sc1YtINgQYpvuGV0hdiNP3m4ZPFaa3D7wQVZI4OCObDjzpKX1DuwzsTLM/Disc%20with%20Triangular%20Shaped%20Hole%20for%20ANU.png?psid=1" alt="Disc with Triangular Shaped Hole for ANU"></a>

顺时针转动手轮可增大阀门开度，从而降低立管压力；逆时针转动手轮则减小阀门开度，从而增加立管压力。

常用阀芯为三角形通孔阀芯(a triangular shaped disc)，其转换关系见表5.

三角形通孔阀芯也可用于BPA/ABPA中以节省成本。

阀芯过流面积与开启角度(黄色手轮)间的换算关系如下：

<table id="customers" align="center">
<caption><b>表5</b> 三角形通孔的开启角度与过流面积的换算关系</caption>
<tr class="alt">
<td>0</td>
<td>7.4</td>
<td>9.4</td>
<td>11.1</td>
<td>12.6</td>
<td>13.9</td>
<td>15.1</td>
<td>16.3</td>
<td>17.4</td>
<td>18.4</td>
<td>19.3</td>
<td>20.2</td>
<td>21.1</td>
<td>22</td>
</tr>

<tr>
<td>5</td>
<td>10</td>
<td>15</td>
<td>20</td>
<td>25</td>
<td>30</td>
<td>35</td>
<td>40</td>
<td>45</td>
<td>50</td>
<td>55</td>
<td>60</td>
<td>65</td>
<td>70</td>
</tr>
</table>

如果你使用的是已淘汰使用的"肾状"阀芯(obsoleted "kidney" shaped disc)，请参考ATK 1.5操作手册获取相应的帮助信息。

#### 操作 ####

大多数情况下，在进行操作前，应首先将阀杆调节到4.5位置使用蓝色手轮或者将阀杆调节到30°位置使用黄色手轮。(Before any operation, adjust the shaft of the hand-wheel to position 4.5 for a blue hand-wheel or 30° for a yellow hand-wheel. This gives a reasonable starting point for most applications.)在工作过程中(没有进行下行数据传输时)可调节手轮位置直至达到最佳旁路流量为止。
