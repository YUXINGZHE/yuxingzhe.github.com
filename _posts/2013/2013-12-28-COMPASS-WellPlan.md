---
layout: post
title: "COMPASS WELLPLAN FOR WINDOWS 功能简介"
tags: [COMPASS]
author_name: YUXINGZHE
author_uri: http://twitter.com/yuxingzhe
---

<div id="table-of-contents">
<h2>目录</h2>
<div id="text-table-of-contents">
<ul>
    <li><a href="#sec-1">1.COMPANY SETUP - CREATE NEW COMPANY：公司设置-建立新的公司</a></li>
    <li><a href="#sec-2">2.PROJECT SETUP- CREATE NEW FIELD：项目设置-建立新的油气田</a></li>
    <li><a href="#sec-3">3.SITE SETUP- CREATE NEW SITE：区块设置-建立新的区块</a></li>
    <li><a href="#sec-4">4.WELLSETUP-CREATE NEW WELL：单井设置-建立新井</a></li>
    <li><a href="#sec-5">5.WELLPATH SETUP-CREATE NEW WELLPATH：轨迹设置-建立新的轨迹</a></li>
    <li><a href="#sec-6">6.TARGET EDITOR：靶点编辑器</a></li>
    <li><a href="#sec-7">7.NEW PLAN & OPEN PLAN：井眼轨迹设计</a></li>
    <li><a href="#sec-8">8.NEW SERVEY& OPEN SERVEY：实测数据建立与编辑</a></li>
    <li><a href="#sec-9">9.ANTICOLLISION：防碰计算</a></li>
    <li><a href="#sec-10">10.常用功能简介</a></li>
</ul>
</div></div>


<span class="dropcap">C</span>OMPASS(指南针)有三个核心功能：

<ul style="margin-left:50px;">
<li>PLANNING(设计)&#32;&#32;&#32;&#32;&#32;按计划井眼形状设计井眼轨迹</li>
<li>SURVEY(实测计算)&#32;&#32;&#32;&#32;&#32;已钻井眼实测数据的计算及轨迹预测</li>
<li>ANTICOLLISION(防碰计算)&#32;&#32;&#32;&#32;&#32;井眼轨迹之间的距离计算</li></ul>

除此之外，COMPASS还有以下功能：

<ul style="margin-left:50px;">
<li>COMPANY SETUP&#32;&#32;&#32;&#32;&#32;允许你为不同的公司设置COMPASS</li>
<li>PROJECT SETUP&#32;&#32;&#32;&#32;&#32;为同一油田的所有平台定义通用的水平或垂直参考系统</li>
<li>TARGET EDITOR&#32;&#32;&#32;&#32;&#32;靶点编辑器，设置靶点位置及靶区形状</li>
<li>TEMPLATE EDITOR&#32;&#32;&#32;&#32;&#32;井口编辑器，用于丛式井井口坐标计算</li>
<li>REFERENCE DATUM ELEVATIONS&#32;&#32;&#32;&#32;&#32;定义不同的海拔高度参照基准</li>
<li>MAGNETIC CALCULATOR&#32;&#32;&#32;&#32;&#32;计算不同磁场模型的磁场值</li>
<li>GEODETIC CALCULATOR&#32;&#32;&#32;&#32;&#32;不同地质坐标系之间的数值转换计算</li>
<li>SURVEY TOOLS&#32;&#32;&#32;&#32;&#32;定义不同测量工具的测量误差</li></ul>

<h4><a name="sec-1">COMPANY SETUP - CREATE NEW COMPANY公司设置-建立新的公司</a></h4>

建立一个新的公司，实际上就是为你建立的这个新公司对COMPASS软件进行一些基础参数设置，也就是COMPANY SETUP(公司设置)。下面按步骤说明：

<ol>
<li>在菜单栏上单击File 菜单，选取New Company选项或单击工具栏中<img src="https://qgiqmw.blu.livefilestore.com/y2pvUkkpr4eKndk7FvP-Z1RoKqY9yOR_WdZRQPMLXsLSKPmPBTtM8FGVGv0voozdhvXKVP4GKe5JuAUcUFVYfKKaAuMWGDKcQNSNYN0jHHzQsY/Company%20Setup.png?psid=1" alt="Company Setup">图标(编辑当前已打开公司)，将会出现以下对话框：</li>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2pDm2y2McUQn0iucL7nAd99q-7zOPbeC2p3IwsS6Q3Azl-YsCJKJ23r4-uHlLGE8hUu5F41Fmmj4I9kUx3Ha6ynQ5C4L25BcC7f9V1NDVQMiE/Company%20Properties.png?psid=1">
<img class="aligncenter" title="Company Properties" style="width:480px;height:450px;" src="https://qgiqmw.blu.livefilestore.com/y2pDm2y2McUQn0iucL7nAd99q-7zOPbeC2p3IwsS6Q3Azl-YsCJKJ23r4-uHlLGE8hUu5F41Fmmj4I9kUx3Ha6ynQ5C4L25BcC7f9V1NDVQMiE/Company%20Properties.png?psid=1" alt="Company Properties"></a>

<li>对话框中：在Company栏填入所在公司的名称，Division栏中填入子公司或专业公司的名称，Group栏中填作业组的名称。Logo下拉栏中可以选择已制作好的公司标志，用在图形或报告中。</li>

<li>选中Locked复选框后，在COMPASS中的一些缺省值将不能被改动。可以配合密码使用，单击Company Level和Locked Data旁边的按钮，在出现的对话框中可输入密码。</li>

<li>Anticollision防碰参数设定：Survey Error Model下拉栏中可以选择所需的系统误差模型，一般选择<b>ISCESA</b>；Anticollision Setting中的Scan 下拉栏中可以选择扫描模式，一般选择<b>Closest Approach 3D</b>；Error下拉栏中选择表面形状误差，一般为<b>Elliptical Conic</b>(椭圆锥体)。Warning Levels对话框中可以设定防碰警告距离。</li>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2p91JqYVt0D_GjxelHyggPtKgl-UuTDLCi2AMjTmvwzM6epldR3uv5Da1jazMg4CJQwxEFPWVcWvCfxet5-25H7MLgPBVPFamVJgfyYzbx89k/Anticollision%20Preference.png?psid=1">
<img class="aligncenter" title="Anticollision Preference" style="width:480px;height:450px;" src="https://qgiqmw.blu.livefilestore.com/y2p91JqYVt0D_GjxelHyggPtKgl-UuTDLCi2AMjTmvwzM6epldR3uv5Da1jazMg4CJQwxEFPWVcWvCfxet5-25H7MLgPBVPFamVJgfyYzbx89k/Anticollision%20Preference.png?psid=1" alt="Anticollision Preference"></a>

