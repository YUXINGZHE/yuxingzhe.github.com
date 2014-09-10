---
layout: post
title: "Landmark钻完井工程综合设计分析系统"
tags: [MWD]
author_name: YUXINGZHE
author_uri: http://twitter.com/yuxingzhe
---

<div id="table-of-contents">
<h2>目录</h2>
<div id="text-table-of-contents">
<ul>
    <li><a href="#sec-1">1&#32;定向井设计系统COMPASS (Directional Advanced Package)</a></li>
    <li><a href="#sec-2">2&#32;套管柱设计软件 Tubular Basic Package - StressCheck</a></li>
    <li><a href="#sec-3">3&#32;高温高压井管柱设计和分析软件WellCat (Tubular Advanced Package)</a></li>
    <li><a href="#sec-4">4&#32;钻井工程设计和分析系统--WELLPLAN (Drilling Fluids Basic Package, Drilling Fluids Advanced Package, Drilling Mechanics Basic Package, Drilling Mechanics Advanced Package, Cementing Opticem)</a></li>
    <ul>
        <li><a href="#sec-4-1">(1)&#32;底部钻具组合分析－BHA Drill ahead</a></li>
        <li><a href="#sec-4-2">(2)&#32;临界转速分析－Critical Speed</a></li>
        <li><a href="#sec-4-3">(3)&#32;水力计算－Hydraulics</a></li>
        <li><a href="#sec-4-4">(4)&#32;卡钻计算－StuckPipe</a></li>
        <li><a href="#sec-4-5">(5)&#32;波动压力分析－Surge/Swab</a></li>
        <li><a href="#sec-4-6">(6)&#32;扭矩和摩阻－Torque/Drag</a></li>
        <li><a href="#sec-4-7">(7)&#32;井控计算－WellControl</a></li>
        <li><a href="#sec-4-8">(8)&#32;优化固井设计－OptiCem</a></li>
        <li><a href="#sec-4-9">(9)&#32;电子工程手册－Notebook</a></li>
    </ul>
</ul>
</div></div>

<span class="dropcap">L</span>andmark 钻完井工程综合分析系统基本覆盖油田钻完井工程各个工作流程，工作内容包括地层压力预测，三维地学模型下的井网设计，单井轨迹设计及井身结构设计，工程参数分析、现场实时数据传输、钻完井信息采集、管理及分析，完井设计等。

Landmark 钻完井工程综合设计分析系统通过工程数据模型EDM 进行合理的数据管理。这种数据管理方式利用强大的SQL Server 数据管理功能，能有效减少数据冗余，提高数据管理效率，无需用户重复录入相同数据。而且EDM 管理的数据结构层次分明，清晰合理，有严格的数据权限管理功能，适于作为企业数据库平台。工程数据模型EDM 也为该系统提供了一个高度集成的设计平台，系统中的每个软件既有独立性又属于一体化的设计流程。我们可以使用其中一个模块来解决相应的问题，也可以完成从井眼轨迹到钻完井施工管理的整个工作流程。

Landmark 公司拥有先进的图形展示技术，用户可以直观地查看所做的设计。Landmark 钻完井施工设计分析系统中的所有功能基本上都可以用视图方式展示出来，且很多情况下都以三维可视化技术展现设计与分析结果，从而简化工作流程，提高工作效率。

Landmark 钻完井工程综合分析系统主要包括以下十大功能模块：定向井设计系统、套管下深设计软件、套管柱设计软件、高温高压管柱设计和分析软件、钻井工程设计和分析系统、失效分析及成本控制、钻完井数据管理和分析系统、钻完井数据查询及分析、DecisionSpace<sup>&#174;</sup> Well Planning油田开发钻井规划及井网设计、地层压力预测软件等。下面对部分用到的软件功能进行了概述。

<h4><a name="sec-1">1 定向井设计系统COMPASS (Directional Advanced Package)</a></h4>

COMPASS 可使用户在进行各类定向井设计时比以往任何时候都容易， COMPASS 广泛应用了众多的软件工具，这些工具不仅适用于所有石油公司同时也适用于所有的定向井承包商，从初始设计到工程作业，COMPASS 可提供快速、准确的轨迹设计并在初始阶段判断出潜在的问题所在。

