# 下载RSA公私钥<a name="sms_api_0033"></a>

## 功能介绍<a name="section1895014135314"></a>

当源端服务器为Linux操作系统时，安装在源端服务器上的迁移Agent通过SSH来和目的端服务器通信。该接口会返回RSA算法下的一组公私钥，用来做目的端服务器SSH主机秘钥。

>![](public_sys-resources/icon-note.gif) **说明：**   
>迁移Agent自动调用此接口用于下载RSA公私钥，您无需调用此接口。  

## URI<a name="section1995114445316"></a>

GET /v1/sms/tasks/\{task\_id\}/rsakeypair

参数说明请参见[表1](#table9128848172010)。

**表 1**  参数说明

<a name="table9128848172010"></a>
<table><thead align="left"><tr id="row1112910489205"><th class="cellrowborder" valign="top" width="23.892124588503417%" id="mcps1.2.4.1.1"><p id="p104028261162"><a name="p104028261162"></a><a name="p104028261162"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="27.298050139275766%" id="mcps1.2.4.1.2"><p id="p10405142620613"><a name="p10405142620613"></a><a name="p10405142620613"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="48.80982527222081%" id="mcps1.2.4.1.3"><p id="p1840511267613"><a name="p1840511267613"></a><a name="p1840511267613"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row113113489201"><td class="cellrowborder" valign="top" width="23.892124588503417%" headers="mcps1.2.4.1.1 "><p id="p16171102703018"><a name="p16171102703018"></a><a name="p16171102703018"></a>task_id</p>
</td>
<td class="cellrowborder" valign="top" width="27.298050139275766%" headers="mcps1.2.4.1.2 "><p id="p20576145114318"><a name="p20576145114318"></a><a name="p20576145114318"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="48.80982527222081%" headers="mcps1.2.4.1.3 "><p id="p85782051174319"><a name="p85782051174319"></a><a name="p85782051174319"></a>任务的ID</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section29606465314"></a>

无

## 响应消息<a name="section1996224145311"></a>

**响应参数**

响应参数如[表2](#table1396294135317)所示。

**表 2**  响应参数

<a name="table1396294135317"></a>
<table><thead align="left"><tr id="row196115115315"><th class="cellrowborder" valign="top" width="19.09%" id="mcps1.2.4.1.1"><p id="p8131164842014"><a name="p8131164842014"></a><a name="p8131164842014"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.88%" id="mcps1.2.4.1.2"><p id="p13131114815209"><a name="p13131114815209"></a><a name="p13131114815209"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.029999999999994%" id="mcps1.2.4.1.3"><p id="p17131144872019"><a name="p17131144872019"></a><a name="p17131144872019"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row3610519531"><td class="cellrowborder" valign="top" width="19.09%" headers="mcps1.2.4.1.1 "><p id="p1761654532"><a name="p1761654532"></a><a name="p1761654532"></a>private_key</p>
</td>
<td class="cellrowborder" valign="top" width="19.88%" headers="mcps1.2.4.1.2 "><p id="p7626512538"><a name="p7626512538"></a><a name="p7626512538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.029999999999994%" headers="mcps1.2.4.1.3 "><p id="p43801930145015"><a name="p43801930145015"></a><a name="p43801930145015"></a>PEM格式的私钥</p>
</td>
</tr>
<tr id="row146225165315"><td class="cellrowborder" valign="top" width="19.09%" headers="mcps1.2.4.1.1 "><p id="p1862185105318"><a name="p1862185105318"></a><a name="p1862185105318"></a>public_key</p>
</td>
<td class="cellrowborder" valign="top" width="19.88%" headers="mcps1.2.4.1.2 "><p id="p462185195311"><a name="p462185195311"></a><a name="p462185195311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.029999999999994%" headers="mcps1.2.4.1.3 "><p id="p10380153035014"><a name="p10380153035014"></a><a name="p10380153035014"></a>PEM格式的公钥</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section291635211532"></a>

-   请求示例

    无


-   响应示例

    ```
    {
    "private_key ":"-----BEGIN RSA PRIVATE KEY-----\nMIIEoAIBAAKCAQEAo9rcDbwylbq73zmv3IL9cxgBqe+POIIOguVo7ZKqxwOLm2sz\nAf7y/taAtdQdIwGOeuhTXS1o3Ea3sc96XwJhCJbCZwZck/6yO2zq041qL6YQ3VZY\nU1XHJnYp50Fd7mQA2ud5M48DE6ggs5sJ5DDr8g0GzscnIPHB1mg1tP+f1tcTEhFq\nmZiU208VGGetoHFIdgvbcw9V3Ci/INMcoMWe1AsKDNeRVTNdT+qgzqFUEgOUa21/\n8s25Tdv38pHwKobh9GNAICThsoQuOzmuMPv4nxyoNy43CEuGmj+3qdXe6+nJYug6\ndEjP9RCJ5LVt5QEflG81+xDfuTXGjIE/aHqhTQIDAQABAoH/JcNK899ryRZANjIV\nVbzarKvbtk5/s4ZF0eUNSbODqFoo0qjiGJOpbRICl+VK0caKD8l7bP4KLLofm9s1\nWLAzrMcSBqxwqasJaKixdhAhaNndCSXdNVePjk2tWp62BzsE925hgIB1NRKKdtpE\nbVLZDe/yobVET1NoWQGrXwuKyvhn9+z/hDkZJDVoQRolUa2SiNYWh7QiU+GeZ5DD\nPjpiAJfmBe4Zs611AhJMiBQohGDy+L8thGRx3bl69fIIn3Sa1ZTC49sW+82qGHsP\nqhXiB6OCsmVy44DmOUUG/qClY/aSer/a4cNLaZTzzx3IhCeI30ats/0aLEw5Szyb\nsIgBAoGBANO55QA14SgAR+XjGsMOq8/rHU/x3cquJO1COeFF8xCgAOulmRmQbpYC\ni34fJlpNTbi5czTy8JuPsKAcSGnbnFVZtEEB1XpZCDZ5ChSqaiCZECdl79RjZ4GZ\nJMa3uXnwioPh9eHx8RSl+qGAT/15LdkPzDDHrt6QTgTt9rrCxWdNAoGBAMYeU5yJ\nzsq7UufGnZ76q+hvH+lfYrrFz/wE2ZdN2ISGlWV9rr7KEjDNP24rrAzgwNosyepl\nhoBq/nM8k0/GSQTWn2U1qpwdM7tzdFfPsi5NjFP4sufqhXtXJt5xcGTnX275Cu2i\nX6TaeB8aVdomrAD6nEq2/w15nEWPhpqpcSIBAoGAWg3QZFWGbgAolJQTFvIPjAEB\n17YVUxbc5/lqKvIYn3Ke0Zv+0YvILY/pivxu0KveqfpfER9fzZrBUmiVOElLZlYg\nQCIqjb5+qsSyz/Vn7HOOFmPaLWkWZl4f8VHF1yLDl7KtZawFkXXDc5vi6fn30UJR\n5FGahFm2hYw9jFQ5qGUCgYAKAAXgZORXP1VT9aaHG8gJl3JY6UOmgc2ZvvTsujUv\nm0t3L/zeDH0WkYWeHf41ODMD0Dbw6eb8HGpzjp8w66VL5TludmMCNkciMxWwSP+J\nbsiihG8jXacXLrL7j2ZI8ZTTmSaAEC4buBtQFpg2xrTv57Zz3wDIwVat/CyjKeJY\nAQKBgHZGsTBBRMBUEMlSmuctTh41otWjKx34jMtfRzY+zsq59Qy4JMLICOu1rQ8O\nrebbmoRoApEB9xkWDRZe56/Y3cKcImTjiuGAiP/+49srJJz+Wu3lYvukyDs9viCE\n58M/hMpCLNcJEmpB8mr5Eb7+aC2UYZdqIY2Wa56MUiicTX/c\n-----END RSA PRIVATE KEY-----\n",
    "public_key":"ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCj2twNvDKVurvfOa/cgv1zGAGp7484gg6C5WjtkqrHA4ubazMB/vL+1oC11B0jAY566FNdLWjcRrexz3pfAmEIlsJnBlyT/rI7bOrTjWovphDdVlhTVccmdinnQV3uZADa53kzjwMTqCCzmwnkMOvyDQbOxycg8cHWaDW0/5/W1xMSEWqZmJTbTxUYZ62gcUh2C9tzD1XcKL8g0xygxZ7UCwoM15FVM11P6qDOoVQSA5RrbX/yzblN2/fykfAqhuH0Y0AgJOGyhC47Oa4w+/ifHKg3LjcIS4aaP7ep1d7r6cli6Dp0SM/1EInktW3lAR+UbzX7EN+5NcaMgT9oeqFN \n"
    }
    ```


## 状态码<a name="section1973012935418"></a>

状态码请参见[状态码](状态码.md)。

## 错误码<a name="section659701616548"></a>

请参见[错误码](错误码.md)。

