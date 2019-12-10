# 查询指定ID模板信息<a name="sms_api_0040"></a>

## 功能介绍<a name="section65772294354"></a>

查询指定ID的弹性云服务器模板信息。

## URI<a name="section1957962916358"></a>

GET /v1/sms/vm/template/\{id\}

参数说明请参见[表1](#table19581102993519)。

**表 1**  参数说明

<a name="table19581102993519"></a>
<table><thead align="left"><tr id="row7821330173515"><th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.1"><p id="p182153033516"><a name="p182153033516"></a><a name="p182153033516"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="p1821730193510"><a name="p1821730193510"></a><a name="p1821730193510"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20.407959204079592%" id="mcps1.2.5.1.3"><p id="p682530193511"><a name="p682530193511"></a><a name="p682530193511"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.89551044895511%" id="mcps1.2.5.1.4"><p id="p1982930133519"><a name="p1982930133519"></a><a name="p1982930133519"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row5827303351"><td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.1 "><p id="p782130203517"><a name="p782130203517"></a><a name="p782130203517"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p118217307354"><a name="p118217307354"></a><a name="p118217307354"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.5.1.3 "><p id="p28223019354"><a name="p28223019354"></a><a name="p28223019354"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p682130173513"><a name="p682130173513"></a><a name="p682130173513"></a>模板ID，具体ID请参见<a href="查询模板列表.md">查询模板列表</a>查询出的ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section14592122973518"></a>

无

## 响应消息<a name="section35933293352"></a>

**响应参数**

响应参数如[表3](#table259510297352)所示。

**表 2**  响应参数

<a name="table109771821195210"></a>
<table><thead align="left"><tr id="row13977192110526"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.2.4.1.1"><p id="p149781121105216"><a name="p149781121105216"></a><a name="p149781121105216"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.41%" id="mcps1.2.4.1.2"><p id="p19782211525"><a name="p19782211525"></a><a name="p19782211525"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.160000000000004%" id="mcps1.2.4.1.3"><p id="p11978321145217"><a name="p11978321145217"></a><a name="p11978321145217"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row199787219524"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.4.1.1 "><p id="p1978321205217"><a name="p1978321205217"></a><a name="p1978321205217"></a>template</p>
</td>
<td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.4.1.2 "><p id="p149789216525"><a name="p149789216525"></a><a name="p149789216525"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.160000000000004%" headers="mcps1.2.4.1.3 "><p id="p49781421135217"><a name="p49781421135217"></a><a name="p49781421135217"></a>模板信息，请参见<a href="#table259510297352">表3</a></p>
</td>
</tr>
<tr id="row197814211521"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.4.1.1 "><p id="p19978172115215"><a name="p19978172115215"></a><a name="p19978172115215"></a>disks</p>
</td>
<td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.4.1.2 "><p id="p11978122125218"><a name="p11978122125218"></a><a name="p11978122125218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.160000000000004%" headers="mcps1.2.4.1.3 "><p id="p179783217527"><a name="p179783217527"></a><a name="p179783217527"></a>磁盘信息，请参见<a href="#table157391129203519">表9</a></p>
</td>
</tr>
</tbody>
</table>

**表 3**  template信息

<a name="table259510297352"></a>
<table><thead align="left"><tr id="row15832305353"><th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.2.4.1.1"><p id="p88303043516"><a name="p88303043516"></a><a name="p88303043516"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.09%" id="mcps1.2.4.1.2"><p id="p9831430173519"><a name="p9831430173519"></a><a name="p9831430173519"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.919999999999995%" id="mcps1.2.4.1.3"><p id="p1683930113515"><a name="p1683930113515"></a><a name="p1683930113515"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row11832030103515"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p88319304354"><a name="p88319304354"></a><a name="p88319304354"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.2.4.1.2 "><p id="p6838308355"><a name="p6838308355"></a><a name="p6838308355"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.919999999999995%" headers="mcps1.2.4.1.3 "><p id="p12837309352"><a name="p12837309352"></a><a name="p12837309352"></a>模板名称</p>
</td>
</tr>
<tr id="row17834302353"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p5834301359"><a name="p5834301359"></a><a name="p5834301359"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.2.4.1.2 "><p id="p178317307350"><a name="p178317307350"></a><a name="p178317307350"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.919999999999995%" headers="mcps1.2.4.1.3 "><p id="p78373093519"><a name="p78373093519"></a><a name="p78373093519"></a>模板ID</p>
</td>
</tr>
<tr id="row783830143520"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p1583103016358"><a name="p1583103016358"></a><a name="p1583103016358"></a>is_template</p>
</td>
<td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.2.4.1.2 "><p id="p583173013510"><a name="p583173013510"></a><a name="p583173013510"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="58.919999999999995%" headers="mcps1.2.4.1.3 "><p id="p283330103518"><a name="p283330103518"></a><a name="p283330103518"></a>是否是模板，单击按钮保存时该值为true，没有单击保存模板直接创建任务时该值为false</p>
</td>
</tr>
<tr id="row1837305350"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p28393015353"><a name="p28393015353"></a><a name="p28393015353"></a>region</p>
</td>
<td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.2.4.1.2 "><p id="p108315303358"><a name="p108315303358"></a><a name="p108315303358"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.919999999999995%" headers="mcps1.2.4.1.3 "><p id="p78383043515"><a name="p78383043515"></a><a name="p78383043515"></a>区域</p>
</td>
</tr>
<tr id="row1783630123512"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p7835306351"><a name="p7835306351"></a><a name="p7835306351"></a>target_server_name</p>
</td>
<td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.2.4.1.2 "><p id="p683143013356"><a name="p683143013356"></a><a name="p683143013356"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.919999999999995%" headers="mcps1.2.4.1.3 "><p id="p1483183033519"><a name="p1483183033519"></a><a name="p1483183033519"></a>目的端名称</p>
</td>
</tr>
<tr id="row19838309358"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p178383010352"><a name="p178383010352"></a><a name="p178383010352"></a>availability_zone</p>
</td>
<td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.2.4.1.2 "><p id="p7831830163513"><a name="p7831830163513"></a><a name="p7831830163513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.919999999999995%" headers="mcps1.2.4.1.3 "><p id="p1783153011354"><a name="p1783153011354"></a><a name="p1783153011354"></a>可用区</p>
</td>
</tr>
<tr id="row1841230103510"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p084103017358"><a name="p084103017358"></a><a name="p084103017358"></a>volumetype</p>
</td>
<td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.2.4.1.2 "><p id="p13843304354"><a name="p13843304354"></a><a name="p13843304354"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.919999999999995%" headers="mcps1.2.4.1.3 "><p id="p1584530133515"><a name="p1584530133515"></a><a name="p1584530133515"></a>磁盘类型</p>
</td>
</tr>
<tr id="row484183012356"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p48443033513"><a name="p48443033513"></a><a name="p48443033513"></a>vpc</p>
</td>
<td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.2.4.1.2 "><p id="p1884930173511"><a name="p1884930173511"></a><a name="p1884930173511"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="58.919999999999995%" headers="mcps1.2.4.1.3 "><p id="p3841930193514"><a name="p3841930193514"></a><a name="p3841930193514"></a>Vpc信息，自动创建时为{}，请参见<a href="#table1864412983517">表4</a>。</p>
</td>
</tr>
<tr id="row17842301355"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p58433053517"><a name="p58433053517"></a><a name="p58433053517"></a>security_groups</p>
</td>
<td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.2.4.1.2 "><p id="p185730143513"><a name="p185730143513"></a><a name="p185730143513"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="58.919999999999995%" headers="mcps1.2.4.1.3 "><p id="p1185173073520"><a name="p1185173073520"></a><a name="p1185173073520"></a>安全组，自动创建时为[]，请参见<a href="#table76545291358">表5</a>。</p>
</td>
</tr>
<tr id="row128513014357"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p685153033520"><a name="p685153033520"></a><a name="p685153033520"></a>nics</p>
</td>
<td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.2.4.1.2 "><p id="p1985203053519"><a name="p1985203053519"></a><a name="p1985203053519"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="58.919999999999995%" headers="mcps1.2.4.1.3 "><p id="p385193053519"><a name="p385193053519"></a><a name="p385193053519"></a>子网，自动创建时为[]，请参见<a href="#table6669929153517">表6</a>。</p>
</td>
</tr>
<tr id="row1267375416188"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p1667335431816"><a name="p1667335431816"></a><a name="p1667335431816"></a>flavors</p>
</td>
<td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.2.4.1.2 "><p id="p1467345415189"><a name="p1467345415189"></a><a name="p1467345415189"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="58.919999999999995%" headers="mcps1.2.4.1.3 "><p id="p136734546187"><a name="p136734546187"></a><a name="p136734546187"></a>规格，自动创建时为[]，请参见<a href="#table11688329183518">表7</a>。</p>
</td>
</tr>
<tr id="row98513301355"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p1585530193512"><a name="p1585530193512"></a><a name="p1585530193512"></a>publicip</p>
</td>
<td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.2.4.1.2 "><p id="p118515308353"><a name="p118515308353"></a><a name="p118515308353"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="58.919999999999995%" headers="mcps1.2.4.1.3 "><p id="p1386153010357"><a name="p1386153010357"></a><a name="p1386153010357"></a>弹性公网IP，请参见<a href="#table770511297354">表8</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  vpc信息

<a name="table1864412983517"></a>
<table><thead align="left"><tr id="row186143043511"><th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.2.4.1.1"><p id="p18864305356"><a name="p18864305356"></a><a name="p18864305356"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.09%" id="mcps1.2.4.1.2"><p id="p168613033513"><a name="p168613033513"></a><a name="p168613033513"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.919999999999995%" id="mcps1.2.4.1.3"><p id="p1686193063513"><a name="p1686193063513"></a><a name="p1686193063513"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row186133012351"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p38653053517"><a name="p38653053517"></a><a name="p38653053517"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.2.4.1.2 "><p id="p3871630143510"><a name="p3871630143510"></a><a name="p3871630143510"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.919999999999995%" headers="mcps1.2.4.1.3 "><p id="p78711308358"><a name="p78711308358"></a><a name="p78711308358"></a>VPC ID</p>
</td>
</tr>
<tr id="row28753010352"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p78773014355"><a name="p78773014355"></a><a name="p78773014355"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.2.4.1.2 "><p id="p987193023512"><a name="p987193023512"></a><a name="p987193023512"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.919999999999995%" headers="mcps1.2.4.1.3 "><p id="p2087430103516"><a name="p2087430103516"></a><a name="p2087430103516"></a>VPC 名称</p>
</td>
</tr>
</tbody>
</table>

**表 5**  security\_groups信息

<a name="table76545291358"></a>
<table><thead align="left"><tr id="row687173003518"><th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.2.4.1.1"><p id="p1287430173520"><a name="p1287430173520"></a><a name="p1287430173520"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.24%" id="mcps1.2.4.1.2"><p id="p108713033516"><a name="p108713033516"></a><a name="p108713033516"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.77%" id="mcps1.2.4.1.3"><p id="p78712304357"><a name="p78712304357"></a><a name="p78712304357"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1188930183517"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p1288173013354"><a name="p1288173013354"></a><a name="p1288173013354"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.2.4.1.2 "><p id="p16882030143515"><a name="p16882030143515"></a><a name="p16882030143515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.77%" headers="mcps1.2.4.1.3 "><p id="p1188730113519"><a name="p1188730113519"></a><a name="p1188730113519"></a>安全组ID</p>
</td>
</tr>
<tr id="row1488113043516"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p1388830183519"><a name="p1388830183519"></a><a name="p1388830183519"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.2.4.1.2 "><p id="p5881030183518"><a name="p5881030183518"></a><a name="p5881030183518"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.77%" headers="mcps1.2.4.1.3 "><p id="p11888303352"><a name="p11888303352"></a><a name="p11888303352"></a>安全组名称</p>
</td>
</tr>
</tbody>
</table>

**表 6**  nics信息

<a name="table6669929153517"></a>
<table><thead align="left"><tr id="row11881030143519"><th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.2.4.1.1"><p id="p18893010354"><a name="p18893010354"></a><a name="p18893010354"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.24%" id="mcps1.2.4.1.2"><p id="p1788143083515"><a name="p1788143083515"></a><a name="p1788143083515"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.77%" id="mcps1.2.4.1.3"><p id="p1882308355"><a name="p1882308355"></a><a name="p1882308355"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row17881230173512"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p198833015357"><a name="p198833015357"></a><a name="p198833015357"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.2.4.1.2 "><p id="p13891930153510"><a name="p13891930153510"></a><a name="p13891930153510"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.77%" headers="mcps1.2.4.1.3 "><p id="p88903043520"><a name="p88903043520"></a><a name="p88903043520"></a>子网ID</p>
</td>
</tr>
<tr id="row1089230183519"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p178919307351"><a name="p178919307351"></a><a name="p178919307351"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.2.4.1.2 "><p id="p16892030123511"><a name="p16892030123511"></a><a name="p16892030123511"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.77%" headers="mcps1.2.4.1.3 "><p id="p289330133512"><a name="p289330133512"></a><a name="p289330133512"></a>名称</p>
</td>
</tr>
<tr id="row48993020350"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p4898306359"><a name="p4898306359"></a><a name="p4898306359"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.2.4.1.2 "><p id="p989163013518"><a name="p989163013518"></a><a name="p989163013518"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.77%" headers="mcps1.2.4.1.3 "><p id="p188973043515"><a name="p188973043515"></a><a name="p188973043515"></a>网关/掩码</p>
</td>
</tr>
<tr id="row1289130173510"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p12899303359"><a name="p12899303359"></a><a name="p12899303359"></a>ip</p>
</td>
<td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.2.4.1.2 "><p id="p138903083510"><a name="p138903083510"></a><a name="p138903083510"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.77%" headers="mcps1.2.4.1.3 "><p id="p188983013350"><a name="p188983013350"></a><a name="p188983013350"></a>私有IP</p>
</td>
</tr>
</tbody>
</table>

**表 7**  flavors信息

<a name="table11688329183518"></a>
<table><thead align="left"><tr id="row2089133016359"><th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.2.4.1.1"><p id="p1589173011351"><a name="p1589173011351"></a><a name="p1589173011351"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.380000000000003%" id="mcps1.2.4.1.2"><p id="p39053015354"><a name="p39053015354"></a><a name="p39053015354"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.63%" id="mcps1.2.4.1.3"><p id="p390103011350"><a name="p390103011350"></a><a name="p390103011350"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row19043013358"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p0902304359"><a name="p0902304359"></a><a name="p0902304359"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p7900300358"><a name="p7900300358"></a><a name="p7900300358"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.63%" headers="mcps1.2.4.1.3 "><p id="p1090183033516"><a name="p1090183033516"></a><a name="p1090183033516"></a>规格ID</p>
</td>
</tr>
<tr id="row1290123033511"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p290113043516"><a name="p290113043516"></a><a name="p290113043516"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p790113014353"><a name="p790113014353"></a><a name="p790113014353"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.63%" headers="mcps1.2.4.1.3 "><p id="p1690230153514"><a name="p1690230153514"></a><a name="p1690230153514"></a>规格名称</p>
</td>
</tr>
</tbody>
</table>

**表 8**  publicip信息

<a name="table770511297354"></a>
<table><thead align="left"><tr id="row129073012353"><th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.2.4.1.1"><p id="p19063014350"><a name="p19063014350"></a><a name="p19063014350"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.53%" id="mcps1.2.4.1.2"><p id="p090530133515"><a name="p090530133515"></a><a name="p090530133515"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.48%" id="mcps1.2.4.1.3"><p id="p2090103019357"><a name="p2090103019357"></a><a name="p2090103019357"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1490183033510"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p69063023513"><a name="p69063023513"></a><a name="p69063023513"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20.53%" headers="mcps1.2.4.1.2 "><p id="p7918305358"><a name="p7918305358"></a><a name="p7918305358"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.48%" headers="mcps1.2.4.1.3 "><p id="p15914307350"><a name="p15914307350"></a><a name="p15914307350"></a>ID，新增必填</p>
</td>
</tr>
<tr id="row129119306359"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p991153003512"><a name="p991153003512"></a><a name="p991153003512"></a>ip</p>
</td>
<td class="cellrowborder" valign="top" width="20.53%" headers="mcps1.2.4.1.2 "><p id="p1491530133517"><a name="p1491530133517"></a><a name="p1491530133517"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.48%" headers="mcps1.2.4.1.3 "><p id="p49133023518"><a name="p49133023518"></a><a name="p49133023518"></a>弹性IP，新增必填</p>
</td>
</tr>
<tr id="row4912302356"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p179113017352"><a name="p179113017352"></a><a name="p179113017352"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20.53%" headers="mcps1.2.4.1.2 "><p id="p891330153511"><a name="p891330153511"></a><a name="p891330153511"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.48%" headers="mcps1.2.4.1.3 "><p id="p291113073515"><a name="p291113073515"></a><a name="p291113073515"></a>弹性公网IP类型，默认为5_bgp</p>
</td>
</tr>
<tr id="row391103043512"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p69143014358"><a name="p69143014358"></a><a name="p69143014358"></a>bandwidth_size</p>
</td>
<td class="cellrowborder" valign="top" width="20.53%" headers="mcps1.2.4.1.2 "><p id="p591330173511"><a name="p591330173511"></a><a name="p591330173511"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.48%" headers="mcps1.2.4.1.3 "><p id="p29173033512"><a name="p29173033512"></a><a name="p29173033512"></a>功能说明：带宽大小带宽（Mbit/s），取值范围为[1,2000]。</p>
<p id="p6913305355"><a name="p6913305355"></a><a name="p6913305355"></a>调整带宽时的最小单位会根据带宽范围不同存在差异。小于等于300Mbit/s：默认最小单位为1Mbit/s。300Mbit/s~1000Mbit/s：默认最小单位为50Mbit/s。大于1000Mbit/s：默认最小单位为500Mbit/s。</p>
<div class="note" id="note14258152954818"><a name="note14258152954818"></a><a name="note14258152954818"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p122591229114820"><a name="p122591229114820"></a><a name="p122591229114820"></a>如果share_type是PER，该参数必选项；如果share_type是WHOLE并且id有值，该参数会忽略。</p>
</div></div>
</td>
</tr>
<tr id="row29173063515"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p199193013520"><a name="p199193013520"></a><a name="p199193013520"></a>bandwidth_share_type</p>
</td>
<td class="cellrowborder" valign="top" width="20.53%" headers="mcps1.2.4.1.2 "><p id="p99215307351"><a name="p99215307351"></a><a name="p99215307351"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.48%" headers="mcps1.2.4.1.3 "><p id="p10921630103512"><a name="p10921630103512"></a><a name="p10921630103512"></a>带宽的共享类型。共享类型枚举：PER，表示独享。WHOLE，表示共享。默认使用PER</p>
</td>
</tr>
</tbody>
</table>

**表 9**  disk信息

<a name="table157391129203519"></a>
<table><thead align="left"><tr id="row16921330193516"><th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.2.4.1.1"><p id="p179218309352"><a name="p179218309352"></a><a name="p179218309352"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.830000000000002%" id="mcps1.2.4.1.2"><p id="p19233013514"><a name="p19233013514"></a><a name="p19233013514"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.18%" id="mcps1.2.4.1.3"><p id="p792730113512"><a name="p792730113512"></a><a name="p792730113512"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row392173018355"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p7921430143513"><a name="p7921430143513"></a><a name="p7921430143513"></a>index</p>
</td>
<td class="cellrowborder" valign="top" width="20.830000000000002%" headers="mcps1.2.4.1.2 "><p id="p199213307350"><a name="p199213307350"></a><a name="p199213307350"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.18%" headers="mcps1.2.4.1.3 "><p id="p10927302358"><a name="p10927302358"></a><a name="p10927302358"></a>磁盘序号，从0开始</p>
</td>
</tr>
<tr id="row392173014353"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p59218307352"><a name="p59218307352"></a><a name="p59218307352"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20.830000000000002%" headers="mcps1.2.4.1.2 "><p id="p492183019352"><a name="p492183019352"></a><a name="p492183019352"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.18%" headers="mcps1.2.4.1.3 "><p id="p992530103518"><a name="p992530103518"></a><a name="p992530103518"></a>磁盘名称</p>
</td>
</tr>
<tr id="row592153016356"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p7938300359"><a name="p7938300359"></a><a name="p7938300359"></a>disktype</p>
</td>
<td class="cellrowborder" valign="top" width="20.830000000000002%" headers="mcps1.2.4.1.2 "><p id="p3931030123518"><a name="p3931030123518"></a><a name="p3931030123518"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.18%" headers="mcps1.2.4.1.3 "><p id="p393103020356"><a name="p393103020356"></a><a name="p393103020356"></a>磁盘类型，同volumetype字段</p>
</td>
</tr>
<tr id="row393143053510"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.2.4.1.1 "><p id="p119314308357"><a name="p119314308357"></a><a name="p119314308357"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20.830000000000002%" headers="mcps1.2.4.1.2 "><p id="p79363016359"><a name="p79363016359"></a><a name="p79363016359"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.18%" headers="mcps1.2.4.1.3 "><p id="p39353093517"><a name="p39353093517"></a><a name="p39353093517"></a>磁盘大小，GB</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section147622299355"></a>

-   请求示例

    ```
    GET  v1/sms/vm/template/90c950d7-d184-4b5e-87c0-f0bd09dfa0c1
    ```

-   响应示例

    ```
    {
        "template": {
            "id":"aaaa-bbbb",
            "name": "模板名称",
            "is_template":"false",// 创建任务为false，保存模板为true
            "region":"cn-north-1",
            
            
            "target_server_name":"目的端1",
            "availability_zone":"az1-dc1", //可用区名称
            "volumetype": "DESS_SSD_FC",
            "vpc": {
              "id":"0dae26c9-9a70-4392-93f3-87d53115d171",
              "name":"vpc1" 
            },
            "security_groups":[
              {
    	    "id":"507ca48f-814c-4293-8706-300564d54620", 
                "name":"default"
    	   }
             ], 
            "nics":[
              {
                "id":"157ee789-03ea-45b1-a698-76c92660dd83",
                "name": "subnet-1637",
                "cidr": "192.168.0.0/24"，
    	    "ip":"192.168.0.0"
               }
            ],
            "flavors":[
              {
                "id": "c3.2xlarge.4",
    	    "name": "c3.2xlarge.4",
              }
            ],
            "publicip":  {
                 "id":"1111",
                 "ip ":"x.x.x.x",
                 "type": "5_bgp",
                 "bandwidth_size":10,
                 "bandwidth_share_type":"PER"
            }
        },
        "disks":[
          {
            "index":0,
            "name":"磁盘01",
            "disktype":"DESS_SSD_FC",
            "size":40
         }
        ]
    }
    ```


## 状态码<a name="section1973012935418"></a>

状态码请参见[状态码](状态码.md)。

## 错误码<a name="section8616450105718"></a>

请参见[错误码](错误码.md)。

