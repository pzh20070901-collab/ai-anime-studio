# AI Anime Studio

线上前端＋Windows 本机后端，无需安装 Codex。当前为私人仓库的预览版。

- [线上工作台](https://anime-studio-local-workbench.pzh20070901.chatgpt.site)
- [下载预览版与完整源码快照](https://github.com/pzh20070901-collab/ai-anime-studio/releases)

## 使用

1. 下载 `AI-Anime-Studio-Windows.zip`，完整解压到可写目录，双击 `启动工作台.cmd`。
2. 打开线上工作台，再打开本机配对页，核对网站域名并输入一次性码。
3. Windows 同一设备、同一浏览器首次配置后长期记住；关闭网页、重启后端可恢复。清除网站数据、更换浏览器/Windows用户或手动撤销后需重新配对。
4. 配置自己的 API。MJ、豆包另需 Ego Lite、自己的登录账号与任务空间设置。包内没有作者的账号或个人数据。

后端仅监听 127.0.0.1:8791。设备授权与 API 密钥在本机用 Windows DPAPI 加密；网页只保存自己的设备连接令牌。不要配对不可信的网站。电脑与本机后端需要保持运行。

## 文件

Release 中的 `ai-anime-studio-source.zip` 是完整可审查源码快照，包含 `workbench` 后端、`vendor/infinite-canvas/web` 前端源码、依赖锁定文件与构建产物。它是源码快照包，不是只有 README 的自动生成 GitHub Source code 包。Windows ZIP 另包含独立 Python 运行环境。

不包含 state 数据库、密钥、微信聊天、任务日志、个人知识库、私人 Skill、浏览器资料或登录状态。GitHub 仓库和网站均暂未开放给所有人。

## 验证边界

后端测试与类型/构建检查、真实 HTTPS 网页到本机的项目/图片/成果读取已验证。同机全新解压目录运行通过；第二台干净 Windows 设备尚未验收，不宣称所有浏览器兼容。当前模型 Agent 工具限项目/Skill读取、知识检索、Markdown保存，不是无限制电脑控制。

## 开源来源

画布基于 [basketikun/infinite-canvas](https://github.com/basketikun/infinite-canvas)，MIT。源码包保留上游 LICENSE，Windows 包内为 THIRD-PARTY-LICENSE.txt；Python及随附库的许可证保留在各自运行时目录。当前仓库未额外授予自有代码开源许可证。
