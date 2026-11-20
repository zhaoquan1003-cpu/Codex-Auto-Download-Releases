# HomeAlone · Codex / Claude Setup

Windows 原生安装与配置助手，提供 **Codex CLI + ChatGPT** 和 **Claude Code CLI + Claude Desktop** 两种模式。本仓库只提供下载说明、正式安装包和软件更新清单，不包含私有源码、签名私钥或用户配置。

## 下载 1.7.1

打开 [1.7.1 正式版](https://github.com/zhaoquan1003-cpu/Codex-Auto-Download-Releases/releases/tag/v1.7.1) 或 [最新版本](https://github.com/zhaoquan1003-cpu/Codex-Auto-Download-Releases/releases/latest)，也可直接下载对应安装包：

| 安装包 | 适用情况 | 大小 |
| --- | --- | ---: |
| [在线版](https://github.com/zhaoquan1003-cpu/Codex-Auto-Download-Releases/releases/download/v1.7.1/CodexSetup-Online.exe) | 网络可访问官方来源，希望下载更小的安装助手 | 2.31 MiB（2,421,760 字节） |
| [x64 CLI 离线版](https://github.com/zhaoquan1003-cpu/Codex-Auto-Download-Releases/releases/download/v1.7.1/CodexSetup-Offline-x64.exe) | 普通 Intel / AMD 64 位 Windows，内置官方 Codex CLI 0.170.0 | 202.68 MiB（212,521,984 字节） |
| [ARM64 CLI 离线版](https://github.com/zhaoquan1003-cpu/Codex-Auto-Download-Releases/releases/download/v1.7.1/CodexSetup-Offline-arm64.exe) | Windows ARM64，内置对应官方 Codex CLI 0.170.0 | 187.80 MiB（196,927,488 字节） |

**离线版仅让 Codex CLI 安装不依赖下载网络。** ChatGPT 仍需联网通过 Microsoft 安装；所有版本中的 Claude Code 和 Claude Desktop 均从官方来源在线下载。账号、充值和模型使用也需要联网。Claude Code 采用原生安装，无需 Node.js，Git 为可选工具。

## 三步开始

首次打开默认 **Codex**，以后记住上次选择。Codex 使用蓝色配色；Claude 使用暖白背景、深灰主按钮和陶土橙强调色，页面、控件与原生弹窗一起切换。

1. **准备应用**：打开 EXE，阅读使用须知并自行决定是否同意，在首页点击 **一键准备并继续**。默认只准备 Codex CLI，ChatGPT Desktop 为可选项；软件检查、准备并安装缺少的应用，已有可用版本直接复用。官方安装窗口需要操作时按提示完成，再重新检测。
2. **注册 / 连接**：在 **连接账号** 注册或登录独立的 [HomeAlone](https://aloneapi.top/) 账号，注册时按提示完成邮箱验证。唯一兼容方案自动连接；多个方案按用途与计费倍率选择。Codex 使用 OpenAI 分组，Claude 使用 Anthropic 分组；软件自动创建或复用专用 API Key 并完成本地连接，无需手动复制 Key。余额不足时在账号页 **充值 / 兑换**，将小铺交付的兑换码粘贴到兑换框并核对到账结果。
3. **启动官方客户端**：在首页或 **连接账号** 页打开已安装的 Codex CLI、ChatGPT、Claude Code 或 Claude Desktop。Codex CLI 默认从 `文档/HomeAlone/Codex CLI` 启动；进入官方客户端后选择项目文件夹并开始任务。连接配置变化后，已运行的客户端请退出并重开。

两种模式共用 HomeAlone 账号、余额和充值，分别保存平台分组与加密密钥。切换模式保留另一模式的连接；主动退出账号会同时断开两种模式。登录会话在本机加密保存，密码不保存；旧版手动密钥连接仍可使用。

**1.7.1 已移除软件内原生 Codex 工作台、内嵌 app-server、工作文件夹选择器、流式对话和任务审批界面。** 对话、项目文件夹、模型、文件操作和审批由官方客户端管理。本版不会删除旧版本已有的 provider、auth、workspace 或 `workbench-preferences.json`；工作台偏好保留，但不再读取。

Codex 的共享 API 配置适用于 Codex CLI 和 ChatGPT 桌面版的本地 Work / Codex；普通云端聊天和 Work Cloud 仍使用官方账号机制。Claude Desktop 需要支持第三方模式的版本及兼容分组；仅限 Claude Code 的分组不能用于 Desktop。Desktop 配置完成后进入第三方提供商模式，可在助手中恢复原配置。

## 费用与使用范围

**软件和安装包不包含免费额度。** 注册、登录或连接成功不代表赠送额度。发送任务会使用账号额度，相关任务和文件内容会交由服务商处理；费用以服务商当前方案、模型规则和实际账单为准。软件不承诺固定任务价格或未经确认的积分换算。

本软件仅供符合使用资格的用户进行合法学习研究，不向中国大陆地区用户提供使用。不得用于违反适用法律、监管要求或第三方服务条款的场景，完整声明见软件启动公告。

## GitHub 部署加速

1.7.1 保留在线部署 Codex CLI 时按需启动的 GitHub 下载加速，自动测试最多 8 条线路并选择测试成功且延迟最低的一条。Mihomo 内核按架构首次下载并校验，所需文件下载完成、取消或失败后自动关闭；安装器退出时回收进程。仅允许 GitHub 及必要发布资源域名，不修改 Windows 系统代理。

**本次公开发行未预置公共加速网关。** 未配置网关或本机订阅时仍使用普通官方下载；个人订阅和节点凭据不随安装包分发。下载失败可在 **环境检测 → 下载网络与诊断** 检查代理并重试。

## 验证范围

1.7.1 已完成核心安装、配置、账号与布局隔离回归、实际安装包资源检查，以及 x64 离线安装后实际运行 Codex CLI 0.170.0 的验证。账号、模型和兑换自动测试使用合成夹具，不代表真实业务全部通过。ARM64 仅完成解包、哈希和 PE 架构检查，未完成 ARM64 真机运行。

真实 HomeAlone 注册收信、充值兑换、付费模型推理、Claude Desktop 完整安装与推理、干净 Windows 官方保护准备、原生文件工具、缺失 WebView2 Runtime 的真实安装恢复和 ARM64 真机仍需相应条件验收。官方安装、连接和兑换结果以实际检测与服务返回为准。

## 更新与校验

已有版本可点击软件中的 **检测更新**，获取本仓库 latest Release 的签名 `update.json`。用户选择更新后，助手校验签名、文件大小、SHA-256 和版本，再应用同类型更新；失败时保留或恢复原版本。在线版、x64 离线版和 ARM64 离线版分别更新为对应类型。

每次发布提供 [SHA256SUMS.txt](https://github.com/zhaoquan1003-cpu/Codex-Auto-Download-Releases/releases/download/v1.7.1/SHA256SUMS.txt)、[中文使用说明](https://github.com/zhaoquan1003-cpu/Codex-Auto-Download-Releases/releases/download/v1.7.1/USAGE-zh-CN.txt) 和 [更新说明](https://github.com/zhaoquan1003-cpu/Codex-Auto-Download-Releases/releases/download/v1.7.1/release-notes.md)。安装器尚未进行 Windows Authenticode 商业签名，Windows 可能显示未知发布者；请核对下载来源和校验和，不要关闭系统安全保护。应用更新清单签名独立于 Windows 发布者签名。

本工具与 OpenAI、Anthropic 或 Apple 无隶属关系。