<li>在Calc Defaults(缺省值)对话栏中，可以在Survey Calculation Method下拉栏中选择实测计算方法(包括最小曲率、曲率半径、平均角、平衡切线等方法)，一般为<b>Minimum Curvature</b>(最小曲率)。而在下面的起始点设定中，可以设定V.Section Origin(垂直投影剖面原点)在Slot(井口)或Site(区块中心)，一般选<b>Slot</b>；在Walk/Turn Rate中设定比率基准，一般以<b>MD</b>(斜深)为基准。Validation中为变坐标系统下对相关数据进行重新计算。</li>

<li>在如图选中公司后下面的视图中点击Survey Tools可以打开测井工具的设置界面，在这个界面中可以新建所使用的测井工具，并设置该工具的误差模型。</li></ol>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2p_6KsZge4pPkiJv2VXoA6WZumqZjH_OXlcplkyKNq7dlJLyMgklQF_Yn6ILZJuKI6AUKp7Q7YT2UCUHanZ1gs9CPKhIWAxePLAsQ13CBbdJ0/Survey%20Tool%20Setup.png?psid=1">
<img class="aligncenter" title="Survey Tool Setup" style="width:500px;height:270px;" src="https://qgiqmw.blu.livefilestore.com/y2p_6KsZge4pPkiJv2VXoA6WZumqZjH_OXlcplkyKNq7dlJLyMgklQF_Yn6ILZJuKI6AUKp7Q7YT2UCUHanZ1gs9CPKhIWAxePLAsQ13CBbdJ0/Survey%20Tool%20Setup.png?psid=1" alt="Survey Tool Setup"></a>

<h4><a name="sec-2">PROJECT SETUP - CREATE NEW FIELD项目设置-建立新的油气田</a></h4>

新油气田的建立，是对一个将要开发的油气田进行包括地质系统、海拔基准等在内的基础参数进行设定(PROJECT SETUP)。每个公司下可以建立多个油气田。下面按步骤说明：

<ol>
<li>在菜单栏上单击File 菜单，选取New Field选项或单击工具栏中<img src="https://qgiqmw.blu.livefilestore.com/y2p-HxRRT4FChH-4uX1XolncEJSH_wuxSrTRDeHAkwVpD3hUE8sbrK_tB4AYJS0FQKnlorzzgVXUGwVfOue1t__KE91krzX_qBrndevLkvFVxU/Project.png?psid=1" alt="Project">图标(编辑当前已打开油气田)，将会出现以下对话框：</li>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2pl_PF28R2EWMOyI5vdbUxE5U_XFTxzhMZqUmBIq2m2l34y_BaqxRQ1NGq1k8ev1Mn675Ws5QZSReJavD1e4LXmjwThnNsIyIjj62xJj97_4Y/Project%20Properties-General.png?psid=1">
<img class="aligncenter" title="Project Properties-General" style="width:460px;height:390px;" src="https://qgiqmw.blu.livefilestore.com/y2pl_PF28R2EWMOyI5vdbUxE5U_XFTxzhMZqUmBIq2m2l34y_BaqxRQ1NGq1k8ev1Mn675Ws5QZSReJavD1e4LXmjwThnNsIyIjj62xJj97_4Y/Project%20Properties-General.png?psid=1" alt="Project Properties-General"></a>

<li>对话框中，Project栏中填入油气田的名称；Location栏填入油气田所在地区的描述或其他相关信息(可不填)；选中Project is locked复选框，可设置锁，避免被他人或无意中修改。</li>

<li>System Datum Description下拉栏中选择系统垂直基准面(一般以海平面为基准，<b>Mean Sea Level</b>)。Survey References中的Default Magnetic为磁偏角模型，一般选取最新模型即可。Project Unit选择计算单位，一般选择公制单位SI。</li>

<li>在Geodetic system、Geodetic Datum、Map Zone这三个下拉栏中，可以选择不同的大地坐标投影系统、投影形状基准及其所在区域(一般就是地理东西坐标前两位)，以备计算大地坐标之用，一般选取Gauss-Kruger (Pulkovo 1942) Coordinate Systems(坐标系不同时，需选择Flat Earth)。Local Coordinate System为本地参考坐标系统，单井设计一般选取Well Center即可。</li></ol>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2pfVWZ2x13lS5PqDitOMS4Tn7-v9t5Ku5b2_cuDptQkp4cvKHdRU4I0NMSHElEW90dfIrtVP8N8Vg5u9vPQI7qiS_ElygUEI1XunROnEE5wVU/Project%20Properties-Map%20Info.png?psid=1">
<img class="aligncenter" title="Project Properties-Map Info" style="width:460px;height:390px;" src="https://qgiqmw.blu.livefilestore.com/y2pfVWZ2x13lS5PqDitOMS4Tn7-v9t5Ku5b2_cuDptQkp4cvKHdRU4I0NMSHElEW90dfIrtVP8N8Vg5u9vPQI7qiS_ElygUEI1XunROnEE5wVU/Project%20Properties-Map%20Info.png?psid=1" alt="Project Properties-Map Info"></a>


<h4><a name="sec-3">SITE SETUP - CREATE NEW SITE区块设置-建立新的区块</a></h4>

这里讲的区块是指，在一个将要开发的油气田中，可能分为一个或多个小区建一个或多个平台进行开发。一个区块就是一个平台。建立新区块，需输入这个区块的基本参数，包括中心坐标、水深等，下面按步骤说明：

