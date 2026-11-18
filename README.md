# HomeAlone · Codex / Claude Setup

Windows 原生安装与配置助手，提供 **Codex CLI + ChatGPT** 和 **Claude Code CLI + Claude Desktop** 两种模式。本仓库提供正式安装包和软件更新清单。

## 下载 1.6.0

打开 [最新版本](https://github.com/zhaoquan1003-cpu/Codex-Auto-Download-Releases/releases/latest)，或直接下载对应安装包：

| 安装包 | 适用情况 | 大小 |
| --- | --- | ---: |
| [在线版](https://github.com/zhaoquan1003-cpu/Codex-Auto-Download-Releases/releases/latest/download/CodexSetup-Online.exe) | 联网下载安装，通常选择此版本 | 2.22 MiB |
| [x64 CLI 离线版](https://github.com/zhaoquan1003-cpu/Codex-Auto-Download-Releases/releases/latest/download/CodexSetup-Offline-x64.exe) | Intel / AMD 64 位 Windows，内置官方 Codex CLI 0.170.0 | 202.59 MiB |
| [ARM64 CLI 离线版](https://github.com/zhaoquan1003-cpu/Codex-Auto-Download-Releases/releases/latest/download/CodexSetup-Offline-arm64.exe) | Windows ARM64，内置对应官方 Codex CLI 0.170.0 | 187.72 MiB |

**离线版仅让 Codex CLI 安装不依赖下载网络。** ChatGPT 仍需联网通过 Microsoft 安装；所有版本中的 Claude Code 和 Claude Desktop 均从官方来源在线下载。账号、充值和模型使用也需要联网。Claude Code 采用原生安装，无需 Node.js，Git 为可选工具。

## 选择模式并部署

首次打开默认 **Codex**，以后记住上次选择。Codex 保留原有蓝色配色；Claude 使用官网暖白背景、深灰主按钮和陶土橙强调色，页面、控件与原生弹窗一起切换，便于区分。

1. 阅读并同意启动公告，在侧栏选择模式，勾选需要的应用。软件检测对应运行环境和已有安装。
2. 点击 **一键部署**，依次检查、准备并安装缺少的应用；已有可用版本直接复用。官方安装窗口需要操作时按提示完成，再重新检测。也可选择 **只准备环境**，随后手动安装或更新。
3. 在 **连接账号** 注册或登录 [HomeAlone](https://aloneapi.top/)，注册时按提示完成邮箱验证。Codex 选择 OpenAI 分组，Claude 选择 Anthropic 分组；软件自动创建或复用专用 API Key 并完成本地连接。
4. 需要充值时点击 **充值 / 兑换**，在内嵌链动小铺付款，将获得的兑换码粘贴到兑换框；兑换成功后自动刷新余额。宽窗口左右对照，小窗口上下排列。
5. 完全退出并重新打开对应 CLI 或桌面应用，使连接生效。模型由你在客户端中选择，余额为零也可以先完成配置。

两种模式共用 HomeAlone 账号、余额和充值，分别保存平台分组与加密密钥。切换模式保留另一模式的连接；主动退出账号会同时断开两种模式。登录会话在本机加密保存，密码不保存；旧版手动密钥连接仍可使用。

Codex 的共享 API 配置适用于 Codex CLI 和 ChatGPT 桌面版的本地 Work / Codex；普通云端聊天和 Work Cloud 仍使用官方账号机制。Claude Desktop 需要支持第三方模式的版本及兼容分组；仅限 Claude Code 的分组不能用于 Desktop。Desktop 配置完成后进入第三方提供商模式，可在助手中恢复原配置。

官方安装、连接和兑换结果以实际检测与服务返回为准。账号与兑换流程已通过隔离测试；真实支付到账、Claude Desktop 完整安装与推理及 ARM64 真机运行尚待专用环境验证。下载失败可在 **环境检测 → 下载网络与诊断** 检查代理并重试。

本软件仅供符合使用资格的用户进行合法学习研究，不向中国大陆地区用户提供使用。不得用于违反适用法律、监管要求或第三方服务条款的场景，完整声明见软件启动公告。

## 更新与校验

已有版本可点击软件中的 **检测更新**，获取本仓库 latest Release 的签名 `update.json`。用户选择更新后，助手校验签名、文件大小、SHA-256 和版本，再应用同类型更新；失败时保留或恢复原版本。在线版、x64 离线版和 ARM64 离线版分别更新为对应类型。

每次发布提供 `SHA256SUMS.txt` 和中文说明 `USAGE-zh-CN.txt`。安装器尚未进行 Windows Authenticode 商业签名，应用更新清单签名独立于 Windows 发布者签名。

本工具与 OpenAI 或 Apple 无隶属关系。
