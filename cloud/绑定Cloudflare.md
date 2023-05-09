# 绑定Cloudflare
## 创建API令牌
1、进入 **Cloudflare** [个人资料 - API 令牌](https://dash.cloudflare.com/profile/api-tokens) 页面，并点击`创建令牌`

![创建API令牌](/img/20230429104407.png)

2、下滑页面，找到`创建自定义令牌`，点击`开始使用`

![创建自定义令牌](/img/20230429104544.png)

3、创建一个令牌 `TDPCloudAccess`，权限如下：

![设置权限](/img/20230429112447.png)

```text
User.User Details, Zone.Zone Settings, Zone.Zone, Zone.SSL and Certificates, Zone.DNS
```
完成设置后下滑页面点击`继续以显示摘要`，在摘要页面点击`创建令牌`

![继续以显示摘要](/img/20230429113356.png)

4、在随后弹出的页面复制并保存 `API Token`

## 绑定账号
1、进入 **TDP Cloud** 后台，`厂商管理 - Cloudflare`，

![添加账号](/img/20230429113902.png)

2、在弹出的窗口设置**别名、邮箱、以及获取到的 `API Token`**，点击`提交`保存

![设置账号](/img/20230429114251.png)

3、在 `厂商管理 - Cloudflare` 中找到刚添加的账号，点击`管理`进入`域名列表`页面

![管理账号](/img/20230429114709.png)

4、在`域名列表`页面，选择需要导入资源，点击 `导入` 按钮，完成绑定操作

![导入资源](/img/20230429114943.png)
