# 删除指定ID的模板<a name="sms_api_0043"></a>

## 功能介绍<a name="section528316424396"></a>

删除指定ID的模板。

## URI<a name="section22871742153917"></a>

DELETE /v1/sms/vm/template/\{id\}

## 请求消息<a name="section628824216396"></a>

**请求参数**

请求参数如[表1](#table12293242203915)所示。

**表 1**  参数说明

<a name="table12293242203915"></a>
<table><thead align="left"><tr id="row203731642153910"><th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.1"><p id="p23732042123919"><a name="p23732042123919"></a><a name="p23732042123919"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="p43736427394"><a name="p43736427394"></a><a name="p43736427394"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20.407959204079592%" id="mcps1.2.5.1.3"><p id="p837334223913"><a name="p837334223913"></a><a name="p837334223913"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.89551044895511%" id="mcps1.2.5.1.4"><p id="p1137324253911"><a name="p1137324253911"></a><a name="p1137324253911"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row637310429398"><td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.1 "><p id="p103741142143917"><a name="p103741142143917"></a><a name="p103741142143917"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p4374134213912"><a name="p4374134213912"></a><a name="p4374134213912"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.5.1.3 "><p id="p1374104253915"><a name="p1374104253915"></a><a name="p1374104253915"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p1737464216394"><a name="p1737464216394"></a><a name="p1737464216394"></a>模板ID，具体ID请参见<a href="查询模板列表.md">查询模板列表</a>查询出的ID。</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section03082042133918"></a>

无

## 示例<a name="section130954211394"></a>

-   请求示例

    ```
    DELETE  v1/sms/vm/template/aaaaa-bbbb-cccc
    ```

-   响应示例

    无


## 状态码<a name="section1973012935418"></a>

状态码请参见[状态码](状态码.md)。

## 错误码<a name="section8616450105718"></a>

请参见[错误码](错误码.md)。