<ol>
<li>在菜单栏上单击File菜单，选取New Site选项或单击工具栏中<img src="https://qgiqmw.blu.livefilestore.com/y2pKfziKqLReTeK7Y1D5QFc5LimELHQIsCNJx5UvUf3W9r1QN3GG6U7uUa6Njb2xPmVuBLQUs9doM4kyaiKYf0Qp3tvlaKNolhDTAmvAkLtosE/Site.png?psid=1" alt="Site">图标(编辑当前已打开区块)，将会出现以下对话框：</li>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2p4KJKMDAHI5KFI2cp3hVO5bQ-G2UoH9eLDWx1AUfkIOdbpwO_s5z5axsxUcxjb8Kqm8S6cPzYbV-DC3ODhhMp4oZCCZcauyfutCpiUxRpTTg/Site%20Properties-General.png?psid=1">
<img class="aligncenter" title="Site Properties-General" style="width:500px;height:300px;" src="https://qgiqmw.blu.livefilestore.com/y2p4KJKMDAHI5KFI2cp3hVO5bQ-G2UoH9eLDWx1AUfkIOdbpwO_s5z5axsxUcxjb8Kqm8S6cPzYbV-DC3ODhhMp4oZCCZcauyfutCpiUxRpTTg/Site%20Properties-General.png?psid=1" alt="Site Properties-General"></a>

<li>Site栏中填入区块或平台名称，District栏中填入区块或平台的区域信息或其他描述(可不填)，选中Site is locked复选框可设置锁，避免被他人或无意中修改。Default Site Elevation为该区块的海拔高度，不需要很精确。</li>

<li>在Location选项栏中，选None-Use Co-ordinates Only将以本地为中心；选Map Co-ordinates需输入区块或平台中心的大地坐标；选Geographic Co-ordinates需输入区块或平台中心的经、纬度(必须在Field Setup中已选大地坐标系)；选From Lease Lines需输入方位基线位移。这里可选填，有些区块较大，海拔高度差也较大，无法精确。<b>Azimuth Reference为方位计算基准。</b></li></ol>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2p54kRgvPq_QFAaYi60kj4eHFutNpCwDIbsFXvJhUfXmOM_oTqgCjgQ-JDeiy012YN5Dnp0Hor3QAyQXNe-GonuM0KM40Y1PN3PPkzLCDpXSw/Site%20Properties-Location.png?psid=1">
<img class="aligncenter" title="Site Properties-Location" style="width:500px;height:300px;" src="https://qgiqmw.blu.livefilestore.com/y2p54kRgvPq_QFAaYi60kj4eHFutNpCwDIbsFXvJhUfXmOM_oTqgCjgQ-JDeiy012YN5Dnp0Hor3QAyQXNe-GonuM0KM40Y1PN3PPkzLCDpXSw/Site%20Properties-Location.png?psid=1" alt="Site Properties-Location"></a>


<h4><a name="sec-4">WELLSETUP-CREATE NEW WELL单井设置-建立新井</a></h4>

WELLSEUP-CREATE NEW WELL的功能是创建一口新井并设置该井的基本数据或对已存在的井进行编辑修改。下面按步骤说明：

<ol>
<li>在菜单栏上单击File 菜单，选取New Well选项或单击工具栏中<img src="https://qgiqmw.blu.livefilestore.com/y2pSBTjFq17lYaoiD-u28iSBY8W_RLEsKRiWoFG-IVHLRI_oxI-SQmy7cbPKuTT-EB_h9skJR3lsBjyQIpoWOLcQaxIRzMCdrnyDCkh_oGkU3M/Well.png?psid=1" alt="Well">图标(编辑当前已打开的井)，将会出现以下对话框：</li>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2p0orwsNahk442dmxMCVwt2Nhg-v2FBPgR2-Bi5LgnS6XlO8vy8GmIzGLKCV0v9CQAePyONz2FLgs0Eg_Qu2Q4MjtE0KMXeiMYnlcAcqLBqPk/Well-General.png?psid=1">
<img class="aligncenter" title="Well-General" style="width:500px;height:350px;" src="https://qgiqmw.blu.livefilestore.com/y2p0orwsNahk442dmxMCVwt2Nhg-v2FBPgR2-Bi5LgnS6XlO8vy8GmIzGLKCV0v9CQAePyONz2FLgs0Eg_Qu2Q4MjtE0KMXeiMYnlcAcqLBqPk/Well-General.png?psid=1" alt="Well-General"></a>

<li>在Well栏中填入井名，Description栏中可输入一些关于本井信息的描述，Active Unit System选择该井的设计测量单位。</li>

<li>在Depth Reference标签中，Ground Elevation为当地海拔高度，Wellhead为井口海拔。在上面的Datum elevation above : Mean Sea Level中可以设置井深计算基准面，这里可以设置多个计算基准面，当后面有相应的设计与之配合后，数据就不允许再改动了，因此最好在此处设置完全。右下角图中的Air Gap即为补心高度，即地面与钻盘面之间的高度差。如是海上油田，则应选中Configuration中的Offshore，如果参考井口在海底，则还应选中Subsea。</li>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2ptWxQy0j6ziLKFpsfet8hVWQRY-r7opqZmtk-m3GyUqkGliDBruiEXIQSLjZhdxOZjoQ9rCVNLs9fiZj1sKddgGYtNl5ehf0iMipbdJSU4gE/Well-Depth%20Reference.png?psid=1">
<img class="aligncenter" title="Well-Depth Reference" style="width:500px;height:350px;" src="https://qgiqmw.blu.livefilestore.com/y2ptWxQy0j6ziLKFpsfet8hVWQRY-r7opqZmtk-m3GyUqkGliDBruiEXIQSLjZhdxOZjoQ9rCVNLs9fiZj1sKddgGYtNl5ehf0iMipbdJSU4gE/Well-Depth%20Reference.png?psid=1" alt="Well-Depth Reference"></a>

<li>Location选项卡中选择井口的参考坐标，slot为槽口，在海上平台和地面丛式井中会有所应用。Offset from Site为该井口相对区块中心的偏移坐标。</li></ol>


<h4><a name="sec-5">WELLPATH SETUP-CREATE NEW WELLPATH轨迹设置-建立新的轨迹</a></h4>

轨迹的建立和设置，是对一口井的轨迹基本参数进行设定，包括轨迹起点、轨迹方向、井的类型等。一口井可以有多条轨迹。下面具体说明：

