# API概览<a name="sms_api_0006"></a>

主机迁移服务所提供的接口为SMS接口。通过使用SMS接口，您可以完整的使用主机迁移服务的所有功能，包括查询源端服务器列表、创建迁移任务和查看迁移进度等。

**表 1**  主机迁移服务接口列表

<a name="table3122181416560"></a>
<table><thead align="left"><tr id="row412310143562"><th class="cellrowborder" valign="top" width="31%" id="mcps1.2.3.1.1"><p id="p512381418569"><a name="p512381418569"></a><a name="p512381418569"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="69%" id="mcps1.2.3.1.2"><p id="p10123151475619"><a name="p10123151475619"></a><a name="p10123151475619"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row212311435619"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.3.1.1 "><p id="p10123121495618"><a name="p10123121495618"></a><a name="p10123121495618"></a>源端管理</p>
</td>
<td class="cellrowborder" valign="top" width="69%" headers="mcps1.2.3.1.2 "><p id="p9123514165619"><a name="p9123514165619"></a><a name="p9123514165619"></a>可以实现上报源端服务器基本信息、查询源端服务器列表以及删除源端服务器的操作。</p>
</td>
</tr>
<tr id="row3123814115611"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.3.1.1 "><p id="p15123151416561"><a name="p15123151416561"></a><a name="p15123151416561"></a>任务管理</p>
</td>
<td class="cellrowborder" valign="top" width="69%" headers="mcps1.2.3.1.2 "><p id="p1812381425617"><a name="p1812381425617"></a><a name="p1812381425617"></a>租户用于管理迁移任务的相关接口，包括迁移任务的创建、启动、停止、查询和删除等操作。</p>
</td>
</tr>
<tr id="row141231614145614"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.3.1.1 "><p id="p41231414135612"><a name="p41231414135612"></a><a name="p41231414135612"></a>证书管理</p>
</td>
<td class="cellrowborder" valign="top" width="69%" headers="mcps1.2.3.1.2 "><p id="p6123121415613"><a name="p6123121415613"></a><a name="p6123121415613"></a>可以实现下载SSLsocket证书和私钥、下载RSA公私钥以及下载ECDSA公私钥的操作。</p>
</td>
</tr>
<tr id="row151231814105611"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.3.1.1 "><p id="p8123131419560"><a name="p8123131419560"></a><a name="p8123131419560"></a>命令管理</p>
</td>
<td class="cellrowborder" valign="top" width="69%" headers="mcps1.2.3.1.2 "><p id="p2123121415617"><a name="p2123121415617"></a><a name="p2123121415617"></a>可以实现获取服务端命令以及上报服务端命令执行结果的操作。</p>
</td>
</tr>
<tr id="row153823410175"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.3.1.1 "><p id="p7597138101714"><a name="p7597138101714"></a><a name="p7597138101714"></a>模板管理</p>
</td>
<td class="cellrowborder" valign="top" width="69%" headers="mcps1.2.3.1.2 "><p id="p1507103415233"><a name="p1507103415233"></a><a name="p1507103415233"></a>可以实现查询模板列表、查询制定ID模板信息以及新增、修改、删除模板信息等操作。</p>
</td>
</tr>
</tbody>
</table>

