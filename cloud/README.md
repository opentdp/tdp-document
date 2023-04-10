# 土豆片控制面板

[![TDP Cloud Builder](https://github.com/open-tdp/tdp-cloud/actions/workflows/release.yml/badge.svg)](https://github.com/open-tdp/tdp-cloud/actions/workflows/release.yml)

可以跨平台部署的云资源管理面板

- 支持管理多个云账号资源

  - **腾讯云**（*含国际版*）：DNSPod、CVM、Lighthouse
  - **阿里云**（*含国际版*）：AliDNS、ECS、SWAS
  - **CloudFlare**：DNS、Custom Hostnames

- 支持添加子节点 (`TDP Worker`)

  - **Linux**：完整功能
  - **Macos**：部分功能
  - **Windows**：部分功能
  - **Android**：有限支持

- 支持自动签发`SSL证书`，CA对比参见[使用指引](#使用指引)

  - **Let's Encrypt**
  - **Buypass**
  - **Googel Public**
  - **SSL.com**
  - **ZeroSSL**

- 支持 `WebSSH` 终端及`密钥对`管理

  - 支持使用已存储的密钥快速登录

  - 支持执行快捷命令

- 支持敏感数据加密存储（`3DES`）

  - 安装时，生成`通用密钥`，并保存至配置文件

  - 添加敏感资源时，将部分字段加密后存储至数据库

## 功能预览

- 功能支持和开发进度，请参阅 [Issues #1](https://github.com/open-tdp/tdp-cloud/issues/1)

- 在线体验开发版功能，请进入 [演示站点](https://cloud.opentdp.org)，自行注册账号后登录
