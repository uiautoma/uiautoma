# UIAutoma

面向 Windows 的桌面与网页自动化工具。

通过 App 捕获和管理元素，使用 Python SDK 编写可重复运行的脚本；也可以让 AI Agent
通过 UIAutoma CLI 和 SDK 完成观察、元素捕获与自动化操作。

本仓库用于提供 UIAutoma 安装包、版本说明和公开使用信息。

## 下载与安装

前往 [Releases](https://github.com/uiautoma/uiautoma/releases) 查看已发布版本。
如果列表为空，表示尚无公开安装包。

1. 下载所需版本的 `UIAutoma-Setup-<version>-x64.exe`。
2. 运行 Setup，按提示完成安装。可按需选择安装浏览器插件和 Skills，也可以稍后在 App 的插件页面安装。
3. 打开 UIAutoma App。自动化时请保持 App 运行。

每个 Setup Release 提供 `SHA256SUMS`，可用于核对下载文件的 SHA-256。
安装包的签名状态以对应版本说明为准。

## 使用要求

- Windows 10/11 x64；安装 Setup 需要管理员权限。
- 网页自动化需要在目标 Chrome 或 Edge 中启用 UIAutoma 扩展。
- 自动化命令或脚本与 App 在同一台 Windows 计算机、同一登录会话中运行。
- 使用自己的 Python 环境运行 SDK 脚本时，需要 Python 3.10 及以上版本。

## 使用 AI Agent（推荐）

1. 在 App 的插件页面切换到 **Skills**，为使用的 Agent 安装 Skills。
2. 安装后开启新的 Agent 会话，使用 UIAutoma CLI 观察应用或网页、捕获目标并执行操作。
3. 需要重复运行的任务，可让 Agent 使用 SDK 编写 Python 脚本。

支持的 Skills 安装目标包括 **Codex、Claude Code、WorkBuddy 和 DeepSeek Harness**。
安装后可重新打开终端，让 `uia` 命令的环境配置生效。

## 使用 App 与 Python SDK

1. 在 App 中创建或打开元素库，捕获并验证目标元素。
2. 在自己的 Python 环境中使用 UIAutoma SDK，读取元素库并编写自动化脚本。
3. 网页自动化可连接已打开的 Chrome 或 Edge，操作现有标签页或新建标签页。

SDK 单独发布，安装方式以对应 SDK 发行说明为准。
App 与 SDK 独立编号，不要求版本号相同；安装或更新 App 不会自动更新用户 Python 环境中的 SDK。

## 许可

UIAutoma Python SDK 采用 MIT 许可。该许可不覆盖 App 及其他产品组件；
第三方组件适用各自的许可。
