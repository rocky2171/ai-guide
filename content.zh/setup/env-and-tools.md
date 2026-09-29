---
aliases:
  - /ai-programming/env-and-tools/
title: 环境配置：工具与增强
weight: 20
bookToc: false
noTocArea: true
bookHidden: false
---

## 🛠️ AI 编程环境配置与增强工具集

本合集汇整 Claude Code、Codex、Gemini CLI 的增强工具，按用途分为桌面（配置·账号 / 工作区 / 周边）、路由代理、终端增强、配置与插件。表格按收录时大致 star 数降序（快照，非实时）；🔥 为站内有专页的推荐项。解读列：有 Zread 用 Zread，否则 GitHub / 官网。

环境变量与基础栈见 [开发环境准备]({{< relref "setup/dev-start" >}})；供应商 / MCP 可视化深读见 [CC Switch]({{< relref "setup/cc-switch" >}})、[ZCF]({{< relref "setup/zcf" >}})、[CPA]({{< relref "setup/cpa" >}})。

**怎么选（按任务）**

- 换供应商 / 管 MCP·Skills → [CC Switch]({{< relref "setup/cc-switch" >}}) 或 CLI 版 `cc-switch-cli`；一键初始化看 [ZCF]({{< relref "setup/zcf" >}})
- 多账号 / 配额监控 → Cockpit Tools、quotio、Antigravity Manager
- 订阅转兼容 API / 多模型路由 → [CPA]({{< relref "setup/cpa" >}})、Sub2API、Claude Code Router
- 多 Agent 并行工作区 → Orca、OpenChamber、Nezha、Desktop CC GUI、CLI-Manager
- 终端里写代码 / 状态栏 → Pi、oh-my-pi、Warp、Pebrel、Claude HUD
- 团队共享 Skills / Rules / MCP → TeamAI
- Windows 一键装环境 → Claude Code Quickstart (CCQ)
- 远程盯会话 → hapi；任务完成提醒 → AI CLI Complete Notify

### 桌面：配置 · 账号 · 配额

切供应商、管 MCP/Skills、多账号与配额；不是完整 IDE。

