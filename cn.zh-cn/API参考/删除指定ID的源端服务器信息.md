# 删除指定ID的源端服务器信息<a name="sms_api_0016"></a>

## 功能介绍<a name="section188551911122919"></a>

从主机迁移服务界面上删除指定ID的源端服务器信息。一旦源端服务器信息被删除，则只能通过重启源端服务器上的迁移Agent来将源端服务器信息重新添加在主机迁移服务界面。

## URI<a name="section1785712112291"></a>

DELETE /v1/sms/sources/\{source\_id\}

参数说明请参见[表1](#table4257958937)。

**表 1**  参数说明

<a name="table4257958937"></a>
<table><thead align="left"><tr id="row10257758336"><th class="cellrowborder" valign="top" width="17.080413350754245%" id="mcps1.2.4.1.1"><p id="p1625714581132"><a name="p1625714581132"></a><a name="p1625714581132"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.880745931820881%" id="mcps1.2.4.1.2"><p id="p16257195814319"><a name="p16257195814319"></a><a name="p16257195814319"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="67.03884071742486%" id="mcps1.2.4.1.3"><p id="p17257758736"><a name="p17257758736"></a><a name="p17257758736"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row19257155811320"><td class="cellrowborder" valign="top" width="17.080413350754245%" headers="mcps1.2.4.1.1 "><p id="p72572586316"><a name="p72572586316"></a><a name="p72572586316"></a>source_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.880745931820881%" headers="mcps1.2.4.1.2 "><p id="p5257105815318"><a name="p5257105815318"></a><a name="p5257105815318"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="67.03884071742486%" headers="mcps1.2.4.1.3 "><p id="p0257165811313"><a name="p0257165811313"></a><a name="p0257165811313"></a>源端服务器的ID</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section286991112292"></a>

无

## 响应消息<a name="section68711011102917"></a>

不涉及

## 示例<a name="section148721611132911"></a>

-   请求示例

    无请求消息


-   响应示例

    无响应消息


## 状态码<a name="section1973012935418"></a>

状态码请参见[状态码](状态码.md)。

## 错误码<a name="section787341114298"></a>

请参见[错误码](错误码.md)。