<ol>
<li>在菜单栏上单击File 菜单，选取New Wellpath选项或单击工具栏中<img src="https://qgiqmw.blu.livefilestore.com/y2p3-7a73e3iQYzv8nzrKMKZa_M1diQOqMBKQYZ4q5hM8UX5i-Yj1xzXj09t2BaC9a1hmZj3RFbpweRLP10YbCMUOdgwJrLgXr5u3qaYj-gxtE/Wellbore.png?psid=1" alt="Wellbore">图标(编辑当前井的轨迹)，将会出现以下对话框：</li>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2p9O-D5_BMljlF6sI_dBfH-pbIOIIUOQHvkHpwqAk1lM5MJ2bzl-qreGzEpuoClMkkZ_b4YfBScsoINZfFaOhuTcqSFnuRTGvZeXe2lOdvxGA/Wellbore%20Properties-General.png?psid=1">
<img class="aligncenter" title="Wellbore Properties-General" style="width:600px;height:330px;" src="https://qgiqmw.blu.livefilestore.com/y2p9O-D5_BMljlF6sI_dBfH-pbIOIIUOQHvkHpwqAk1lM5MJ2bzl-qreGzEpuoClMkkZ_b4YfBScsoINZfFaOhuTcqSFnuRTGvZeXe2lOdvxGA/Wellbore%20Properties-General.png?psid=1" alt="Wellbore Properties-General"></a>

<li>Wellpath栏输入轨迹名(如S型、J型等)，Description栏输入对轨迹的描述及其他附加信息(可不填)。如果该井眼为侧钻分支井眼，那么可以在下面的Parent中选择其父井眼名称。</li>

<li>Magnetic选项卡中设置该井设计时的磁偏角参数，在以后进行设计校核或者在该井眼基础上设计新的井眼时必须注意当时已有井眼的磁偏角参数。</li></ol>


<h4><a name="sec-6">TARGET EDITOR  靶点编辑器</a></h4>

TARGET EDITOR靶点编辑器，其功能是对单井或多井的一个或多个靶点设定靶点位置及靶区形状。其具体操作如下：

<ol>
<li>在菜单栏上单击<img src="https://qgiqmw.blu.livefilestore.com/y2pG8XtDY2y4yPiEw_FBaKa2BEqt8ADTeRRiuqLupT-34Q-jqsb40IFSqi0bIYpq2sry6RIS1pELFA44I_mZsAcLZatih4TLATKDd3mk8dvV3E/Target.png?psid=1" alt="Target">图标，或者在区块或井眼下的界面中双击该图标将会出现左下对话框：</li>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2pmEXiicekX-UvGPzbQPOzqZMCmIItu2BCxxLwnmzrDdcCnBDCCjeA-tDiT8aHh02vpMRo-XJKVaVGybpd35MdGoRjK9TdCHS_7XtcgSRHYDs/Target%20Editot.png?psid=1">
<img class="aligncenter" title="Target Editot" style="width:700px;height:390px;" src="https://qgiqmw.blu.livefilestore.com/y2pmEXiicekX-UvGPzbQPOzqZMCmIItu2BCxxLwnmzrDdcCnBDCCjeA-tDiT8aHh02vpMRo-XJKVaVGybpd35MdGoRjK9TdCHS_7XtcgSRHYDs/Target%20Editot.png?psid=1" alt="Target Editot"></a>

<li>Target Editor对话框最上边对于Target靶点列表有二个选项：Project List选项为整个油田的靶点列表；Site List选项栏为整个区块或平台的靶点列表；Well List选项为当前轨迹的靶点列表；Design List为当前设计轨迹靶点列表。</li>

<li>编辑一个靶点，首先在Name栏中输入靶点名，可在Description栏输入此靶点的描述或相关信息(可不输)，接下来在TVD栏中输入此靶点的垂深，在上面工具栏下的Datum下拉栏中选择与垂深相对应的深度基准，然后选择一种方式输入靶点位置参数：Local中可输入东西、南北位移；Map中可输入大地坐标；Geographic中可输入经纬度(必须在Field Setup中已选大地坐标系)；Polar可输入水平位移及方位角，最后单击Save按钮，此靶点数据将被储存，靶点名显示在靶点列表中。想删除一个靶点，只需在列表中选择该靶点，单击DELETE按钮即可(已被选用的靶点不可删除)。</li>

<li>Geometry靶区编辑：首先选择靶区形状(Point是点；Circle是圆；Ellipse是椭圆；Rectangle是矩形；Polygon是多边形)，以选择圆为例，将出现下面左边的对话框。在Radius中输入靶区半径，Offset of Circle Centre from Target Centre中输入靶区中心相对靶点的偏移量，Thickness中输入靶区厚度(UP靶点以上、DOWN靶点以下)，最后二项输入靶区的倾角和方向。</li></ol>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2prYgxo65FpI4la98HXAGgGDGeADBvdj8AoyQoOhEWViYkkuSJzz6yardH4HP30PaKBT_Z53VCRfXetremtHEYgsZfqP6fuvUGMaQUIj216VA/Target-Circle.png?psid=1">
<img class="aligncenter" title="Target-Circle" style="width:450px;height:400px;" src="https://qgiqmw.blu.livefilestore.com/y2prYgxo65FpI4la98HXAGgGDGeADBvdj8AoyQoOhEWViYkkuSJzz6yardH4HP30PaKBT_Z53VCRfXetremtHEYgsZfqP6fuvUGMaQUIj216VA/Target-Circle.png?psid=1" alt="Target-Circle"></a>


<h4><a name="sec-7">NEW PLAN & OPEN PLAN  井眼轨迹设计</a></h4>

通常定向井应用在开发井中较多，因此在设计一口定向井前，将会有详尽的资料可供参考，有时会有一些具体的限制，如规定井形、限制造斜率、强制降斜等。COMPASS WELLPLAN中的PLAN提供了强大的设计功能，基本上满足了各种常规和特殊的设计需要。下面按步骤具体说明：

