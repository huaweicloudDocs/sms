# SMS自定义策略<a name="sms_03_0054"></a>

如果系统预置的SMS权限，不满足您的授权要求，可以创建自定义策略。

目前华为云支持以下两种方式创建自定义策略：

-   可视化视图创建自定义策略：无需了解策略语法，按可视化视图导航栏选择云服务、操作、资源、条件等策略内容，可自动生成策略。
-   JSON视图创建自定义策略：可以在选择策略模板后，根据具体需求编辑策略内容；也可以直接在编辑框内编写JSON格式的策略内容。

具体创建步骤请参见：[创建自定义策略](https://support.huaweicloud.com/usermanual-iam/iam_01_0605.html)。本章为您介绍常用的SMS自定义策略样例。

## SMS自定义策略样例<a name="section51981826152017"></a>

```
{

    "Version": "1.1",
    "Statement": [
        {
            "Action": [
                "vpc:securityGroups:create",
                "vpc:vpcs:create",
                "vpc:publicIps:create",
                "vpc:subnets:create",
                "ecs:cloudServers:create",
                "ecs:cloudServers:updateMetadata",
                "ecs:cloudServers:detachVolume",
                "ecs:cloudServers:attach",
                "ecs:cloudServers:start",
                "ecs:cloudServers:stop",
                "evs:volumes:use",
                "evs:snapshots:create",
                "evs:volumes:update",
                "evs:volumes:create",
                "evs:volumes:delete",
                "evs:volumes:detach",
                "evs:volumes:attach",
                "evs:snapshots:delete",
                "ecs:*:get*",
                "ecs:*:list*",
                "ecs:serverGroups:manage",
                "ecs:serverVolumes:use",
                "evs:*:get*",
                "evs:*:list*",
                "vpc:*:get*",
                "vpc:*:list*",
                "ims:*:list*",
                "SMS:*:*"
            ],
            "Effect": "Allow"
        }
    ]
}
```

