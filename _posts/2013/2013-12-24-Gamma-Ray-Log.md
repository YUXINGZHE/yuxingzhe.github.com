---
layout: post
title: "伽马测井"
tags: [MWD]
author_name: YUXINGZHE
author_uri: http://twitter.com/yuxingzhe
---

<div id="table-of-contents">
<h2>目录</h2>
<div id="text-table-of-contents">
<ul>
    <li><a href="#sec-1">1 伽马射线与物质的作用与探测</a></li>
    <li><a href="#sec-2">2 伽马探测原理</a></li>
    <li><a href="#sec-3">3 自然伽马测井仪的标定</a>
        <ul>
            <li><a href="#sec-3-1">3.1 主标定程序(Master Calibration)</a></li>
            <li><a href="#sec-3-2">3.2 标定数据解释</a></li>
            <li><a href="#sec-3-3">3.3 井场仪器验证(Wellsite Verification)</a></li></ul></li>
    <li><a href="#sec-4">4 环境因素校正</a>
        <ul>
            <li><a href="#sec-4-1">4.1 环境影响因素</a></li>
            <li><a href="#sec-4-2">4.2 井眼尺寸与泥浆比重校正案例</a></li>
            <li><a href="#sec-4-3">4.3 钾元素校正案例</a></li>
            <li><a href="#sec-4-4">4.4 钾元素泥浆报告(Potassium Content - Mud Report)</a></li></ul></li>
    <li><a href="#sec-5">5 探测深度(Depth of Investigation)</a></li>
    <li><a href="#sec-6">6 纵向分辨率(Vertical Resolution)</a></li>
    <li><a href="#sec-7">7 伽马测井响应曲线</a>
        <ul>
            <li><a href="#sec-7-1">7.1 放射性涨落误差(Statistical Fluctuation)</a></li>
            <li><a href="#sec-7-2">7.2 测井速度(Logging Speed)</a></li>
            <li><a href="#sec-7-3">7.3 测井响应曲线(Primary Curves)</a></li></ul></li>
    <li><a href ="#sec-8">8 数据遥测(Telemetry)</a></li>
    <li><a href="#sec-9">9 伽马曲线的应用</a>
        <ul>
            <li><a href="#sec-9-1">9.1 划分岩性和地层对比(Lithology Identification)</a></li>
            <li><a href="#sec-9-2">9.2 计算地层泥质含量(Determination of Shale Content)</a></li>
            <li><a href="#sec-9-3">9.3 地质导向(Geo-Steering)</a></li></ul></li>
    <li><a href="#sec-10">10 LWD伽马测井仪与电缆伽马测井仪的区别</a></li>
    <li><a href="#sec-11">11 伽马测井曲线质量控制(Gamma Log Quality Control)</a></li>
</ul></div></div>

<span class="dropcap">岩</span>石中含有天然的放射性核素，主要是铀系、钍系和钾的放射性同位素，它们自然衰变时发射伽马射线，使岩石具有天然放射性。自然伽马测井(Natural Gamma Ray Log)是用伽马射线探测器测量岩石总的自然伽马射线强度，以研究井剖面地层性质的测井方法。

<h4><a name="sec-1">1 伽马射线与物质的作用与探测</a></h4>

岩石总的自然伽马放射性与岩石大类有关，<u>一般沉积岩的自然伽马放射性要低于岩浆岩和变质岩</u>。因为沉积岩一般不含放射性矿物，其自然放射性主要是岩石吸附放射性物质引起的，而岩石吸附能力又很有限。而岩浆岩及变质岩含有较多的放射性矿物，如长石、云母、角闪石、辉石、锆石、独居石、揭帘石等。

<p><u>沉积岩的自然放射性随岩石泥质含量增加而增加</u>，但含放射性矿物的岩石(如海绿石砂岩、独居石砂岩、钾盐等)例外。沉积岩中粘土岩反射性最高，而石膏、硬石膏、岩盐等化学岩放射性最低。生油粘土岩矿物常以蒙脱石和伊利石为主，而且富含有机质，容易吸附含铀和钍的放射性物质，因而比普通泥岩有更高的放射性。</p>

放射性原子核衰变放射出的伽马光子与物质的相互作用主要有<b>光电效应、康普顿效应和电子对效应</b>。这些效应都能产生次级电子，这些电子可引起物质中的原子发生电离和激发，伽马探测器通过检测这些电离和激发出来的电子来间接探测地层中的伽马射线强度。

光电效应
: 伽马光子与原子核外的束缚电子作用，光子把全部能量转移给某个束缚电子，使之发射出去(光电子)，而光子本身被吸收。

康普顿效应
: 伽马光子与原子核外电子发生非弹性碰撞，一部分能量转移给电子，使它脱离
原子成为反冲电子，而光子(散射光子)的能量和运动方向发生变化。

电子对效应
: 当伽马光子从原子核旁经过时，在原子核的库仑场的作用下，伽马光子转变为一个正电子和一个负电子，这种过程称为电子对效应。


<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pi7c6of-MQPWP-AMtPK0sVMfyn-3gtb8gdEd4v0s_d1JxBnWVVlvRgcf_ezhKEe835QlxWr_DICAk0oiWCr64OqvEiE2mI8taZd8X23T_eIk/threeeffectstoinduceelectron.png?psid=1">
<img class="aligncenter" title="three effects to induce electron" style="width:450px;height:230px;" src="https://lneprw.blu.livefilestore.com/y2pi7c6of-MQPWP-AMtPK0sVMfyn-3gtb8gdEd4v0s_d1JxBnWVVlvRgcf_ezhKEe835QlxWr_DICAk0oiWCr64OqvEiE2mI8taZd8X23T_eIk/threeeffectstoinduceelectron.png?psid=1" alt="three effects to induce electron"></a>

电离作用是带电粒子与组成物质的束缚电子发生非弹性碰撞的结果。盖革-弥勒计数管就是利用气体电离作用的脉冲探测器。如果束缚电子获得的嫩两不足以使它成为自由电子，而只能激发到更高的能级，这种现象成为激发作用。受激发的原子在退激过程中放出光子，发生闪光(荧光)，利用荧光来进行探测的为闪烁计数器。

闪烁记数器(scintillation counter)由光电倍增管和碘化钠晶体组成。当伽马射线进入NaI晶体时，通过上述三种效应产生次级电子，这些次级电子使得晶体中的原子受激而产生荧光。利用光导和反射物质把大部分荧光光子收集到光电倍增管的阴极上。光子在光阴极上打出光电子，光电子在光电倍增管内不断倍增，最后形成电子束在阳极上产生电压脉冲，并被记录系统记录。

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pM847OQwV-VbYH3lzjmH1rcPFpjVS_eYVNE_hQxVfUKSrO406liEM0U_QuTQNf74HENFCG6vSbv79V0bAiynQejUUOIa-JeIO8LkXGMYVRHI/Scintillation%20Counter.png?psid=1">
<img class="aligncenter" title="Scintillation Counter" style="width:600px;height:200px;" src="https://lneprw.blu.livefilestore.com/y2pM847OQwV-VbYH3lzjmH1rcPFpjVS_eYVNE_hQxVfUKSrO406liEM0U_QuTQNf74HENFCG6vSbv79V0bAiynQejUUOIa-JeIO8LkXGMYVRHI/Scintillation%20Counter.png?psid=1" alt="Scintillation Counter"></a>

闪烁记数器的输出脉冲幅度与入射伽马光子在闪烁体中损失的能量(次级电子能量)成正比，输出脉冲的个数与入射光子的强度(单位时间伽马光子数)成正比，一般用计数率(脉冲数/分钟)来表示。

<h4><a name="sec-2">2 伽马探测原理</a></h4>

伽马探测器根据与之同步的工具面数据将采集到的伽马射线(一次计数事件)分布到与探测器垂直的的8个扇区面内，然后根按照下图所示的方法将相邻的计数率相加形成四个分区再传送到地面上进行解码。

当接头旋转时，<u>每个扇区会累记25s内所检测到的信号数量，定向探头测得的工具面值每16ms更新一次(60Hz)</u>。而处于扇区边界处的信号则会根据各扇区边界和工具面的相对距离进行划分(探测器只能识别处于两次工具面数据之间的计数率总数，无法确知具体的扇区边界在哪，但通过程序可以预设一个扇区边界工具面值，处于这个值两侧所测得的两个工具面间的计数率总数就根据这三个值的比例关系进行分配)。每个扇区所接收到的信号总数除以探测器在各扇区停留的时间就得到了相应扇区每秒钟所接收到的信号数量(cps)。