<ol>
<li>新设计计划的创建。在井眼上右键新建井眼轨迹后将会出现左下对话框：</li>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2pv-ZUJauhzpr9gj0-KVJevc1P0U5OrGogd9HnPfQ1O0pwy89V4XkOUzK9w35Uh_I2X7Zv0nW9hpOSrhNKM_KfuHFN1qPu0MngUqWwJanZBcM/Plan%20Design%20Properties-General.png?psid=1">
<img class="aligncenter" title="Plan Design Properties-General" style="width:700px;height:370px;" src="https://qgiqmw.blu.livefilestore.com/y2pv-ZUJauhzpr9gj0-KVJevc1P0U5OrGogd9HnPfQ1O0pwy89V4XkOUzK9w35Uh_I2X7Zv0nW9hpOSrhNKM_KfuHFN1qPu0MngUqWwJanZBcM/Plan%20Design%20Properties-General.png?psid=1" alt="Plan Design Properties-General"></a>

<li>此对话框中，在Name栏中输入设计的名称，Description栏中输入对此设计的描述或相关信息，Version栏中输入版本号，<b>选择Planned (Principal)复选框将使此设计被作为主设计，一个井眼只能有一个主设计井眼</b>。下图中给出了三种不同井眼的树状图，它们依次为实际井眼(Actual Design)、主设计井眼(Planned)、设计井眼(Prototype)，实际井眼是由实际的测井数据(Survey)组成的。</li>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2p8_jNHsg-3DBO94tFnNn79edNWq6tDQAPe_oatOYcvpRSPpV4H-_PNzEMX__m_dqdtnGn5dL7CKOPXkHGNI8JRtfnGwBLMCK3c8L2M7uYwx8/Plan%20Wells.png?psid=1">
<img class="aligncenter" title="Plan Wells" style="width:130px;height:80px;" src="https://qgiqmw.blu.livefilestore.com/y2p8_jNHsg-3DBO94tFnNn79edNWq6tDQAPe_oatOYcvpRSPpV4H-_PNzEMX__m_dqdtnGn5dL7CKOPXkHGNI8JRtfnGwBLMCK3c8L2M7uYwx8/Plan%20Wells.png?psid=1" alt="Plan Wells"></a>

<li>在Tie-on选项卡中可以选择设计起始点(User为将自定义的点作为起始点、From Surface为以井口作为起始点、From Survey-point为从实际已钻井眼开始设计)。在Survey Tool Program选项卡中可以选择井段的测井工具。</li>

<li>输入结束后确认，双击井眼图标将会出现下述设计界面。在此屏幕中，工具栏下是数据栏，数据栏下面是当前所选择点的数据，最下一排是设计所需的各种设计方法：三段制(Slant)、五段制(S Well)、造斜率与扭方位设计方法(Build Turn，转盘钻)、狗腿度与工具面设计方法(Dogleg Toolface，动力钻具)、稳斜设计(Hold)、优化对齐(Optimum Align)、手动设计(Nudge)。</li>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2poSu7oFRlTwfqrzRKKaqaOpRrfbJHrIyACo5_M91aZcH2W5P_eShjWrqt3lQWDdAc653Rx965ZGsv5g503WFgCq5eiuAXBqo_ycgCnhaUe9w/Plan%20Editor.png?psid=1">
<img class="aligncenter" title="Plan Editor" style="width:700px;height:470px;" src="https://qgiqmw.blu.livefilestore.com/y2poSu7oFRlTwfqrzRKKaqaOpRrfbJHrIyACo5_M91aZcH2W5P_eShjWrqt3lQWDdAc653Rx965ZGsv5g503WFgCq5eiuAXBqo_ycgCnhaUe9w/Plan%20Editor.png?psid=1" alt="Plan Editor"></a>

<li>井眼轨迹设计：
<ol><li>2D 三段制设计(直-增-稳)，出现如下对话框：

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2pZXoRcaw2XBXQST2O6pSyUwbjjTlhvqtXJhpcegZkNGSXFY6wsT9uX41GILvBtlDCru2wHtijF_Hr5PoGQoxmCToxNuMBwxWPk1Or39Nlk0k/Slant%20Design.png?psid=1">
<img class="aligncenter" title="Slant Design" style="width:700px;height:140px;" src="https://qgiqmw.blu.livefilestore.com/y2pZXoRcaw2XBXQST2O6pSyUwbjjTlhvqtXJhpcegZkNGSXFY6wsT9uX41GILvBtlDCru2wHtijF_Hr5PoGQoxmCToxNuMBwxWPk1Or39Nlk0k/Slant%20Design.png?psid=1" alt="Slant Design"></a>

在此对话框中，1st Hold Len栏输入造斜点，1st Build栏输入造斜率， Maximum Angle栏输入最大井斜角，2nd Hold Len栏输入第二稳斜段长，右边Target下拉栏中可以选择靶点。单击计算按钮计算，单击OK按钮确认，否则单击CANCEL按钮取消。最大井斜角和第二稳斜段长可以不输(可只任给两个参数)，但其右边的复选框必需点击，显示为叉，否则不能计算。</li>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2pSckkCC_vrSipmJ-7q8jENxM5T7BejQ7J9VrQa3TcMaLwwbpArxy0qV02AoLJwlLhN3pISP-N7AaYwRkKJeSS1VfwH5paDMelhvdXj6TzhNk/Slant%20Parameter.png?psid=1">
<img class="aligncenter" title="Slant Parameter" style="width:450px;height:240px;" src="https://qgiqmw.blu.livefilestore.com/y2pSckkCC_vrSipmJ-7q8jENxM5T7BejQ7J9VrQa3TcMaLwwbpArxy0qV02AoLJwlLhN3pISP-N7AaYwRkKJeSS1VfwH5paDMelhvdXj6TzhNk/Slant%20Parameter.png?psid=1" alt="Slant Parameter"></a>

<li>2D 五段制井眼设计，出现如下对话框：

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2p4RNfqnvGvF73Sy98Ylfh1jcoq9bC9MLpoQuHhPegoQ3WR6nHnNKb1P3IEFGhrri7XnsKgM82rKTJ9OT2xA9UYjJG16_U_gcXX_bU4tZNa7M/S%20Well%20Design.png?psid=1">
<img class="aligncenter" title="S Well Design" style="width:700px;height:140px;" src="https://qgiqmw.blu.livefilestore.com/y2p4RNfqnvGvF73Sy98Ylfh1jcoq9bC9MLpoQuHhPegoQ3WR6nHnNKb1P3IEFGhrri7XnsKgM82rKTJ9OT2xA9UYjJG16_U_gcXX_bU4tZNa7M/S%20Well%20Design.png?psid=1" alt="S Well Design"></a>

