# Ohmbo 插件

[Ohmbo](https://ohmbo.com/zh/) 是覆盖硬件开发全旅程的一站式平台：需求与架构、电子、固件、仿真、3D 结构与外壳、样机与实测，都在同一个项目里完成。这个插件把项目带进 Claude Code：规划产品、整理需求、通过 Ohmbo MCP 发起并跟进设计任务，再回到 ohmbo.com 的完整工作区继续。

## 安装

Claude Code 2.1.275 或更高版本：

```
/plugin install ohmbo --marketplace ohmbo-Official/ohmbo-plugin
```

## 账号与授权

插件内置的生产 MCP（`https://mcp.ohmbo.com/mcp`）使用 OAuth 2.1。Claude Code 会打开 Ohmbo 网站，让用户登录并授权；插件不保存 API key，也不要求用户把密钥或 token 粘贴到对话中。授权后，通过 MCP 创建的任务会出现在网站的 [Agent designs](https://ohmbo.com/dashboard/mcp-designs) 页面，工具结果也会返回对应的网站链接。

可以先从 Free 套餐开始：无需订阅，含一次性试用工作积分；其他套餐及其包含内容见[定价页](https://ohmbo.com/zh/pricing)。创建或修改设计会消耗账号的工作积分。整理需求和服务咨询两项技能无需账号即可使用。

Ohmbo 同时提供 [Developer API v1](https://ohmbo.com/zh/docs/api)，其已测试范围 **Compatible with OpenAI SDKs**，包括 models、Responses 和 Chat Completions。用户可在 [Developer 设置](https://ohmbo.com/zh/settings/apikeys)创建和撤销 `sk-ohmbo-live-...` 或 `sk-ohmbo-test-...` 密钥。MCP OAuth、网站任务和 API key 在各自环境中共用同一 Ohmbo 账户与计算账本。

## 功能

- `ohmbo-services`：介绍 Ohmbo 的服务并帮助选择起点。
- `ohmbo-brief`：整理可复制的产品、设计或打样需求。不会发送给 Ohmbo，由用户自行粘贴到网站。
- `ohmbo-continue`：找到结果、定价或联系页面，并在用户授权后发起、修改和跟进 MCP 设计任务。

MCP 工具可以用自然语言创建和修改设计、查询任务状态、列出和取消任务、发现能力并返回产物信息。任务异步运行，出现在网站的 Agent designs 页面；完整项目、可视化审阅、已发布结果、报价和订单都在网站工作区中。

## 隐私与支持

[隐私政策](https://ohmbo.com/zh/privacy) · [服务条款](https://ohmbo.com/zh/terms) · [founder@ohmbo.com](mailto:founder@ohmbo.com)

## 本地开发

使用 `claude --plugin-dir /absolute/path/to/ohmbo-plugin` 启动，修改后重启或重新加载 Claude Code。建议测试：询问 Ohmbo 服务、整理硬件需求、明确要求创建一个 PCB。创建流程中完成浏览器授权，从 Claude Code 查看任务，再打开工具返回的 Ohmbo 页面。

## 许可证

MIT 许可证仅适用于本仓库中的文件。运行在 `ohmbo.com` 和 `mcp.ohmbo.com` 的服务仍是 Ohmbo 专有的 SaaS，不会因本仓库而开源。