<a target="_blank" href="https://9giq1q.bl3302.livefilestore.com/y2pimxv87wSx1i6OUAxUdwSRQB0JrH9SRu8xPDO0bme2z7vYzfuTTTGGTDKXSGmZxz-hnmGJ4FLzE7Z7zxYQnO5QS-kuHMqoKpCxaYIQn7Lf3w/COMPASS.png?psid=1">
<img class="aligncenter" title="COMPASS" style="width:600px;height:470px;" src="https://9giq1q.bl3302.livefilestore.com/y2pimxv87wSx1i6OUAxUdwSRQB0JrH9SRu8xPDO0bme2z7vYzfuTTTGGTDKXSGmZxz-hnmGJ4FLzE7Z7zxYQnO5QS-kuHMqoKpCxaYIQn7Lf3w/COMPASS.png?psid=1" alt="COMPASS"></a>

(1)COMPASS的三大主要功能

<b>定向井轨迹设计</b>：可以分段进行多了行二维及三维轨迹设计，用户界面友好，既适用于初学者也适用于相关领域的专家进行设计操作。

<b>定向井测斜数据处理</b>：多种计算方法进行测斜数据处理，利用特定方法进行质量控制。

<b>防碰和最近距离计算</b>：多种方法提供进行防碰计算，提供网状绘图、控制圆柱和打印输出最近距离扫描结果，特别是可进行三维最近距离分析，并可以对图形进行任意放大缩小、旋转、预测、TVD断面检查等。

(2)COMPASS还拥有如下的一些使用功能：

数据质量校核：COMPASS测量系统是全世界第一个采用可变曲线质量控制的软件，这个方法可查询到标准方法的缺陷，例如：①假设井眼轨迹与一已知和定性的几何模型相符合，这样所产生的形状没必要与实际井眼轨迹相符合；②每一测点相互独立不考虑相邻测点的影响元素，如何仔细观察变化曲线数据进行质量控制的具体步骤根据使用者的要求确定，数据的输入可以手工键入也可以从文件中录入，这样数据处理的成本会大大地降低。

使复杂问题简单化：由于设计模式具有多功能和操作灵活简便的特点，几乎所有复杂井都可以设计并节省时间和人力，井的分段设计可以固定造斜/扭方位定为常数和固定狗腿为常数，变化率既可以计算得来也可以给一定值以满足某一特定的需要，或由程序推荐以优化井眼轨迹。例如象救援井靶点总是在变化，这就可以用靶点投影到任意位置轻而易举的完成。COMPASS 提供的"优选定位"计算可根据约束提供极限值，例如利用给定井斜计算中靶井深和给定狗腿计算方位，中靶时要求一定的井斜和方位等。井眼轨迹设计的结果是：最小狗腿和最短起下钻距离，节省了费用。

UTM和地理数据输出：这个模式提供了UTM输出设施，所有测量均可建立在球体坐标或地理坐标上。

惯性测斜数据输入：这个功能允许使用者输入测斜数据时采用直角坐标系而不用输入测深、井斜和方位。当用最小曲率进行下部预测时数学模式可反算出测深、井斜和方位，随后进行处理以使误差最小化。

绘制壁挂大图：支持各种大型绘图机并由使用者完全控制的高质量壁挂展示图。

<h4><a name="sec-2">2 套管柱设计软件 Tubular Basic Package - StressCheck</a></h4>

Landmark 公司的StressCheck 采用了不同工况下的三轴应力设计方法，能够快捷完成强度设计，在确保安全的同时，大幅削减套管成本。其抗内压、抗外挤和轴向载荷设计结果可在曲线图示中观察，同时，独一无二的"点击－拖拉"图形设计使设计变得非常简单方便。

