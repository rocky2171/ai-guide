---
title: AI 编程工具：汇总与对比
weight: 20
bookHidden: false
bookToc: false
noTocArea: true
---

# AI 编程工具：汇总与对比


> BYOK = Bring Your Own Key（自带模型 API Key）。

## 工具对照表

| 工具 | 类型 | BYOK | 开源 | 规模参考 | 一句话定位 | 定价 |
|---|---|---|---|---|---|---|
| [Claude Code](https://claude.com/product/claude-code) | CLI / IDE / 桌面 / Web | 有限（Anthropic / Bedrock 等） | 闭源 | VS Code 约 1150 万安装 | Anthropic 代理式编码：整库读写、MCP、子代理、钩子 | [定价](https://claude.com/pricing) · Pro $20/月起 |
| [Codex](https://developers.openai.com/codex) | CLI / IDE / 桌面 / 云 | 有限（OpenAI） | Apache-2.0（CLI） | GitHub 约 12.7 万★ · VS Code 约 760 万安装 | OpenAI 编码代理；优先 ChatGPT 原生登录控成本 | [定价](https://developers.openai.com/codex/pricing) · Plus $20/月起 |
| [Cursor](https://cursor.com/) | 独立 IDE / CLI / 云 | ✅ | 闭源（VS Code fork） | — | Agent + Tab + 云代理；规则 / MCP / Bugbot 偏团队 | [定价](https://cursor.com/pricing) · Pro $20/月起 |
| [GitHub Copilot](https://github.com/features/copilot) | IDE / CLI / 平台 | ✅（多模型） | 闭源 | VS Code 约 7300 万安装 | 补全 + Chat + Agent；与 GitHub 工作流绑定最深 | [定价](https://github.com/features/copilot/plans) · Pro $10/月起 |
| [Devin](https://devin.ai/desktop) | 独立 IDE / 桌面 | ✅（部分） | 闭源 | 官网约 100 万用户 | Cognition 多智能体指挥台（原 Windsurf）：本地/云 Agent + IDE | [定价](https://devin.ai/desktop) · Pro $20/月起 |
| [Cline](https://github.com/cline/cline) | IDE 扩展 / CLI | ✅ | Apache-2.0 | GitHub 约 6.9 万★ · VS Code 约 370 万安装 | 开源 IDE 内代理；人工确认后改文件 / 跑命令 / MCP | [仓库](https://github.com/cline/cline) · 免费 BYOK |
| [OpenCode](https://opencode.ai/) | CLI / 桌面 / IDE | ✅ | MIT | GitHub 约 21.0 万★ | 模型无关开源代理；终端 + 桌面 + 扩展一体 | [官网](https://opencode.ai/) · 免费 BYOK / Zen 充值 |
| [Gemini CLI](https://github.com/google-gemini/gemini-cli) | CLI | 有限（Google） | Apache-2.0 | GitHub 约 10.7 万★ | 终端里的 Gemini：大上下文、Search、MCP | [配额说明](https://github.com/google-gemini/gemini-cli/blob/main/docs/resources/quota-and-pricing.md) · 免费档可用 |
| [Gemini Code Assist](https://codeassist.google/) | IDE 扩展 | 有限（Google） | 闭源 | VS Code 约 390 万安装 | Google 云 / IDE 侧编程助手；企业配额与治理 | [商业定价](https://codeassist.google/products/business) · 个人免费 |
| [Google Antigravity](https://antigravity.google/) | 独立 IDE / 桌面 | ❌ | 闭源 | — | 多智能体并行开发平台；编辑器 + 管理视图 | [定价](https://antigravity.google/pricing) · 个人免费 / AI Pro 起 |
| [Kiro](https://kiro.dev/) | 独立 IDE / CLI | ❌ | 闭源 | — | 规格驱动 + 钩子 / Powers；默认托管模型路由 | [定价](https://kiro.dev/pricing/) · Pro $20/月起 |
| [Trae](https://www.trae.ai/) | 独立 IDE / CLI | ✅ | 部分（CLI MIT） | CLI 约 1.2 万★ | 字节跳动 AI IDE；SOLO/Builder + 开源 Trae Agent | [定价](https://www.trae.ai/pricing) · 免费档 / Pro $10/月起 |
| [通义灵码](https://lingma.aliyun.com/) | 独立 IDE / 插件 | 有限（阿里云） | 闭源 | VS Code 约 240 万安装 | 阿里云智能编码；企业知识库与私有化 | [定价](https://lingma.aliyun.com/pricing) · 个人基础免费 |
| [CodeBuddy](https://www.codebuddy.ai/) | IDE / CLI | 有限（混元等） | 闭源 | VS Code 约 45 万安装 | 腾讯云编码助手；Craft 智能体 + MCP | [定价](https://www.codebuddy.ai/docs/ide/Account/pricing) · 免费档 / 专业约 $10/月 |
| [文心快码](https://comate.baidu.com/) | IDE 扩展 | 有限（文心） | 闭源 | VS Code 约 36 万安装 | 百度 Comate：补全 / 对话 / Zulu 智能体 | [定价](https://comate.baidu.com/zh/pricing) · 个人标准免费 |
| [Aider](https://aider.chat/) | CLI | ✅ | Apache-2.0 | GitHub 约 4.9 万★ | 终端结对编程；代码库映射 + 自动 Git 提交 | [官网](https://aider.chat/) · 免费 BYOK |
| [Continue](https://www.continue.dev/) | IDE / CLI | ✅ | Apache-2.0 | GitHub 约 3.6 万★ · VS Code 约 270 万安装 | 开源编码代理；适合把规范 / 检查写入仓库 | [定价](https://www.continue.dev/pricing) · 按量 / 团队 $20/席 |
| [Kilo Code](https://kilo.ai/) | IDE / CLI / 云 | ✅ | MIT | GitHub 约 2.7 万★ · VS Code 约 100 万安装 | 开源全栈 Agent；多模式 + 多模型 | [定价](https://kilo.ai/pricing) · 免费 BYOK / Pass $19/月起 |
| [Junie](https://junie.jetbrains.com/) | CLI / JetBrains / CI | ✅ | 闭源 | — | JetBrains 模型无关代理；IDE + CI 一体 | [官网](https://junie.jetbrains.com/) · 免费 BYOK / AI Pro $10/月起 |
| [Amazon Q Developer](https://aws.amazon.com/q/developer/) | IDE / CLI | ❌ | 扩展 Apache-2.0 | VS Code 约 170 万安装 | AWS 托管编码助手；安全分析与 Java 升级 | [定价](https://aws.amazon.com/q/developer/pricing/) · 免费档 / 专业 $19/月 |
| [Augment](https://www.augmentcode.com/) | IDE 扩展 / CLI | ❌ | 闭源 | VS Code 约 74 万安装 | 大型代码库上下文引擎 + 代理 | [定价](https://www.augmentcode.com/pricing) · $20/月起 |
| [Tabnine](https://www.tabnine.com/) | IDE / CLI | ✅ | 闭源 | VS Code 约 950 万安装 | 企业隐私与私有化部署向编码平台 | [定价](https://www.tabnine.com/pricing/) · 助手约 $39/席・月 |
| [Zed](https://zed.dev/) | 独立 IDE | ✅ | 开源（多协议） | GitHub 约 9.1 万★ | Rust 高性能协作编辑器；Agent 面板 + 多模型 | [定价](https://zed.dev/pricing) · 个人免费 / Pro $10/月 |
| [Warp](https://www.warp.dev/) | AI 终端 / 工作区 | ✅（付费档） | AGPL-3.0（客户端） | GitHub 约 6.5 万★ · 官网约 70 万用户 | 终端 + 代理编排；可挂 Claude Code / Codex 等 | [定价](https://www.warp.dev/pricing) · 免费档 / Build $18/月起 |
| [Replit](https://replit.com/) | 云 IDE / 平台 | ❌ | 闭源 | 官网约 5000 万用户级 | 浏览器 IDE + Agent；从需求到部署一条链 | [定价](https://replit.com/pricing) · Core $20/月起（年付） |
| [OpenHands](https://openhands.dev/) | 平台 / CLI / SDK | ✅ | 部分 MIT | GitHub 约 8.9 万★ | 端到端工程代理；本地 / 云 / 企业自托管 | [定价](https://openhands.dev/pricing) · 开源本地免费 |
| [goose](https://goose-docs.ai/) | CLI / 桌面 / API | ✅ | Apache-2.0 | GitHub 约 5.5 万★ | AAIF 本地开源代理；多提供商 + MCP | [文档](https://goose-docs.ai/) · 免费 BYOK |
| [Qwen Code](https://github.com/QwenLM/qwen-code) | CLI / IDE / SDK | ✅ | Apache-2.0 | GitHub 约 2.8 万★ | 通义系终端编程代理；可接阿里云 Coding Plan | [Coding Plan](https://www.alibabacloud.com/help/en/model-studio/coding-plan) · BYOK / Plan $50/月起 |
| [Amp](https://ampcode.com/) | CLI / IDE | 有限（平台代管） | 闭源 | VS Code 约 10 万安装 | Sourcegraph 终端优先多模型代理 | [定价](https://ampcode.com/manual#pricing) · 按量充值 |
| [Pi](https://github.com/earendil-works/pi) | CLI / SDK 运行时 | ✅ | MIT | GitHub 约 11.0 万★ | 可扩展终端 Coding Agent；亦作 SDK 底座（Extensions/Skills） | [仓库](https://github.com/earendil-works/pi) · 免费 BYOK |
| [oh-my-pi (omp)](https://github.com/can1357/oh-my-pi) | CLI（Pi fork） | ✅ | MIT | GitHub 约 3.3 万★ | Pi 增强：LSP/DAP、子 Agent、ACP 接 Zed 等 | [omp.sh](https://omp.sh) · 免费 BYOK |
| [DeepSeek-Reasonix](https://github.com/esengine/DeepSeek-Reasonix) | CLI / 桌面 / 浏览器 | ✅ | MIT | GitHub 约 3.6 万★ | DeepSeek 原生终端 Agent；prefix-cache 向长时运行 | [reasonix.io](https://reasonix.io/) · 免费 BYOK |
| [Orca](https://www.onorca.dev/) | ADE 桌面工作区 | 依赖外挂 Agent | MIT | GitHub 约 7.9 万★ | 隔离 worktree 并行跑 Claude Code / Codex / OpenCode 等 | [GitHub](https://github.com/stablyai/orca) · 开源免费 |
| [Desktop CC GUI (ccgui)](https://github.com/zhukunpenglinyutong/desktop-cc-gui) | 多引擎桌面客户端 | 依赖外挂 CLI | MIT | GitHub 约 4400★ | 一窗挂 Claude Code / Codex / Pi / OpenCode / DSH 等；聊天 + 终端 + Git | [下载](https://www.mossx.ai/download) · 开源免费 |

## 怎么选（速查）

1. **闭源全家桶、少折腾**：Cursor / Devin / Copilot；要规格驱动看 Kiro。
2. **代理式深度改库**：Claude Code；要 OpenAI 生态优先 Codex（原生登录）。
3. **开源 + 多模型 BYOK**：Cline / OpenCode / Kilo Code / Continue / Aider。
4. **终端优先、可扩展底座**：Pi（成品 CLI + 可嵌入 SDK）；要 IDE 能力增强用 oh-my-pi；DeepSeek 向用 Reasonix。
5. **多引擎 / 多 Agent 桌面编排**：要一窗切多 CLI 用 Desktop CC GUI；要隔离 worktree 并行跑用 Orca；终端内编排可看 Warp。
6. **国内云厂商 / 企业私有化**：通义灵码、CodeBuddy、文心快码、Tabnine、Amazon Q。

账号切换、CPA 路由、Skills 管理等**增强工具**不在本表展开，请到 [环境配置：工具与增强]({{< relref "setup/env-and-tools" >}})。
