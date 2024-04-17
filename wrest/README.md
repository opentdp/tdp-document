# Wrest Chat

智能聊天助手，是一个通用的聊天辅助程序，通过 [Nanomsg 协议](https://github.com/opentdp/wrest-chat/blob/master/wcferry/proto/wcferry.proto) 与聊天软件互通，内置 WEB 管理界面，可接入GPT、Gemini、星火、文心、混元、通义千问等大语言模型。目前已适配 *PC微信*，更多聊天软件适配中，敬请期待！

> 本项目**未对微信程序进行任何破解或修改**，与微信互操作的能力均基于开源项目 [WeChatFerry RPC](https://github.com/lich0821/WeChatFerry/tree/master/WeChatFerry) 实现，感谢各位开源贡献者。

## 主要特性

- 使用 Go 语言编写，无运行时依赖
- 提供 HTTP 接口，便于对接各类编程语言
- 提供 Websocket 接口，接收推送的新消息
- 支持 HTTP/WS 接口授权，参见 [配置说明](#配置说明)
- 支持作为 SDK 使用，参见 [SDK 模块](/wrest/开发指南/SDK模块.md)
- 内置 AI 机器人，参见 [Bot 模块](/wrest/开发指南/BOT模块.md)
- 内置 Web 管理界面，可以管理机器人各项配置
- 内置 Api 调试工具，所有接口都可以在线调试
- 尽可能将消息中的 Xml 转为 Object，便于前端解析
- 支持计划任务、外部指令、指令插件等扩展功能，详见 [wrest-plugin](https://github.com/opentdp/wrest-plugin)