# 修改指定ID的源端服务器名称<a name="sms_api_0017"></a>

## 功能介绍<a name="section14544151814114"></a>

该功能用来修改SMS服务端的源端名称，方便用户对源端进行管理。

## URI<a name="section1903172311413"></a>

PUT /v1/sms/sources/\{source\_id\}

参数说明请参见[表1](#table9128848172010)。

**表 1**  参数说明

<a name="table9128848172010"></a>
<table><thead align="left"><tr id="row1112910489205"><th class="cellrowborder" valign="top" width="17.37303397766839%" id="mcps1.2.4.1.1"><p id="p195779557578"><a name="p195779557578"></a><a name="p195779557578"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="17.901308680513868%" id="mcps1.2.4.1.2"><p id="p13580185545711"><a name="p13580185545711"></a><a name="p13580185545711"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="64.72565734181775%" id="mcps1.2.4.1.3"><p id="p1758275519571"><a name="p1758275519571"></a><a name="p1758275519571"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row113113489201"><td class="cellrowborder" valign="top" width="17.37303397766839%" headers="mcps1.2.4.1.1 "><p id="p31316487207"><a name="p31316487207"></a><a name="p31316487207"></a>source_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.901308680513868%" headers="mcps1.2.4.1.2 "><p id="p1589831384012"><a name="p1589831384012"></a><a name="p1589831384012"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="64.72565734181775%" headers="mcps1.2.4.1.3 "><p id="p17899181312404"><a name="p17899181312404"></a><a name="p17899181312404"></a>源端服务器的ID</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section15121040144114"></a>

**请求参数**

请求参数如[表2](#table969262217173)所示。

**表 2**  请求参数

<a name="table969262217173"></a>
<table><thead align="left"><tr id="row57801623151717"><th class="cellrowborder" valign="top" width="17.849999999999998%" id="mcps1.2.5.1.1"><p id="p8131164842014"><a name="p8131164842014"></a><a name="p8131164842014"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.62%" id="mcps1.2.5.1.2"><p id="p150663312713"><a name="p150663312713"></a><a name="p150663312713"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.53%" id="mcps1.2.5.1.3"><p id="p13131114815209"><a name="p13131114815209"></a><a name="p13131114815209"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="52%" id="mcps1.2.5.1.4"><p id="p17131144872019"><a name="p17131144872019"></a><a name="p17131144872019"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1078014235177"><td class="cellrowborder" valign="top" width="17.849999999999998%" headers="mcps1.2.5.1.1 "><p id="p97801223111719"><a name="p97801223111719"></a><a name="p97801223111719"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.62%" headers="mcps1.2.5.1.2 "><p id="p135069331472"><a name="p135069331472"></a><a name="p135069331472"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.53%" headers="mcps1.2.5.1.3 "><p id="p18780523101710"><a name="p18780523101710"></a><a name="p18780523101710"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.5.1.4 "><p id="p678092317173"><a name="p678092317173"></a><a name="p678092317173"></a>新的源端名称</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section5203345194117"></a>

无

## 示例<a name="section7195431428"></a>

-   请求示例

    ```
    {
      "name": "newName"
    }
    ```

-   响应示例

    无响应消息。


## 状态码<a name="section1973012935418"></a>

状态码请参见[状态码](状态码.md)。

## 错误码<a name="section10457168420"></a>

请参见[错误码](错误码.md)。

