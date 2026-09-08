# 造作画布（ZZHB AI Canvas）

造作画布是一款面向 AI 图片、视频和音频工作流的 Windows 本地可视化画布。

**[直接下载造作画布 v0.5.0](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/download/v0.5.0/ZZHB-0.5.0-win-x64.zip)** · [画布使用手册](https://acaiy.cn/article/canvas-guide/) · [查看 v0.5.0 发布说明](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/tag/v0.5.0) · [全部历史版本](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases)

你可以在同一个项目里整理参考图、提示词、音频、视频、模型结果和设计说明，再把它们连接成可持续修改的工作流程。本仓库只用于发布 Windows 成品和公开使用说明，不提供商业产品源码。

<img width="1709" height="799" alt="造作画布项目界面" src="https://github.com/user-attachments/assets/f179aed0-7a0c-44c8-81fb-35bda2fe947b" />

<img width="1718" height="815" alt="造作画布节点与模型配置" src="https://github.com/user-attachments/assets/c7eeac40-cc13-4b90-9e60-c885bb0792de" />

<img width="1718" height="815" alt="造作画布工作流界面" src="https://github.com/user-attachments/assets/07815762-94f0-46b3-b6cc-fc62d322f36e" />

欢迎加入 画布交流群！反馈问题、交流使用体验或提出新功能建议。

<img width="400" height="400" alt="PixPin_2026-08-29_09-06-45" src="https://github.com/user-attachments/assets/afa78df7-6500-440a-874e-6446fdfa7f43" />




## 下载与安装

1. 下载 [`ZZHB-0.5.0-win-x64.zip`](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/download/v0.5.0/ZZHB-0.5.0-win-x64.zip)。
2. 将 ZIP **完整解压**到普通文件夹，不要直接在压缩包内运行。
3. 双击 `ZZHB\ZZHB.exe`，等待本地服务启动并自动打开 Windows 默认浏览器。
4. 使用期间保持程序运行；关闭程序会同时停止本地服务。

当前程序尚未代码签名，Windows 可能提示“未知发布者”。请确认文件来自本仓库，并使用下方 SHA-256 核对下载内容。

## 第一次使用

- 打开“模型与供应商”，按需填写官方或第三方服务的 API Key；发布包内置的连接模板不包含任何 Key。也可以连接自己的 ComfyUI。
- Agent 已内置固定版本的 OpenAI 官方 Codex CLI，不需要另行安装；第一次使用仍需按提示完成当前 Windows 用户的 Codex 登录。
- 模型调用可能产生费用，网络、价格、额度、隐私政策和模型可用性由所选服务决定，请先从少量测试开始。
- 不要公开分享 API Key，也不要在 Issue 中粘贴 Key、客户资料、私人项目、未脱敏截图或完整日志。
- ComfyUI 工作流需要你自行安装并启动对应的本机或云端 ComfyUI 服务，再填写可访问的 Base URL。

## v0.5.0 主要更新

这一版把画布、项目、Agent、笔记和情绪板整合成更完整的本地工作空间：

- **项目文件更可控**：新项目保存到你选择的普通文件夹；首页可重新关联项目目录，并区分项目备份导入与画布模板导入。
- **项目 Agent 正式整合**：Agent 可以结合当前项目、画布选中内容和项目文件继续工作，支持对话历史、续聊、分叉、停止、审批和结果回到画布。
- **Codex CLI 随包提供**：内置 OpenAI 官方 Windows x64 Codex CLI `0.153.4`，解压后无需再单独安装 CLI；登录和个人配置仍归当前 Windows 用户所有。
- **独立项目笔记**：Notes 可在项目内持续记录文字、清单和结构化内容，并与 Agent、画布共享同一项目上下文。
- **情绪板能力扩展**：栏目、内容板、本地图片、文档、表格和专属连线已进入整合版，便于把灵感资料与制作任务放在同一画布。
- **模板与备份更清楚**：首页提供三份官方模板；模板用于复用画布结构，项目备份用于迁移完整项目，两类入口和反馈不再混淆。
- **模型配置更新**：发布包提供 53 条无 Key 连接，TK、LK、AM 按固定顺序显示；三家均加入 GPT-6、Gemini 3.8 Flash、Gemini 3.7 Flash，MiniMax 官方独立归入“官方来源”。

## 下载校验

| 项目 | 内容 |
| --- | --- |
| 文件名 | `ZZHB-0.5.0-win-x64.zip` |
| 文件大小 | 225,571,345 bytes |
| SHA-256 | `d5b43016e4abf9d9d96f4cd5435d67dd160018e43c94da2e6b5eddda0ad30ae2` |

## 已知边界

程序当前尚未代码签名，Windows 可能提示“未知发布者”。Agent 虽已内置 Codex CLI，但不会携带登录信息、Skills、MCP、API Key 或 Token；未登录时不影响画布其它功能。具体模型、付费路径、联网能力和自定义 ComfyUI 节点仍取决于用户自己的账号、服务、网络和节点定义。本说明不表示所有真实付费渠道、所有公网素材服务或所有自定义节点组合都已经完成验证。

## 使用范围

允许个人学习、研究、试用和课程内容制作。未经授权，不允许转售、改名分发、重新打包，或将本程序作为 SaaS、托管服务或付费产品再次发布。


## 反馈

欢迎通过 [GitHub Issues](https://github.com/yangwc18181/zaozuohuabu-windows-preview/issues) 反馈启动失败、模型配置、生成失败、画布交互或功能建议。请尽量提供 Windows 版本、软件版本、操作步骤和脱敏后的错误信息。