<a target="_blank" href="https://9wiq1q.bl3302.livefilestore.com/y2pKOmpI__RPkTmnE0N7VGXfTNsmtaTSV17Dx73zIdKkOD1ITgIcyLLCx-bY5ylwLD969F6erYX-uaxyu50iOxqbMejqJ2y6PbNnmU84s7XzVQ/StressCheck.png?psid=1">
<img class="aligncenter" title="Stress Check" style="width:700px;height:550px;"
src="https://9wiq1q.bl3302.livefilestore.com/y2pKOmpI__RPkTmnE0N7VGXfTNsmtaTSV17Dx73zIdKkOD1ITgIcyLLCx-bY5ylwLD969F6erYX-uaxyu50iOxqbMejqJ2y6PbNnmU84s7XzVQ/StressCheck.png?psid=1" alt="Stress Check"></a>

<ul style="margin-left:50px;">
<li>包含从简单到复杂的外部载荷剖面，具有诸如好/坏固井质量，渗透层，泥浆降解，环空泥浆液面下降和环空气串等选项，并允许自定义其它外部载荷，实现不同工况下的三轴应力设计</li>

<li>不同外部载荷对强度设计的影响用应力椭圆直观显示</li>

<li>采用缺省的温度曲线来评估在钻井、采油和注入工况中由地热所引起的载荷，可自定义初始条件，可采用静温梯度或作业工况温度</li> 

<li>独一无二的鼠标"点击－拖拉"方法修正强度设计，其他设计曲线与结果自动计算更新</li> 

<li>对直井和定向井都适用的精确的载荷，应力和弯曲解决方案</li> 

<li>可模拟盐岩蠕变所引起的外挤载荷</li> 

<li>抗硫及防腐设计</li> 

<li>设计系数可依载荷工况而定，本体和接箍的系数可以不相同，内压和轴向安全系数取本体或接箍的较小值</li> 

<li>考虑了温度对屈服极限的折减率</li> 

<li>完整的API管材库，并可加入用户自定义的管材</li> 

<li>标准的API接箍及其机械性能，并可加入用户自定义的接箍</li> 

<li>使用现有管材库存自动进行复合管串的最小成本设计</li> 

<li>利用电子表格使数据录入更容易，包括拷贝、剪切、粘贴及拖放等功能。具有油公司套管设计的标准模板。能以图形方式显示井身结构、定向井轨迹、孔隙压力、破裂压力、拉力、内外压力和温度曲线等等</li> 

<li>方便而灵活的输出方式，提供一个关于整个管串的最小内压、外挤、拉伸及三轴安全系数的标准总结性报告。具有标准的报告格式和用户自定义的报告格式。结果可以多窗格的方式显示</li> 

<li>现基于Landmark 公司的新一代钻井和油井服务软件的基础模型&#8212;&#8212;公共数据模型(EDM)，真正实现设计和施工流程上的无缝集成</li> 

<li>界面清晰，充分应用Windows 易用的界面特点，并具有上下文相关的向导帮助用户输入数据</li>

<li>向导模板，数据传输简便：具有公英制和用户自定义的单位系统，完善的在线帮助。可与其它应用程序交换数据</li>

<li>强大的报表功能</li></ul> 

<h4><a name="sec-3">3 高温高压井管柱设计和分析软件WellCat (Tubular Advanced Package)</a></h4>

WellCat 可为管柱设计提供一体化设计和分析解决方案。WellCat 解决了管柱设计学科中的最复杂问题，即精确预测井下温度、压力剖面、管柱载荷和由之引起的位移等难题。在Windows 操作环境下的Wellcat 软件由5 个可独立运行的模块(Drill 钻井、Pro 开发、Casing 套管、Tube 油管、Multistring 多管串) 组成。

对高温高压油井不采用WellCat 进行设计的潜在危险是，由于环空流体膨胀可能造成管柱失效，造成井漏和井喷，考虑到油藏的油气损失、勘探和开发费用以及对健康安全和环境(HSE)的影响。

<a target="_blank" href="https://9miq1q.bl3302.livefilestore.com/y2ps__SFC5aylwNxMiYzGlF3hDKc0rN7o6tuO5a3NuIk0D-yC0FXmVQz5fMh6dn3TLqGPyQdx7g17w66AMSBbTrbWbdkqc-n2Wam8u41H19-ak/WellCat.png?psid=1">
<img class="aligncenter" title="WellCat" style="width:700px;height:570px;" src="https://9miq1q.bl3302.livefilestore.com/y2ps__SFC5aylwNxMiYzGlF3hDKc0rN7o6tuO5a3NuIk0D-yC0FXmVQz5fMh6dn3TLqGPyQdx7g17w66AMSBbTrbWbdkqc-n2Wam8u41H19-ak/WellCat.png?psid=1" alt="WellCat"></a>

