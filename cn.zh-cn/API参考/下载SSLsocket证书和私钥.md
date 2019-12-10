# 下载SSLsocket证书和私钥<a name="sms_api_0032"></a>

## 功能介绍<a name="section3297183017508"></a>

当源端服务器为Windows操作系统时，安装在源端服务器上的迁移Agent通过SSLSocket同目的端服务器通信，该接口用于下载目的端服务器所需要的证书和私钥\(PEM格式\)。

>![](public_sys-resources/icon-note.gif) **说明：**   
>迁移Agent自动调用此接口用于下载SSLsocket证书和私钥，您无需调用此接口。  

## URI<a name="section19298530155013"></a>

GET /v1/sms/tasks/\{task\_id\}/certkey

参数说明请参见[表1](#table9128848172010)。

**表 1**  参数说明

<a name="table9128848172010"></a>
<table><thead align="left"><tr id="row1112910489205"><th class="cellrowborder" valign="top" width="21.016990888943607%" id="mcps1.2.4.1.1"><p id="p26621457458"><a name="p26621457458"></a><a name="p26621457458"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="21.12780103422802%" id="mcps1.2.4.1.2"><p id="p666435715514"><a name="p666435715514"></a><a name="p666435715514"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="57.85520807682837%" id="mcps1.2.4.1.3"><p id="p8665657256"><a name="p8665657256"></a><a name="p8665657256"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row113113489201"><td class="cellrowborder" valign="top" width="21.016990888943607%" headers="mcps1.2.4.1.1 "><p id="p16171102703018"><a name="p16171102703018"></a><a name="p16171102703018"></a>task_id</p>
</td>
<td class="cellrowborder" valign="top" width="21.12780103422802%" headers="mcps1.2.4.1.2 "><p id="p7260143210433"><a name="p7260143210433"></a><a name="p7260143210433"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="57.85520807682837%" headers="mcps1.2.4.1.3 "><p id="p1626033216432"><a name="p1626033216432"></a><a name="p1626033216432"></a>任务的ID</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section9305130145012"></a>

无

## 响应消息<a name="section193058304502"></a>

**响应参数**

响应参数如[表2](#table1130633010504)所示。

**表 2**  响应参数

<a name="table1130633010504"></a>
<table><thead align="left"><tr id="row638011309503"><th class="cellrowborder" valign="top" width="20.84%" id="mcps1.2.4.1.1"><p id="p8131164842014"><a name="p8131164842014"></a><a name="p8131164842014"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.09%" id="mcps1.2.4.1.2"><p id="p13131114815209"><a name="p13131114815209"></a><a name="p13131114815209"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60.07%" id="mcps1.2.4.1.3"><p id="p17131144872019"><a name="p17131144872019"></a><a name="p17131144872019"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row73802030195011"><td class="cellrowborder" valign="top" width="20.84%" headers="mcps1.2.4.1.1 "><p id="p11380193095014"><a name="p11380193095014"></a><a name="p11380193095014"></a>cert</p>
</td>
<td class="cellrowborder" valign="top" width="19.09%" headers="mcps1.2.4.1.2 "><p id="p143801730145011"><a name="p143801730145011"></a><a name="p143801730145011"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60.07%" headers="mcps1.2.4.1.3 "><p id="p43801930145015"><a name="p43801930145015"></a><a name="p43801930145015"></a>PEM格式的自签名证书</p>
</td>
</tr>
<tr id="row10380173045011"><td class="cellrowborder" valign="top" width="20.84%" headers="mcps1.2.4.1.1 "><p id="p163801930155015"><a name="p163801930155015"></a><a name="p163801930155015"></a>private_key</p>
</td>
<td class="cellrowborder" valign="top" width="19.09%" headers="mcps1.2.4.1.2 "><p id="p113801630205019"><a name="p113801630205019"></a><a name="p113801630205019"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60.07%" headers="mcps1.2.4.1.3 "><p id="p10380153035014"><a name="p10380153035014"></a><a name="p10380153035014"></a>PEM格式的私钥</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section17313173055018"></a>

-   请求示例

    无请求消息


-   响应示例

    ```
    {
    "cert":"  -----BEGIN CERTIFICATE-----
    MIICrjCCAhegAwIBAgIBADANBgkqhkiG9w0BAQUFADCBnDELMAkGA1UEBhMCQ04x
    EjAQBgNVBAgMCUd1YW5nRG9uZzERMA8GA1UEBwwIU2hlbnpoZW4xDTALBgNVBAoM
    BE1hYVMxFDASBgNVBAsMC0Nsb3VkYmlsaXR5MSIwIAYDVQQDDBlBdGxhcyBQZXJz
    b25hbCBMaWNlbnNlIENBMR0wGwYJKoZIhvcNAQkBFg5jd2pjc3VAMTI2LmNvbTAe
    Fw0xODAzMTYwMTQzMDFaFw0xOTAzMTYwMTQzMDFaMIGcMQswCQYDVQQGEwJDTjES
    MBAGA1UECAwJR3VhbmdEb25nMREwDwYDVQQHDAhTaGVuemhlbjENMAsGA1UECgwE
    TWFhUzEUMBIGA1UECwwLQ2xvdWRiaWxpdHkxIjAgBgNVBAMMGUF0bGFzIFBlcnNv
    bmFsIExpY2Vuc2UgQ0ExHTAbBgkqhkiG9w0BCQEWDmN3amNzdUAxMjYuY29tMIGf
    MA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDGA3ahP8o4h9B6BLlfOVECpbeHbB4+
    H8dNB+NtAopv9NKg2fz9KPTxJKw037L/dCNE/DCFFlu9dczxXmJRFIRRz677LcBj
    T+05VEjil86qeucnWGVZJjTqG11f5eTUGzUlV12cT425Q/y/BdWAniW70XfjOeeS
    hOW6CZefJ9Q0FwIDAQABMA0GCSqGSIb3DQEBBQUAA4GBAH16ASRuNjbJ5eIBPAig
    9vmQ3iPgUYJFCMPoJeZWecrqj+pGhVJDsviLimNmEnCkEJpRf0sFvPG64R/BISsB
    v/PXvfDLwfTcx1q2j9Y4i3sPe2JfwPKcQLKPdZIyakk9tYsRztFPoxlK0F7YQKd+
    rvbHNGLkWxDArm44wURYFA1t
    -----END CERTIFICATE-----",
    "private_key":"-----BEGIN RSA PRIVATE KEY-----
    MIICXAIBAAKBgQDGA3ahP8o4h9B6BLlfOVECpbeHbB4+H8dNB+NtAopv9NKg2fz9
    KPTxJKw037L/dCNE/DCFFlu9dczxXmJRFIRRz677LcBjT+05VEjil86qeucnWGVZ
    JjTqG11f5eTUGzUlV12cT425Q/y/BdWAniW70XfjOeeShOW6CZefJ9Q0FwIDAQAB
    AoGAG753fC9iZ5pL8RTBXmC7A4pxlRVmhWDRfW8KBAeTmw0sB+KTKmt3KmRvhncD
    bvx4Rp2pNLSFxR2Ayh7l2qNryIWcuxTrlDowGrUg+QzwMfJixczAEU7IHCRC2k3t
    7yf0EILYoM+A+SgvDO8YWhaJ6SYe0zAHFZbabNsSbWzbb8kCQQDlggnh5CN/nDHb
    URZ1FoUrQ8pzk3rc6krWe4WWPx9YJ33zgCOut1w2y2eJ0SN1m+yxAAZ22fnY47kj
    HrS8TjvZAkEA3N7DnLggtQcOC6Ye2v5SGLzv0O6Gw5Xl3NLWiiGK8kY/3Q1Aa5gh
    /8qBnqKLfxpe+3IKfN+wrXUG5PV+XdapbwJAbKbdatWIgLc/WybOTOw2az8SrxiY
    x9EbUOL1YSXM/vzjQc3eFq6ztzUgdTxPXzRMH5d1d/rFr4pPcXLt+V/IMQJBAJQB
    AnumNuSX0aWkr9B303OYR+ttqwitDdcnwXPWflFTGcB6/MwcqcvKW4l9ypRli3hb
    NwPusWnKndAXYZJoIikCQGe7Nb+e59Ksm5+BoSXp/07FriqvwPrDkr+e1Xpfmoai
    s4U4T0RA/NkYRTX/jN/HtpXkjR/dEf7RAAmNO3WtKm4=
    -----END RSA PRIVATE KEY-----"
    }
    ```


## 状态码<a name="section1973012935418"></a>

状态码请参见[状态码](状态码.md)。

## 错误码<a name="section19154339135213"></a>

请参见[错误码](错误码.md)。

