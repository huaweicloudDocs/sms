# 创建用户并授权使用SMS<a name="sms_03_0033"></a>

如果您需要对您所拥有的SMS进行精细的权限管理，您可以使用[统一身份认证服务](https://support.huaweicloud.com/usermanual-iam/iam_01_0001.html)（Identity and Access Management，简称IAM），通过IAM，您可以：

-   根据企业的业务组织，在您的华为云账号中，给企业中不同职能部门的员工创建IAM用户，让员工拥有唯一安全凭证，并使用SMS。
-   根据企业用户的职能，设置不同的访问权限，以达到用户之间的权限隔离。
-   将SMS委托给更专业、高效的其他华为云账号或者云服务，这些账号或者云服务可以根据权限进行代运维。

如果华为云账号已经能满足您的要求，不需要创建独立的IAM用户，您可以跳过本章节，不影响您使用SMS的其它功能。

本章节为您介绍对用户授权的方法，操作流程如[图1](#zh-cn_topic_0248056439_fig22491610111212)所示。

## 前提条件<a name="zh-cn_topic_0248056439_section667633414252"></a>

给用户组授权之前，请您了解用户组可以添加的SMS权限，并结合实际需求进行选择，SMS支持的系统权限，请参见：[SMS系统权限](https://support.huaweicloud.com/productdesc-sms/sms_01_0015.html)。若您需要对除SMS之外的其它服务授权，IAM支持服务的所有权限请参见[权限策略](https://support.huaweicloud.com/permissions/policy_list.html?product=sms)。

## 示例流程<a name="zh-cn_topic_0248056439_section0134123631120"></a>

**图 1**  给用户授权SMS权限流程<a name="zh-cn_topic_0248056439_fig22491610111212"></a>  
![](figures/给用户授权SMS权限流程.png "给用户授权SMS权限流程")

1.  <a name="zh-cn_topic_0248056439_li752124051217"></a>[创建用户组并授权](https://support.huaweicloud.com/usermanual-iam/iam_03_0001.html)

    在IAM控制台创建用户组，并授予“SMS Administrator”、"OBS OperateAccess"、“ECS FullAccess”。

2.  [创建用户并加入用户组](https://support.huaweicloud.com/usermanual-iam/iam_02_0001.html)

    在IAM控制台创建用户，并将其加入[1](#zh-cn_topic_0248056439_li752124051217)中创建的用户组。

3.  [用户登录](https://support.huaweicloud.com/usermanual-iam/iam_01_0552.html)并验证权限

    新创建的用户登录控制台，切换至授权区域，验证权限：

    -   在“服务列表”中选择主机迁移服务，进入主机迁移服务主界面，在服务器列表页面找到待迁移的服务器，在“目的端服务器”列下单击![](figures/2-7-1.png)，设置目的端服务器。若可以设置目的端服务器，表示授予的权限已生效。
    -   在“服务列表”中选择除主机迁移服务外的任一服务，若提示权限不足，表示授予的权限已生效。

        >![](public_sys-resources/icon-note.gif) **说明：** 
        >若默认SMS权限不满足您的授权要求，可参考[SMS自定义策略](SMS自定义策略.md)使用SMS细粒度策略。



