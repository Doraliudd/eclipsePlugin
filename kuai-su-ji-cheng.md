# 快速集成

配置销售易Eclipse Plugin

1. 获取销售易Eclipse插件后，请将插件放入Eclipse安装目录下的plugins文件夹下。
   ![](/assets/com.png)
2. 打开本地Eclipse，新建一个Project。
   ![](/assets/newproject.png)
3. 选择XSYproject，点击Next 按钮进行下一步操作。
   ![](/assets/xsyproject.png)
4. 创建project 名称和package，填写相关登录信息。
   ![](/assets/newxsyproject.png)

相关参数说明：

| **参数** | **说明** |
| :--- | :--- |
| Project name | 创建的项目业务逻辑代码名称 |
| Project package | 创建的包名称，必须是三级包路径，以other 开头。例如： other.xsy.sample |
| User name | 系统用户登录名 |
| Password | 系统用户登录密码 |
| ClientId、ClientSecret | 创建连接器后，获取的连接器详细信息。详见《PaaS 平台 开发手册》中连接器章节 |
| SecretCode | 在**个人设置&gt; 安全令牌**，获取安全令牌 |
| host | 填写URL，用来区分生产环境和沙盒环境 |

**NOTE:**

> * _**一个Eclipseworkspace 下的所有project 享有同一套登陆信息，并且修改任一projectcredentials 都会影响相同workspace 下的其他proejct。**_
>
> * _**如果在多租户并行开发时，需要给每个租户单独创建一个Eclipseworkspace，做到一个租户享有一个workspace。**_

5.点击Finish 按钮，查看创建的项目。我们的开发人员已经进行了集成和封装，您创建项目需要的SDK 等一系列相关配置文件已经存在。

![](/assets/sdk.png)