在接头上相隔180°安装着两个相互独立的闪烁计数器，这样不但可以提高计数精度，而且还能保证在其中一个发生故障后，另外一个仍能继续完成测量任务，从而提高了系统的可靠性。当转速高达400RPM时探测器仍能十分精确地分辨出各相邻扇区的边界。

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pgdv25Qhb_zA-K2b-DxzkvwzWjB54qTaxmGc0yn_Xxx6gfJ-SXv5uUvU28Anj_cFzldVVWFWsHdqN7CIJiuS1qC8TY1dfRPoBPTYStuDPtWw/Sector%20Orientation.png?psid=1">
<img class="aligncenter" title="Sector Orientation" style="width:500px;height:230px;" src="https://lneprw.blu.livefilestore.com/y2pgdv25Qhb_zA-K2b-DxzkvwzWjB54qTaxmGc0yn_Xxx6gfJ-SXv5uUvU28Anj_cFzldVVWFWsHdqN7CIJiuS1qC8TY1dfRPoBPTYStuDPtWw/Sector%20Orientation.png?psid=1" alt="Sector Orientation"></a>

在工具上沿X轴和Y轴分别放置着两个磁通门传感器，他们之间测得的波形相位差正好为90°。当工具旋转时，当地磁场在这两个传感器上的分量不断发生变化，并呈现正弦曲线的规律，这样<u>从以下两条正弦曲线上就可以将垂直于探测器的平面分成8个扇区</u>(两条曲线的交点处正好为45°)。

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pqqd5hP7Ykm9MHDYsqg_R3nAtC9ZpZ5HWXZBtJtSdKknNgViW0_SqLVBxKN1-2c4cQfzbWfd7pGBiiG1xpWAsYqP9SQk6RZa2hBpg6UCbmNU/Azimuth%20Orientation.png?psid=1">
<img class="aligncenter" title="Azimuth Orientation" style="width:700px;height:260px;" src="https://lneprw.blu.livefilestore.com/y2pqqd5hP7Ykm9MHDYsqg_R3nAtC9ZpZ5HWXZBtJtSdKknNgViW0_SqLVBxKN1-2c4cQfzbWfd7pGBiiG1xpWAsYqP9SQk6RZa2hBpg6UCbmNU/Azimuth%20Orientation.png?psid=1" alt="Azimuth Orientation"></a>

<u>为了校正上述两条正弦曲线的零点，我们需要用到重力工具面(即高边工具面)数据。</u>Gamma Elite需要使用动态测井(flow on survey)所获取的井眼方位和井斜数据来从磁工具面计算重力工具面。这样就需要在每次接单根的时候进行一次全面测井(a full survey)，然后将相关数据存储起来以供这跟单根钻进过程中的分区计算(假定在一根钻杆的范围内HSTF和MTF之间的差值保持不变)。如果测井数据有误或者在钻进过程中数据已经发生了变化，分区计算还可以通过后处理的方式加以校正(sector allocation can be corrected through post-processing)。

伽马探测器计数分区过程的精度严重依赖于测井数据的准确性！在现场操作中，一次全面测井(a full survey)过程需要19s时间(9s用于系统配置，10s用于测井)。为了确定测井过程确已完成，我们还要观察测井格式标识符FID(format identification parameter)来确定我们已经得到了所需要的数据(如AutoTrak中的FID为0或2，OnTrak中的FID为0或4)。如果对于测井数据怀有疑虑，必须重新进行测井以保证计数分区过程的正确性。

伽马数据累记原则如下(具体数据请参考具体工具规范)：

<ul style="margin-left:50px;">
<li>如果井斜小于3°，定向探头将传输磁工具面(MTF)数据；</li>
<li>如果井斜大于3°，定向探头将传输重力工具面(GTF)数据。利用动态测井("flow on" survey)所获取的方位与井斜数据，再通过磁通门传感器可以得到以上信息。(This information is derived from the magnetometers using the azimuth and inclination determined by the "flow on" survey.)</li></ul>

在以下工况下将无法保证获取准确的伽马数据("no go zone")：

<ul style="margin-left:50px;">
<li>井斜与地磁倾角的夹角小于5°时；</li>
<li>井眼磁北方位角小于5°时。</li></ul>

在南半球时，以下工况下将无法保证获取准确的伽马数据("no go zone")：

<ul style="margin-left:50px;">
<li>井斜与地磁倾角的夹角小于5°时；</li>
<li>井眼磁南方位角小于5°时。。</li></ul>

在上述情况下，井眼轨迹与地磁场磁力线几乎平行，此时X轴和Y轴上的磁通门传感器读数接近零值，无法确定工具在旋转时的扇区方位。

<b>Case 1：</b>井眼磁北方位角在355°与5°之间

当井眼轨迹朝向正北时，在<b>(90°-磁倾角)</b>的井斜范围内探测仪将无法保证获取准确的伽马数据。

Example 1：井位处于北半球，当地磁倾角为60°时，不准确探测井斜角为90°-60°=30°。考虑到仪器的操作误差窗口，我们认为当井斜为25°~35°之间时所测得的伽马值是不准确的。

Example 2：井位处于南半球，当地磁倾角为<b>-10°</b>时，不准确探测井斜角为90°-(-10°)=100°。同样，考虑到仪器的操作误差窗口，我们认为当井斜为95°~105°之间时所测得的伽马值是不准确的。

<b>Case 2：</b>井眼磁南方位角在175°与185°之间

当井眼轨迹朝向正南时，在<b>(90°+磁倾角)</b>的井斜范围内探测仪将无法保证获取准确的伽马数据。当井位处于北半球或南半球时的不准确井斜范围计算方法同上。

>注意：规定在北半球地磁倾角为正值，在南半球地磁倾角为负值。

<h4><a name="sec-3">3 自然伽马测井仪的标定</a></h4>

自然伽马测井仪以脉冲数/分钟为单位进行输出，不仅和岩层的放射性强度有关，而且和测量仪器(包括探测器和整个记录系统)的灵敏度有关，即在相同的地层条件下，使用不同的仪器可能得到不同的输出信号。为了便于资料对比和定量解释，必须使仪器标准化。标准化的基本方法是把不同的测量仪器在同一个已知的放射性标准化装置上进行检查测量，并调节仪器系统的灵敏度使它们有相同的输出，或者求得不同仪器的换算系数。

在实际应用中自然伽马测井的放射性单位为API，它是基于美国得州休斯敦大学内的<b>人工放射性水泥柱</b>而定义的。美国石油协会规定将标定井中高放射性地层与低放射性地层读数之差定为200个API单位。下图为美国休斯敦大学建造的世界上第一个自然伽马标定井的示意图。它上面是厚度为3/8"(0.953cm)的钢盖板，以阻隔宇宙射线。境内有三个厚度都是8ft(2.44m)的模拟地层，其直径为4ft(1.22m)，中心位套管，管内充满水。

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pyqzwsscx6IajacyTpRiAYtfkp_1l8FXHneYKT_s8DegOwaTQS_4U54WJslSFjhe7hV4fZcbNDw-I9F_GOV7ahKMo-vSRuSJqZ7F3bKPDVkg/APIpit.png?psid=1">
<img class="aligncenter" title="API pit" style="width:400px;height:480px;" src="https://lneprw.blu.livefilestore.com/y2pyqzwsscx6IajacyTpRiAYtfkp_1l8FXHneYKT_s8DegOwaTQS_4U54WJslSFjhe7hV4fZcbNDw-I9F_GOV7ahKMo-vSRuSJqZ7F3bKPDVkg/APIpit.png?psid=1" alt="API pit"></a>

然而，大多数LWD工具都无法放入标准API标定井中进行标定，因此建立了以下二级标定标准：

<ul style="margin-left:50px;">
<li>标定井的伽马刻度值由在API GR标准标定井中进行标定过的钢丝绳伽马测井仪确定</li>
<li>标定环境设定为10"井眼，内部充满密度为8.33lb/gal的水</li>
<li>所有LWD GR测井仪在标定井的花岗岩块内的刻度值都相等</li>
<li>使用6"井眼对仪器的标定值进行验证</li>
<li>使用石灰岩来评价不同伽马射线能谱带组成对标定结果造成的影响</li></ul>

在全国统一的标准标定井中进行的刻度，称为一级标定。各大油田也可建立自己的标定井，其单位应与一级标定井有对应关系。在井场，可用标定井标定过的标准伽马源作标定器进行现场标定。

<h5><a name="sec-3-1">3.1 主标定程序(Master Calibration)</a></h5>