在上面的对话框中，1st Hold Len栏输入第一造斜点，1st Build栏输入第一次的造斜率， Maximum Angle栏输入最大井斜角，2nd Hold Len栏输入第二稳斜段长，右边Target下拉栏中可以选择靶点，2nd Build栏输入第二次造斜率，Final Inclination栏输入最终井斜角，Final Hold栏输入最终稳斜段长。这7个参数可任给5个进行计算。</li>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2paKkhZuOb6jP_reN94Ve-1M-q0TTjwBtIhffVjLCWC0iJB_AGYTmuEGqUBNbyYUE9iLSvCqAwixPDE6C0yNV4tjHl7ZhcHBD4JdjxGtvZr8g/S%20Well%20Parameter.png?psid=1">
<img class="aligncenter" title="S Well Parameter" style="width:450px;height:260px;" src="https://qgiqmw.blu.livefilestore.com/y2paKkhZuOb6jP_reN94Ve-1M-q0TTjwBtIhffVjLCWC0iJB_AGYTmuEGqUBNbyYUE9iLSvCqAwixPDE6C0yNV4tjHl7ZhcHBD4JdjxGtvZr8g/S%20Well%20Parameter.png?psid=1" alt="S Well Parameter"></a>

<li>三维分段设计(井斜、方位的变化率，柱面设计法)，出现如下对话框：

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2pfINfEqhDn03SkSYxVfWynKujMnNbvTP_zlzjmwQNuH9X-QkiCGtifBaA776ekez7OmWLU6e1vc2WKjjj-UqiLqbEeYq5UU1Lad2yWoIaQq0/Build%20Turn%20Design.png?psid=1">
<img class="aligncenter" title="Build Turn Design" style="width:700px;height:140px;" src="https://qgiqmw.blu.livefilestore.com/y2pfINfEqhDn03SkSYxVfWynKujMnNbvTP_zlzjmwQNuH9X-QkiCGtifBaA776ekez7OmWLU6e1vc2WKjjj-UqiLqbEeYq5UU1Lad2yWoIaQq0/Build%20Turn%20Design.png?psid=1" alt="Build Turn Design"></a>

在此对话框中，最下面一排图标中，带有曲线的图标为不同定义的单段设计按钮，分别是：点击MD按钮，输入井斜、方位变化率及斜深；点击TVD按钮，输入井斜、方位变化率及垂深(或选择靶点)；点击Inclination按钮，输入井斜、方位变化率及所需井斜值；点击Azimuth按钮，输入井斜、方位变化率及所需方位值；点击Tangent按钮，输入井斜、方位变化率并输入一个点的值(或选择靶点)；点击Point按钮，输入点的值或选择靶点；点击Online TVD按钮，输入一个基准垂深然后输入点的值或选择靶点。</li>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2pYgbj-oo8UToIKiG5w0ArFIL_Ch9ehdtEMzPmmckDycFJ2VcghH1EqH8PXvNrkp1zP7Mj0h5dvELKXYXbNvyE6uZ7Wk2vGmsrpeYG35hBTew/Build%20Turn%20Parameter.png?psid=1">
<img class="aligncenter" title="Build Turn Parameter" style="width:450px;height:330px;" src="https://qgiqmw.blu.livefilestore.com/y2pYgbj-oo8UToIKiG5w0ArFIL_Ch9ehdtEMzPmmckDycFJ2VcghH1EqH8PXvNrkp1zP7Mj0h5dvELKXYXbNvyE6uZ7Wk2vGmsrpeYG35hBTew/Build%20Turn%20Parameter.png?psid=1" alt="Build Turn Parameter"></a>

<li>三维分段设计(按工具面及狗腿的变化率，<b>球面设计法</b>)，出现的对话框基本与上面的对话框相同，只是井斜、方位栏变成了工具面、狗腿栏，使用方法同3一样。</li>

<li>稳斜设计，出现如下对话框，给定段长或测深并直线钻至该点即可。</li>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2pTYN-7Wnk_gnNj6LJtNVLztZo6_o0HfsbDxpL9aco2472IjQFCTEJCTCUxWbQ_6IrmxkzNoE020-tVWOBr39W--uLUi1aQI01tAaKIWd0FAE/Hold%20Design.png?psid=1">
<img class="aligncenter" title="Hold Design" style="width:700px;height:140px;" src="https://qgiqmw.blu.livefilestore.com/y2pTYN-7Wnk_gnNj6LJtNVLztZo6_o0HfsbDxpL9aco2472IjQFCTEJCTCUxWbQ_6IrmxkzNoE020-tVWOBr39W--uLUi1aQI01tAaKIWd0FAE/Hold%20Design.png?psid=1" alt="Hold Design"></a>

<li>优化对齐设计方法(Optimum Align)，出现如下对话框，即按一定设计方法顺次穿过几个靶点。在工具栏上点击图标可以设置穿靶顺序以及穿靶的方法。</li>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2pfUwNqAomEyf7jcFTZLchc1stvnMeV4jYLsS-A1VZ2pIzThm07Dbo9BcMtIeqvThBCJ49U3Q_CPRbAZBbeufh7VclgYQnvzXclFcpi6khBwg/Optimum%20Align%20Design.png?psid=1">
<img class="aligncenter" title="Optimum Align Design" style="width:700px;height:140px;" src="https://qgiqmw.blu.livefilestore.com/y2pfUwNqAomEyf7jcFTZLchc1stvnMeV4jYLsS-A1VZ2pIzThm07Dbo9BcMtIeqvThBCJ49U3Q_CPRbAZBbeufh7VclgYQnvzXclFcpi6khBwg/Optimum%20Align%20Design.png?psid=1" alt="Optimum Align Design"></a>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2pqzUnOTXD-qgxpfFJdNsFjf0x2aZnEV4Dx_RAGsYWtoPTAtSTxSLWXyUSQ7uuPkqHo8ZgzliTr64ay7Rl8NgSq2CuLu4n9hXpLR2vJcivrxw/Optimum%20Align%20Parameter.png?psid=1">
<img class="aligncenter" title="Optimum Align Parameter" style="width:450px;height:260px;" src="https://qgiqmw.blu.livefilestore.com/y2pqzUnOTXD-qgxpfFJdNsFjf0x2aZnEV4Dx_RAGsYWtoPTAtSTxSLWXyUSQ7uuPkqHo8ZgzliTr64ay7Rl8NgSq2CuLu4n9hXpLR2vJcivrxw/Optimum%20Align%20Parameter.png?psid=1" alt="Optimum Align Parameter"></a>