该软件主要解决常温套管设计软件所不能解决的如下管柱设计中的最复杂的难题：

<ol style="margin-left:50px;">
<li>下油井的环空热膨胀是否会引起套管损坏---内层管柱挤毁，外层管柱崩裂？</li> 

<li>由温度、压力产生的对整个套管和油管系统的载荷会不会引起井口移位运动及载荷的重新分布？</li> 

<li>如何消除套管和油管的弯曲，或将其限制在一定的范围内？</li> 

<li>在深井钻井过程中，套管在未凝固的水泥中是否弯曲，在采油过程中，如何避免这类问题？</li> 

<li>小排量的反循环顶替封隔液对油管是起加热还是冷却作用？</li> 

<li>在确保安全和可靠的前提下，有没有大幅度降低管材成本的途径？</li> </ol> 

<h5>功能特点</h5>

<ul style="margin-left:50px;">
<li>精确的温度模拟：固井过程的温度，高温高压流体，采油，注汽， 关井，油井泄漏，压井，掏空，酸化压裂等等</li> 

<li>通过精确的温度模拟，计算不同温度下管柱的强度变化，预测油井寿命分析</li> 

<li>复杂的油管应力和位移分析</li> 

<li>支持多管串分析</li> 

<li>向导模块</li></ul> 

<h4><a name="sec-4">4 钻井工程设计和分析系统--WELLPLAN (Drilling Fluids Basic Package, Drilling Fluids Advanced Package, Drilling Mechanics Basic Package, Drilling Mechanics Advanced Package, Cementing Opticem)</a></h4>

钻井工程设计和分析系统(WELLPLAN)能完成钻井施工过程中所涉及的几乎所有的计算，并具有强大的分析能力，考虑因素充分，能预测钻井过程中经常发生的事故，对卡钻、井涌井漏、钻具失效等事故的处理提供方案，确保钻井施工的顺利进行。

该系统包括九大功能：底部钻具组合分析(BHA Drill Ahead)、临界转速分析(Critical Speed)、水力计算(Hydraulics)、卡钻计算(StuckPipe)、波动压力分析(Surge/Swab)、扭矩和摩阻(Torque/Drag)、井控计算(WellControl)、优化固井设计(OptiCem)、电子工程手册(Notebook)。

<h5><a name="sec-4-1">(1)底部钻具组合分析－BHA Drill ahead</a></h5>

利用有限单元分析技术预测、模拟和分析各种旋转和导向钻具组合的钻井特性。Landmark 公司利用目前工业界权威精确的有限元分析技术对定向钻井和钻具组合特性进行充分研究。该程序所使用的技术由兰德马克公司独创。它由两部分组成，第一部分是利用非线性、三维有限单元技术来解决所限定钻具组合的结构问题。第二部分是利用分析和规律相结合的方法来确定钻具组合的趋向，BHA 向前钻进使我们对井下钻具组合的认识从盲目阶段走向了科学化阶段。 

该软件除计算钻具组合力学参数外，还具有三大分析功能：停钻/静态分析、超前预测分析、优选WOB/ROP 参数。 

<h5><a name="sec-4-2">(2)临界转速分析－Critical Speed</a></h5> 

钻井过程中碰撞和振动载荷非常激烈，钻柱会发生纵向震动、扭转震动和横(侧)向震动。经研究发现，在接近井底的一段钻具内，横向震动异常突出，是引起钻具不稳定和疲劳破坏的主要原因。

利用有限单元分析和受力频率反应技术模拟和鉴定临界转速及钻具中的高应力集中。这是一个功能强大、技术领先的软件，在预测钻具的振动方面代表着世界目前最先进的实用技术。它主要基于钻具的有限单元模式和被受力频率反应技术来确定钻具的动态行为。这个程序的灵活性高且使用范围广。利用临界转速分析的设计模式可帮助避免耗费巨大的钻具井下失效，而利用实际作业模式可帮助分析失效的原因以便在下一步钻井过程中避免钻具失效。