由于LWD伽马探测仪需要每隔60天进行一次标定，因此<u>在现场基地里面又使用了另外一套标定方法</u>，主要由一对Amersham标定器(Amersham Source、Amersham Blank)以及GammaGal标定软件组成，其中Amersham Blank中没有伽马源，Amersham Source中则包括已标定过的已知刻度值的伽马源。在标定过程中，必须保证其他所有伽马源(如钢质构件等)都处于标定器15ft以外。首先将LWD伽马探测仪放入Amersham Blank中测得背景刻度值(Background Only)；然后再将LWD伽马探测仪放入Amersham Source中测得在给定刻度值伽马源环境下的读数；最后根据这两个读数即可计算出LWD伽马探测仪的标定因子<b>GRSECF</b>：

Calibration Factor GRSECF = Amersham API value /[(Source+Background) - Background]

在上述标定值中已经将已知刻度值(Background & Source)校正到了标准井眼环境(即10"井眼，内部充满密度为8.33lb/gal的水)，除此以外，还需要对实际井眼尺寸、泥浆比重和泥浆中的KCl含量等对标定值的影响加以校正。<u>对于探针式LWD传感器(Probe Module/Sensor)</u>，考虑到钻铤对伽马射线的耗散阻挡效应，还需要<u>根据钻铤的内径和外径将GRSEF校正为<b>GRAPICF</b>(Gamma Ray API Correction Factor)</u>，并输入到Advantage中去。所得报告如下图所示：

<p style="text-align:center;">
<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2peDh0wjYuuNZFMQzqNUIgH8peqQqv3ml6brASNt4nHsPWbzpLIJpI84BiFg0jKsftWlMbhmmEHey_2WEGrSw0txF8WwBsdvxlRLRQfFE8N_M/CollarCorrectedforGRAPICF.png?psid=1">
<img title="Collar Corrected for GRAPICF" style="width:420px;height:340px;" src="https://lneprw.blu.livefilestore.com/y2peDh0wjYuuNZFMQzqNUIgH8peqQqv3ml6brASNt4nHsPWbzpLIJpI84BiFg0jKsftWlMbhmmEHey_2WEGrSw0txF8WwBsdvxlRLRQfFE8N_M/CollarCorrectedforGRAPICF.png?psid=1" alt="Collar Corrected for GRAPICF"></a>
<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2px57iurUz5gE9EbBKkfFpOb7RK9XjT7kNk-FDGn-fj0Suzi2HfKC-1r3dnyv19x6xRqiZWuR7bPc11WmR2BuAN4SMn144r9HTbcoRT_CSVxY/CollarCorrectedforGRAPICF2.png?psid=1">
<img title="Collar Corrected for GRAPICF" style="width:420px;height:340px;" src="https://lneprw.blu.livefilestore.com/y2px57iurUz5gE9EbBKkfFpOb7RK9XjT7kNk-FDGn-fj0Suzi2HfKC-1r3dnyv19x6xRqiZWuR7bPc11WmR2BuAN4SMn144r9HTbcoRT_CSVxY/CollarCorrectedforGRAPICF2.png?psid=1" alt="Collar Corrected for GRAPICF"></a></p>

<h5><a name="sec-3-2">3.2 标定数据解释</a></h5>

下面给出了一个6-3/4"OnTrak探测仪的Amersham标定报告：

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pbpQfZ8SSuXay6ScR-TSJ1gNc1_rHTaT7rrjQVgUUWu4wYVyfFyldE7n9BrRjhWDlOzaiRxpzCyMLoF9TLsVAmNRlnu2Qyg1-7IB1IF9bcxY/Gamma%20Ray%20Calibration%20Summary.png?psid=1">
<img class="aligncenter" title="Gamma Ray Calibration Summary" style="width:600px;height:270px;" src="https://lneprw.blu.livefilestore.com/y2pbpQfZ8SSuXay6ScR-TSJ1gNc1_rHTaT7rrjQVgUUWu4wYVyfFyldE7n9BrRjhWDlOzaiRxpzCyMLoF9TLsVAmNRlnu2Qyg1-7IB1IF9bcxY/Gamma%20Ray%20Calibration%20Summary.png?psid=1" alt="Gamma Ray Calibration Summary"></a>

上述报告中各项数值说明如下：

Background(cps)：在无伽马源环境下测得的背景计数率(Amersham Blank)。

Calibration On(cps)：在已知刻度值伽马源环境下测得的计数率(Amersham Source)。

CR Differential：上述两个计数率读数之差Calibration On(cps) - Background(cps)。

API Correction Factor：API校正因子(<b>GRAPICF</b>)，将原始计数率(cps)校正到工程单位(API)下。[Calibrator ON - Background] × GRAPICF即为标定API值。对于#1传感器，<u>2.2883=200/[93.88-6.48]</u>即为其API校正因子(<b>GRAPICF</b>)。

HV：作用于光电倍增管上的电压值。


Background(gAPI)：在无伽马源环境下测得的背景API值。

Calibration On(gAPI)：在已知刻度值伽马源环境下测得的API值。

Calibrator(gAPI)：已知刻度值伽马源标定器(Amersham Source)的名义API值。

对于每个四分区，LWD仪器中的处理器使用API校正因子(<b>GRAPICF</b>)将来自两个伽马闪烁记数器的计数率进行归一化处理("normalized" for the API correction factors)后传输到地面系统中，然后再乘以平均API校正因子来获取每个扇区的API读数(不明白为什么要这样做？)：

$$
\begin{align*}
& { CR }_ { Quadrant }=\frac { CR1\times API1+CR2\times API2 } { 2 }\times { (\frac { API1+API2 } { 2 } ) }^ { -1 } \\
& { API }_{ Quadrant }={ CR }_{ Quadrant }\times \frac { API1+API2 } { 2 } 
\end{align*}
$$

<h5><a name="sec-3-3">3.3 井场仪器验证(Wellsite Verification)</a></h5>

为了确保仪器工作正常，在每次入井前和出井后都要对仪器进行一次检查，在井场上只需要直接验证仪器对于背景伽马计数率的读数即可。此时必须保证在检测现场周围不存在其他伽马源(如密度和中子测井仪)或钢质构件等以免对读数造成影响。井场仪器验证报告如下图所示：

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pbm23oFTl29bBdSf8e_v5hlojpNIZFTaUW_0f9mb1DrfEaV69ZXYercIApqmEB7tWeIlLFL_zKX4lpz7t4M7SHPRie85uC1nVfrbt3eHFMkg/Gamma%20Ray%20pre-%20and%20post-run%20verification%20summary.png?psid=1">
<img class="aligncenter" title="Gamma Ray pre- and post-run verification summary" style="width:600px;height:270px;" src="https://lneprw.blu.livefilestore.com/y2pbm23oFTl29bBdSf8e_v5hlojpNIZFTaUW_0f9mb1DrfEaV69ZXYercIApqmEB7tWeIlLFL_zKX4lpz7t4M7SHPRie85uC1nVfrbt3eHFMkg/Gamma%20Ray%20pre-%20and%20post-run%20verification%20summary.png?psid=1" alt="Gamma Ray pre- and post-run verification summary"></a>

其中，Background(cps)为仪器在井场上所测得的背景伽马计数率，Standard Deviation(σ)为10次检测结果的标准偏差值。AA，BB，CC和DD的值设定为以车间标定值(shop calibration)为基准的-0.1σ & +10.0σ范围内的计数率。

温度突变可能造成检测值超出仪器的容许范围，因此在仪器出井后最好等待10分钟使得高压供电系统稳定后再进行检测。再次申明在检测时确保周围不存在其他的伽马射线源。

<h4><a name="sec-4">4 环境因素校正</a></h4>

对仪器进行标定可以保证不同型号的探测仪在参考标准环境下(10"井眼，内部充满密度为8.33ppg的水)都能得到统一的伽马测井曲线，然而我们需要得到的是纯地层的伽马射线曲线，这样就需要去除井眼尺寸和泥浆对原始测井曲线造成的影响。

<h5><a name="sec-4-1">4.1 环境影响因素</a></h5>

伽马探测仪测量的是整个环境中的伽马射线强度，因此我们必须将纯地层的伽马响应曲线从中分离出来。最主要的非地层伽马源来自于泥浆中的KCl，KOH和K-Lig等，这些都是泥浆中经常添加的化学药剂。泥浆中的钾核素将向外发射1.46MeV的单频谱伽马射线，他们分散到泥浆、钻铤中并被探测仪探测到，导致所测得的伽马射线强度要比纯地层的伽马测井响应大得多。钾核素校正的目的就在于设法移除泥浆中的钾元素对测井曲线造成的影响，而这种影响又是井眼尺寸、泥浆比重和泥浆中钾元素含量的函数。

此外，随着泥浆密度的增加，泥浆对伽马射线的衰减耗散效应逐渐增大，衰减程度与井眼尺寸以及泥浆密度有关，因此还需要对测井数据(<b>表观伽马读数，the apparent gamma value</b>)进行井眼尺寸和泥浆比重的校正计算。

在井场上，定向工程师需要随时记录泥浆的参数以及泥浆性能发生变化的具体时间。实时传输的伽马数据(real-time gamma data)使用最新的泥浆比重和钾元素含量进行校正，而存储的伽马数据(memory data)则在仪器出井后使用同步记录的泥浆参数进行校正。现场使用某一固定的井眼尺寸对伽马数据进行井眼尺寸的校正计算。如果可以获得井径数据(caliper data，如密度-声波偏距测井)，就可以对存储的伽马数据在井下进行实时的校正计算。

<h5><a name="sec-4-2">4.2 井眼尺寸与泥浆比重校正案例</a></h5>

给定以下信息，请确定经井眼尺寸与泥浆比重校正后的校正伽马API值(the corrected API gamma ray value)：

    泥浆密度：10lb/gal
    工具：OnTrak
    工具尺寸：4-3/4"
    井眼尺寸：7.5"
    表观GR：85API

首先在INTEQ Log Interpretation Chartbook中找出与4-3/4"OnTrak对应的校正曲线，然后根据泥浆密度与井眼尺寸从图中确定校正因子为0.9。伽马校正API值(the corrected API gamma ray value)为0.9×85=76.5API。

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2px97wVDI664Mx8CXtBUXwSSpeUVZXPU3AG_BiM_hJEVX5NtvjCKCXbko8-fjiMYLsFhd0Tadt4UGwFHLRwnP6_HWCEXIyOkolci0OuWFGs6I/4.75%20Borehole%20size%20and%20mud%20weight%20correction%20chart.png?psid=1">
<img class="aligncenter" title="4.75 Borehole size and mud weight correction chart" style="width:600px;height:400px;" src="https://lneprw.blu.livefilestore.com/y2px97wVDI664Mx8CXtBUXwSSpeUVZXPU3AG_BiM_hJEVX5NtvjCKCXbko8-fjiMYLsFhd0Tadt4UGwFHLRwnP6_HWCEXIyOkolci0OuWFGs6I/4.75%20Borehole%20size%20and%20mud%20weight%20correction%20chart.png?psid=1" alt="4.75 Borehole size and mud weight correction chart"></a>

<h5><a name="sec-4-3">4.3 钾元素校正案例</a></h5>

在自然界中钾的放射性同位素K40占全部钾元素的0.0118%，这部分伽马放射源必须从探测仪的伽马测井计数率中去除掉。钾元素校正图(potassium correction chart)中给出了<u>泥浆中每1 wt%钾元素所需要从伽马测井值中减除的API值</u>。

给定以下信息，请确定经钾元素校正、井眼尺寸和泥浆比重校正后的校正伽马API值(the corrected API gamma ray value)：

    泥浆添加剂：KCl=70000mg/l
    泥浆密度：10lb/gal
    工具：OnTrak
    工具尺寸：4-3/4"
    井眼尺寸：7.5"
    表观GR：85API

<b>第一步：</b>计算泥浆中钾元素的重量比例

相对原子质量：K=39.1 Cl=35.45

KCl中钾原子的重量比：39.1/(39.1+35.45)=0.525

70000mg/l溶液中总的钾原子质量(g)：70000×0.525/1000=36.75

将泥浆密度单位转换为g/cc[1g/cc = 8.33lb/gal]：10/8.33=1.198g/cc

1l泥浆的重量=1198g

泥浆中钾元素的重量比=36.75/1198=3%

如有其它含钾元素的添加剂，按上述步骤计算出各自的重量比然后加在一起。

<b>第二步：</b>确定每1 wt%钾元素的API校正值

在INTEQ Log Interpretation Chartbook中找出与4-3/4"OnTrak对应的钾元素校正曲线，然后根据井眼尺寸和泥浆密度确定每1 wt%钾元素的API校正值为2.5。

<b>第三步：</b>计算钾元素校正API值(potassium corrected API gamma ray value)

钾元素校正后的API值=85-2.5×3=77.5API

<b>第四步：</b><u>按照上一小节中给出的方法再根据井眼尺寸和泥浆密度对上面得到的钾元素校正值进行校正。</u>

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pLS7Q2DWxaHjT6Jg6S59uIBO6Oty6Hxokb6nqZVYopeeKQg-WqzVZKInvxyVxR-jRguNCquDoZPGP57NKm1qnSPovF5b2Akn6LK0Co1N2TNs/4.75%20Potassium%20Content%20correction%20chart.png?psid=1">
<img class="aligncenter" title="4.75 Potassium Content correction chart" style="width:600px;height:400px;" src="https://lneprw.blu.livefilestore.com/y2pLS7Q2DWxaHjT6Jg6S59uIBO6Oty6Hxokb6nqZVYopeeKQg-WqzVZKInvxyVxR-jRguNCquDoZPGP57NKm1qnSPovF5b2Akn6LK0Co1N2TNs/4.75%20Potassium%20Content%20correction%20chart.png?psid=1" alt="4.75 Potassium Content correction chart"></a>

<h5><a name="sec-4-4">4.4 钾元素泥浆报告(Potassium Content - Mud Report)</a></h5>

一般来说，只有在水基泥浆中才需要根据客户的要求进行KCl或K2CO3的API校正计算，油基泥浆中一般没有含钾元素的添加剂。

伽马探测仪会计算出<b>表观伽马计数率</b>(<b>GRA$</b>，其中\&#36;为X时表示实时传输值，\&#36;为M时表示存储值)和<b>校正伽马计数率</b>(<b>GRC$</b>，\&#36;意义同前)。如果在地面系统中输入了泥浆中的钾元素比例值，系统将对这两个参数都进行钾元素的校正计算；如果这个比例为0，那么将只对表观伽马计数率(GRA\&#36;)进行井眼尺寸和泥浆比重的校正计算，以进行下一步的校正伽马计数率(GRC\&#36;)的计算。在实时测井的Advantage地面系统中，钾元素比例在Real-Time Processing > MWD > Re-log Tare and Environmental Information路径下进行输入。在进行存储传输时Advantage Memproc将利用这个值对伽马计数率进行校正。

谨记所输入的钾元素比例必须为钾元素在泥浆中的质量百分比，因此在泥浆报告中KCl或K2CO3的数值必须是占整个钻井液(drilling mud)而非仅仅是泥浆滤液(mud filtrate)的比例(g/l)。下图给出了计算钾元素质量百分比的一般步骤：

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pWi2XlAlKl3d-vCvjPqhGvp2l4hskP_g5xVpOKh9R2mWAXvxH2s--KJIhDbhY-IQJD8z5Vc0qAg2HpghieET8s_ZRfjP7KhW8XAMb53WxtOQ/Basic%20Procedure%20to%20Obtain%20wt%20Percentage%20of%20K%20from%20Mud%20Report.png?psid=1">
<img class="aligncenter" title="Basic Procedure to Obtain wt Percentage of K from Mud Report" style="width:700px;height:260px;" src="https://lneprw.blu.livefilestore.com/y2pWi2XlAlKl3d-vCvjPqhGvp2l4hskP_g5xVpOKh9R2mWAXvxH2s--KJIhDbhY-IQJD8z5Vc0qAg2HpghieET8s_ZRfjP7KhW8XAMb53WxtOQ/Basic%20Procedure%20to%20Obtain%20wt%20Percentage%20of%20K%20from%20Mud%20Report.png?psid=1" alt="Basic Procedure to Obtain wt Percentage of K from Mud Report"></a>

以下为将泥浆滤液(mud filtrate)中的KCl含量(mg/liter)转换为钻井液(drilling mud)中KCl含量(mg/liter)的方法：

假定泥浆滤液中KCl含量为20200mg/l，泥浆中水的比例为80%(其他20%为Solids + Oil Fractions)。使用泥浆性质参考书(Mud Facts book)根据泥浆滤液中的KCl含量来获取KCl溶液的密度为1.011g/cm<sup>3</sup>或8.42lb/gal，因此可以得到KCl在钻井液中的密度为1.011×0.8=0.8088g/cm<sup>3</sup>。注意，KCl不溶于油相，且不以固态形式存在。

<h4><a name="sec-5">5 探测深度(Depth of Investigation)</a></h4>

从地层放射源发出的伽马射线在经过地层和泥浆到达伽马探测仪时会由于康普顿散射效应(Compton Scattering)发生衰减，衰减程度与地质环境以及泥浆密度等有关。一般估计认为，探测仪检测到的90%伽马射线来自于以6"为半径的球体地层内的伽马放射源。我们<u>将贡献50%伽马射线的球体地层半径定义为探测仪的探测深度</u>，显然它要小于6"(从井壁计算起)，而且随着泥浆和地层密度的增加还会进一步减小。

<h4><a name="sec-6">6 纵向分辨率(Vertical Resolution)</a></h4>

伽马探测仪的纵向分辨率与测井速度(R)、探测仪长度(L)和数据采集时间(DT)。通常LWD仪器的数据采集时间为4×2.5(10s采样率)，这样既能尽量降低仪器的固有统计涨落误差，又可以保证足够高的纵向分辨率。方位伽马探测仪的采样时间为25s。<u>INTEQ LWD的纵向分辨率大约为6"。</u>

<h4><a name="sec-7">7 伽马测井响应曲线</a></h4>

伽马测井曲线的显示范围通常在0-100或0-150API内，在套管内时伽马读数甚至会降到50API以下，伽马测井数据可以实时传输到地面上来也可以保存在井下工具的存储器中进行读取。

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pPJwlIsXljn6W2qJVr9zCNfsvk6d159whoLV7KjCfNhIYVoEX51gpmxNc2P1fKQsHdjZG9B31XFsmHPB2hNFXTNA63ayKh7n0qLGfvEj53sI/Gamma%20log%20presentation.png?psid=1">
<img class="aligncenter" title="Gamma log presentation" style="width:450px;height:210px;" src="https://lneprw.blu.livefilestore.com/y2pPJwlIsXljn6W2qJVr9zCNfsvk6d159whoLV7KjCfNhIYVoEX51gpmxNc2P1fKQsHdjZG9B31XFsmHPB2hNFXTNA63ayKh7n0qLGfvEj53sI/Gamma%20log%20presentation.png?psid=1" alt="Gamma log presentation"></a>

<h5><a name="sec-7-1">7.1 放射性涨落误差(Statistical Fluctuation)</a></h5>

自然伽马曲线不是一条光滑曲线，即使在岩性很均匀的地段曲线也有明显的起伏。这也是放射性测井曲线共同的特征，它是各种核物理现象和对这些现象的探测具有随机性和统计性特性的表示，通常称为放射性涨落变化。这些涨落性变化对其平均值形成的误差称为放射性测井曲线的涨落误差$ { \sigma } $，它包括两部分：曲线上没点计数率的涨落误差$ { \sigma  }_ { 1 } $和测量的平均计数率含有的涨落误差$ { \sigma  }_ { 2 } $，即$ \sigma ={ \sigma  }_ { 1 }+{ \sigma  }_{ 2 } $。

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pV0yhWkTlG98qPbBFMzpYd-W1fwgiZGYmFoJnQQhPVrxoqEoKvFOGdTrH0SDBbIG3EdSmgBe9oO24xip9w0Jm95WLhC3-FZO7EWIx1qDpG00/Statistical%20Fluctuation.png?psid=1">
<img class="aligncenter" title="Statistical Fluctuation" style="width:300px;height:490px;" src="https://lneprw.blu.livefilestore.com/y2pV0yhWkTlG98qPbBFMzpYd-W1fwgiZGYmFoJnQQhPVrxoqEoKvFOGdTrH0SDBbIG3EdSmgBe9oO24xip9w0Jm95WLhC3-FZO7EWIx1qDpG00/Statistical%20Fluctuation.png?psid=1" alt="Statistical Fluctuation"></a>

按照误差理论，在一个岩性均匀和厚度足够大的地层中，若自然伽马平均计数率为$\overline{n}$，则实测的自然伽马曲线在涨落范围$ (\overline { n } -\sigma )\sim (\overline { n } +\sigma ) $内的累积曲线厚度应占平均值曲线厚度的68.3%。达到这一要求的曲线，质量是好的，否则应视为质量不合格。只有明显超出涨落范围和有适当厚度的曲线变化才认为是岩性变化，应另分层或另作取值区。这一版凭经验判断，但也可取常数K=1.5~3.0，当曲线变化在$ \overline { n } \pm K\sigma $内时为同一地层，超出此范围应考虑另分层或另取值。

放射性曲线涨落误差还可以用来检查仪器的稳定性。同一个仪器，在同样的测量条件下对同一对象做多次测量，则每次平均计数$\overline{n}$落在$ \overline { n } \pm { \sigma  }_{ 1 } $范围内的概率应是68.3%，否则认为仪器稳定性或可重复性不好。

<h5><a name="sec-7-2">7.2 测井速度(Logging Speed)</a></h5>

由于存在放射性涨落变化，如果地层本身的伽马计数率比较高，那么就可以通过时间平均来降低这种放射性涨落误差，但往往地层中的伽马放射强度比较低，那么就必须考虑放射性涨落误差对伽马测井曲线造成的影响。在伽马探测仪中一般将一段时间内(Time Constant T<sub>c</sub>，时间常数)闪烁记数器采集到的伽马数量进行时间平均来降低这种统计涨落误差。

按照理论，我们应该尽量增加这个时间常数T<sub>c</sub>以获取更高质量的测井数据，然而随着测井仪器的不断移动，过大的时间常数T<sub>c</sub>会降低纵向分辨率(因为仪器会将这段时间内经过的地层伽马数量进行平均，从而使得地层边界处的伽马值对比度降低)。考虑到延长数据采集时间会引起钻井成本增加，我们必须设法在测井速度和测井质量之间取得一个妥协，在应用当中，通常规定仪器的测井速度(ft/s)与时间常数T<sub>c</sub>的乘积保持为1ft。这样，测井仪在经过1ft后将对上部1ft地层所测得的伽马数量进行时间平均，即伽马曲线值实际上是以1ft为单位的伽马射线强度平均值。

下表中给出了在具有稳定放射源的单一地层中统计涨落现象，伽马计数率和时间常数T<sub>c</sub>之间的相互影响关系，在这个例子中我们假定测井速度为1ft/s。如果时间常数为1/3s，在3s时间内就可以得到9个测量值，此时的纵向分辨率可以达到4in(每个不同的测量值即可认为属于不同的地层)，但这些伽马测量值在9-18之间不断发生变化。如果时间常数为1s，在3s时间内就可以得到3个测量值，此时的纵向分辨率为12in，但各个伽马测量值之间的误差要小得多(此时的变化范围缩小到了12-14之间)。如果时间常数设定得更高，此时所得到的伽马测量值的变化范围将更进一步缩小，但纵向分辨率却急剧下降，当T<sub>c</sub>=3s时，纵向分辨率降低到了3ft。从表中可以看出，当时间常数为1s时可以在测井数据的稳定性和纵向分辨率之间取得最佳平衡。

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pYQXdq8E0Xy946ZdBJqJK1M1iUmeclu-0py14bPvK_rBeCMklObRisApraJgFtPELFG3LGGS4oTKb_uWadmYLZOYk9InvfGzlDxC_37Spprc/Variations%20in%20count%20rate%20in%20gamma%20ray%20logging.png?psid=1">
<img class="aligncenter" title="Variations in count rate in gamma ray logging" style="width:700px;height:300px;" src="https://lneprw.blu.livefilestore.com/y2pYQXdq8E0Xy946ZdBJqJK1M1iUmeclu-0py14bPvK_rBeCMklObRisApraJgFtPELFG3LGGS4oTKb_uWadmYLZOYk9InvfGzlDxC_37Spprc/Variations%20in%20count%20rate%20in%20gamma%20ray%20logging.png?psid=1" alt="Variations in count rate in gamma ray logging"></a>

从下面这张图中也可以更直观地看到时间常数T<sub>c</sub>对伽马测井响应曲线所造成的影响：

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2p0Met8GGKKMvncwJyxte-3cXWwrRkEYtb9rc_ib6SVVOFv7OYE8wYMQ1hwykvzBZFDCPh9wsxCO_kOYsywVoeYntHOmv9l0jC7QUfwO5qWGo/Effect%20of%20Time%20Constant%20on%20Gamma%20Ray%20Response.png?psid=1">
<img class="aligncenter" title="Effect of Time Constant on Gamma Ray Response" style="width:500px;height:310px;" src="https://lneprw.blu.livefilestore.com/y2p0Met8GGKKMvncwJyxte-3cXWwrRkEYtb9rc_ib6SVVOFv7OYE8wYMQ1hwykvzBZFDCPh9wsxCO_kOYsywVoeYntHOmv9l0jC7QUfwO5qWGo/Effect%20of%20Time%20Constant%20on%20Gamma%20Ray%20Response.png?psid=1" alt="Effect of Time Constant on Gamma Ray Response"></a>

<h5><a name="sec-7-3">7.3 测井响应曲线(Primary Curves)</a></h5>

伽马测井响应曲线的标识符一般为XXX\&#36;，其中\\&#36;为X时表示实时传输值，\\&#36;为M时表示存储值。以下给出了三种不同伽马探测仪所能提供的伽马曲线：

单探测器伽马测井(Single detector)

<table id="customers" align="center">
<tr class="alt">
<td>GRAM</td>
<td>Gamma Ray - Apparent</td>
<td>API</td>
</tr>

<tr>
<td>GRBM</td>
<td>Gamma Ray - Base</td>
<td>cps</td>
</tr>

<tr class="alt">
<td>GRCM</td>
<td>Gamma Ray - Corrected</td>
<td>MWD-API</td>
</tr>

<tr>
<td>GRAFM</td>
<td>Gamma Ray - Filtered</td>
<td>API</td>
</tr>

<tr class="alt">
<td>GRCFM</td>
<td>Gamma Ray - Borehole Corrected - Filtered</td>
<td>API</td>
</tr>

<tr>
<td>GRIM</td>
<td>Gamma Ray - Data Point Indicator</td>
<td>point</td>
</tr>

<tr class="alt">
<td>GRSIM</td>
<td>Gamma Ray - Sliding Indicator</td>
<td>no units</td>
</tr>

<tr>
<td>GRTM</td>
<td>Gamma Ray - Time Since Drilled</td>
<td>minutes</td>
</tr>

<tr class="alt">
<td>GRDDM</td>
<td>Gamma Ray - Data Density</td>
<td>pts/ft</td>
</tr>
</table>

双探测器伽马测井(Dual detector，在以上曲线基础上再添加下列曲线)

<table id="customers" align="center">
<tr class="alt">
<td>GR1AM</td>
<td>Gamma Ray - Apparent - Detector 1</td>
<td>MWD-API</td>
</tr>

<tr>
<td>GR2AM</td>
<td>Gamma Ray - Apparent - Detector 2</td>
<td>MWD-API</td>
</tr>

<tr class="alt">
<td>GR1BM</td>
<td>Gamma Ray - Base - Detector 1</td>
<td>cps</td>
</tr>

<tr>
<td>GR2BM</td>
<td>Gamma Ray - Base - Detector 2</td>
<td>cps</td>
</tr>

<tr class="alt">
<td>GR1CM</td>
<td>Gamma Ray - Corrected - Detector 1</td>
<td>MWD-API</td>
</tr>

<tr>
<td>GR2CM</td>
<td>Gamma Ray - Corrected - Detector 2</td>
<td>MWD-API</td>
</tr>

<tr class="alt">
<td>GR1AFM</td>
<td>Gamma Ray - Detector 1 - Apparent - Filtered</td>
<td>API</td>
</tr>

<tr>
<td>GR2AFM</td>
<td>Gamma Ray - Detector 2 - Apparent - Filtered</td>
<td>API</td>
</tr>

<tr class="alt">
<td>GTFM</td>
<td>Gamma Tool-face</td>
<td>degrees</td>
</tr>
</table>

方位伽马探测器(Azimuthal Gamma，在以上曲线基础上再添加下列曲线)

<table id="customers" align="center">
<tr class="alt">
<td>GRAM</td>
<td>Gamma Ray</td>
<td>API</td>
</tr>

<tr>
<td>GRAS0M</td>
<td>Azimuthal Gamma Ray - Apparent - Sector 0</td>
<td>API</td>
</tr>

<tr class="alt">
<td>GRAS1M</td>
<td>Azimuthal Gamma Ray - Apparent - Sector 1</td>
<td>API</td>
</tr>

<tr>
<td>GRAS2M</td>
<td>Azimuthal Gamma Ray - Apparent - Sector 2</td>
<td>API</td>
</tr>

<tr class="alt">
<td>GRAS3M</td>
<td>Azimuthal Gamma Ray - Apparent - Sector 3</td>
<td>API</td>
</tr>

<tr>
<td>GRAS4M</td>
<td>Azimuthal Gamma Ray - Apparent - Sector 4</td>
<td>API</td>
</tr>

<tr class="alt">
<td>GRAS5M</td>
<td>Azimuthal Gamma Ray - Apparent - Sector 5</td>
<td>API</td>
</tr>

<tr>
<td>GRAS6M</td>
<td>Azimuthal Gamma Ray - Apparent - Sector 6</td>
<td>API</td>
</tr>

<tr class="alt">
<td>GRAS7M</td>
<td>Azimuthal Gamma Ray - Apparent - Sector 7</td>
<td>API</td>
</tr>
</table>

在能获取所有4个分区的伽马数据的情况下，可以使用RigLink 2.4 U2软件(或更高版本的应用程序)绘制出实时的变化图，如下图所示。

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pg0BIs9AcfC4I3mDZJcw-eSRxkFgMUYaufpD-KN3M7tawhWM73nK51t5lrzavgnEaPms5VbPyM_eTtH0H7y_0dQWZ5uE9P-mxLyZisgQU1R0/RigLink.png?psid=1">
<img class="aligncenter" title="RigLink" style="width:600px;height:450px;" src="https://lneprw.blu.livefilestore.com/y2pg0BIs9AcfC4I3mDZJcw-eSRxkFgMUYaufpD-KN3M7tawhWM73nK51t5lrzavgnEaPms5VbPyM_eTtH0H7y_0dQWZ5uE9P-mxLyZisgQU1R0/RigLink.png?psid=1" alt="RigLink"></a>

高级伽马存储器中的数据经过MemProc处理后可以导出到ASCII格式或xtf格式的文件中。图形包Case可如下图那样绘制静态彩色图像(从xtf文件输入原始数据)。其中纵向与横向的内插值均可由用户自行定义。


<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pQRF7lmPAPTb_0AENiCyAMUK4yHCRwW3uVnk5ji2GuZWtLRG2N8Ecv71NTkExCh_JiaY06mwN9dAlOFEtqmwuMHInmhnxVdtQzF8NxRqJBOk/Sectored%20Gamma%20Data.png?psid=1">
<img class="aligncenter" title="Sectored Gamma Data" style="width:300px;height:450px;" src="https://lneprw.blu.livefilestore.com/y2pQRF7lmPAPTb_0AENiCyAMUK4yHCRwW3uVnk5ji2GuZWtLRG2N8Ecv71NTkExCh_JiaY06mwN9dAlOFEtqmwuMHInmhnxVdtQzF8NxRqJBOk/Sectored%20Gamma%20Data.png?psid=1" alt="Sectored Gamma Data"></a>

根据用户需求，贝克阿特拉斯地质部(Baker Atlas GeoScience department)可以提供地质构造解释以及地层倾角等高级后处理功能。

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pqwghilmjcDShGS3QwtQ6Bk0lLTyt6DHBXPW5jNs7BeFUgl_bzAogTJ46SrVxZS_RYCoVaA8z7m4hygxmPd-MR7j5rEi8NeglvLYPjWb2BpQ/Dip%20Picking.png?psid=1">
<img class="aligncenter" title="Dip Picking" style="width:660px;height:640px;" src="https://lneprw.blu.livefilestore.com/y2pqwghilmjcDShGS3QwtQ6Bk0lLTyt6DHBXPW5jNs7BeFUgl_bzAogTJ46SrVxZS_RYCoVaA8z7m4hygxmPd-MR7j5rEi8NeglvLYPjWb2BpQ/Dip%20Picking.png?psid=1" alt="Dip Picking"></a>

<h4><a name="sec-8">8 数据遥测(Telemetry)</a></h4>

遥测所需的各扇区每秒接收到的信号数量(CPS)可以通过以下两种方式得到：

<ul style="margin-left:50px;">
<li>使用更加可靠的双探测器模式("归一化方法")，或者</li>
<li>单独选择A通道或B通道(如果其中之一发生故障的话)</li></ul>

接头可以自动检测闪烁计数器的好坏，如果检测到其中一个闪烁计数器发生了故障，接头将自动切换到单通道模式下发送实时计数数据。

由于接头具有自动检测功能，因此通过下行指令指定某一个或同时指定两个探测器来进行实时数据传输并不会对方位伽马的测量精度产生任何影响。

四个区域的信号频率经过归一化后进行上行传输：

<table id="customers" align="center" style="width:80%;">
<caption>伽马信号</caption>
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

对于井下伽马测井仪的数据存储模式，请参考OnTrak Sensor Sub中遥测部分的相关内容。

下面以单探测器伽马测井实时传输模式为例介绍伽马数据的传输与处理过程。我们在前面标定一节中已经得到了伽马API校正因子(GRAPICF)，将原始伽马计数率GRBX乘以这个校正因子(如需进行钾元素校正，还需要将钾元素质量百分比输入到Advantage中进一步进行校正)，就得到了表观伽马值GRAX。接着，Advantage会根据输入的井眼尺寸和泥浆比重对GRAX进行几何校正，得到归一化到充满密度为8.33ppg水的10"井眼参考标准下的修正伽马API值GRCX。基本的数据处理流程如下所示：

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2p1Ye7bjpFVyD6A1pD1o04cuUyR3dkOWTH5RIfYSjXDQTu7WYzz3mnVWRR1YOgrS1UQXHiR5e8jD93UpWR5dUpVqqwLoW7e8toa1O93RqGqLc/Flow%20Chart%20of%20Gamma%20Log%20Processing.png?psid=1">
<img class="aligncenter" title="Flow Chart of Gamma Log Processing" style="width:700px;height:380px;" src="https://lneprw.blu.livefilestore.com/y2p1Ye7bjpFVyD6A1pD1o04cuUyR3dkOWTH5RIfYSjXDQTu7WYzz3mnVWRR1YOgrS1UQXHiR5e8jD93UpWR5dUpVqqwLoW7e8toa1O93RqGqLc/Flow%20Chart%20of%20Gamma%20Log%20Processing.png?psid=1" alt="Flow Chart of Gamma Log Processing"></a>

在上图中，对表观伽马API值GRAX和修正伽马API值GRCX还可以进行滤波处理，分别得到<b>滤波表观伽马API值GRAFX</b>和<b>滤波修正API值GRCFX</b>，如下图所示：

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pTWBp63q7sTlkIEmG7WHVcxwcujekNZzAj8KEJ7Rihi4MUTNI4LQsNp47pblOR2qdAxTFV2O9AWIV1pnDn9XzlnGSdxbV5S6iDWxGlrHxD-M/08%20MPR%20PRESSTEQ%20GAMMA-RES_Day7-StudentGuide.bmp?psid=1">
<img class="aligncenter" title="08 MPR PRESSTEQ GAMMA-RES_Day7-StudentGuide" style="width:700px;height:450px;" src="https://lneprw.blu.livefilestore.com/y2pTWBp63q7sTlkIEmG7WHVcxwcujekNZzAj8KEJ7Rihi4MUTNI4LQsNp47pblOR2qdAxTFV2O9AWIV1pnDn9XzlnGSdxbV5S6iDWxGlrHxD-M/08%20MPR%20PRESSTEQ%20GAMMA-RES_Day7-StudentGuide.bmp?psid=1" alt="08 MPR PRESSTEQ GAMMA-RES_Day7-StudentGuide"></a>

<h4><a name="sec-9">9 伽马曲线的应用</a></h4>

<h5><a name="sec-9-1">9.1 划分岩性和地层对比(Lithology Identification)</a></h5>

根据不同的岩性自然伽马射线强度不同可以划分岩性。在自然伽马测井曲线上，泥岩和页岩(shale)显示明显的放射性，而且可以连成一条相当稳定的泥岩线。超过这条泥岩线的是岩浆岩(igneous，如花岗岩granite)、富含放射性矿物的砂岩(sandstone)或石灰岩(limestone)及海相泥岩(marine mudstone)等。石膏(gypsum)、硬石膏(anhydrite)、岩盐(halite)和纯的石灰岩、白云岩(dolomite)的放射性很低，形成井剖面上的基值线，白云岩往往比石灰岩具有较高的放射性，这是由于含放射性物质的地层水在碳酸盐白云岩化的过程中将放射性物质带入了岩石。

<p style="text-align:center;">
<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pXMAeBR758IvZWRAt2Lo9GKEwL6BkWPCNwipxjbzpq56dz9q_q1VmmtVimzWClZnbw47DBVNKS7CRDTQNzg6-knpOx2AnnLhqhWFwzqgFUkE/Gamma%20Log%20Lithology%20Determination.bmp?psid=1">
<img title="Gamma Log Lithology Determination" style="width:450px;height:600px;" src="https://lneprw.blu.livefilestore.com/y2pXMAeBR758IvZWRAt2Lo9GKEwL6BkWPCNwipxjbzpq56dz9q_q1VmmtVimzWClZnbw47DBVNKS7CRDTQNzg6-knpOx2AnnLhqhWFwzqgFUkE/Gamma%20Log%20Lithology%20Determination.bmp?psid=1" alt="Gamma Log Lithology Determination"></a>
<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pcmsQUAjfhOWETHpgb_erCIzXEi0ejxDJvBCPyKq05A9XvXT6oq5YJA_wNHF6IKJjjP8iEFPeCgCA-PbvMnpZCHsD5JKFs1iCBr7cZzuEu4w/Determination%20of%20Lithology.png?psid=1">
<img title="Determination of Lithology" style="width:450px;height:600px;" src="https://lneprw.blu.livefilestore.com/y2pcmsQUAjfhOWETHpgb_erCIzXEi0ejxDJvBCPyKq05A9XvXT6oq5YJA_wNHF6IKJjjP8iEFPeCgCA-PbvMnpZCHsD5JKFs1iCBr7cZzuEu4w/Determination%20of%20Lithology.png?psid=1" alt="Determination of Lithology"></a></p>

在砂泥岩剖面中，纯砂岩在自然伽马曲线上显示为最低值，而泥岩显示为最高值，粉砂岩(siltstone)、泥质砂岩介于中间，并随着砂岩中含泥量的增高自然伽马读数也增高。

在碳酸盐岩剖面中，粘土岩(泥岩、页岩)的自然伽马读数最高，纯的石灰岩、白云岩读数最低，而泥质岩、泥质灰岩、泥质白云岩介于两者之间，且随泥质含量增加而增高。

在砂泥岩剖面，低自然伽马异常一般就是砂岩储集层，异常半幅点确定储集层界面。在碳酸盐岩剖面，低自然伽马异常只指出泥质含量较少的纯岩石，而是否为储集层，还必须有相对高一点的孔隙度显示和明显低的电阻率显示，这些事纯岩石发育裂缝带的特征。如果砂泥岩剖面岩性复杂，也应按此判断。

<h5><a name="sec-9-2">9.2 计算地层泥质含量(Determination of Shale Content)</a></h5>

当地层不含泥质以外的放射性物质时，自然伽马曲线时指示地层泥质含量的最好方法。如前所述，地层的自然伽马异常随泥质含量含量增加而减小。经过适当的刻度，便可用自然伽马异常计算地层泥质含量。

纯泥岩泥质含量V<sub>sh</sub>=100%，将纯泥岩线的自然伽马读数记为GR<sub>max</sub>。而纯岩石V<sub>sh</sub>=0，将其自然伽马读数记为GR<sub>min</sub>。若解释层的自然伽马读数为GR<sub>log</sub>，则比值$ ({ GR }_ { log }-{ GR }_ { min })/({ GR }_ { max }-{ GR }_{ min }) $应当同地层泥质含量密切相关。通常将这一比值称为<b>自然伽马相对值或泥质含量指数(I<sub>GR</sub>)</b>，对纯岩石为0，对纯泥岩为100%，记为

$$
\begin{align*}
& { I }_{ GR }=\frac { { GR }_{ log }-{ GR }_{ min } }{ { GR }_{ max }-{ GR }_{ min } }
\end{align*}
$$

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2p4ynnoHH4CmN5L8V-TEgyXH_Rdew6erbf2njtxkdvWH-1ZoNVOcho01Klc_5RWLvA7uISe2ia8k7TJQD3yI5IZQStX9G8kNvo8lJ4Eo-xI78/Shale%20Volume%20Calculation.bmp?psid=1">
<img class="aligncenter" title="" style="width:400px;height:480px;" src="https://lneprw.blu.livefilestore.com/y2p4ynnoHH4CmN5L8V-TEgyXH_Rdew6erbf2njtxkdvWH-1ZoNVOcho01Klc_5RWLvA7uISe2ia8k7TJQD3yI5IZQStX9G8kNvo8lJ4Eo-xI78/Shale%20Volume%20Calculation.bmp?psid=1" alt=""></a>

很多地质学家都简单地将地层中的泥质含量等同于上面的泥质含量指数V<sub>sh</sub>=I<sub>GR</sub>，但严格来说应如下图所示根据SHI来查找相应的地层泥质含量。影响计算结果的另两个参数是GR<sub>max</sub>和GR<sub>min</sub>，不能简单地把它们理解成自然伽马的最大值和最小值。GR<sub>max</sub>应是本井段纯泥岩自然伽马平均值，在泥岩中是最大的，应当把其它高放射性岩石的读数排除在外。GR<sub>min</sub>应是本井段最纯的储集层岩石(V<sub>sh</sub>=0)的自然伽马读数，在储集层中应是最小的，如果没有纯岩石，GR<sub>min</sub>可比实际最小值略低一些。

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2p_Iv4Rp-DZFaP_8l_QmouuP6DKVw4vNBvEA5VmGOUbnkXJO4PXU3MbBnSQpxQn55ty-4HeK_3tazAWJ3ttBnm2s8dSElIfLDKCJPEDQroY8s/Calculation%20of%20Shale%20Volume.png?psid=1">
<img class="aligncenter" title="Calculation of Shale Volume" style="width:550px;height:500px;" src="https://lneprw.blu.livefilestore.com/y2p_Iv4Rp-DZFaP_8l_QmouuP6DKVw4vNBvEA5VmGOUbnkXJO4PXU3MbBnSQpxQn55ty-4HeK_3tazAWJ3ttBnm2s8dSElIfLDKCJPEDQroY8s/Calculation%20of%20Shale%20Volume.png?psid=1" alt="Calculation of Shale Volume"></a>

<h5><a name="sec-9-3">9.3 地质导向(Geo-Steering)</a></h5>

利用分区方位伽马的读数差异可以实时了解井下钻进岩性并计算地层分界面的地质倾角。如下图所示，伽马探测仪向地面实时传输上下左右四个分区的伽马数据，从上面的两条曲线可以看出，上四分区伽马读数落后5m才检测到新的地层，这说明钻头正进入到泥质含量较少的地层中，且地层倾角是沿着井眼方向向右下倾斜的。从下面的四分区热力图像中也可以得到同样的结论。

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pO_GCfduFLoN8Hen1gmzthnHQM1rd4dpV9L_BMRT3RD-pAfann2OJyY1e9oceMlGA1VsF071oorxI1fwHJxU6oWYlhrC9z4hJ1M_4Qk1czAY/Azimuthal%20Gamma%20Geo-Steering.png?psid=1">
<img class="aligncenter" title="Azimuthal Gamma Geo-Steering" style="width:600px;height:470px;" src="https://lneprw.blu.livefilestore.com/y2pO_GCfduFLoN8Hen1gmzthnHQM1rd4dpV9L_BMRT3RD-pAfann2OJyY1e9oceMlGA1VsF071oorxI1fwHJxU6oWYlhrC9z4hJ1M_4Qk1czAY/Azimuthal%20Gamma%20Geo-Steering.png?psid=1" alt="Azimuthal Gamma Geo-Steering"></a>

下图中给出了一个计算地质倾角的实例，图中的X为上下四分区分别接触到地层分界面时钻头钻进的距离：

<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pUDa_s2tDxq8f1-ONruKvhNicnH6_S8_zyTPREMFgWqywihQGVjuoqlyJmnAISO9VqTX1F5199M-wK_XxDTLVvVJ6tpJXYxdX5Xwiy5BwT8Q/Example%20showing%20UP-DOWN%20quadrant%20data%20for%20an%20inclined%20bed.bmp?psid=1">
<img class="aligncenter" title="Example showing UP-DOWN quadrant data for an inclined bed" style="width:700px;height:300px;" src="https://lneprw.blu.livefilestore.com/y2pUDa_s2tDxq8f1-ONruKvhNicnH6_S8_zyTPREMFgWqywihQGVjuoqlyJmnAISO9VqTX1F5199M-wK_XxDTLVvVJ6tpJXYxdX5Xwiy5BwT8Q/Example%20showing%20UP-DOWN%20quadrant%20data%20for%20an%20inclined%20bed.bmp?psid=1" alt="Example showing UP-DOWN quadrant data for an inclined bed"></a>


<a target="_blank" href="https://lneprw.blu.livefilestore.com/y2pSjxO_-E84LdpBZUQV2OhtMxOgFEnNCpI6OrPStOVlooTcIf8YpK1GqwL7GHZCf-udsUZcquzdxXD1NFDwon436Vv_vE5MDyjQeJxUSIdZfs/Geo-Steering%20Schematic.png?psid=1">
<img class="aligncenter" title="Geo-Steering Schematic" style="width:600px;height:300px;" src="https://lneprw.blu.livefilestore.com/y2pSjxO_-E84LdpBZUQV2OhtMxOgFEnNCpI6OrPStOVlooTcIf8YpK1GqwL7GHZCf-udsUZcquzdxXD1NFDwon436Vv_vE5MDyjQeJxUSIdZfs/Geo-Steering%20Schematic.png?psid=1" alt="Geo-Steering Schematic"></a>

除了上面所介绍的三种主要应用外，利用伽马测井曲线还可以确定地层的粒度中值，与其他工具一起进行深度匹配，进行漏点、漏层等固井质量的检查等。

<h4><a name="sec-10">10 LWD伽马测井仪与电缆伽马测井仪的区别</a></h4>

由于电缆测井的速度(1800ft/hr)比LWD测井速度(200ft/hr)快得多，因此电缆测井曲线的统计性涨落误差也要大得多，两者的伽马曲线不可能完全重合。

电缆伽马测井仪直接检测地层的真实API读数，而LWD伽马测井仪则通过测量伽马计数率得到原始伽马数据后再转化为地层的API值。此外，LWD伽马探测器外的钻铤厚度可达1/2"~3"，电缆伽马探测器外壳的厚度只有1/4"~3/8"，这就导致LWD伽马测井仪的伽马能谱带向钾元素的特征峰发生偏移(因为钍和铀更容易受到康普顿散射效应的影响)，特别是在含钍和铀较多的地层中钻进时，LWD伽马曲线要比电缆伽马测井曲线低得多。但经过井眼几何校正后，这两种伽马测井结果可以得到比较一致的结果。

由于LWD伽马测井仪的测井速度较慢，其纵向分辨率得到明显的提高，而且LWD随钻伽马测井能实时获取钻时地层伽马值，减少了井眼校正的不确定性。除此以外，LWD伽马测井仪较厚的外壳也能使得伽马探测器尽量降低受到来自泥浆的不利影响。在每次入井测试时，电缆伽马测井仪在井中的居中度都不可能在一定范围内保证一致(相比LWD伽马测井仪而言)，因此电缆伽马测井仪的可重复性也不如LWD伽马测井仪。

<h4><a name="sec-10">10 LWD伽马测井仪与电缆伽马测井仪的区别</a></h4>

由于电缆测井的速度(1800ft/hr)比LWD测井速度(200ft/hr)快得多，因此电缆测井曲线的统计性涨落误差也要大得多，两者的伽马曲线不可能完全重合。

电缆伽马测井仪直接检测地层的真实API读数，而LWD伽马测井仪则通过测量伽马计数率得到原始伽马数据后再转化为地层的API值。此外，LWD伽马探测器外的钻铤厚度可达1/2"~3"，电缆伽马探测器外壳的厚度只有1/4"~3/8"，这就导致LWD伽马测井仪的伽马能谱带向钾元素的特征峰发生偏移(因为钍和铀更容易受到康普顿散射效应的影响)，特别是在含钍和铀较多的地层中钻进时，LWD伽马曲线要比电缆伽马测井曲线低得多。但经过井眼几何校正后，这两种伽马测井结果可以得到比较一致的结果。

由于LWD伽马测井仪的测井速度较慢，其纵向分辨率得到明显的提高，而且LWD随钻伽马测井能实时获取钻时地层伽马值，减少了井眼校正的不确定性。除此以外，LWD伽马测井仪较厚的外壳也能使得伽马探测器尽量降低受到来自泥浆的不利影响。在每次入井测试时，电缆伽马测井仪在井中的居中度都不可能在一定范围内保证一致(相比LWD伽马测井仪而言)，因此电缆伽马测井仪的可重复性也不如LWD伽马测井仪。

<h4><a name="sec-10">11 伽马测井曲线质量控制(Gamma Log Quality Control)</a></h4>

请参考08 MPR PRESSTEQ GAMMA-RES_Day 7-StudentGuide.pdf中相应章节中的内容。