<li>手动设计方法(Nudge)，出现如下对话框，即一段段手动微调设计方法。</li></ol></li></ol>

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2prSDCJ2_tPBhFX7HtD5wgk8odQ3ZUMiq1swOPXeZJhzpMFG33aYst03NErPk5QlKbEeH-jwgEMGSRkRKRDlDJPKvdZR8oG674EtWeXC_LJ_o/Nudge%20Design.png?psid=1">
<img class="aligncenter" title="Nudge Design" style="width:700px;height:140px;" src="https://qgiqmw.blu.livefilestore.com/y2prSDCJ2_tPBhFX7HtD5wgk8odQ3ZUMiq1swOPXeZJhzpMFG33aYst03NErPk5QlKbEeH-jwgEMGSRkRKRDlDJPKvdZR8oG674EtWeXC_LJ_o/Nudge%20Design.png?psid=1" alt="Nudge Design"></a>


<h4><a name="sec-8">NEW SERVEY& OPEN SERVEY实测数据建立与编辑</a></h4>

定向井钻进中，需要实时对井眼轨迹进行监测，根据由测量工具提供的已钻井眼的测量数据，一般为某一深度时的井斜、方位的值，利用COMPASS中提供的SURVEY的功能，可以计算出该点的垂深、东/北位移、狗腿度等数值，监控实钻轨迹，并可对轨迹趋势进行预测和计算。下面按步骤具体说明：

<ol>
<li>新的实测数据创建。在井眼上右键点击新建Survey，将会出现以下对话框：

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2pY_RkBdq6k0ufBBgTNdi0AD86qjEGRRqiZm_RmcnjY6oFlm--3QW5H_6mVGQBWs8XzxYQ1AIYvmKyTVhIJs8pWH3PRg6xfX4vpKz_2HGmJA8/Survey%20Properties-General.png?psid=1">
<img class="aligncenter" title="Survey Properties-General" style="width:400px;height:400px;" src="https://qgiqmw.blu.livefilestore.com/y2pY_RkBdq6k0ufBBgTNdi0AD86qjEGRRqiZm_RmcnjY6oFlm--3QW5H_6mVGQBWs8XzxYQ1AIYvmKyTVhIJs8pWH3PRg6xfX4vpKz_2HGmJA8/Survey%20Properties-General.png?psid=1" alt="Survey Properties-General"></a>

在此对话框中，Name栏中填入实测数据名，Description栏输入对此数据的描述(可不填)，Company栏填入公司名(可不填)，Engineer栏填入工程师名(可不填)，Survey Date栏输入日期。Edit tools可设置测井工具的具体参数。在Tie-on选项卡中可选择测井数据起点。</li>

<li>单击确定按钮后，屏幕变为下图所示测量数据编辑屏幕：

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2ppiz91_hVT4zoJzw3RmbL1K6RejEPoUVNXtAwTz3RTBgfrmQsXKXjjtXfjfEJoLvwjL1-VdUBCGtTZzi-hQoiYfqCVxk-dKymRPIWmVEw46Y/Survey%20Editor.png?psid=1">
<img class="aligncenter" title="Survey Editor" style="width:600px;height:470px;" src="https://qgiqmw.blu.livefilestore.com/y2ppiz91_hVT4zoJzw3RmbL1K6RejEPoUVNXtAwTz3RTBgfrmQsXKXjjtXfjfEJoLvwjL1-VdUBCGtTZzi-hQoiYfqCVxk-dKymRPIWmVEw46Y/Survey%20Editor.png?psid=1" alt="Survey Editor"></a>

在此屏幕中，数据拦可以输入实测得到的数据(输入斜深、井斜和方位，回车后自动计算)。单击数据栏的行号，此行变黑，这时用键盘上的Insert和Delete键任意添加和删除(第一行不能删除)。当前深度值必须大于前一点的值，井斜值必须在0~180°之间，方位值必须在0~360°之间。数据栏中如没有输入数值而回车，会自动按前两行的变化量输入数值。若计算出的狗腿值大于确定的最大狗腿值时被显示为红色。</li>

<li>单击<img src="https://qgiqmw.blu.livefilestore.com/y2pOiuv8G6kLcNA_32TowRt2pEAMW8NSpeluTE9EmkaWqRpgPgrKtPWlf3lpgsMDoG571BVoRhVwGE92fKduv-p10nY1-S0DL_1sD3X0LUaFWI/Interpolate.png?psid=1" alt="Interpolate">图标(Interpolate)，在出现的对话框中可通过内插计算给定点的所有相关数据。</li>

<li>预测。单击<img src="https://qgiqmw.blu.livefilestore.com/y2pTsVTtkRiGlzAznzUGDarlxIo_suX80OOLYzKOCZWwevohyk6ZBIuiS7AhPWHTw357UzKVP7PF9Mv8ZVPT2CbA_5sXtB4ybc7AKdBDp7rIy8/Project%20Ahead.png?psid=1" alt="Project Ahead">图标(Project Ahead)，在出现的对话框中可按照一定规则预测测点以后井眼轨迹的数据。</li></ol>


<h4><a name="sec-9">ANTICOLLISION  防碰计算</a></h4>

ANTICOLLISION(防碰计算)的功能是，丛式井各井或相邻井设计后或实钻中计算井眼轨迹之间的距离，是否在安全距离之外。下面按步骤具体说明：

<ol>
<li>在进行防碰计算之前，必须在Company Properties中，选择需要的Scan Method 。在Scan Method下拉栏中有三种扫描模式可以选择：Closest Approach 3D(3D渐近、球形)；Travelling Cylinder(圆柱面、柱状)；Horizontal Plan(平面法、水平面)。</li>

<li>点击工具栏上的Offset Design图标，进入Offset Design Selection对话框，可在这个对话框中选择需要进行防碰扫描的相关井眼。</li>

