# Linux 服务端

> 说明：本文档仅适用于部署 wrest 主体程序，不包含 [wcf 补丁](https://github.com/lich0821/WeChatFerry) 和 [wechat](https://github.com/opentdp/wrest-chat/releases/download/v0.27.1/WeChatSetup-3.9.10.27.exe)，需要您自行下载安装，安装后请配置 WCF_ADDRESS 连接外部 wcf 服务使用。如您是新手，建议您参考[快速入门](/wrest/快速入门.md)。

## 手动部署

- 根据系统类型下载编译好的[二进制程序](https://github.com/opentdp/wrest-chat/releases)，解压后，重命名为 `wrest`

- `Linux` 可能需要添加可执行权限，参考命令 `chmod +x ./wrest`

- 在终端执行 `./wrest [config.yml]` 启动服务器

> 说明：`config.yml` 为配置文件路径，可选参数，配置说明请参考[配置文件解析](/wrest/配置文件解析.md)。

## 容器部署

> 此镜像仅用于部署 wrest 主体程序，不包含 wcf.exe 和 wechat，请配置 WCF_ADDRESS 连接外部 wcf 服务使用。

### docker cli

```shell
docker run -d -p 7600:7600 \
    -e WCF_ADDRESS="192.168.1.2:7601" \
    -v ./storage:/srv/storage \
    rehiy/wrest-chat
```

### 参数说明

- `-e WCF_ADDRESS="192.168.1.2:7601"` 指定 wcf 地址
- `-v ./storage:/srv/storage` 指定数据存储路径
- `-v ./plugin:/srv/plugin` 指定插件存储路径
- `-v ./logs:/srv/logs` 指定日志存储路径
- `rehiy/wrest-chat /srv/storage/config.yml` 自定义配置文件路径

> 配置说明请参考[配置文件解析](/wrest/配置文件解析.md)。