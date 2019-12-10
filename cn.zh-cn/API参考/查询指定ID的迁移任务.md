# 查询指定ID的迁移任务<a name="sms_api_0025"></a>

## 功能介绍<a name="section1843113112355"></a>

查询指定ID的迁移任务。

## URI<a name="section20843831103513"></a>

GET /v1/sms/tasks/\{task\_id\}

参数说明请参见[表1](#table9128848172010)。

**表 1**  参数说明

<a name="table9128848172010"></a>
<table><thead align="left"><tr id="row1112910489205"><th class="cellrowborder" valign="top" width="24.452105392760405%" id="mcps1.2.4.1.1"><p id="p131041331233"><a name="p131041331233"></a><a name="p131041331233"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="22.235902487072153%" id="mcps1.2.4.1.2"><p id="p18115233734"><a name="p18115233734"></a><a name="p18115233734"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="53.31199212016744%" id="mcps1.2.4.1.3"><p id="p1312111336312"><a name="p1312111336312"></a><a name="p1312111336312"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row113113489201"><td class="cellrowborder" valign="top" width="24.452105392760405%" headers="mcps1.2.4.1.1 "><p id="p52072412255"><a name="p52072412255"></a><a name="p52072412255"></a>task_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.235902487072153%" headers="mcps1.2.4.1.2 "><p id="p1299515124210"><a name="p1299515124210"></a><a name="p1299515124210"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="53.31199212016744%" headers="mcps1.2.4.1.3 "><p id="p1211252164212"><a name="p1211252164212"></a><a name="p1211252164212"></a>任务的ID</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section9855173163512"></a>

不涉及

## 响应消息<a name="section1185663153516"></a>

**响应参数**

响应参数如[表2](#table1985993110351)所示。

**表 2**  响应参数

<a name="table1985993110351"></a>
<table><thead align="left"><tr id="row111092332359"><th class="cellrowborder" valign="top" width="19.54%" id="mcps1.2.4.1.1"><p id="p8131164842014"><a name="p8131164842014"></a><a name="p8131164842014"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.39%" id="mcps1.2.4.1.2"><p id="p13131114815209"><a name="p13131114815209"></a><a name="p13131114815209"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="62.07%" id="mcps1.2.4.1.3"><p id="p17131144872019"><a name="p17131144872019"></a><a name="p17131144872019"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1109163383517"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p16109153314358"><a name="p16109153314358"></a><a name="p16109153314358"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p4109183353516"><a name="p4109183353516"></a><a name="p4109183353516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p611053318355"><a name="p611053318355"></a><a name="p611053318355"></a>任务ID</p>
</td>
</tr>
<tr id="row311083313355"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p8110103319353"><a name="p8110103319353"></a><a name="p8110103319353"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p1311063353510"><a name="p1311063353510"></a><a name="p1311063353510"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p31109338355"><a name="p31109338355"></a><a name="p31109338355"></a>任务名称</p>
</td>
</tr>
<tr id="row16110133363514"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p191101533103510"><a name="p191101533103510"></a><a name="p191101533103510"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p51100332359"><a name="p51100332359"></a><a name="p51100332359"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p171102332354"><a name="p171102332354"></a><a name="p171102332354"></a>任务类型</p>
<a name="ul19661725154010"></a><a name="ul19661725154010"></a><ul id="ul19661725154010"><li>MIGRATE_FILE：文件级</li><li>MIGRATE_BLOCK：块级</li></ul>
</td>
</tr>
<tr id="row1311043313356"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p01101933173513"><a name="p01101933173513"></a><a name="p01101933173513"></a>os_type</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p91101133143517"><a name="p91101133143517"></a><a name="p91101133143517"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><a name="ul764953044013"></a><a name="ul764953044013"></a><ul id="ul764953044013"><li>WINDOWS：Windows迁移任务</li><li>LINUX：Linux迁移任务</li></ul>
</td>
</tr>
<tr id="row811073353513"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p1711043313511"><a name="p1711043313511"></a><a name="p1711043313511"></a>state</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p711083383512"><a name="p711083383512"></a><a name="p711083383512"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p20110183363517"><a name="p20110183363517"></a><a name="p20110183363517"></a>任务状态</p>
<a name="ul4380144614012"></a><a name="ul4380144614012"></a><ul id="ul4380144614012"><li>READY：就绪</li><li>RUNNING：迁移中</li><li>SYNCING:同步中</li><li>ABORTING：暂停中</li><li>ABORT：暂停</li><li>MIGRATE_FAIL：迁移失败</li><li>MIGRATE_SUCCESS：迁移成功</li><li>SYNC_FAIL：同步失败</li><li>SYNC_SUCCESS：同步成功</li></ul>
</td>
</tr>
<tr id="row19110433203519"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p18110143303513"><a name="p18110143303513"></a><a name="p18110143303513"></a>connected</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p17110193343518"><a name="p17110193343518"></a><a name="p17110193343518"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p56391633514"><a name="p56391633514"></a><a name="p56391633514"></a>连接状态</p>
<a name="ul14547251154016"></a><a name="ul14547251154016"></a><ul id="ul14547251154016"><li>true：迁移任务同主机迁移服务连接正常</li><li>false：迁移任务同主机迁移服务失去连接</li></ul>
</td>
</tr>
<tr id="row1110933143519"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p8110183313355"><a name="p8110183313355"></a><a name="p8110183313355"></a>create_date</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p81101533113518"><a name="p81101533113518"></a><a name="p81101533113518"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p151101733153512"><a name="p151101733153512"></a><a name="p151101733153512"></a>任务创建时间</p>
</td>
</tr>
<tr id="row1011063310356"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p6111103311357"><a name="p6111103311357"></a><a name="p6111103311357"></a>start_date</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p7111143315358"><a name="p7111143315358"></a><a name="p7111143315358"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p19111193312353"><a name="p19111193312353"></a><a name="p19111193312353"></a>任务开始时间</p>
</td>
</tr>
<tr id="row20111433203510"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p1011173303513"><a name="p1011173303513"></a><a name="p1011173303513"></a>finish_date</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p4111113313352"><a name="p4111113313352"></a><a name="p4111113313352"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p1011153373511"><a name="p1011153373511"></a><a name="p1011153373511"></a>任务结束时间</p>
</td>
</tr>
<tr id="row81111033163510"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p6111113343519"><a name="p6111113343519"></a><a name="p6111113343519"></a>priority</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p2111163363516"><a name="p2111163363516"></a><a name="p2111163363516"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p141114332352"><a name="p141114332352"></a><a name="p141114332352"></a>迁移进程优先级</p>
<a name="ul1113102384114"></a><a name="ul1113102384114"></a><ul id="ul1113102384114"><li>0：低</li><li>1：标准 （默认）</li><li>2：高</li></ul>
</td>
</tr>
<tr id="row15111633193510"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p1111117333352"><a name="p1111117333352"></a><a name="p1111117333352"></a>speed_limit</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p4111123313355"><a name="p4111123313355"></a><a name="p4111123313355"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p12111233163516"><a name="p12111233163516"></a><a name="p12111233163516"></a>迁移速率限制，单位MB</p>
<p id="p211143393518"><a name="p211143393518"></a><a name="p211143393518"></a>默认为0（不限制）</p>
</td>
</tr>
<tr id="row17111163313518"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p11111133113518"><a name="p11111133113518"></a><a name="p11111133113518"></a>migrate_speed</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p711193353520"><a name="p711193353520"></a><a name="p711193353520"></a>float</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p4111233203519"><a name="p4111233203519"></a><a name="p4111233203519"></a>迁移速率</p>
</td>
</tr>
<tr id="row81131733173513"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p8113143313356"><a name="p8113143313356"></a><a name="p8113143313356"></a>start_target_server</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p18113333143510"><a name="p18113333143510"></a><a name="p18113333143510"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p1113233133516"><a name="p1113233133516"></a><a name="p1113233133516"></a>迁移完成后目的端服务器的状态</p>
<a name="ul1571418414412"></a><a name="ul1571418414412"></a><ul id="ul1571418414412"><li>true：启动（默认值）</li><li>false：停止</li></ul>
</td>
</tr>
<tr id="row1284155915554"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p1286155920559"><a name="p1286155920559"></a><a name="p1286155920559"></a>error_json</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p82861559145515"><a name="p82861559145515"></a><a name="p82861559145515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p6286195915555"><a name="p6286195915555"></a><a name="p6286195915555"></a>任务失败原因</p>
</td>
</tr>
<tr id="row211343316354"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p911314334359"><a name="p911314334359"></a><a name="p911314334359"></a>total_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p1649111215438"><a name="p1649111215438"></a><a name="p1649111215438"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p311319335358"><a name="p311319335358"></a><a name="p311319335358"></a>任务总耗时，单位ms</p>
</td>
</tr>
<tr id="row81135332355"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p131131933203513"><a name="p131131933203513"></a><a name="p131131933203513"></a>migration_ip</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p21131533153517"><a name="p21131533153517"></a><a name="p21131533153517"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p839274518445"><a name="p839274518445"></a><a name="p839274518445"></a>目的端服务器的IP地址。</p>
<a name="ul94182104519"></a><a name="ul94182104519"></a><ul id="ul94182104519"><li>公网迁移时请填写弹性IP地址</li><li>专线迁移时请填写私有IP地址</li></ul>
</td>
</tr>
<tr id="row11113163314355"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p19113133313352"><a name="p19113133313352"></a><a name="p19113133313352"></a>region_name</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p01131733103516"><a name="p01131733103516"></a><a name="p01131733103516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p442302783116"><a name="p442302783116"></a><a name="p442302783116"></a>目的端服务器的区域名称</p>
</td>
</tr>
<tr id="row19113153303519"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p91131339357"><a name="p91131339357"></a><a name="p91131339357"></a>region_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p7113183317351"><a name="p7113183317351"></a><a name="p7113183317351"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p2042372793112"><a name="p2042372793112"></a><a name="p2042372793112"></a>目的端服务器的区域ID</p>
</td>
</tr>
<tr id="row1711323323511"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p21131733193519"><a name="p21131733193519"></a><a name="p21131733193519"></a>project_name</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p121131330352"><a name="p121131330352"></a><a name="p121131330352"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p942542711313"><a name="p942542711313"></a><a name="p942542711313"></a>目的端服务器所在项目名称</p>
</td>
</tr>
<tr id="row21131233153515"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p16113133383518"><a name="p16113133383518"></a><a name="p16113133383518"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p10113143318350"><a name="p10113143318350"></a><a name="p10113143318350"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p1542562783115"><a name="p1542562783115"></a><a name="p1542562783115"></a>目的端服务器所在项目ID，参见<a href="获取项目ID.md">获取项目ID</a></p>
</td>
</tr>
<tr id="row7113633133520"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p10113123383513"><a name="p10113123383513"></a><a name="p10113123383513"></a>sub_task_list</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p91131733183519"><a name="p91131733183519"></a><a name="p91131733183519"></a>JSON数组</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p21132334358"><a name="p21132334358"></a><a name="p21132334358"></a>子任务信息列表，参见<a href="#table1218133213354">表3</a></p>
</td>
</tr>
<tr id="row011383343511"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p1411363333512"><a name="p1411363333512"></a><a name="p1411363333512"></a>source_server</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p151136337355"><a name="p151136337355"></a><a name="p151136337355"></a>JSON</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p6113173343513"><a name="p6113173343513"></a><a name="p6113173343513"></a>源端服务器信息，参见<a href="#table247133203519">表4</a></p>
</td>
</tr>
<tr id="row511353313356"><td class="cellrowborder" valign="top" width="19.54%" headers="mcps1.2.4.1.1 "><p id="p21131133193514"><a name="p21131133193514"></a><a name="p21131133193514"></a>target_server</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.4.1.2 "><p id="p1211373323511"><a name="p1211373323511"></a><a name="p1211373323511"></a>JSON</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.4.1.3 "><p id="p12113133383514"><a name="p12113133383514"></a><a name="p12113133383514"></a>目的端服务器的信息，参见<a href="#table129793243515">表5</a></p>
</td>
</tr>
</tbody>
</table>

**表 3**  sub\_task\_list中成员结构

<a name="table1218133213354"></a>
<table><thead align="left"><tr id="row2011317339355"><th class="cellrowborder" valign="top" width="19.62%" id="mcps1.2.4.1.1"><p id="p447418564319"><a name="p447418564319"></a><a name="p447418564319"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.48%" id="mcps1.2.4.1.2"><p id="p174791556234"><a name="p174791556234"></a><a name="p174791556234"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.9%" id="mcps1.2.4.1.3"><p id="p1649155612311"><a name="p1649155612311"></a><a name="p1649155612311"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row161131933113519"><td class="cellrowborder" valign="top" width="19.62%" headers="mcps1.2.4.1.1 "><p id="p131141833183519"><a name="p131141833183519"></a><a name="p131141833183519"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.48%" headers="mcps1.2.4.1.2 "><p id="p411413313357"><a name="p411413313357"></a><a name="p411413313357"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="61.9%" headers="mcps1.2.4.1.3 "><p id="p41145338351"><a name="p41145338351"></a><a name="p41145338351"></a>子任务ID</p>
</td>
</tr>
<tr id="row1811415339357"><td class="cellrowborder" valign="top" width="19.62%" headers="mcps1.2.4.1.1 "><p id="p15114103313519"><a name="p15114103313519"></a><a name="p15114103313519"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.48%" headers="mcps1.2.4.1.2 "><p id="p611419338359"><a name="p611419338359"></a><a name="p611419338359"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.9%" headers="mcps1.2.4.1.3 "><p id="p1811453363516"><a name="p1811453363516"></a><a name="p1811453363516"></a>子任务名称</p>
<a name="ul37541022184316"></a><a name="ul37541022184316"></a><ul id="ul37541022184316"><li>ATTACH_AGENT_IMAGE：挂载代理镜像</li><li>DETTACH_AGENT_IMAGE：卸载载代理镜像</li><li>FORMAT_DISK_LINUX：Linux分区格式化</li><li>FORMAT_DISK_WINDOWS：Windows分区格式化</li><li>MIGRATE_LINUX_FILE：Linux文件级数据迁移</li><li>MIGRATE_WINDOWS_BLOCK：Windows块级数据迁移</li><li>SYNC_LINUX_FILE：Linux文件级数据同步</li><li>SYNC_WINDOWS_BLOCK：Windows块级数据同步</li><li>CONFIGURE_LINUX：Linux配置修改</li><li>CONFIGURE_WINDOWS：Windows配置修改</li></ul>
</td>
</tr>
<tr id="row14114833113513"><td class="cellrowborder" valign="top" width="19.62%" headers="mcps1.2.4.1.1 "><p id="p121141433133515"><a name="p121141433133515"></a><a name="p121141433133515"></a>progress</p>
</td>
<td class="cellrowborder" valign="top" width="18.48%" headers="mcps1.2.4.1.2 "><p id="p1011493353519"><a name="p1011493353519"></a><a name="p1011493353519"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="61.9%" headers="mcps1.2.4.1.3 "><p id="p61143337358"><a name="p61143337358"></a><a name="p61143337358"></a>子任务进度</p>
</td>
</tr>
<tr id="row9114233163513"><td class="cellrowborder" valign="top" width="19.62%" headers="mcps1.2.4.1.1 "><p id="p181141833163513"><a name="p181141833163513"></a><a name="p181141833163513"></a>start_date</p>
</td>
<td class="cellrowborder" valign="top" width="18.48%" headers="mcps1.2.4.1.2 "><p id="p3114193319357"><a name="p3114193319357"></a><a name="p3114193319357"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="61.9%" headers="mcps1.2.4.1.3 "><p id="p7114633153512"><a name="p7114633153512"></a><a name="p7114633153512"></a>子任务开始时间</p>
</td>
</tr>
<tr id="row2114033123517"><td class="cellrowborder" valign="top" width="19.62%" headers="mcps1.2.4.1.1 "><p id="p1711493383514"><a name="p1711493383514"></a><a name="p1711493383514"></a>end_date</p>
</td>
<td class="cellrowborder" valign="top" width="18.48%" headers="mcps1.2.4.1.2 "><p id="p18115033173516"><a name="p18115033173516"></a><a name="p18115033173516"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="61.9%" headers="mcps1.2.4.1.3 "><p id="p911573343511"><a name="p911573343511"></a><a name="p911573343511"></a>子任务结束时间</p>
</td>
</tr>
</tbody>
</table>

**表 4**  source\_server结构

<a name="table247133203519"></a>
<table><thead align="left"><tr id="row1058512440312"><th class="cellrowborder" valign="top" width="19.88%" id="mcps1.2.4.1.1"><p id="p65129181948"><a name="p65129181948"></a><a name="p65129181948"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.310000000000002%" id="mcps1.2.4.1.2"><p id="p1252061819415"><a name="p1252061819415"></a><a name="p1252061819415"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.809999999999995%" id="mcps1.2.4.1.3"><p id="p85368182410"><a name="p85368182410"></a><a name="p85368182410"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row11115153318350"><td class="cellrowborder" valign="top" width="19.88%" headers="mcps1.2.4.1.1 "><p id="p211533373512"><a name="p211533373512"></a><a name="p211533373512"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.310000000000002%" headers="mcps1.2.4.1.2 "><p id="p20115163320352"><a name="p20115163320352"></a><a name="p20115163320352"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.809999999999995%" headers="mcps1.2.4.1.3 "><p id="p6115103312353"><a name="p6115103312353"></a><a name="p6115103312353"></a>该源端服务器在主机迁移服务上的ID</p>
</td>
</tr>
<tr id="row19115133353510"><td class="cellrowborder" valign="top" width="19.88%" headers="mcps1.2.4.1.1 "><p id="p13115173316352"><a name="p13115173316352"></a><a name="p13115173316352"></a>ip</p>
</td>
<td class="cellrowborder" valign="top" width="18.310000000000002%" headers="mcps1.2.4.1.2 "><p id="p1811523333511"><a name="p1811523333511"></a><a name="p1811523333511"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.809999999999995%" headers="mcps1.2.4.1.3 "><p id="p9115143323520"><a name="p9115143323520"></a><a name="p9115143323520"></a>源端服务器的IP地址</p>
</td>
</tr>
<tr id="row12115133143513"><td class="cellrowborder" valign="top" width="19.88%" headers="mcps1.2.4.1.1 "><p id="p61151333143516"><a name="p61151333143516"></a><a name="p61151333143516"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.310000000000002%" headers="mcps1.2.4.1.2 "><p id="p91151033203518"><a name="p91151033203518"></a><a name="p91151033203518"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.809999999999995%" headers="mcps1.2.4.1.3 "><p id="p1011513353517"><a name="p1011513353517"></a><a name="p1011513353517"></a>源端服务器的名称，用户可以在添加后进行修改，默认和hostname一致</p>
</td>
</tr>
<tr id="row811633363510"><td class="cellrowborder" valign="top" width="19.88%" headers="mcps1.2.4.1.1 "><p id="p1411611337350"><a name="p1411611337350"></a><a name="p1411611337350"></a>os_type</p>
</td>
<td class="cellrowborder" valign="top" width="18.310000000000002%" headers="mcps1.2.4.1.2 "><p id="p18116173311352"><a name="p18116173311352"></a><a name="p18116173311352"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.809999999999995%" headers="mcps1.2.4.1.3 "><a name="ul94118350149"></a><a name="ul94118350149"></a><ul id="ul94118350149"><li>WINDOWS：源端服务器为Windows系统</li><li>LINUX：源端服务器为Linux系统</li></ul>
</td>
</tr>
<tr id="row0116233123510"><td class="cellrowborder" valign="top" width="19.88%" headers="mcps1.2.4.1.1 "><p id="p811663315353"><a name="p811663315353"></a><a name="p811663315353"></a>os_version</p>
</td>
<td class="cellrowborder" valign="top" width="18.310000000000002%" headers="mcps1.2.4.1.2 "><p id="p1611617331357"><a name="p1611617331357"></a><a name="p1611617331357"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.809999999999995%" headers="mcps1.2.4.1.3 "><p id="p311673316354"><a name="p311673316354"></a><a name="p311673316354"></a>操作系统版本</p>
<p id="p612924318311"><a name="p612924318311"></a><a name="p612924318311"></a>例如：WINDOWS2008_R2_64BIT</p>
</td>
</tr>
<tr id="row5116163343517"><td class="cellrowborder" valign="top" width="19.88%" headers="mcps1.2.4.1.1 "><p id="p1411653312352"><a name="p1411653312352"></a><a name="p1411653312352"></a>oem_system</p>
</td>
<td class="cellrowborder" valign="top" width="18.310000000000002%" headers="mcps1.2.4.1.2 "><p id="p111633353514"><a name="p111633353514"></a><a name="p111633353514"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="61.809999999999995%" headers="mcps1.2.4.1.3 "><p id="p1411633316356"><a name="p1411633316356"></a><a name="p1411633316356"></a>是否是oem类型</p>
</td>
</tr>
<tr id="row1211653312356"><td class="cellrowborder" valign="top" width="19.88%" headers="mcps1.2.4.1.1 "><p id="p16116133333512"><a name="p16116133333512"></a><a name="p16116133333512"></a>state</p>
</td>
<td class="cellrowborder" valign="top" width="18.310000000000002%" headers="mcps1.2.4.1.2 "><p id="p911617336357"><a name="p911617336357"></a><a name="p911617336357"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.809999999999995%" headers="mcps1.2.4.1.3 "><p id="p117801523101715"><a name="p117801523101715"></a><a name="p117801523101715"></a>源端服务器的检查状态</p>
<a name="ul144031825131520"></a><a name="ul144031825131520"></a><ul id="ul144031825131520"><li>CHECKING：检查中</li><li>AVAILABLE：检查通过，可以迁移</li><li>UNAVAILABLE：检查失败，不能迁移</li></ul>
</td>
</tr>
</tbody>
</table>

**表 5**  target\_server结构

<a name="table129793243515"></a>
<table><thead align="left"><tr id="row17772452323"><th class="cellrowborder" valign="top" width="20.05%" id="mcps1.2.4.1.1"><p id="p1585723417413"><a name="p1585723417413"></a><a name="p1585723417413"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.05%" id="mcps1.2.4.1.2"><p id="p128624345418"><a name="p128624345418"></a><a name="p128624345418"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.9%" id="mcps1.2.4.1.3"><p id="p68741734644"><a name="p68741734644"></a><a name="p68741734644"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row121161633103514"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p011619334351"><a name="p011619334351"></a><a name="p011619334351"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.2.4.1.2 "><p id="p7116113353513"><a name="p7116113353513"></a><a name="p7116113353513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.9%" headers="mcps1.2.4.1.3 "><p id="p111723323517"><a name="p111723323517"></a><a name="p111723323517"></a>该源端服务器在主机迁移服务上的ID</p>
</td>
</tr>
<tr id="row12117233133519"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p611712335353"><a name="p611712335353"></a><a name="p611712335353"></a>vm_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.2.4.1.2 "><p id="p1711793316354"><a name="p1711793316354"></a><a name="p1711793316354"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.9%" headers="mcps1.2.4.1.3 "><p id="p8117133343513"><a name="p8117133343513"></a><a name="p8117133343513"></a>目的端服务器的ID</p>
</td>
</tr>
<tr id="row19117103383512"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p0117103320354"><a name="p0117103320354"></a><a name="p0117103320354"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.2.4.1.2 "><p id="p1711743312359"><a name="p1711743312359"></a><a name="p1711743312359"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.9%" headers="mcps1.2.4.1.3 "><p id="p011753303518"><a name="p011753303518"></a><a name="p011753303518"></a>目的端服务器的名称</p>
</td>
</tr>
<tr id="row81172334359"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p10117133323514"><a name="p10117133323514"></a><a name="p10117133323514"></a>ip</p>
</td>
<td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.2.4.1.2 "><p id="p311712331359"><a name="p311712331359"></a><a name="p311712331359"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.9%" headers="mcps1.2.4.1.3 "><p id="p14117143316351"><a name="p14117143316351"></a><a name="p14117143316351"></a>目的端服务器的私有IP</p>
</td>
</tr>
<tr id="row111179334352"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p111171333113518"><a name="p111171333113518"></a><a name="p111171333113518"></a>os_type</p>
</td>
<td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.2.4.1.2 "><p id="p14117183310359"><a name="p14117183310359"></a><a name="p14117183310359"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.9%" headers="mcps1.2.4.1.3 "><p id="p31171533163515"><a name="p31171533163515"></a><a name="p31171533163515"></a>目的端服务器的类型</p>
<a name="ul19582194416165"></a><a name="ul19582194416165"></a><ul id="ul19582194416165"><li>WINDOWS：目的端服务器为Windows</li><li>LINUX：目的端服务器为Linux</li></ul>
</td>
</tr>
<tr id="row14117193343514"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p1811713331351"><a name="p1811713331351"></a><a name="p1811713331351"></a>os_version</p>
</td>
<td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.2.4.1.2 "><p id="p161171833183512"><a name="p161171833183512"></a><a name="p161171833183512"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.9%" headers="mcps1.2.4.1.3 "><p id="p611793333517"><a name="p611793333517"></a><a name="p611793333517"></a>目的端服务器的版本号</p>
</td>
</tr>
<tr id="row121171733193514"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p1811783313518"><a name="p1811783313518"></a><a name="p1811783313518"></a>system_dir</p>
</td>
<td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.2.4.1.2 "><p id="p01171233153511"><a name="p01171233153511"></a><a name="p01171233153511"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.9%" headers="mcps1.2.4.1.3 "><p id="p311763317353"><a name="p311763317353"></a><a name="p311763317353"></a>系统目录</p>
<p id="p281419351264"><a name="p281419351264"></a><a name="p281419351264"></a>例如：C:\\Windows\\System32</p>
</td>
</tr>
<tr id="row121171332353"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p9117193315351"><a name="p9117193315351"></a><a name="p9117193315351"></a>disks</p>
</td>
<td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.2.4.1.2 "><p id="p211793393514"><a name="p211793393514"></a><a name="p211793393514"></a>JSON数组</p>
</td>
<td class="cellrowborder" valign="top" width="61.9%" headers="mcps1.2.4.1.3 "><p id="p2117633133512"><a name="p2117633133512"></a><a name="p2117633133512"></a>目的端服务器的磁盘信息</p>
</td>
</tr>
<tr id="row3117533103517"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="p10117333183514"><a name="p10117333183514"></a><a name="p10117333183514"></a>volume_groups</p>
</td>
<td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.2.4.1.2 "><p id="p15117143315351"><a name="p15117143315351"></a><a name="p15117143315351"></a>JSON数组</p>
</td>
<td class="cellrowborder" valign="top" width="61.9%" headers="mcps1.2.4.1.3 "><p id="p811843393511"><a name="p811843393511"></a><a name="p811843393511"></a>目的端服务器的卷组信息</p>
</td>
</tr>
</tbody>
</table>

**表 6**  disks成员数据结构

<a name="table215163223513"></a>
<table><thead align="left"><tr id="row5964629133215"><th class="cellrowborder" valign="top" width="20.23%" id="mcps1.2.4.1.1"><p id="p7991184918419"><a name="p7991184918419"></a><a name="p7991184918419"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.310000000000002%" id="mcps1.2.4.1.2"><p id="p179964491742"><a name="p179964491742"></a><a name="p179964491742"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.46%" id="mcps1.2.4.1.3"><p id="p811050344"><a name="p811050344"></a><a name="p811050344"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row19118233113520"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="p11118153313352"><a name="p11118153313352"></a><a name="p11118153313352"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.310000000000002%" headers="mcps1.2.4.1.2 "><p id="p6118933183519"><a name="p6118933183519"></a><a name="p6118933183519"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="61.46%" headers="mcps1.2.4.1.3 "><p id="p1811818331357"><a name="p1811818331357"></a><a name="p1811818331357"></a>该磁盘在SMS端数据库中的ID</p>
</td>
</tr>
<tr id="row16118183313510"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="p61185333350"><a name="p61185333350"></a><a name="p61185333350"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.310000000000002%" headers="mcps1.2.4.1.2 "><p id="p71188335351"><a name="p71188335351"></a><a name="p71188335351"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.46%" headers="mcps1.2.4.1.3 "><p id="p3118633133518"><a name="p3118633133518"></a><a name="p3118633133518"></a>磁盘的名称</p>
</td>
</tr>
<tr id="row16819130114312"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="p16821909431"><a name="p16821909431"></a><a name="p16821909431"></a>relation_name</p>
</td>
<td class="cellrowborder" valign="top" width="18.310000000000002%" headers="mcps1.2.4.1.2 "><p id="p682113012438"><a name="p682113012438"></a><a name="p682113012438"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.46%" headers="mcps1.2.4.1.3 "><p id="p18821501437"><a name="p18821501437"></a><a name="p18821501437"></a>该磁盘对应的源端磁盘名称</p>
</td>
</tr>
<tr id="row1311818334355"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="p2118123323510"><a name="p2118123323510"></a><a name="p2118123323510"></a>disk_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.310000000000002%" headers="mcps1.2.4.1.2 "><p id="p41189331351"><a name="p41189331351"></a><a name="p41189331351"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.46%" headers="mcps1.2.4.1.3 "><p id="p711853353512"><a name="p711853353512"></a><a name="p711853353512"></a>该块磁盘在EVS服务上的ID</p>
</td>
</tr>
<tr id="row1211883316355"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="p13118183313516"><a name="p13118183313516"></a><a name="p13118183313516"></a>partition_style</p>
</td>
<td class="cellrowborder" valign="top" width="18.310000000000002%" headers="mcps1.2.4.1.2 "><p id="p1118143320354"><a name="p1118143320354"></a><a name="p1118143320354"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.46%" headers="mcps1.2.4.1.3 "><p id="p1711816339357"><a name="p1711816339357"></a><a name="p1711816339357"></a>磁盘分区类型</p>
<a name="ul8723173820215"></a><a name="ul8723173820215"></a><ul id="ul8723173820215"><li>MBR：磁盘分区类型为MBR</li><li>GPT：磁盘分区类型为GPT</li></ul>
</td>
</tr>
<tr id="row18118333203511"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="p181185334357"><a name="p181185334357"></a><a name="p181185334357"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="18.310000000000002%" headers="mcps1.2.4.1.2 "><p id="p6118173316354"><a name="p6118173316354"></a><a name="p6118173316354"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="61.46%" headers="mcps1.2.4.1.3 "><p id="p211883303517"><a name="p211883303517"></a><a name="p211883303517"></a>磁盘大小</p>
</td>
</tr>
<tr id="row13124511101010"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="p4199172141014"><a name="p4199172141014"></a><a name="p4199172141014"></a>os_disk</p>
</td>
<td class="cellrowborder" valign="top" width="18.310000000000002%" headers="mcps1.2.4.1.2 "><p id="p121012218109"><a name="p121012218109"></a><a name="p121012218109"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.46%" headers="mcps1.2.4.1.3 "><p id="p14229112118103"><a name="p14229112118103"></a><a name="p14229112118103"></a>是否是系统盘</p>
</td>
</tr>
<tr id="row17118133323513"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="p61181333143513"><a name="p61181333143513"></a><a name="p61181333143513"></a>used_size</p>
</td>
<td class="cellrowborder" valign="top" width="18.310000000000002%" headers="mcps1.2.4.1.2 "><p id="p1611843314353"><a name="p1611843314353"></a><a name="p1611843314353"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.46%" headers="mcps1.2.4.1.3 "><p id="p3118193383515"><a name="p3118193383515"></a><a name="p3118193383515"></a>磁盘已使用大小</p>
</td>
</tr>
<tr id="row19118103323511"><td class="cellrowborder" valign="top" width="20.23%" headers="mcps1.2.4.1.1 "><p id="p111181533183519"><a name="p111181533183519"></a><a name="p111181533183519"></a>physical_volumes</p>
</td>
<td class="cellrowborder" valign="top" width="18.310000000000002%" headers="mcps1.2.4.1.2 "><p id="p1712033317358"><a name="p1712033317358"></a><a name="p1712033317358"></a>JSON数组</p>
</td>
<td class="cellrowborder" valign="top" width="61.46%" headers="mcps1.2.4.1.3 "><p id="p4120163353512"><a name="p4120163353512"></a><a name="p4120163353512"></a>该磁盘下的物理卷信息，参见<a href="#table319553210354">表7</a></p>
</td>
</tr>
</tbody>
</table>

**表 7**  physical\_volumes成员结构

<a name="table319553210354"></a>
<table><thead align="left"><tr id="row1512013338356"><th class="cellrowborder" valign="top" width="20.052005200520053%" id="mcps1.2.4.1.1"><p id="p75711460510"><a name="p75711460510"></a><a name="p75711460510"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.48184818481848%" id="mcps1.2.4.1.2"><p id="p10578963518"><a name="p10578963518"></a><a name="p10578963518"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.46614661466147%" id="mcps1.2.4.1.3"><p id="p19592860512"><a name="p19592860512"></a><a name="p19592860512"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row14120193393515"><td class="cellrowborder" valign="top" width="20.052005200520053%" headers="mcps1.2.4.1.1 "><p id="p612003318353"><a name="p612003318353"></a><a name="p612003318353"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.48184818481848%" headers="mcps1.2.4.1.2 "><p id="p18120433193512"><a name="p18120433193512"></a><a name="p18120433193512"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="61.46614661466147%" headers="mcps1.2.4.1.3 "><p id="p1912018337355"><a name="p1912018337355"></a><a name="p1912018337355"></a>该物理分区在数据库中id</p>
</td>
</tr>
<tr id="row141201338351"><td class="cellrowborder" valign="top" width="20.052005200520053%" headers="mcps1.2.4.1.1 "><p id="p812023314356"><a name="p812023314356"></a><a name="p812023314356"></a>uuid</p>
</td>
<td class="cellrowborder" valign="top" width="18.48184818481848%" headers="mcps1.2.4.1.2 "><p id="p5120163318358"><a name="p5120163318358"></a><a name="p5120163318358"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.46614661466147%" headers="mcps1.2.4.1.3 "><p id="p1912023312357"><a name="p1912023312357"></a><a name="p1912023312357"></a>分区的UUID</p>
</td>
</tr>
<tr id="row612093333519"><td class="cellrowborder" valign="top" width="20.052005200520053%" headers="mcps1.2.4.1.1 "><p id="p17120433183510"><a name="p17120433183510"></a><a name="p17120433183510"></a>index</p>
</td>
<td class="cellrowborder" valign="top" width="18.48184818481848%" headers="mcps1.2.4.1.2 "><p id="p112053315357"><a name="p112053315357"></a><a name="p112053315357"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="61.46614661466147%" headers="mcps1.2.4.1.3 "><p id="p1112093343515"><a name="p1112093343515"></a><a name="p1112093343515"></a>该分区的序号</p>
</td>
</tr>
<tr id="row944512244411"><td class="cellrowborder" valign="top" width="20.052005200520053%" headers="mcps1.2.4.1.1 "><p id="p1548410299446"><a name="p1548410299446"></a><a name="p1548410299446"></a>relation_name</p>
</td>
<td class="cellrowborder" valign="top" width="18.48184818481848%" headers="mcps1.2.4.1.2 "><p id="p44459221449"><a name="p44459221449"></a><a name="p44459221449"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.46614661466147%" headers="mcps1.2.4.1.3 "><p id="p7445422124419"><a name="p7445422124419"></a><a name="p7445422124419"></a>该分区对应的源端分区名称</p>
</td>
</tr>
<tr id="row12120133173516"><td class="cellrowborder" valign="top" width="20.052005200520053%" headers="mcps1.2.4.1.1 "><p id="p151201133163515"><a name="p151201133163515"></a><a name="p151201133163515"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.48184818481848%" headers="mcps1.2.4.1.2 "><p id="p4120193315354"><a name="p4120193315354"></a><a name="p4120193315354"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.46614661466147%" headers="mcps1.2.4.1.3 "><p id="p19120153315352"><a name="p19120153315352"></a><a name="p19120153315352"></a>分区名称，如Windows的C和Linux的/dev/vda1</p>
</td>
</tr>
<tr id="row712016333355"><td class="cellrowborder" valign="top" width="20.052005200520053%" headers="mcps1.2.4.1.1 "><p id="p9120433203510"><a name="p9120433203510"></a><a name="p9120433203510"></a>device_use</p>
</td>
<td class="cellrowborder" valign="top" width="18.48184818481848%" headers="mcps1.2.4.1.2 "><p id="p3120143343519"><a name="p3120143343519"></a><a name="p3120143343519"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.46614661466147%" headers="mcps1.2.4.1.3 "><p id="p8228132013166"><a name="p8228132013166"></a><a name="p8228132013166"></a>该分区的用户</p>
<a name="ul1550319251232"></a><a name="ul1550319251232"></a><ul id="ul1550319251232"><li>BOOT：引导分区</li><li>OS：系统分区</li><li>NORMAL：普通分区</li></ul>
</td>
</tr>
<tr id="row101207332356"><td class="cellrowborder" valign="top" width="20.052005200520053%" headers="mcps1.2.4.1.1 "><p id="p11120203313518"><a name="p11120203313518"></a><a name="p11120203313518"></a>file_system</p>
</td>
<td class="cellrowborder" valign="top" width="18.48184818481848%" headers="mcps1.2.4.1.2 "><p id="p141209333353"><a name="p141209333353"></a><a name="p141209333353"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.46614661466147%" headers="mcps1.2.4.1.3 "><p id="p1912083317358"><a name="p1912083317358"></a><a name="p1912083317358"></a>分区的文件系统类型</p>
<p id="p1775095941619"><a name="p1775095941619"></a><a name="p1775095941619"></a>例如：NTFS</p>
</td>
</tr>
<tr id="row1120733183514"><td class="cellrowborder" valign="top" width="20.052005200520053%" headers="mcps1.2.4.1.1 "><p id="p181201933183520"><a name="p181201933183520"></a><a name="p181201933183520"></a>mount_point</p>
</td>
<td class="cellrowborder" valign="top" width="18.48184818481848%" headers="mcps1.2.4.1.2 "><p id="p3120633123512"><a name="p3120633123512"></a><a name="p3120633123512"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.46614661466147%" headers="mcps1.2.4.1.3 "><p id="p012012333352"><a name="p012012333352"></a><a name="p012012333352"></a>该分区的挂载点</p>
</td>
</tr>
<tr id="row1812073317359"><td class="cellrowborder" valign="top" width="20.052005200520053%" headers="mcps1.2.4.1.1 "><p id="p151206337354"><a name="p151206337354"></a><a name="p151206337354"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="18.48184818481848%" headers="mcps1.2.4.1.2 "><p id="p143631357162320"><a name="p143631357162320"></a><a name="p143631357162320"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="61.46614661466147%" headers="mcps1.2.4.1.3 "><p id="p7120173323515"><a name="p7120173323515"></a><a name="p7120173323515"></a>该分区总共大小</p>
</td>
</tr>
<tr id="row161209335356"><td class="cellrowborder" valign="top" width="20.052005200520053%" headers="mcps1.2.4.1.1 "><p id="p13120143319355"><a name="p13120143319355"></a><a name="p13120143319355"></a>used_size</p>
</td>
<td class="cellrowborder" valign="top" width="18.48184818481848%" headers="mcps1.2.4.1.2 "><p id="p1237375772315"><a name="p1237375772315"></a><a name="p1237375772315"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="61.46614661466147%" headers="mcps1.2.4.1.3 "><p id="p712013314353"><a name="p712013314353"></a><a name="p712013314353"></a>该分区已使用大小</p>
</td>
</tr>
<tr id="row5120193318350"><td class="cellrowborder" valign="top" width="20.052005200520053%" headers="mcps1.2.4.1.1 "><p id="p912011330351"><a name="p912011330351"></a><a name="p912011330351"></a>free_size</p>
</td>
<td class="cellrowborder" valign="top" width="18.48184818481848%" headers="mcps1.2.4.1.2 "><p id="p1379257182311"><a name="p1379257182311"></a><a name="p1379257182311"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="61.46614661466147%" headers="mcps1.2.4.1.3 "><p id="p19120433183513"><a name="p19120433183513"></a><a name="p19120433183513"></a>该分区剩余大小</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section62802032193520"></a>

-   请求示例

    无请求消息。


-   响应示例

    ```
    {
     "id": "65da430b-9538-4296-abd0-86a5aaf13c77",
     "name": "sms_task_smssource",
     "type": "MIGRATE_BLOCK",
     "os_type": "WINDOWS",
     "state": "READY",
     "connected": true,
     "estimate_complete_time": null,
     "create_date": 1528699579000,
     "start_date": null,
     "finish_date": null,
     "priority": 1,
     "speed_limit": 0,
     "migrate_speed": 0.0,
     "start_target_server": true,
     "error_json": "",
     "total_time": 0,
     "migration_ip": "192.168.1.175",
     "region_name":"north-china",
     "region_id":"cn-north-1",
     "project_name":"cn-north-1",
     
     
     
     
     
     
     "project_id": "962def8b6e984888b80501c851d534b2",
     "sub_tasks": [{
       "id": 477,
       "name": "ATTACH_AGENT_IMAGE",
       "progress": 0,
       "start_date": null,
       "end_date": null,
       "totalTime": 0
      }, {
       "id": 484,
       "name": "FORMAT_DISK_WINDOWS",
       "progress": 0,
       "start_date": null,
       "end_date": null,
       "totalTime": 0
      }, {
       "id": 491,
       "name": "MIGRATE_WINDOWS_BLOCK",
       "progress": 0,
       "start_date": null,
       "end_date": null,
       "totalTime": 0
      }, {
       "id": 498,
       "name": "CONFIGURE_WINDOWS",
       "progress": 0,
       "start_date": null,
       "end_date": null,
       "totalTime": 0
      }, {
       "id": 505,
       "name": "DETTACH_AGENT_IMAGE",
       "progress": 0,
       "start_date": null,
       "end_date": null,
       "totalTime": 0
      }
     ],
     "source_server": {
      "id": "a013ec5f-00d6-456b-8c1f-085599cb97e9",
      "ip": "192.168.1.57",
      "name": "smssource",
      "os_type": "WINDOWS",
      "os_version": "WINDOWS2008_R2_64BIT",
      "oem_system": false,
      "state": "AVAILABLE"
     },
     "target_server": {
      "id": "ec5eca22-db21-49b0-ae53-56a74f0318ec",
      "vm_id": "7c804c50-e9eb-40af-86ec-c78da64f22e2",
      "name": "smssrc",
      "ip": null,
      "os_type": "WINDOWS",
      "os_version": "WINDOWS2008_R2_64BIT",
      "system_dir": "Y:\\Windows\\System32",
      "disks": [{
        "id": 736,
        "name": "Disk 1",
        "disk_id": "e853bb2d-57e0-42b2-96c0-68794063fb0f",
        "partition_style": "MBR",
        "size": 53687091200,
        "used_size": 42964353024,
        "os_disk": true,
        "physical_volumes": [{
          "id": 1135,
          "uuid": "\\?\Volume{f5a31ed9-cde8-11e6-9dd0-806e6f6e6963}\",
          "index": 1,
          "name": "Z:",
          "device_use": "BOOT",
          "file_system": "NTFS",
          "mount_point": null,
          "size": 113246208,
          "used_size": 25624064,
          "free_size": 87622144
         }, {
          "id": 1142,
          "uuid": "\\?\Volume{f5a31eda-cde8-11e6-9dd0-806e6f6e6963}\",
          "index": 2,
          "name": "Y:",
          "device_use": "OS",
          "file_system": "NTFS",
          "mount_point": null,
          "size": 42851106816,
          "used_size": 26961067520,
          "free_size": 15890039296
         }
        ]
       }
      ],
      "volume_groups": []
     }
    }
    ```


## 状态码<a name="section1973012935418"></a>

状态码请参见[状态码](状态码.md)。

## 错误码<a name="section11559103243512"></a>

请参见[错误码](错误码.md)。

