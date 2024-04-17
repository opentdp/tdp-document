# 开发指南

模块依赖示意：`WEB ---> API ---> BOT ---> SDK ---> Wcferry ---> WeChat`。其中 `BOT` 模块并非必须的，可根据自己的需求选择是否开启，`Wcferry` 模块为第三方开源依赖，必须和 `WeChat` 版本匹配使用。

查看和调试 *HTTP/WS* 接口，可使用浏览器访问 `http://localhost:7600/swagger/`。更多插件开发资源请查阅 [wrest-plugin](https://github.com/opentdp/wrest-plugin) 项目。

## API 模块

实现了 HTTP/WS 接口，详情查看 [API 模块](/wrest/开发指南/API模块.md)

## BOT 模块

实现了群聊机器人，详情查看 [BOT 模块](/wrest/开发指南/BOT模块.md)

## SDK 模块

实现了 WCF 客户端，详情查看 [SDK 模块](/wrest/开发指南/SDK模块.md)

## WEB 模块

实现了 WEB 控制台，详情查看 [webview/README.md](./webview/README.md)