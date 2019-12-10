# 查询指定ID的源端服务器<a name="ZH-CN_TOPIC_0114396645"></a>

## 功能介绍<a name="section8136152152415"></a>

迁移Agent将源端服务器信息上报到主机迁移服务后，主机迁移服务会对迁移的可行性进行检测，该接口返回源端服务器的基本信息和检查结果。

## URI<a name="section1214245292416"></a>

GET /v1/sms/sources/\{source\_id\}

参数说明请参见[表1](#table19401936124514)。

**表 1**  参数说明

<a name="table19401936124514"></a>
<table><thead align="left"><tr id="row2381836204510"><th class="cellrowborder" valign="top" width="15.21485287248949%" id="mcps1.2.4.1.1"><p id="p1238336194516"><a name="p1238336194516"></a><a name="p1238336194516"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="17.106492293320876%" id="mcps1.2.4.1.2"><p id="p838173612451"><a name="p838173612451"></a><a name="p838173612451"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="67.67865483418962%" id="mcps1.2.4.1.3"><p id="p8389363452"><a name="p8389363452"></a><a name="p8389363452"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row140136154515"><td class="cellrowborder" valign="top" width="15.21485287248949%" headers="mcps1.2.4.1.1 "><p id="p1138736174513"><a name="p1138736174513"></a><a name="p1138736174513"></a>source_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.106492293320876%" headers="mcps1.2.4.1.2 "><p id="p538113644516"><a name="p538113644516"></a><a name="p538113644516"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="67.67865483418962%" headers="mcps1.2.4.1.3 "><p id="p1040123624514"><a name="p1040123624514"></a><a name="p1040123624514"></a>源端服务器的ID</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section7166135222420"></a>

不涉及

## 响应消息<a name="section116618528243"></a>

**响应参数**

响应参数如[表2](#table19174145211249)所示。

**表 2**  响应参数

<a name="table19174145211249"></a>
<table><thead align="left"><tr id="row16833549248"><th class="cellrowborder" valign="top" width="18.22%" id="mcps1.2.4.1.1"><p id="p69379014542"><a name="p69379014542"></a><a name="p69379014542"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.4%" id="mcps1.2.4.1.2"><p id="p394510010544"><a name="p394510010544"></a><a name="p394510010544"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="63.38%" id="mcps1.2.4.1.3"><p id="p39638005415"><a name="p39638005415"></a><a name="p39638005415"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row15836543241"><td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.2.4.1.1 "><p id="p17837544242"><a name="p17837544242"></a><a name="p17837544242"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.4.1.2 "><p id="p198315412248"><a name="p198315412248"></a><a name="p198315412248"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="63.38%" headers="mcps1.2.4.1.3 "><p id="p178305472410"><a name="p178305472410"></a><a name="p178305472410"></a>该源端服务器在主机迁移服务上的ID</p>
</td>
</tr>
<tr id="row783454152412"><td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.2.4.1.1 "><p id="p48311544240"><a name="p48311544240"></a><a name="p48311544240"></a>ip</p>
</td>
<td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.4.1.2 "><p id="p1883205418245"><a name="p1883205418245"></a><a name="p1883205418245"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="63.38%" headers="mcps1.2.4.1.3 "><p id="p783195432416"><a name="p783195432416"></a><a name="p783195432416"></a>源端服务器的IP地址</p>
</td>
</tr>
<tr id="row5497174242115"><td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.2.4.1.1 "><p id="p1544116216222"><a name="p1544116216222"></a><a name="p1544116216222"></a>os_type</p>
</td>
<td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.4.1.2 "><p id="p1044872172214"><a name="p1044872172214"></a><a name="p1044872172214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="63.38%" headers="mcps1.2.4.1.3 "><p id="p64601024226"><a name="p64601024226"></a><a name="p64601024226"></a>源端服务器的OS类型，分为WINDOWS或者LINUX</p>
</td>
</tr>
<tr id="row284446192115"><td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.2.4.1.1 "><p id="p184671126227"><a name="p184671126227"></a><a name="p184671126227"></a>os_version</p>
</td>
<td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.4.1.2 "><p id="p94741522228"><a name="p94741522228"></a><a name="p94741522228"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="63.38%" headers="mcps1.2.4.1.3 "><p id="p164850262211"><a name="p164850262211"></a><a name="p164850262211"></a>操作系统版本，如WINDOWS7_64BIT</p>
</td>
</tr>
<tr id="row2073219162205"><td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.2.4.1.1 "><p id="p073212165207"><a name="p073212165207"></a><a name="p073212165207"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.4.1.2 "><p id="p167341816152019"><a name="p167341816152019"></a><a name="p167341816152019"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="63.38%" headers="mcps1.2.4.1.3 "><p id="p1373461652014"><a name="p1373461652014"></a><a name="p1373461652014"></a>源端服务器的名称，可以更改</p>
</td>
</tr>
<tr id="row128345432415"><td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.2.4.1.1 "><p id="p88395452410"><a name="p88395452410"></a><a name="p88395452410"></a>hostname</p>
</td>
<td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.4.1.2 "><p id="p16831354132420"><a name="p16831354132420"></a><a name="p16831354132420"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="63.38%" headers="mcps1.2.4.1.3 "><p id="p17837544241"><a name="p17837544241"></a><a name="p17837544241"></a>登录源端服务器后显示的名称</p>
</td>
</tr>
<tr id="row16831054132415"><td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.2.4.1.1 "><p id="p148310540247"><a name="p148310540247"></a><a name="p148310540247"></a>add_date</p>
</td>
<td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.4.1.2 "><p id="p118305482415"><a name="p118305482415"></a><a name="p118305482415"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="63.38%" headers="mcps1.2.4.1.3 "><p id="p1883185472414"><a name="p1883185472414"></a><a name="p1883185472414"></a>源端服务器被添加到主机迁移服务的时间。单位毫秒</p>
</td>
</tr>
<tr id="row884554152410"><td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.2.4.1.1 "><p id="p1084155422419"><a name="p1084155422419"></a><a name="p1084155422419"></a>oem_system</p>
</td>
<td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.4.1.2 "><p id="p138445417242"><a name="p138445417242"></a><a name="p138445417242"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="63.38%" headers="mcps1.2.4.1.3 "><p id="p6847548242"><a name="p6847548242"></a><a name="p6847548242"></a>源端服务器是否为oem操作系统</p>
</td>
</tr>
<tr id="row188455442416"><td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.2.4.1.1 "><p id="p19840540245"><a name="p19840540245"></a><a name="p19840540245"></a>state</p>
</td>
<td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.4.1.2 "><p id="p1184125482414"><a name="p1184125482414"></a><a name="p1184125482414"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="63.38%" headers="mcps1.2.4.1.3 "><p id="p117801523101715"><a name="p117801523101715"></a><a name="p117801523101715"></a>源端服务器的检查状态</p>
<a name="ul18448111319556"></a><a name="ul18448111319556"></a><ul id="ul18448111319556"><li>CHECKING：检查中</li><li>AVAILABLE：检查通过，可以迁移上云</li><li>UNAVAILABLE：检查失败，不能迁移</li></ul>
</td>
</tr>
<tr id="row138475417243"><td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.2.4.1.1 "><p id="p148411547242"><a name="p148411547242"></a><a name="p148411547242"></a>connected</p>
</td>
<td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.4.1.2 "><p id="p168425412249"><a name="p168425412249"></a><a name="p168425412249"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="63.38%" headers="mcps1.2.4.1.3 "><p id="p784155412241"><a name="p784155412241"></a><a name="p784155412241"></a>该源端服务器与主机迁移服务是否处于连接状态</p>
<a name="ul1589316302564"></a><a name="ul1589316302564"></a><ul id="ul1589316302564"><li>true：源端服务器同主机迁移服务连接正常</li><li>false：源端服务器同主机迁移服务失去连接</li></ul>
</td>
</tr>
<tr id="row88485417245"><td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.2.4.1.1 "><p id="p20845548247"><a name="p20845548247"></a><a name="p20845548247"></a>firmware</p>
</td>
<td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.4.1.2 "><p id="p15841854182415"><a name="p15841854182415"></a><a name="p15841854182415"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="63.38%" headers="mcps1.2.4.1.3 "><p id="p1984165402417"><a name="p1984165402417"></a><a name="p1984165402417"></a>源端服务器启动类型，如BIOS或者UEFI</p>
</td>
</tr>
<tr id="row1784145452415"><td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.2.4.1.1 "><p id="p38419547243"><a name="p38419547243"></a><a name="p38419547243"></a>cpu_quantity</p>
</td>
<td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.4.1.2 "><p id="p3846543246"><a name="p3846543246"></a><a name="p3846543246"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="63.38%" headers="mcps1.2.4.1.3 "><p id="p198485412248"><a name="p198485412248"></a><a name="p198485412248"></a>CPU个数，单位个</p>
</td>
</tr>
<tr id="row128475417248"><td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.2.4.1.1 "><p id="p1884115482412"><a name="p1884115482412"></a><a name="p1884115482412"></a>memory</p>
</td>
<td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.4.1.2 "><p id="p15841554192416"><a name="p15841554192416"></a><a name="p15841554192416"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="63.38%" headers="mcps1.2.4.1.3 "><p id="p384954182417"><a name="p384954182417"></a><a name="p384954182417"></a>内存大小，单位MB</p>
</td>
</tr>
<tr id="row084155402412"><td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.2.4.1.1 "><p id="p1184185442418"><a name="p1184185442418"></a><a name="p1184185442418"></a>disks</p>
</td>
<td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.4.1.2 "><p id="p1184354182414"><a name="p1184354182414"></a><a name="p1184354182414"></a>JSON数组</p>
</td>
<td class="cellrowborder" valign="top" width="63.38%" headers="mcps1.2.4.1.3 "><p id="p184105492413"><a name="p184105492413"></a><a name="p184105492413"></a>源端服务器的磁盘信息，参见<a href="#table153490523246">表3</a></p>
</td>
</tr>
<tr id="row1284754142416"><td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.2.4.1.1 "><p id="p4841054192418"><a name="p4841054192418"></a><a name="p4841054192418"></a>volume_groups</p>
</td>
<td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.4.1.2 "><p id="p58435412411"><a name="p58435412411"></a><a name="p58435412411"></a>JSON数组</p>
</td>
<td class="cellrowborder" valign="top" width="63.38%" headers="mcps1.2.4.1.3 "><p id="p1984195432412"><a name="p1984195432412"></a><a name="p1984195432412"></a>Linux主机的卷组信息，参见<a href="#table134651752132414">表5</a></p>
</td>
</tr>
<tr id="row6847548249"><td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.2.4.1.1 "><p id="p6862541242"><a name="p6862541242"></a><a name="p6862541242"></a>network</p>
</td>
<td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.4.1.2 "><p id="p286175416244"><a name="p286175416244"></a><a name="p286175416244"></a>JSON数组</p>
</td>
<td class="cellrowborder" valign="top" width="63.38%" headers="mcps1.2.4.1.3 "><p id="p986135412247"><a name="p986135412247"></a><a name="p986135412247"></a>源端服务器的网卡信息，参见<a href="#table1258675272414">表7</a></p>
</td>
</tr>
<tr id="row18863548244"><td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.2.4.1.1 "><p id="p08665442411"><a name="p08665442411"></a><a name="p08665442411"></a>checks</p>
</td>
<td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.4.1.2 "><p id="p986754112412"><a name="p986754112412"></a><a name="p986754112412"></a>JSON数组</p>
</td>
<td class="cellrowborder" valign="top" width="63.38%" headers="mcps1.2.4.1.3 "><p id="p1086754112418"><a name="p1086754112418"></a><a name="p1086754112418"></a>源端服务器的检查项，参见<a href="#table32630264308">表8</a></p>
</td>
</tr>
<tr id="row198695492414"><td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.2.4.1.1 "><p id="p38665482419"><a name="p38665482419"></a><a name="p38665482419"></a>init_target_server</p>
</td>
<td class="cellrowborder" valign="top" width="18.4%" headers="mcps1.2.4.1.2 "><p id="p19861254102413"><a name="p19861254102413"></a><a name="p19861254102413"></a>JSON</p>
</td>
<td class="cellrowborder" valign="top" width="63.38%" headers="mcps1.2.4.1.3 "><p id="p986854202418"><a name="p986854202418"></a><a name="p986854202418"></a>推荐的目的端服务器配置，参见<a href="#table1862585272417">表9</a></p>
</td>
</tr>
</tbody>
</table>

**表 3**  disks数据结构

<a name="table153490523246"></a>
<table><thead align="left"><tr id="row16861454142410"><th class="cellrowborder" valign="top" width="18.13181318131813%" id="mcps1.2.4.1.1"><p id="p1310784112543"><a name="p1310784112543"></a><a name="p1310784112543"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.57185718571857%" id="mcps1.2.4.1.2"><p id="p811974113547"><a name="p811974113547"></a><a name="p811974113547"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="63.2963296329633%" id="mcps1.2.4.1.3"><p id="p171315411541"><a name="p171315411541"></a><a name="p171315411541"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1286145492416"><td class="cellrowborder" valign="top" width="18.13181318131813%" headers="mcps1.2.4.1.1 "><p id="p4869543242"><a name="p4869543242"></a><a name="p4869543242"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.57185718571857%" headers="mcps1.2.4.1.2 "><p id="p18861454192414"><a name="p18861454192414"></a><a name="p18861454192414"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="63.2963296329633%" headers="mcps1.2.4.1.3 "><p id="p138611545242"><a name="p138611545242"></a><a name="p138611545242"></a>磁盘名称</p>
</td>
</tr>
<tr id="row1486135417248"><td class="cellrowborder" valign="top" width="18.13181318131813%" headers="mcps1.2.4.1.1 "><p id="p78695482412"><a name="p78695482412"></a><a name="p78695482412"></a>partition_style</p>
</td>
<td class="cellrowborder" valign="top" width="18.57185718571857%" headers="mcps1.2.4.1.2 "><p id="p08625412410"><a name="p08625412410"></a><a name="p08625412410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="63.2963296329633%" headers="mcps1.2.4.1.3 "><p id="p178675422417"><a name="p178675422417"></a><a name="p178675422417"></a>磁盘的分区类型。如MBR、GPT等</p>
</td>
</tr>
<tr id="row1186135415241"><td class="cellrowborder" valign="top" width="18.13181318131813%" headers="mcps1.2.4.1.1 "><p id="p186155402412"><a name="p186155402412"></a><a name="p186155402412"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="18.57185718571857%" headers="mcps1.2.4.1.2 "><p id="p1386135416244"><a name="p1386135416244"></a><a name="p1386135416244"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="63.2963296329633%" headers="mcps1.2.4.1.3 "><p id="p14874541249"><a name="p14874541249"></a><a name="p14874541249"></a>磁盘总大小，以字节为单位</p>
</td>
</tr>
<tr id="row188775442418"><td class="cellrowborder" valign="top" width="18.13181318131813%" headers="mcps1.2.4.1.1 "><p id="p58785442414"><a name="p58785442414"></a><a name="p58785442414"></a>used_size</p>
</td>
<td class="cellrowborder" valign="top" width="18.57185718571857%" headers="mcps1.2.4.1.2 "><p id="p58713546244"><a name="p58713546244"></a><a name="p58713546244"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="63.2963296329633%" headers="mcps1.2.4.1.3 "><p id="p887105414242"><a name="p887105414242"></a><a name="p887105414242"></a>磁盘已使用大小，以字节为单位</p>
</td>
</tr>
<tr id="row18775442419"><td class="cellrowborder" valign="top" width="18.13181318131813%" headers="mcps1.2.4.1.1 "><p id="p387454112411"><a name="p387454112411"></a><a name="p387454112411"></a>device_use</p>
</td>
<td class="cellrowborder" valign="top" width="18.57185718571857%" headers="mcps1.2.4.1.2 "><p id="p5871854162416"><a name="p5871854162416"></a><a name="p5871854162416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="63.2963296329633%" headers="mcps1.2.4.1.3 "><p id="p054818933513"><a name="p054818933513"></a><a name="p054818933513"></a>磁盘用途</p>
<a name="ul1688584918598"></a><a name="ul1688584918598"></a><ul id="ul1688584918598"><li>BOOT：引导分区在该磁盘上</li><li>OS：系统分区在该磁盘上</li></ul>
</td>
</tr>
<tr id="row13871954122410"><td class="cellrowborder" valign="top" width="18.13181318131813%" headers="mcps1.2.4.1.1 "><p id="p187254102417"><a name="p187254102417"></a><a name="p187254102417"></a>os_disk</p>
</td>
<td class="cellrowborder" valign="top" width="18.57185718571857%" headers="mcps1.2.4.1.2 "><p id="p58719548246"><a name="p58719548246"></a><a name="p58719548246"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="63.2963296329633%" headers="mcps1.2.4.1.3 "><p id="p28719549241"><a name="p28719549241"></a><a name="p28719549241"></a>是否是系统盘</p>
<a name="ul62465173013"></a><a name="ul62465173013"></a><ul id="ul62465173013"><li>true：该磁盘为系统盘</li><li>false：该磁盘为数据盘</li></ul>
</td>
</tr>
<tr id="row88705418244"><td class="cellrowborder" valign="top" width="18.13181318131813%" headers="mcps1.2.4.1.1 "><p id="p1987105419240"><a name="p1987105419240"></a><a name="p1987105419240"></a>physical_volumes</p>
</td>
<td class="cellrowborder" valign="top" width="18.57185718571857%" headers="mcps1.2.4.1.2 "><p id="p68717548242"><a name="p68717548242"></a><a name="p68717548242"></a>JSON数组</p>
</td>
<td class="cellrowborder" valign="top" width="63.2963296329633%" headers="mcps1.2.4.1.3 "><p id="p88718544243"><a name="p88718544243"></a><a name="p88718544243"></a>磁盘上的物理分区信息，参见<a href="#table641318526244">表4</a></p>
</td>
</tr>
</tbody>
</table>

**表 4**  physical\_volumes中数据元素的数据结构

<a name="table641318526244"></a>
<table><thead align="left"><tr id="row198775442418"><th class="cellrowborder" valign="top" width="18.221822182218222%" id="mcps1.2.4.1.1"><p id="p1030706115516"><a name="p1030706115516"></a><a name="p1030706115516"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.18191819181918%" id="mcps1.2.4.1.2"><p id="p1231815617559"><a name="p1231815617559"></a><a name="p1231815617559"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="62.59625962596259%" id="mcps1.2.4.1.3"><p id="p1933026175515"><a name="p1933026175515"></a><a name="p1933026175515"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row168717542246"><td class="cellrowborder" valign="top" width="18.221822182218222%" headers="mcps1.2.4.1.1 "><p id="p168735432410"><a name="p168735432410"></a><a name="p168735432410"></a>uuid</p>
</td>
<td class="cellrowborder" valign="top" width="19.18191819181918%" headers="mcps1.2.4.1.2 "><p id="p887115412417"><a name="p887115412417"></a><a name="p887115412417"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.59625962596259%" headers="mcps1.2.4.1.3 "><p id="p8873540241"><a name="p8873540241"></a><a name="p8873540241"></a>该分区的UUID</p>
</td>
</tr>
<tr id="row11237224193613"><td class="cellrowborder" valign="top" width="18.221822182218222%" headers="mcps1.2.4.1.1 "><p id="p1023882453610"><a name="p1023882453610"></a><a name="p1023882453610"></a>index</p>
</td>
<td class="cellrowborder" valign="top" width="19.18191819181918%" headers="mcps1.2.4.1.2 "><p id="p12389245366"><a name="p12389245366"></a><a name="p12389245366"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="62.59625962596259%" headers="mcps1.2.4.1.3 "><p id="p023892412362"><a name="p023892412362"></a><a name="p023892412362"></a>该物理分区的序号</p>
<a name="ul03954108115"></a><a name="ul03954108115"></a><ul id="ul03954108115"><li>0：第一个分区</li><li>1：第二个分区</li></ul>
</td>
</tr>
<tr id="row88775472417"><td class="cellrowborder" valign="top" width="18.221822182218222%" headers="mcps1.2.4.1.1 "><p id="p1487205417248"><a name="p1487205417248"></a><a name="p1487205417248"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="19.18191819181918%" headers="mcps1.2.4.1.2 "><p id="p1987454172420"><a name="p1987454172420"></a><a name="p1987454172420"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.59625962596259%" headers="mcps1.2.4.1.3 "><p id="p18885542245"><a name="p18885542245"></a><a name="p18885542245"></a>分区名称，如Windows的C和Linux的/dev/vda1</p>
</td>
</tr>
<tr id="row1888854182420"><td class="cellrowborder" valign="top" width="18.221822182218222%" headers="mcps1.2.4.1.1 "><p id="p88814543242"><a name="p88814543242"></a><a name="p88814543242"></a>device_use</p>
</td>
<td class="cellrowborder" valign="top" width="19.18191819181918%" headers="mcps1.2.4.1.2 "><p id="p588185410241"><a name="p588185410241"></a><a name="p588185410241"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.59625962596259%" headers="mcps1.2.4.1.3 "><p id="p1188115432419"><a name="p1188115432419"></a><a name="p1188115432419"></a>分区的用户，取值OS或者BOOT</p>
</td>
</tr>
<tr id="row088654162412"><td class="cellrowborder" valign="top" width="18.221822182218222%" headers="mcps1.2.4.1.1 "><p id="p28845482417"><a name="p28845482417"></a><a name="p28845482417"></a>file_system</p>
</td>
<td class="cellrowborder" valign="top" width="19.18191819181918%" headers="mcps1.2.4.1.2 "><p id="p3881254142410"><a name="p3881254142410"></a><a name="p3881254142410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.59625962596259%" headers="mcps1.2.4.1.3 "><p id="p788175452413"><a name="p788175452413"></a><a name="p788175452413"></a>分区的文件系统类型</p>
</td>
</tr>
<tr id="row10881354132416"><td class="cellrowborder" valign="top" width="18.221822182218222%" headers="mcps1.2.4.1.1 "><p id="p128810545243"><a name="p128810545243"></a><a name="p128810545243"></a>mount_point</p>
</td>
<td class="cellrowborder" valign="top" width="19.18191819181918%" headers="mcps1.2.4.1.2 "><p id="p108835416241"><a name="p108835416241"></a><a name="p108835416241"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.59625962596259%" headers="mcps1.2.4.1.3 "><p id="p128825402417"><a name="p128825402417"></a><a name="p128825402417"></a>挂载点</p>
</td>
</tr>
<tr id="row588054162412"><td class="cellrowborder" valign="top" width="18.221822182218222%" headers="mcps1.2.4.1.1 "><p id="p88815413243"><a name="p88815413243"></a><a name="p88815413243"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="19.18191819181918%" headers="mcps1.2.4.1.2 "><p id="p488254182410"><a name="p488254182410"></a><a name="p488254182410"></a>Long</p>
</td>
<td class="cellrowborder" valign="top" width="62.59625962596259%" headers="mcps1.2.4.1.3 "><p id="p188875442415"><a name="p188875442415"></a><a name="p188875442415"></a>分区总共大小</p>
</td>
</tr>
<tr id="row16881054202420"><td class="cellrowborder" valign="top" width="18.221822182218222%" headers="mcps1.2.4.1.1 "><p id="p388354152417"><a name="p388354152417"></a><a name="p388354152417"></a>used_size</p>
</td>
<td class="cellrowborder" valign="top" width="19.18191819181918%" headers="mcps1.2.4.1.2 "><p id="p588135419243"><a name="p588135419243"></a><a name="p588135419243"></a>Long</p>
</td>
<td class="cellrowborder" valign="top" width="62.59625962596259%" headers="mcps1.2.4.1.3 "><p id="p988125410246"><a name="p988125410246"></a><a name="p988125410246"></a>分区已使用大小</p>
</td>
</tr>
</tbody>
</table>

**表 5**  volume\_groups数据结构

<a name="table134651752132414"></a>
<table><thead align="left"><tr id="row3881054102414"><th class="cellrowborder" valign="top" width="18.21817818218178%" id="mcps1.2.4.1.1"><p id="p204673288551"><a name="p204673288551"></a><a name="p204673288551"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.26807319268073%" id="mcps1.2.4.1.2"><p id="p1148213281551"><a name="p1148213281551"></a><a name="p1148213281551"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="62.51374862513749%" id="mcps1.2.4.1.3"><p id="p6495132814556"><a name="p6495132814556"></a><a name="p6495132814556"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row148825415241"><td class="cellrowborder" valign="top" width="18.21817818218178%" headers="mcps1.2.4.1.1 "><p id="p588195413241"><a name="p588195413241"></a><a name="p588195413241"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="19.26807319268073%" headers="mcps1.2.4.1.2 "><p id="p148855410241"><a name="p148855410241"></a><a name="p148855410241"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.51374862513749%" headers="mcps1.2.4.1.3 "><p id="p588254112416"><a name="p588254112416"></a><a name="p588254112416"></a>卷组名称</p>
</td>
</tr>
<tr id="row4313193112117"><td class="cellrowborder" valign="top" width="18.21817818218178%" headers="mcps1.2.4.1.1 "><p id="p16315173118219"><a name="p16315173118219"></a><a name="p16315173118219"></a>components</p>
</td>
<td class="cellrowborder" valign="top" width="19.26807319268073%" headers="mcps1.2.4.1.2 "><p id="p16315193118213"><a name="p16315193118213"></a><a name="p16315193118213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.51374862513749%" headers="mcps1.2.4.1.3 "><p id="p33151313213"><a name="p33151313213"></a><a name="p33151313213"></a>组成该卷组的物理分区和磁盘的名称</p>
</td>
</tr>
<tr id="row1883541242"><td class="cellrowborder" valign="top" width="18.21817818218178%" headers="mcps1.2.4.1.1 "><p id="p168855419242"><a name="p168855419242"></a><a name="p168855419242"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="19.26807319268073%" headers="mcps1.2.4.1.2 "><p id="p2088354122412"><a name="p2088354122412"></a><a name="p2088354122412"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="62.51374862513749%" headers="mcps1.2.4.1.3 "><p id="p68865412413"><a name="p68865412413"></a><a name="p68865412413"></a>卷组总大小</p>
</td>
</tr>
<tr id="row088175415244"><td class="cellrowborder" valign="top" width="18.21817818218178%" headers="mcps1.2.4.1.1 "><p id="p1188154152418"><a name="p1188154152418"></a><a name="p1188154152418"></a>free_size</p>
</td>
<td class="cellrowborder" valign="top" width="19.26807319268073%" headers="mcps1.2.4.1.2 "><p id="p1988854102415"><a name="p1988854102415"></a><a name="p1988854102415"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="62.51374862513749%" headers="mcps1.2.4.1.3 "><p id="p38816544248"><a name="p38816544248"></a><a name="p38816544248"></a>剩余空间大小，单位：字节</p>
</td>
</tr>
<tr id="row388105414248"><td class="cellrowborder" valign="top" width="18.21817818218178%" headers="mcps1.2.4.1.1 "><p id="p78875413242"><a name="p78875413242"></a><a name="p78875413242"></a>logic_volumes</p>
</td>
<td class="cellrowborder" valign="top" width="19.26807319268073%" headers="mcps1.2.4.1.2 "><p id="p11881854182410"><a name="p11881854182410"></a><a name="p11881854182410"></a>JSON数组</p>
</td>
<td class="cellrowborder" valign="top" width="62.51374862513749%" headers="mcps1.2.4.1.3 "><p id="p38895414242"><a name="p38895414242"></a><a name="p38895414242"></a>卷组上的逻辑卷信息，参见<a href="#table1851616525247">表6</a></p>
</td>
</tr>
</tbody>
</table>

**表 6**  logic\_volumes数据结构

<a name="table1851616525247"></a>
<table><thead align="left"><tr id="row168819549241"><th class="cellrowborder" valign="top" width="18.568143185681432%" id="mcps1.2.4.1.1"><p id="p44647430551"><a name="p44647430551"></a><a name="p44647430551"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.08809119088091%" id="mcps1.2.4.1.2"><p id="p1347219434551"><a name="p1347219434551"></a><a name="p1347219434551"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="62.34376562343766%" id="mcps1.2.4.1.3"><p id="p048234319550"><a name="p048234319550"></a><a name="p048234319550"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row690454102419"><td class="cellrowborder" valign="top" width="18.568143185681432%" headers="mcps1.2.4.1.1 "><p id="p18901554132414"><a name="p18901554132414"></a><a name="p18901554132414"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="19.08809119088091%" headers="mcps1.2.4.1.2 "><p id="p129055414240"><a name="p129055414240"></a><a name="p129055414240"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.34376562343766%" headers="mcps1.2.4.1.3 "><p id="p12901754152419"><a name="p12901754152419"></a><a name="p12901754152419"></a>该逻辑分区名称</p>
</td>
</tr>
<tr id="row1890165413248"><td class="cellrowborder" valign="top" width="18.568143185681432%" headers="mcps1.2.4.1.1 "><p id="p1490165419243"><a name="p1490165419243"></a><a name="p1490165419243"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="19.08809119088091%" headers="mcps1.2.4.1.2 "><p id="p1890154162413"><a name="p1890154162413"></a><a name="p1890154162413"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="62.34376562343766%" headers="mcps1.2.4.1.3 "><p id="p179095462418"><a name="p179095462418"></a><a name="p179095462418"></a>该分区总大小</p>
</td>
</tr>
<tr id="row490154192415"><td class="cellrowborder" valign="top" width="18.568143185681432%" headers="mcps1.2.4.1.1 "><p id="p109014541240"><a name="p109014541240"></a><a name="p109014541240"></a>used_size</p>
</td>
<td class="cellrowborder" valign="top" width="19.08809119088091%" headers="mcps1.2.4.1.2 "><p id="p119045416245"><a name="p119045416245"></a><a name="p119045416245"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="62.34376562343766%" headers="mcps1.2.4.1.3 "><p id="p690175414248"><a name="p690175414248"></a><a name="p690175414248"></a>该分区已使用大小，单位：字节</p>
</td>
</tr>
<tr id="row13908545249"><td class="cellrowborder" valign="top" width="18.568143185681432%" headers="mcps1.2.4.1.1 "><p id="p139015549243"><a name="p139015549243"></a><a name="p139015549243"></a>free_size</p>
</td>
<td class="cellrowborder" valign="top" width="19.08809119088091%" headers="mcps1.2.4.1.2 "><p id="p790105417247"><a name="p790105417247"></a><a name="p790105417247"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="62.34376562343766%" headers="mcps1.2.4.1.3 "><p id="p10900542240"><a name="p10900542240"></a><a name="p10900542240"></a>该分区剩余空间大小，单位：字节</p>
</td>
</tr>
<tr id="row190195413247"><td class="cellrowborder" valign="top" width="18.568143185681432%" headers="mcps1.2.4.1.1 "><p id="p9901454162414"><a name="p9901454162414"></a><a name="p9901454162414"></a>file_system</p>
</td>
<td class="cellrowborder" valign="top" width="19.08809119088091%" headers="mcps1.2.4.1.2 "><p id="p990175415241"><a name="p990175415241"></a><a name="p990175415241"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.34376562343766%" headers="mcps1.2.4.1.3 "><p id="p129035432416"><a name="p129035432416"></a><a name="p129035432416"></a>该分区的文件系统类型</p>
</td>
</tr>
<tr id="row7905549249"><td class="cellrowborder" valign="top" width="18.568143185681432%" headers="mcps1.2.4.1.1 "><p id="p7905541247"><a name="p7905541247"></a><a name="p7905541247"></a>mount_point</p>
</td>
<td class="cellrowborder" valign="top" width="19.08809119088091%" headers="mcps1.2.4.1.2 "><p id="p290115419248"><a name="p290115419248"></a><a name="p290115419248"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.34376562343766%" headers="mcps1.2.4.1.3 "><p id="p39010547249"><a name="p39010547249"></a><a name="p39010547249"></a>逻辑卷的挂载点</p>
</td>
</tr>
<tr id="row990754142415"><td class="cellrowborder" valign="top" width="18.568143185681432%" headers="mcps1.2.4.1.1 "><p id="p39065492410"><a name="p39065492410"></a><a name="p39065492410"></a>uuid</p>
</td>
<td class="cellrowborder" valign="top" width="19.08809119088091%" headers="mcps1.2.4.1.2 "><p id="p29012545242"><a name="p29012545242"></a><a name="p29012545242"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.34376562343766%" headers="mcps1.2.4.1.3 "><p id="p790135432411"><a name="p790135432411"></a><a name="p790135432411"></a>该分区的UUID</p>
</td>
</tr>
<tr id="row1490165420242"><td class="cellrowborder" valign="top" width="18.568143185681432%" headers="mcps1.2.4.1.1 "><p id="p139045418241"><a name="p139045418241"></a><a name="p139045418241"></a>inode_size</p>
</td>
<td class="cellrowborder" valign="top" width="19.08809119088091%" headers="mcps1.2.4.1.2 "><p id="p5901954182411"><a name="p5901954182411"></a><a name="p5901954182411"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="62.34376562343766%" headers="mcps1.2.4.1.3 "><p id="p4907544245"><a name="p4907544245"></a><a name="p4907544245"></a>文件系统Inode大小</p>
</td>
</tr>
<tr id="row1890175442410"><td class="cellrowborder" valign="top" width="18.568143185681432%" headers="mcps1.2.4.1.1 "><p id="p390145472412"><a name="p390145472412"></a><a name="p390145472412"></a>block_size</p>
</td>
<td class="cellrowborder" valign="top" width="19.08809119088091%" headers="mcps1.2.4.1.2 "><p id="p49005412241"><a name="p49005412241"></a><a name="p49005412241"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="62.34376562343766%" headers="mcps1.2.4.1.3 "><p id="p9901354182418"><a name="p9901354182418"></a><a name="p9901354182418"></a>文件系统块大小，单位：字节</p>
</td>
</tr>
<tr id="row490135452416"><td class="cellrowborder" valign="top" width="18.568143185681432%" headers="mcps1.2.4.1.1 "><p id="p19005432410"><a name="p19005432410"></a><a name="p19005432410"></a>block_count</p>
</td>
<td class="cellrowborder" valign="top" width="19.08809119088091%" headers="mcps1.2.4.1.2 "><p id="p13901354122410"><a name="p13901354122410"></a><a name="p13901354122410"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="62.34376562343766%" headers="mcps1.2.4.1.3 "><p id="p119055442413"><a name="p119055442413"></a><a name="p119055442413"></a>该逻辑分区块的总个数</p>
</td>
</tr>
</tbody>
</table>

**表 7**  network数据结构

<a name="table1258675272414"></a>
<table><thead align="left"><tr id="row79115416243"><th class="cellrowborder" valign="top" width="18.66186618661866%" id="mcps1.2.4.1.1"><p id="p1887155665517"><a name="p1887155665517"></a><a name="p1887155665517"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.01190119011901%" id="mcps1.2.4.1.2"><p id="p15897556105520"><a name="p15897556105520"></a><a name="p15897556105520"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="62.32623262326232%" id="mcps1.2.4.1.3"><p id="p09051356165515"><a name="p09051356165515"></a><a name="p09051356165515"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row149113544246"><td class="cellrowborder" valign="top" width="18.66186618661866%" headers="mcps1.2.4.1.1 "><p id="p391754112418"><a name="p391754112418"></a><a name="p391754112418"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="19.01190119011901%" headers="mcps1.2.4.1.2 "><p id="p10911254142410"><a name="p10911254142410"></a><a name="p10911254142410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.32623262326232%" headers="mcps1.2.4.1.3 "><p id="p10911554102418"><a name="p10911554102418"></a><a name="p10911554102418"></a>网卡的名称</p>
</td>
</tr>
<tr id="row191165482411"><td class="cellrowborder" valign="top" width="18.66186618661866%" headers="mcps1.2.4.1.1 "><p id="p1991254162413"><a name="p1991254162413"></a><a name="p1991254162413"></a>ip</p>
</td>
<td class="cellrowborder" valign="top" width="19.01190119011901%" headers="mcps1.2.4.1.2 "><p id="p1191195492418"><a name="p1191195492418"></a><a name="p1191195492418"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.32623262326232%" headers="mcps1.2.4.1.3 "><p id="p491145422415"><a name="p491145422415"></a><a name="p491145422415"></a>该网卡绑定的IP</p>
</td>
</tr>
<tr id="row291115472411"><td class="cellrowborder" valign="top" width="18.66186618661866%" headers="mcps1.2.4.1.1 "><p id="p39125418248"><a name="p39125418248"></a><a name="p39125418248"></a>netmask</p>
</td>
<td class="cellrowborder" valign="top" width="19.01190119011901%" headers="mcps1.2.4.1.2 "><p id="p891254192418"><a name="p891254192418"></a><a name="p891254192418"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.32623262326232%" headers="mcps1.2.4.1.3 "><p id="p1691754162412"><a name="p1691754162412"></a><a name="p1691754162412"></a>掩码</p>
</td>
</tr>
<tr id="row1691954102411"><td class="cellrowborder" valign="top" width="18.66186618661866%" headers="mcps1.2.4.1.1 "><p id="p1291954182415"><a name="p1291954182415"></a><a name="p1291954182415"></a>gateway</p>
</td>
<td class="cellrowborder" valign="top" width="19.01190119011901%" headers="mcps1.2.4.1.2 "><p id="p8916544247"><a name="p8916544247"></a><a name="p8916544247"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.32623262326232%" headers="mcps1.2.4.1.3 "><p id="p391754132418"><a name="p391754132418"></a><a name="p391754132418"></a>网关</p>
</td>
</tr>
<tr id="row20931154202418"><td class="cellrowborder" valign="top" width="18.66186618661866%" headers="mcps1.2.4.1.1 "><p id="p209375417247"><a name="p209375417247"></a><a name="p209375417247"></a>mtu</p>
</td>
<td class="cellrowborder" valign="top" width="19.01190119011901%" headers="mcps1.2.4.1.2 "><p id="p793175413241"><a name="p793175413241"></a><a name="p793175413241"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="62.32623262326232%" headers="mcps1.2.4.1.3 "><p id="p193165418245"><a name="p193165418245"></a><a name="p193165418245"></a>网卡的MTU</p>
</td>
</tr>
</tbody>
</table>

**表 8**  checks数据结构

<a name="table32630264308"></a>
<table><thead align="left"><tr id="row228711269308"><th class="cellrowborder" valign="top" width="18.66186618661866%" id="mcps1.2.4.1.1"><p id="p1843851214568"><a name="p1843851214568"></a><a name="p1843851214568"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.53195319531953%" id="mcps1.2.4.1.2"><p id="p15447131285615"><a name="p15447131285615"></a><a name="p15447131285615"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.8061806180618%" id="mcps1.2.4.1.3"><p id="p64531712115610"><a name="p64531712115610"></a><a name="p64531712115610"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row231812653019"><td class="cellrowborder" valign="top" width="18.66186618661866%" headers="mcps1.2.4.1.1 "><p id="p1427141910496"><a name="p1427141910496"></a><a name="p1427141910496"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="19.53195319531953%" headers="mcps1.2.4.1.2 "><p id="p232942693012"><a name="p232942693012"></a><a name="p232942693012"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.8061806180618%" headers="mcps1.2.4.1.3 "><p id="p1734320261305"><a name="p1734320261305"></a><a name="p1734320261305"></a>该检查项的ID</p>
</td>
</tr>
<tr id="row134532620302"><td class="cellrowborder" valign="top" width="18.66186618661866%" headers="mcps1.2.4.1.1 "><p id="p16350142683014"><a name="p16350142683014"></a><a name="p16350142683014"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="19.53195319531953%" headers="mcps1.2.4.1.2 "><p id="p9357102617301"><a name="p9357102617301"></a><a name="p9357102617301"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.8061806180618%" headers="mcps1.2.4.1.3 "><p id="p437092618308"><a name="p437092618308"></a><a name="p437092618308"></a>检查项名称</p>
</td>
</tr>
<tr id="row1937532613013"><td class="cellrowborder" valign="top" width="18.66186618661866%" headers="mcps1.2.4.1.1 "><p id="p7380182613309"><a name="p7380182613309"></a><a name="p7380182613309"></a>result</p>
</td>
<td class="cellrowborder" valign="top" width="19.53195319531953%" headers="mcps1.2.4.1.2 "><p id="p14388112611302"><a name="p14388112611302"></a><a name="p14388112611302"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.8061806180618%" headers="mcps1.2.4.1.3 "><p id="p739615261308"><a name="p739615261308"></a><a name="p739615261308"></a>检查结果</p>
<a name="ul1686516274329"></a><a name="ul1686516274329"></a><ul id="ul1686516274329"><li>OK：检查通过</li><li>WARN：告警</li><li>ERROR：检查不通过</li></ul>
</td>
</tr>
<tr id="row184021526143020"><td class="cellrowborder" valign="top" width="18.66186618661866%" headers="mcps1.2.4.1.1 "><p id="p1740832623012"><a name="p1740832623012"></a><a name="p1740832623012"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="19.53195319531953%" headers="mcps1.2.4.1.2 "><p id="p54126263304"><a name="p54126263304"></a><a name="p54126263304"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.8061806180618%" headers="mcps1.2.4.1.3 "><p id="p1042542673013"><a name="p1042542673013"></a><a name="p1042542673013"></a>检查不通过的错误码</p>
</td>
</tr>
<tr id="row14427182633011"><td class="cellrowborder" valign="top" width="18.66186618661866%" headers="mcps1.2.4.1.1 "><p id="p943415268309"><a name="p943415268309"></a><a name="p943415268309"></a>error_params</p>
</td>
<td class="cellrowborder" valign="top" width="19.53195319531953%" headers="mcps1.2.4.1.2 "><p id="p174397266307"><a name="p174397266307"></a><a name="p174397266307"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="61.8061806180618%" headers="mcps1.2.4.1.3 "><p id="p12454142617303"><a name="p12454142617303"></a><a name="p12454142617303"></a>检查不通过的错误参数</p>
</td>
</tr>
</tbody>
</table>

**表 9**  init\_target\_server 数据结构

<a name="table1862585272417"></a>
<table><thead align="left"><tr id="row1093105442418"><th class="cellrowborder" valign="top" width="18.66186618661866%" id="mcps1.2.4.1.1"><p id="p2749143317562"><a name="p2749143317562"></a><a name="p2749143317562"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.351935193519353%" id="mcps1.2.4.1.2"><p id="p1375963318567"><a name="p1375963318567"></a><a name="p1375963318567"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.98619861986199%" id="mcps1.2.4.1.3"><p id="p11768193315561"><a name="p11768193315561"></a><a name="p11768193315561"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row209345492419"><td class="cellrowborder" valign="top" width="18.66186618661866%" headers="mcps1.2.4.1.1 "><p id="p12931654102410"><a name="p12931654102410"></a><a name="p12931654102410"></a>disks</p>
</td>
<td class="cellrowborder" valign="top" width="19.351935193519353%" headers="mcps1.2.4.1.2 "><p id="p1293254192410"><a name="p1293254192410"></a><a name="p1293254192410"></a>JSON数组</p>
</td>
<td class="cellrowborder" valign="top" width="61.98619861986199%" headers="mcps1.2.4.1.3 "><p id="p39365432418"><a name="p39365432418"></a><a name="p39365432418"></a>推荐的目的端服务器的磁盘信息，参见<a href="#table663955292418">表10</a></p>
</td>
</tr>
</tbody>
</table>

**表 10**  disks数组中成员结构

<a name="table663955292418"></a>
<table><thead align="left"><tr id="row199921756102716"><th class="cellrowborder" valign="top" width="19.09%" id="mcps1.2.4.1.1"><p id="p76367474566"><a name="p76367474566"></a><a name="p76367474566"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.18%" id="mcps1.2.4.1.2"><p id="p19645174711566"><a name="p19645174711566"></a><a name="p19645174711566"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.73%" id="mcps1.2.4.1.3"><p id="p4654154712566"><a name="p4654154712566"></a><a name="p4654154712566"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row394454152411"><td class="cellrowborder" valign="top" width="19.09%" headers="mcps1.2.4.1.1 "><p id="p14944545244"><a name="p14944545244"></a><a name="p14944545244"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.2 "><p id="p1894155419247"><a name="p1894155419247"></a><a name="p1894155419247"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.73%" headers="mcps1.2.4.1.3 "><p id="p29495442417"><a name="p29495442417"></a><a name="p29495442417"></a>磁盘名称</p>
</td>
</tr>
<tr id="row2094195410241"><td class="cellrowborder" valign="top" width="19.09%" headers="mcps1.2.4.1.1 "><p id="p394205462415"><a name="p394205462415"></a><a name="p394205462415"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.2 "><p id="p199485416249"><a name="p199485416249"></a><a name="p199485416249"></a>long</p>
</td>
<td class="cellrowborder" valign="top" width="61.73%" headers="mcps1.2.4.1.3 "><p id="p29411548246"><a name="p29411548246"></a><a name="p29411548246"></a>磁盘大小，单位字节</p>
</td>
</tr>
<tr id="row189495413247"><td class="cellrowborder" valign="top" width="19.09%" headers="mcps1.2.4.1.1 "><p id="p1794175418244"><a name="p1794175418244"></a><a name="p1794175418244"></a>device_use</p>
</td>
<td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.2 "><p id="p394165442413"><a name="p394165442413"></a><a name="p394165442413"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.73%" headers="mcps1.2.4.1.3 "><p id="p1594105410249"><a name="p1594105410249"></a><a name="p1594105410249"></a>磁盘作用</p>
<a name="ul17514314548"></a><a name="ul17514314548"></a><ul id="ul17514314548"><li>OS：系统盘</li><li>NORMAL：数据盘</li></ul>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section1266365232418"></a>

-   请求示例

    无请求消息。


-   响应示例
    -   源端服务器为Windows操作系统时的响应

        ```
        {
          "id": "f36fa247-ac20-48b7-ba80-941b31d7718c",
          "ip": "x.x.x.x",
          "name": "szxy2",
          "hostname": "szxy2",
          "add_date": 1528675263000,
          "os_type": "WINDOWS",
          "os_version": "WINDOWS7_64BIT",
          "oem_system": false,
          "state": "AVAILABLE",
          "connected": false,
          "firmware": "BIOS",
          "cpu_quantity": 4,
          "memory": 17171075072,
          "current_task": null,
          "disks": [
            {
              "name": "Disk 0",
              "partition_style": "MBR",
              "relation_name": null,
              "size": 85897247744,
              "used_size": 85897247744,
              "device_use": "BOOT",
              "os_disk": false,
              "physical_volumes": [
                {
                  "uuid": "\\?\Volume{e36afecb-24da-11e7-b949-806e6f6e6963}\",
                  "index": 0,
                  "name": "(Reserved)",
                  "dos_name": null,
                  "relation_name": null,
                  "file_system": "NTFS",
                  "size_per_cluster": 4096,
                  "start_offset": 1048576,
                  "total_sectors": 0,
                  "hiden_sectors": 0,
                  "sectors_per_track": 0,
                  "start_sectors": 2048,
                  "mount_point": null,
                  "size": 104857088,
                  "used_size": 25878016,
                  "snap_mount_point": null,
                  "device_use": "BOOT"
                },
                {
                  "uuid": "\\?\Volume{e36afecc-24da-11e7-b949-806e6f6e6963}\",
                  "index": 0,
                  "name": "C:\\",
                  "dos_name": null,
                  "relation_name": null,
                  "file_system": "NTFS",
                  "size_per_cluster": 4096,
                  "start_offset": 105906176,
                  "total_sectors": 0,
                  "hiden_sectors": 0,
                  "sectors_per_track": 0,
                  "start_sectors": 206848,
                  "mount_point": null,
                  "size": 85792390656,
                  "used_size": 55866973696,
                  "snap_mount_point": null,
                  "device_use": "OS"
                }
              ]
            },
            {
              "name": "Disk 1",
              "partition_style": "MBR",
              "relation_name": null,
              "size": 214745218560,
              "used_size": 214745218560,
              "device_use": "",
              "os_disk": false,
              "physical_volumes": [
                {
                  "uuid": "\\?\Volume{e36afecd-24da-11e7-b949-806e6f6e6963}\",
                  "index": 0,
                  "name": "D:\\",
                  "dos_name": null,
                  "relation_name": null,
                  "file_system": "NTFS",
                  "size_per_cluster": 4096,
                  "start_offset": 1048576,
                  "total_sectors": 0,
                  "hiden_sectors": 0,
                  "sectors_per_track": 0,
                  "start_sectors": 2048,
                  "mount_point": null,
                  "size": 214745218560,
                  "used_size": 128071798272,
                  "snap_mount_point": null,
                  "device_use": ""
                }
              ]
            }
          ],
          "volume_groups": [],
          "networks": [
            {
              "name": null,
              "ip": null,
              "netmask": null,
              "gateway": null,
              "mtu": 0,
              "mac": "0XB93064096C2C"
            }
          ],
          "checks": [
            {
              "id": 20749,
              "params": [
                ""
              ],
              "name": "OS_VERSION",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 20756,
              "params": [
                ""
              ],
              "name": "FIRMWARE",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 20763,
              "params": [
                ""
              ],
              "name": "CPU",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 20770,
              "params": [
                ""
              ],
              "name": "MEMORY",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 20777,
              "params": [
                ""
              ],
              "name": "SYSTEM_ROOT",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 20784,
              "params": [
                ""
              ],
              "name": "PARTITION_STYLE",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 20791,
              "params": [
                ""
              ],
              "name": "FILE_SYSTEM",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 20798,
              "params": [
                ""
              ],
              "name": "FREE_SPACE",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 20805,
              "params": [
                ""
              ],
              "name": "OEM_SYSTEM",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 20812,
              "params": [
                ""
              ],
              "name": "DRIVER_FILE",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 20819,
              "params": [
                ""
              ],
              "name": "SERVICE",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 20826,
              "params": [
                ""
              ],
              "name": "ACCOUNT_RIGHTS",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            }
          ],
          "init_target_server": null
        }         
        ```

    -   当源端服务器为Linux操作系统时的响应

        ```
        {
          "id": "45a02115-28a9-40c2-8604-0abfc9889c9d",
          "ip": "192.168.0.151",
          "name": "novalocal",
          "hostname": null,
          "add_date": 1532658611000,
          "os_type": "LINUX",
          "os_version": "CENTOS_7_2_64BIT",
          "oem_system": false,
          "state": "AVAILABLE",
          "connected": false,
          "firmware": "BIOS",
          "cpu_quantity": 2,
          "memory": 4,
          "current_task": null,
          "disks": [
            {
              "name": "/dev/xvda",
              "relation_name": null,
              "partition_style": "MBR",
              "size": 42949672960,
              "used_size": 42948606976,
              "device_use": "NORMAL",
              "os_disk": false,
              "physical_volumes": [
                {
                  "uuid": null,
                  "index": 0,
                  "name": "/dev/xvda1",
                  "device_use": "NORMAL",
                  "file_system": "ext3",
                  "mount_point": "/",
                  "size": 42948606976,
                  "used_size": 2853855232
                }
              ]
            },
            {
              "name": "/dev/xvdb",
              "relation_name": null,
              "partition_style": "MBR",
              "size": 10737418240,
              "used_size": 6442450944,
              "device_use": "NORMAL",
              "os_disk": false,
              "physical_volumes": [
                {
                  "uuid": null,
                  "index": 0,
                  "name": "/dev/xvdb1",
                  "device_use": "NORMAL",
                  "file_system": "swap",
                  "mount_point": "",
                  "size": 1073741824,
                  "used_size": 1073741824
                },
                {
                  "uuid": null,
                  "index": 0,
                  "name": "/dev/xvdb2",
                  "device_use": "VOLUME_GROUP",
                  "file_system": "LVM2_member",
                  "mount_point": "",
                  "size": 5368709120,
                  "used_size": 5368709120
                }
              ]
            },
            {
              "name": "/dev/xvdc",
              "relation_name": null,
              "partition_style": "MBR",
              "size": 10737418240,
              "used_size": 10737418240,
              "device_use": "VOLUME_GROUP",
              "os_disk": false,
              "physical_volumes": []
            }
          ],
          "volume_groups": [
            {
              "name": "vgtest",
              "components": "/dev/xvdb2;/dev/xvdc",
              "size": 16106127360,
              "free_size": 0,
              "logical_volumes": [
                {
                  "name": "/dev/mapper/vgtest-data",
                  "size": 1073741824,
                  "used_size": 3047424,
                  "file_system": "ext4",
                  "mount_point": "/data",
                  "uuid": null,
                  "inode_size": 256,
                  "block_size": 0,
                  "block_count": 0
                }
              ]
            }
          ],
          "networks": [
            {
              "name": "eth0",
              "ip": "192.168.0.151",
              "netmask": null,
              "gateway": null,
              "mtu": 0,
              "mac": "fa:16:3e:35:97:71"
            }
          ],
          "checks": [
            {
              "id": 6463,
              "params": [
                ""
              ],
              "name": "OS_VERSION",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 6470,
              "params": [
                ""
              ],
              "name": "CPU",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 6477,
              "params": [
                ""
              ],
              "name": "MEMORY",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 6484,
              "params": [
                ""
              ],
              "name": "PARAVIRTUALIZATION",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 6491,
              "params": [
                ""
              ],
              "name": "FIRMWARE",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 6498,
              "params": [
                ""
              ],
              "name": "BOOT_LOADER",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 6505,
              "params": [
                ""
              ],
              "name": "RSYNC",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 6512,
              "params": [
                ""
              ],
              "name": "RAW_DEVICES",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 6519,
              "params": [
                ""
              ],
              "name": "DISK_INFO",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 6526,
              "params": [
                ""
              ],
              "name": "PARTITION_STYLE",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            },
            {
              "id": 6533,
              "params": [
                ""
              ],
              "name": "FILE_SYSTEM",
              "result": "OK",
              "error_code": null,
              "error_params": ""
            }
          ],
          "init_target_server": {
            "disks": [
              {
                "name": "/dev/xvda",
                "size": 42949672960,
                "used_size": 42948606976,
                "device_use": "NORMAL",
                "physical_volumes": [
                  {
                    "uuid": null,
                    "index": 0,
                    "name": "/dev/xvda1",
                    "device_use": "NORMAL",
                    "file_system": "ext3",
                    "mount_point": "/",
                    "size": 42948606976,
                    "used_size": 2853855232
                  }
                ]
              },
              {
                "name": "/dev/xvdb",
                "size": 10737418240,
                "used_size": 6442450944,
                "device_use": "NORMAL",
                "physical_volumes": [
                  {
                    "uuid": null,
                    "index": 0,
                    "name": "/dev/xvdb1",
                    "device_use": "NORMAL",
                    "file_system": "swap",
                    "mount_point": "",
                    "size": 1073741824,
                    "used_size": 1073741824
                  },
                  {
                    "uuid": null,
                    "index": 0,
                    "name": "/dev/xvdb2",
                    "device_use": "VOLUME_GROUP",
                    "file_system": "LVM2_member",
                    "mount_point": "",
                    "size": 5368709120,
                    "used_size": 5368709120
                  }
                ]
              },
              {
                "name": "/dev/xvdc",
                "size": 10737418240,
                "used_size": 10737418240,
                "device_use": "VOLUME_GROUP",
                "physical_volumes": []
              }
            ]
          }
        }
        ```



## 状态码<a name="section1973012935418"></a>

状态码请参见[状态码](状态码.md)。

## 错误码<a name="section11517539246"></a>

请参见[错误码](错误码.md)。

