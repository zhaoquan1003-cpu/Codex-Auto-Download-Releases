# HomeAlone · Codex Setup

Windows 原生 Codex CLI / ChatGPT 安装与配置助手。本仓库提供正式发布文件和软件更新清单。

## 下载

请从 [最新版本](https://github.com/zhaoquan1003-cpu/Codex-Auto-Download-Releases/releases/latest) 下载：

| 文件 | 适用情况 |
| --- | --- |
| CodexSetup-Online.exe | 轻量在线版，安装时下载官方 Codex CLI |
| CodexSetup-Offline-x64.exe | Intel / AMD 64 位 Windows，内置官方 Codex CLI 原包 |
| CodexSetup-Offline-arm64.exe | Windows ARM64，内置对应官方 Codex CLI 原包 |

离线版可在无法连接官方下载服务时安装 CLI。ChatGPT 仍需联网通过 Microsoft 安装。API 使用也需要连接服务商。ARM64 包已校验、解包，尚未完成 ARM64 真机运行验证。

## 使用

阅读并同意启动公告后，依次完成环境检测、一键配置环境、安装应用。在 [HomeAlone](https://aloneapi.top/) 注册、充值并创建 API Key，通过安装助手获取模型并配置。

共享 API 配置适用于 Codex CLI 和 ChatGPT 桌面版的本地 Work / Codex；普通云端聊天和 Work Cloud 仍使用官方账号机制。

本软件仅供符合使用资格的用户进行合法学习研究，不向中国大陆地区用户提供使用。不得用于违反适用法律、监管要求或第三方服务条款的场景，完整声明见软件启动公告。

## 更新与校验

软件中的「检测更新」读取本仓库 latest Release 的签名 update.json。用户选择更新后，安装助手校验签名、文件大小、SHA-256 和版本，再应用同类型更新；失败时保留或恢复原版本。

每次发布提供 SHA256SUMS.txt 和中文说明 USAGE-zh-CN.txt。安装器尚未进行 Windows Authenticode 商业签名，应用更新清单签名独立于 Windows 发布者签名。

本工具与 OpenAI 或 Apple 无隶属关系。