|工具名称|star 数|项目介绍|解读|
|---|---|---|---|
|[🔥CC Switch]({{< relref "setup/cc-switch" >}})|135k|Claude Code / Codex / Gemini CLI 跨平台桌面辅助：一键切换 API 供应商；统一管理 MCP；Skills 扫描与 Prompts 预设；内置 API 测速（Tauri2+React+Rust）|[Zread](https://zread.ai/farion1231/cc-switch)|
|[Antigravity Manager](https://github.com/lbjlaq/Antigravity-Manager)|32k|Antigravity 多账号管理与切换，偏账号/配额运维|[Zread](https://zread.ai/lbjlaq/Antigravity-Manager)|
|[🔥Cockpit Tools](https://github.com/jlcodes99/cockpit-tools)|18k|通用 AI IDE 账号管理：Antigravity/Codex/Copilot/Windsurf/Kiro 多账号切换、配额监控、自动唤醒与多开|[Zread](https://zread.ai/jlcodes99/cockpit-tools)|
|[Skills Manager](https://github.com/xingkongliang/skills-manager)|4.9k|跨 50+ Agent 的 Skills 桌面管理：中央库安装/同步、Preset，同步到 Claude Code / Codex / Cursor 等|[GitHub](https://github.com/xingkongliang/skills-manager)|
|[quotio](https://github.com/nguyenphutrong/quotio)|4.9k|macOS 菜单栏多账号 AI 配额追踪（仅 macOS）|[Zread](https://zread.ai/nguyenphutrong/quotio)|
|[Codex-X](https://github.com/yynxxxxx/Codex-X)|3.9k|OpenAI Codex 桌面/CLI 可视化：提示词模板、Provider 切换（可从 cc-switch 导入）、会话与 Skills/MCP|[GitHub](https://github.com/yynxxxxx/Codex-X)|
|[claude-code-hub](https://github.com/ding113/claude-code-hub)|3.4k|Claude Code 配置/会话/常用工具的统一入口|[Zread](https://zread.ai/ding113/claude-code-hub)|
|[AI Toolbox](https://github.com/coulsontl/ai-toolbox)|1.7k|个人工具箱：OpenCode / Claude Code / Codex 供应商切换、MCP、Skills；支持 WSL 同步与备份|[Zread](https://zread.ai/coulsontl/ai-toolbox)|
|[AiMaMi](https://github.com/borawong/AiMaMi)|1.5k|Codex 本地桌面伴侣：账号/配额、路由中转、会话清理、MCP/Skills；读写 `~/.codex`|[GitHub](https://github.com/borawong/AiMaMi)|
|[Pi Switch](https://github.com/Wing900/Pi-switch)|0.1k|[Pi](https://github.com/earendil-works/pi) 的 Provider/模型配置工具（Wails）：多 Provider、Anthropic 原生协议适配、一键启动|[GitHub](https://github.com/Wing900/Pi-switch)|

### 桌面：多 Agent 工作区

在同一界面跑 Agent、编辑、预览与会话编排。

|工具名称|star 数|项目介绍|解读|
|---|---|---|---|
|[Orca](https://www.onorca.dev/)|76k|面向 AI Coding Agent 的 ADE（YC）：隔离 git worktree 并行跑 Claude Code / Codex / OpenCode；WebGL 终端、内置编辑器、SSH 远程 worktree、diff 批注回传；MIT，跨平台|[GitHub](https://github.com/stablyai/orca)|
|[AionUi](https://github.com/iOfficeAI/AionUi)|33k|跨平台 AI 编程桌面客户端：CoWork 协作、多引擎集成|[Zread](https://zread.ai/iOfficeAI/AionUi)|
|[happy](https://github.com/slopus/happy)|24k|Claude Code / Codex 端到端加密客户端，覆盖桌面、移动与 Web|[Zread](https://zread.ai/slopus/happy)|
|[OpenChamber](https://openchamber.dev/zh/)|10k|基于 OpenCode 的开源智能体开发环境：桌面 / PWA / VS Code / 移动端；Session Goals、多模型 Multi-run、Issue→PR、Private Relay|[GitHub](https://github.com/openchamber/openchamber)|
|[Terax](https://github.com/crynta/terax-ai)|9.2k|约 7MB 的 Terminal-first 工作区（Tauri2）：WebGL 多标签终端、Agent 侧栏、CodeMirror、Git 图谱；无遥测|[Zread](https://zread.ai/crynta/terax-ai)|
|[PI-Desktop](https://github.com/vastsa/pi-desktop)|5.3k|基于 [Pi](https://github.com/earendil-works/pi) 的 Local-first 桌面工作区：Agent/Plan/Goal、Subagent 编排、插件市场；可导入多端会话|[GitHub](https://github.com/vastsa/pi-desktop)|
|[Octop](https://github.com/TencentCloud/Octop)|4.7k|腾讯云开源自托管多用户多 Agent：Web/CLI/桌面；IM 通道；ACP 对接 OpenCode / Claude Code / Codex|[GitHub](https://github.com/TencentCloud/Octop)|
|[Desktop CC GUI](https://github.com/zhukunpenglinyutong/desktop-cc-gui)|4.3k|开源 VibeCoding 桌面端：Claude Code / Codex / OpenCode；终端、Git、看板、MCP/Skills、多 Agent 并行|[Zread](https://zread.ai/zhukunpenglinyutong/desktop-cc-gui)|
|[codeg](https://github.com/xintaofei/codeg)|3.7k|聚合 Claude Code / Codex / Gemini CLI 等会话的工作台；桌面或自托管 Docker|[GitHub](https://github.com/xintaofei/codeg)|
|[LiveAgent](https://github.com/Stack-Cairn/LiveAgent)|2.2k|Local-first Agent 桌面端：多模型路由、子 Agent/worktree、MCP/Skills、可选 Gateway WebUI|[Zread](https://zread.ai/Stack-Cairn/LiveAgent)|
|[Nezha](https://github.com/hanshuaikang/nezha)|1.9k|Agent-First 桌面 IDE：并行多 Claude Code / Codex；会话回放、轻量编辑器、Token 统计（约 7MB）|[Zread](https://zread.ai/hanshuaikang/nezha)|
|[Any Code](https://github.com/anyme123/Any-code)|1.3k|多引擎 AI 代码助手 GUI：Claude Code / Codex / Gemini CLI 切换；成本追踪、MCP、Hooks|[Zread](https://zread.ai/anyme123/Any-code)|
|[CLI-Manager](https://github.com/dark-hxx/CLI-Manager)|0.8k|跨平台 AI CLI 工作台（Tauri）：本地/SSH 终端、多项目与 Worktree、Claude Code/Codex 深度集成（Hook 通知、会话 Diff、用量看板）；cc-switch 项目级供应商切换；Telegram/飞书手机对话|[GitHub](https://github.com/dark-hxx/CLI-Manager)|
|[OpenCow](https://github.com/OpenCowAI/opencow)|0.4k|任务驱动自治 Agent 平台：每任务一 Agent，并行交付；桌面端 + 本地 MCP|[GitHub](https://github.com/OpenCowAI/opencow)|
|[ZCode](https://zcode.z.ai/cn)|—|智谱 GLM 官方氛围编程桌面端：多智能体、Goal 长程任务、IM Bot 远程唤起|[BigModel](https://www.bigmodel.cn/glm-coding)|
|[Alma](https://alma.now/)|—|AI Provider 编排桌面端：多厂 API 切换、聊天、记忆与工具调用；主测 macOS Apple Silicon|[官网](https://alma.now/)|

### 桌面：周边（通知 · 远程 · 网关 GUI · 创作）

不单独成「工作区」，但常与上两类搭配。

|工具名称|star 数|项目介绍|解读|
|---|---|---|---|
|[hapi](https://github.com/tiann/hapi)|5.1k|Web / Telegram 远程 AI 编程控制台|[Zread](https://zread.ai/tiann/hapi)|
|[ProxyCast](https://github.com/aiclientproxy/proxycast)|1.5k|创作者向 Agent 工作台（写作/出图/改稿）；非纯 Coding IDE|[Zread](https://zread.ai/aiclientproxy/proxycast)|
|[aio-coding-hub](https://github.com/dyndynjyxa/aio-coding-hub)|0.7k|本地 AI CLI 统一网关桌面端：多 CLI 入口、可视化监控与路由|[Zread](https://zread.ai/dyndynjyxa/aio-coding-hub)|
|[AI CLI Complete Notify](https://github.com/ZekerTop/ai-cli-complete-notify)|0.4k|多通道任务完成提醒（桌面+CLI）：飞书/钉钉/企微/Telegram/邮件|[GitHub](https://github.com/ZekerTop/ai-cli-complete-notify)|
|[ccg-gateway](https://github.com/mos1128/ccg-gateway)|0.2k|Claude Code / Codex / Gemini 三合一代理网关桌面端|[Zread](https://zread.ai/mos1128/ccg-gateway)|

### 路由代理与 API 网关

把 CLI / 订阅转成兼容 API，或做多模型路由、负载均衡与拼车中转。远程控制台见上方「桌面：周边」中的 hapi。

|工具名称|star 数|项目介绍|解读|
|---|---|---|---|
|[🔥CLIProxyAPI (CPA)]({{< relref "setup/cpa" >}})|53k|将多种 CLI 封装为 OpenAI/Gemini/Claude/Codex 兼容 API：多账户轮询与故障转移；流式/非流式、多模态、函数调用|[Zread](https://zread.ai/router-for-me/CLIProxyAPI)|
|[Sub2API](https://github.com/Wei-Shaw/sub2api)|42k|开源 API 网关：Claude / OpenAI / Gemini / Antigravity 等订阅转兼容 API；Key 分发、计费、调度、限流与拼车|[Zread](https://zread.ai/Wei-Shaw/sub2api)|
|[🔥Claude Code Router](https://github.com/musistudio/claude-code-router)|37k|Claude Code 请求路由到任意模型；自定义分发逻辑；无需 Anthropic 账号；支持 DeepSeek/Gemini/Groq 等|[Zread](https://zread.ai/musistudio/claude-code-router)|
|[claude-relay-service (crs)](https://github.com/Wei-Shaw/claude-relay-service)|13k|Claude Code 镜像中转与拼车，多用户共享转发|[Zread](https://zread.ai/Wei-Shaw/claude-relay-service)|
|[gpt-load](https://github.com/tbphp/gpt-load)|7.0k|多通道 API Key 轮询与负载均衡，自动容错|[Zread](https://zread.ai/tbphp/gpt-load)|
|[axonhub](https://github.com/looplj/axonhub)|5.3k|AI 流量网关 + RBAC / 多租户权限|[Zread](https://zread.ai/looplj/axonhub)|
|[ccx](https://github.com/BenedictKing/ccx)|4.0k|个人向极简 API 网关，快速配置、轻量使用|[Zread](https://zread.ai/BenedictKing/ccx)|
|[metapi](https://github.com/cita-777/metapi)|3.3k|聚合 New API / One API / Sub2API 等中转站为单一入口与密钥|[Zread](https://zread.ai/cita-777/metapi)|
|[octopus](https://github.com/bestruirui/octopus)|2.6k|个人向 LLM API 聚合与负载均衡；OpenAI ↔ Anthropic 协议转换|[Zread](https://zread.ai/bestruirui/octopus)|
|[Aether](https://github.com/fawney19/Aether)|1.5k|多租户 AI 基础设施网关：Claude / OpenAI / Gemini 及 CLI 统一接入|[Zread](https://zread.ai/fawney19/Aether)|
|[ccNexus](https://github.com/lich0821/ccNexus)|1.0k|Claude Code 端点轮换代理：故障转移；兼容 OpenAI / Gemini 格式|[Zread](https://zread.ai/lich0821/ccNexus)|

### 终端增强与 CLI Agent

AI 原生终端、Coding Agent Harness，以及终端内状态栏 / 多 Agent 协作。

|工具名称|star 数|项目介绍|解读|
|---|---|---|---|
|[🔥Pi](https://github.com/earendil-works/pi)|109k|可自扩展的极简终端 Coding Agent：多厂商 LLM、工具运行时、差分 TUI；用 Extensions/Skills 扩展而非 fork 内核|[Zread](https://zread.ai/earendil-works/pi)|
|[Warp](https://github.com/warpdotdev/warp)|65k|AI 原生终端：命令补全、命令块、工作流与团队协作|[Zread](https://zread.ai/warpdotdev/warp)|
|[DeepSeek-Reasonix](https://github.com/esengine/DeepSeek-Reasonix)|36k|DeepSeek 原生终端 Agent（[reasonix.io](https://reasonix.io/)）：prefix-cache 友好、长时自主；终端/桌面/浏览器/ACP；`reasonix.toml` 驱动 MCP/Plan/沙箱|[GitHub](https://github.com/esengine/DeepSeek-Reasonix)|
|[oh-my-pi (omp)](https://github.com/can1357/oh-my-pi)|33k|[Pi](https://github.com/earendil-works/pi) fork（[omp.sh](https://omp.sh)）：内置 LSP/DAP、子 Agent、Hashline 编辑；Rust 核心；跨平台|[GitHub](https://github.com/can1357/oh-my-pi)|
|[Claude HUD](https://github.com/jarrodwatts/claude-hud)|28k|Claude Code statusline HUD：上下文占用、工具/Agent/Todo、可选 Git 与用量|[Zread](https://zread.ai/jarrodwatts/claude-hud)|
|[cmux](https://cmux.com/zh-CN)|27k|基于 libghostty 的原生 macOS 终端：垂直标签、Agent 通知环、分屏、可编程浏览器；适合 CLI Agent|[GitHub](https://github.com/manaflow-ai/cmux)|
|[jcode](https://github.com/1jehuang/jcode)|20k|轻量命令行开发辅助，作 Claude Code 周边补充|[Zread](https://zread.ai/1jehuang/jcode)|
|[Kaku](https://github.com/tw93/Kaku)|6.0k|WezTerm 深度定制终端（仅 macOS）：零配置、内置 AI 助手与 lazygit/yazi；可接 Claude Code / Codex / Gemini CLI|[GitHub](https://github.com/tw93/Kaku)|
|[claude_code_bridge (ccb)](https://github.com/bfly123/claude_code_bridge)|3.5k|分屏终端联动 Claude / Codex / Gemini / OpenCode；Windows 用 WezTerm，Linux/macOS/WSL 用 tmux|[Zread](https://zread.ai/bfly123/claude_code_bridge)|
|[CCometixLine](https://github.com/Haleclipse/CCometixLine)|3.5k|Rust 写的 Claude Code 状态栏与 TUI：Git、用量、交互配置|[Zread](https://zread.ai/Haleclipse/CCometixLine)|
|[Pebrel](https://github.com/Kuddev/pebrel)|2.6k|GPU 加速 AI 原生终端（Rust+GPUI，原 Nebula）：分屏/标签、SSH/SFTP、会话常驻；Claude Code / Codex 等 CLI 活动态与 Markdown 阅读器；Win 稳定，macOS/Linux Preview|[GitHub](https://github.com/Kuddev/pebrel)|
|[Otty](https://otty.sh/)|—|GPU 加速终端：CLI Agent 并行监控、Prompt 队列、会话分叉与 Web 预览；当前 macOS Apple Silicon|[官网](https://otty.sh/)|

### 配置脚本与编辑器插件

一键环境初始化、CLI 配置切换，以及 IDE / Web 侧辅助工具。

|工具名称|star 数|项目介绍|解读|
|---|---|---|---|
|[paseo.sh](https://github.com/getpaseo/paseo)|18k|Claude Code 相关在线能力与资源入口|[Zread](https://zread.ai/getpaseo/paseo)|
|[IDEA Claude Code GUI Plugin](https://github.com/zhukunpenglinyutong/idea-claude-code-gui)|6.5k|IntelliJ 插件：Claude Code / Codex 可视化；@file、DIFF、MCP/Skills、权限控制|[Zread](https://zread.ai/zhukunpenglinyutong/idea-claude-code-gui)|
|[🔥ZCF (Zero Config)]({{< relref "setup/zcf" >}})|6.1k|零配置一键搞定 Claude Code & Codex：中英双语、智能代理、个性化助手|[Zread](https://zread.ai/UfoMiao/zcf)|
|[cc-switch-cli](https://github.com/SaladDay/cc-switch-cli)|5.2k|cc-switch 的 CLI 版：无 GUI 环境下切换全局配置、MCP 与提示词|[Zread](https://zread.ai/SaladDay/cc-switch-cli)|
|[TeamAI](https://github.com/Tencent/teamai-cli)|5.0k|腾讯开源团队 AI Native 底座：Git 共享 Skills / Rules / MCP / Agents；`teamai init` 同步；覆盖 Claude Code / Codex / Cursor / CodeBuddy|[GitHub](https://github.com/Tencent/teamai-cli)|
|[GPTSession2CPAandSub2API](https://github.com/gtxx3600/GPTSession2CPAandSub2API)|1.8k|纯前端：ChatGPT Web session → CPA / Sub2API 等可导入 JSON；本地解析不上传 token|[GitHub](https://github.com/gtxx3600/GPTSession2CPAandSub2API)|
|[Claudix](https://github.com/Haleclipse/Claudix)|1.1k|VS Code 的 Claude Code 增强扩展|[GitHub](https://github.com/Haleclipse/Claudix)|
|[Claude Code Quickstart (CCQ)](https://github.com/MrNine-666/claude-code-quickstart)|0.2k|Windows PowerShell 一键安装器：依赖、供应商与 MCP 初始化|[Zread](https://zread.ai/MrNine-666/claude-code-quickstart)|
