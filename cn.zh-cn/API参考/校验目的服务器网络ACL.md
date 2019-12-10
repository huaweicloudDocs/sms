# 校验目的服务器网络ACL<a name="sms_api_0030"></a>

## 功能介绍<a name="section38822055785"></a>

校验目的端服务器网络ACL信息。

## URI<a name="section1888316551281"></a>

GET /v1/sms/tasks/\{t\_project\_id\}/networkacl/\{t\_subnet\_id\}/check?region\_id=xx

## 请求消息<a name="section10884155889"></a>

**请求参数**

请求参数如[表1](#table138871552086)所示。

**表 1**  参数说明

<a name="table138871552086"></a>
<table><thead align="left"><tr id="row09935554811"><th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.1"><p id="p199931155683"><a name="p199931155683"></a><a name="p199931155683"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.2"><p id="p9993175511820"><a name="p9993175511820"></a><a name="p9993175511820"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.5.1.3"><p id="p999475510812"><a name="p999475510812"></a><a name="p999475510812"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.01489851014899%" id="mcps1.2.5.1.4"><p id="p169946551783"><a name="p169946551783"></a><a name="p169946551783"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1199415511815"><td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.1 "><p id="p199415555811"><a name="p199415555811"></a><a name="p199415555811"></a>t_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p999418551785"><a name="p999418551785"></a><a name="p999418551785"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p15994255682"><a name="p15994255682"></a><a name="p15994255682"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.01489851014899%" headers="mcps1.2.5.1.4 "><p id="p17994155519812"><a name="p17994155519812"></a><a name="p17994155519812"></a>目的端服务器所在的projectId</p>
</td>
</tr>
<tr id="row119948554815"><td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.1 "><p id="p1799411552817"><a name="p1799411552817"></a><a name="p1799411552817"></a>t_subnet_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p599414551782"><a name="p599414551782"></a><a name="p599414551782"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p699413551083"><a name="p699413551083"></a><a name="p699413551083"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.01489851014899%" headers="mcps1.2.5.1.4 "><p id="p09946556819"><a name="p09946556819"></a><a name="p09946556819"></a>目的端服务器第一个网卡的子网ID</p>
</td>
</tr>
<tr id="row1994105518813"><td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.1 "><p id="p19994175515818"><a name="p19994175515818"></a><a name="p19994175515818"></a>region_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p1299435517817"><a name="p1299435517817"></a><a name="p1299435517817"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p89941255989"><a name="p89941255989"></a><a name="p89941255989"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.01489851014899%" headers="mcps1.2.5.1.4 "><p id="p099415550813"><a name="p099415550813"></a><a name="p099415550813"></a>目的端服务器所在的regionId ,如cn-north-1</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section5912195511816"></a>

不涉及

## 示例<a name="section09132551480"></a>

-   请求示例

    无

-   响应示例

    无响应消息。


## 状态码<a name="section1973012935418"></a>

状态码请参见[状态码](状态码.md)。

## 错误码<a name="section1897875543520"></a>

请参见[错误码](错误码.md)。