<li>点击菜单中Analysis中的Anticollision Settings，出现如下对话框：

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2pyFlqZqCVXC1rqeMdRmO5glzWFkMDsSR3r3UcOTmbwtwyZ5Ab894vWft32PBp-vepe-6PbmX0OSd1_Q184caQ4ZL-mTybzUtAln4h7gZn0lE/Anticollision%20Settings.png?psid=1">
<img class="aligncenter" title="Anticollision Settings" style="width:360px;height:400px;" src="https://qgiqmw.blu.livefilestore.com/y2pyFlqZqCVXC1rqeMdRmO5glzWFkMDsSR3r3UcOTmbwtwyZ5Ab894vWft32PBp-vepe-6PbmX0OSd1_Q184caQ4ZL-mTybzUtAln4h7gZn0lE/Anticollision%20Settings.png?psid=1" alt="Anticollision Settings"></a>

在此对话框中可设置防碰扫描内插间隔(Interpolate Interval)，防碰扫描的扫描范围以及扫描标准等参数。</li></ol>

<h4><a name="sec-10">常用功能简介</a></h4>

COMPASS WELLPLAN提供的功能很多，以上介绍的只是一些主要功能，下面对一些上面没有提到的常用功能做简要的介绍。

<ol>
<li>REPORT报告的生成和打印。

COMPASS WELLPLAN中，设计、实测计算、防碰计算等都可以生成报告，在它们各
自的菜单中，都有Report一项或在工具栏中单击<img src="https://qgiqmw.blu.livefilestore.com/y2pODz2Jcq8fncexqXjMEH6vlOWX3pZ8ROWPtdiaUiE-UP5A3gMj0ZGYwhI_MHLI_hTCalxlzfs3kz2jXBQIsjSe0OQBTOgONaq37dN9pBEYUo/Report.png?psid=1" alt="Report">图标进入报告生成界面。</li>

<li>轨迹图形的显示与编辑。

COMPASS WELLPLAN的三个核心功能中，都有图形显示功能，其中设计和实测计算
的轨迹图是最常用到的，因为它们的基本用法相同，下面同样以实测计算中的轨
迹图显示与编辑为例介绍。在实测数据编辑窗口状态下，单击工具栏中<img src="https://qgiqmw.blu.livefilestore.com/y2pIc8hLAac86mAuvEchPmV6z-9WhvQm5KeEEJlxGCsS-FAoufi9t4ip_gxa7lfMAgfjtRnlqynIVy_KGNPWVROptyt0wNuGLPVGj1MwX5lymk/View.png?psid=1" alt="View">的图标，将显示所需轨迹图。在此图中，用户可以利用图形窗口中的工具栏，对图形做显示或不显示说明标签、特殊点、靶点、网格线、主设计轨迹；坐标原点变换；放大、缩小；打印等功能。</li>

<li>GEODETIC CALCULATOR地质数据计算

单击工具栏中<img src="https://qgiqmw.blu.livefilestore.com/y2pP6faOYsaCPrtYJQXf53uWdl9H2tWEcEMR5iZP4qnU0V1YwgohOA2ISky5yeVqCzs8G2jraqXHLBixSlQ2kw6WBWN2IWTjhiza9TcfyLjbpU/Geodectic%20Calculator.png?psid=1" alt="Geodectic Calculator">图标，将会出现如下对话框：

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2p1Ai71bY8IuWbn1xB9pi1eQ0PPdNEGNjmnP3RE7U__HpcAHfiqWrAaDFMP2lEbKKEF1GEaCRmERzjhoMPuFqqePGsIHF_BbZQcXbOJu803K8/Geodectic%20Calculator%20Parameter.png?psid=1">
<img class="aligncenter" title="Geodectic Calculator Parameter" style="width:450px;height:230px;" src="https://qgiqmw.blu.livefilestore.com/y2p1Ai71bY8IuWbn1xB9pi1eQ0PPdNEGNjmnP3RE7U__HpcAHfiqWrAaDFMP2lEbKKEF1GEaCRmERzjhoMPuFqqePGsIHF_BbZQcXbOJu803K8/Geodectic%20Calculator%20Parameter.png?psid=1" alt="Geodectic Calculator Parameter"></a>

此对话框中，首先在Geodetic system、Geodetic Datum、Map Zone这三个下拉栏中，可以选择不同的大地坐标系及其所在区域，然后输入已知值(相对中心的东/北位移、大地坐标或经纬度)，点击任意另一选项，未知值被计算出。单击NotePad按钮，可将计算结果输出到写字板中编辑或储存。</li>

<li>MAGNETIC CALCULATOR磁场值计算

选单击工具栏中<img src="https://qgiqmw.blu.livefilestore.com/y2pDk0H1eKvJJwRLlJAggwOUEp9OuFIhHXNlI0OqVXmNITivUnqPBe-vCOKbGBXCfCKefGSu-kDhIcrlnRIpTH_xUDYOr38Ss7AoBAlpHm5PHM/Magnetic%20Calculator.png?psid=1" alt="Magnetic Calculator">图标，将会出现如下对话框：

<a target="_blank" href="https://qgiqmw.blu.livefilestore.com/y2pCgdJ8oCnfXkCgSTGyuXCHWCLuqFbkzUH3TAq8u2xn4OvPDeYb5bx9UvXYdu4g91uYM79Og63Fg85vvE19JGn-ybGJmEGeVz9YzTlnGL-O7U/Magnetic%20Calculator%20Parameter.png?psid=1">
<img class="aligncenter" title="Magnetic Calculator Parameter" style="width:450px;height:280px;" src="https://qgiqmw.blu.livefilestore.com/y2pCgdJ8oCnfXkCgSTGyuXCHWCLuqFbkzUH3TAq8u2xn4OvPDeYb5bx9UvXYdu4g91uYM79Og63Fg85vvE19JGn-ybGJmEGeVz9YzTlnGL-O7U/Magnetic%20Calculator%20Parameter.png?psid=1" alt="Magnetic Calculator Parameter"></a>

此对话框中，选择本地坐标及地质磁场模型，回车后，将计算出总磁场强度、矢量角、地磁强度矢量值、磁北角、磁偏角等值。</li></ol>
