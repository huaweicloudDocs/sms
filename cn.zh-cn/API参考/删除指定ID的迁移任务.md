# 删除指定ID的迁移任务<a name="sms_api_0026"></a>

## 功能介绍<a name="section14661745133517"></a>

删除指定ID的迁移任务。

只有任务状态为READY、ABORT、FAIL、SUCCESS时才能执行删除操作。

## URI<a name="section1246744510358"></a>

DELETE /v1/sms/tasks/\{task\_id\}

参数说明请参见[表1](#table9128848172010)。

**表 1**  参数说明

<a name="table9128848172010"></a>
<table><thead align="left"><tr id="row1112910489205"><th class="cellrowborder" valign="top" width="17.75488199353061%" id="mcps1.2.4.1.1"><p id="p2084672419512"><a name="p2084672419512"></a><a name="p2084672419512"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="22.17563196357973%" id="mcps1.2.4.1.2"><p id="p78489241653"><a name="p78489241653"></a><a name="p78489241653"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="60.06948604288965%" id="mcps1.2.4.1.3"><p id="p48486243519"><a name="p48486243519"></a><a name="p48486243519"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row113113489201"><td class="cellrowborder" valign="top" width="17.75488199353061%" headers="mcps1.2.4.1.1 "><p id="p52072412255"><a name="p52072412255"></a><a name="p52072412255"></a>task_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.17563196357973%" headers="mcps1.2.4.1.2 "><p id="p1215169436"><a name="p1215169436"></a><a name="p1215169436"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="60.06948604288965%" headers="mcps1.2.4.1.3 "><p id="p19171269433"><a name="p19171269433"></a><a name="p19171269433"></a>任务的ID</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section14476124553519"></a>

不涉及

## 响应消息<a name="section1947624516357"></a>

不涉及

## 示例<a name="section347794512351"></a>

-   请求示例

    无请求消息。


-   响应示例

    无响应消息。


## 状态码<a name="section1973012935418"></a>

状态码请参见[状态码](状态码.md)。

## 错误码<a name="section2047894523518"></a>

请参见[错误码](错误码.md)。