<h5><a name="sec-4-3">(3)水力计算－Hydraulics</a></h5> 

完整的循环系统分析，钻头水眼优选，压力损耗，抽吸激动压力和井眼清洁计算等，为优化钻井提供依据。 

<h5><a name="sec-4-4">(4)卡钻计算－StuckPipe</a></h5> 

进行失效分析、传送到卡点力的计算、震击器设定和震击所需力的计算、解卡力计算。利用与扭矩/阻力程序相同的钻柱模式它可以精确的计算出摩擦力和其它结果，由于钻柱、测斜及其它数据可能在日常作业已在WELLPLAN 的其它程序中输入，所以，一旦发生卡钻而利用这套程序进行分析计算是相当迅速的。 

<h5><a name="sec-4-5">(5)波动压力分析－Surge/Swab</a></h5> 

可动态模拟由于钻杆运动引起的井下波动压力，Wellplan 波动压力分析是一个技术领先的模块，可为工程师提供最优的起下钻速度和泥浆密度，以避免起下钻和固井作业中发生井控和地层损害问题。波动压力模块可用于设计阶段， 以确定需要控制的波动压力；或用于诊断与波动压力有关的井控问题。 

波动压力模块可研究繁琐的计算，以节省工程师的时间。波动压力模块考虑了许多复杂的因素，如温度和压力对油基或水基泥浆压缩性和流变性的影响。它可模拟循环过程中的钻杆运动、顶替水泥浆，也考虑了钻杆运动的轴向弹性。波动压力可分析随深度变化的起下钻速度、地层性质和流变性。多因素分析也能模拟井底的钻杆运动速度和距离。波动压力考虑了原始影响因素和处理多相流体。波动压力也能模拟循环系统、地层和水泥的弹性。 

<h5><a name="sec-4-6">(6)扭矩和摩阻－Torque/Drag</a></h5> 

在设计阶段工程师利用扭矩和摩阻分析软件可以很容易地研究不同钻具设计在不同的井身结构中的效果,同时对经常存在的问题找出最佳解决办法,设计出合适的钻具组合, 避免钻具失效, 确保所钻井能安全地钻至设计井深。 

<h5><a name="sec-4-7">(7)井控计算－WellControl</a></h5> 

这个程序模拟了井涌的产生及循环出井外的过程，采用常用方法(司钻法和等待加重法)，计算压井作业过程中流体侵入井内时的压力。 

<h5><a name="sec-4-8">(8)优化固井设计－OptiCem</a></h5> 

对不同性能的多流体系统进行泵入模拟，各临界点的压力计算等。这套软件能在固井作业过程中对不同液体进行模拟，包括冲洗液、隔离液、水泥浆和顶替液。它可帮助工程师对可能发生的问题进行准备，例如：U-型管效应、压差等，确保顺利实施平衡压力固井。

<a target="_blank" href="https://82iq1q.bl3302.livefilestore.com/y2ppjoll1dZQpUCKaJaw8vip50GOzgO8XIlA307-PxIMne9HoL4YBfga_A67ypqt8TMl6qt9C5yxiLM2Gjqh1X4vhi9H5Ov2p3D4EXZ_Ca5JUY/Cementing-OptiCem.png?psid=1">
<img class="aligncenter" title="Cementing-OptiCem" style="width:600px;height:490px;" src="https://82iq1q.bl3302.livefilestore.com/y2ppjoll1dZQpUCKaJaw8vip50GOzgO8XIlA307-PxIMne9HoL4YBfga_A67ypqt8TMl6qt9C5yxiLM2Gjqh1X4vhi9H5Ov2p3D4EXZ_Ca5JUY/Cementing-OptiCem.png?psid=1" alt="Cementing-OptiCem"></a>

<h5><a name="sec-4-9">(9)电子工程手册－Notebook</a></h5>

该手册提供钻井手册中常用的计算，如工程管柱计算，容积和高度计算，迟到时间计算，顶替计算，大绳寿命计算，钻柱和环空容积计算，钻机能力计算，单位换算器，水力计算器，流体计算器以及其他的一起计算等。
