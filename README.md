# 造作画布（ZZHB AI Canvas）

造作画布是一款面向 AI 图片、视频和音频工作流的 Windows 本地可视化画布。

**[直接下载造作画布 v0.5.2](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/download/v0.5.2/ZZHB-0.5.1-win-x64.zip)** · [画布使用手册](https://acaiy.cn/article/canvas-guide/) · [查看 v0.5.2 发布说明](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/tag/v0.5.2) · [全部历史版本](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases)

你可以在同一个项目里整理参考图、提示词、音频、视频、模型结果和设计说明，再把它们连接成可持续修改的工作流程。本仓库只用于发布 Windows 成品和公开使用说明，不提供商业产品源码。

<img width="1709" height="799" alt="造作画布项目界面" src="https://github.com/user-attachments/assets/f179aed0-7a0c-44c8-81fb-35bda2fe947b" />

<img width="1718" height="815" alt="造作画布节点与模型配置" src="https://github.com/user-attachments/assets/c7eeac40-cc13-4b90-9e60-c885bb0792de" />

<img width="1718" height="815" alt="造作画布工作流界面" src="https://github.com/user-attachments/assets/07815762-94f0-46b3-b6cc-fc62d322f36e" />

欢迎加入画布交流群
<img width="405" height="403" alt="PixPin_2026-09-16_20-25-57" src="https://github.com/user-attachments/assets/6de8c40f-a8fc-47d6-ba4a-0beb4b9dd3b3" />


## 下载与安装

1. 下载 [`ZZHB-0.5.1-win-x64.zip`](https://github.com/yangwc18181/zaozuohuabu-windows-preview/releases/download/v0.5.2/ZZHB-0.5.1-win-x64.zip)。
2. 将 ZIP **完整解压**到普通文件夹，不要直接在压缩包内运行。
3. 双击 `ZZHB\ZZHB.exe`，等待本地服务启动并自动打开 Windows 默认浏览器。
4. 使用期间保持程序运行；关闭程序会同时停止本地服务。

当前程序尚未代码签名，Windows 可能提示“未知发布者”。请确认文件来自本仓库，并使用下方 SHA-256 核对下载内容。

## 第一次使用

- Windows 完整包已经内置 Codex CLI，不需要另外安装；Codex 模型配置、Agent 使用方法、Notes 续写与补全、Midjourney 预设等详细步骤统一查看[造作画布使用手册](https://acaiy.cn/article/canvas-guide/)。
- 打开“模型与供应商”，按需填写官方或第三方服务的 API Key；发布包内置的连接模板不包含任何 Key。也可以连接自己的 ComfyUI。
- 模型调用可能产生费用，网络、价格、额度、隐私政策和模型可用性由所选服务决定，请先从少量测试开始。
- 不要公开分享 API Key，也不要在 Issue 中粘贴 Key、客户资料、私人项目、未脱敏截图或完整日志。
- ComfyUI 工作流需要你自行安装并启动对应的本机或云端 ComfyUI 服务，再填写可访问的 Base URL。

## v0.5.2 主要更新

这一版在现有完整工作空间基础上，补充图片编辑、全景查看和生成节点交互，并同步新用户默认模型清单：

- **图片标注与蒙版**：图片标注栏支持蒙版绘制、擦除、反选、撤销、重做、保存和导出；普通标注与蒙版相互独立。
- **可编辑曲线箭头**：箭头支持拖动控制点，并可增加或减少控制点。
- **360° 全景节点**：可以在画布内查看全景图片、拖动视角、滚轮缩放和全屏浏览。
- **GPT Image 2.5**：Sunburst / Flare 的 Images 通道增加蒙版编辑和透明背景选项；相关预设均保留最多 16 张输入图能力。
- **生成节点体验**：图片质量显示改为简短标签，失败任务提供重试图标。
- **模型配置同步**：全新数据目录默认提供 47 条无 Key 连接，TK、LK、AM 按固定顺序显示，MiniMax 官方位于“官方来源”；TK Base URL 为 `https://store.forcepic.com/`。已有用户配置不会因升级被清理或覆盖。
- **Codex CLI 随包提供**：内置 OpenAI 官方 Windows x64 Codex CLI `0.153.4`，无需另行安装；登录和个人配置仍归当前 Windows 用户所有。
- **Notes 与 Midjourney**：Notes 继续支持手动续写和自动补全；Midjourney 继续支持提示词/参数分开复用、跨项目生成预设和全局默认设置。

## 下载校验
| 项目 | 内容 |
| --- | --- |
| 文件名 | `ZZHB-0.5.1-win-x64.zip` |
| 文件大小 | 225,728,239 bytes |
| SHA-256 | `f87777867667160ab2339038beac4a3d3f8b655c82e38b27fe6ae83b25ac88ba` |

## 已知边界

程序当前尚未代码签名，Windows 可能提示“未知发布者”。Agent 虽已内置 Codex CLI，但不会携带登录信息、Skills、MCP、API Key 或 Token；未登录时不影响画布其它功能。具体模型、付费路径、联网能力和自定义 ComfyUI 节点仍取决于用户自己的账号、服务、网络和节点定义。本说明不表示所有真实付费渠道、所有公网素材服务或所有自定义节点组合都已经完成验证。

## 使用范围

允许个人学习、研究、试用和课程内容制作。未经授权，不允许转售、改名分发、重新打包，或将本程序作为 SaaS、托管服务或付费产品再次发布。


## 反馈

欢迎通过 [GitHub Issues](https://github.com/yangwc18181/zaozuohuabu-windows-preview/issues) 反馈启动失败、模型配置、生成失败、画布交互或功能建议。请尽量提供 Windows 版本、软件版本、操作步骤和脱敏后的错误信息。
