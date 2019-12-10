# 批量删除指定ID的模板<a name="sms_api_0044"></a>

## 功能介绍<a name="section19440134513471"></a>

批量删除指定ID的模板。

## URI<a name="section1244118457476"></a>

POST /v1/sms/vm/templates/delete

## 请求消息<a name="section13442104574712"></a>

**请求参数**

请求参数如[表1](#table1445645164714)所示。

**表 1**  参数说明

<a name="table1445645164714"></a>
<table><thead align="left"><tr id="row12563114515470"><th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.1"><p id="p19564045144717"><a name="p19564045144717"></a><a name="p19564045144717"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="p256424516478"><a name="p256424516478"></a><a name="p256424516478"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.208479152084792%" id="mcps1.2.5.1.3"><p id="p1556416453470"><a name="p1556416453470"></a><a name="p1556416453470"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50.09499050094991%" id="mcps1.2.5.1.4"><p id="p18564164519479"><a name="p18564164519479"></a><a name="p18564164519479"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1564104514474"><td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.1 "><p id="p155641845204710"><a name="p155641845204710"></a><a name="p155641845204710"></a>ids</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p1356424515476"><a name="p1356424515476"></a><a name="p1356424515476"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.208479152084792%" headers="mcps1.2.5.1.3 "><p id="p8564545124718"><a name="p8564545124718"></a><a name="p8564545124718"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="50.09499050094991%" headers="mcps1.2.5.1.4 "><p id="p13564164584718"><a name="p13564164584718"></a><a name="p13564164584718"></a>模板ID，具体ID请参见<a href="查询模板列表.md">查询模板列表</a>查询出的ID。</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section44641545154711"></a>

无

## 示例<a name="section1746719457474"></a>

-   请求示例

    ```
    POST  v1/sms/vm/templates/delete
    {
     "ids": ["aaaaa-ccc", "eeeee-xxxx"]
    }
    ```

-   响应示例

    无


## 状态码<a name="section1973012935418"></a>

状态码请参见[状态码](状态码.md)。

## 错误码<a name="section8616450105718"></a>

请参见[错误码](错误码.md)。

