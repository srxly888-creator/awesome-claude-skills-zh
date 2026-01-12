# Awesome Claude Skills

## 🇨🇳 中文

<h1 align="center">Awesome Claude 技能精选</h1>

<p align="center">
  <b>默认展示中文文档；英文原文请向下滚动查阅</b>
</p>

### 简介
本仓库收录了精心挑选的 Claude Skills，帮助你在 Claude.ai、Claude Code 以及 Claude API 中提升效率。

## 快速开始：连接 Claude 与 500+ 个应用

**connect-apps** 插件让 Claude 可以执行真实操作：发邮件、创建问题单、发布 Slack 消息等，并通过 Composio 管理认证，与 500 多个应用打通。

### 1. 安装插件
```bash
claude --plugin-dir ./connect-apps-plugin
```

### 2. 运行配置
```
/connect-apps:setup
```
输入提示时粘贴你的 API Key（可在 [platform.composio.dev](https://platform.composio.dev/?utm_source=Github&utm_content=AwesomeSkills) 免费申请）。

### 3. 重启并验证
```bash
exit
claude
```

> **想要 Claude 不只是生成文本？** 接入后 Claude 可以发邮件、创建 issue、发送 Slack 消息，并在 1000+ 个应用间放心执行操作。 [了解详细 →](./connect/)

如果你收到确认邮件，说明 Claude 已成功连接到 500+ 应用。

**[查看支持的所有应用 →](./connect-apps/)**

---

## 目录
- [Claude 技能是什么？](#什么是-claude-技能)
- [技能汇总](#技能)
  - [文档处理](#文档处理)
  - [开发与代码工具](#开发与代码工具)
  - [数据与分析](#数据与分析)
  - [商务与营销](#商务与营销)
  - [沟通与写作](#沟通与写作)
  - [创意与多媒体](#创意与多媒体)
  - [生产力与组织](#生产力与组织)
  - [协作与项目管理](#协作与项目管理)
  - [安全与系统](#安全与系统)
- [上手指南](#上手指南)
- [创建技能](#创建技能)
- [贡献指南](#贡献指南)
- [资源](#资源)
- [许可证](#许可证)

## 什么是 Claude 技能？
Claude Skills 是一组可定制的工作流，指导 Claude 按照你设定的流程完成特定任务，在所有 Claude 平台上实现一致且可重复的操作行为。

## 技能

### 文档处理
- [docx](https://github.com/anthropics/skills/tree/main/skills/docx) - 编辑 Word 文档、跟踪修订、添加批注与格式。
- [pdf](https://github.com/anthropics/skills/tree/main/skills/pdf) - 提取文本、表格与元数据，合并与注释 PDF。
- [pptx](https://github.com/anthropics/skills/tree/main/skills/pptx) - 读取、生成与调整幻灯片、布局与模板。
- [xlsx](https://github.com/anthropics/skills/tree/main/skills/xlsx) - 操作电子表格：公式、图表与数据转换。
- [Markdown to EPUB Converter](https://github.com/smerchek/claude-epub-skill) - 将 Markdown 和聊天总结转换成专业的 EPUB 电子书。*作者 [@smerchek](https://github.com/smerchek)*

### 开发与代码工具
- [artifacts-builder](https://github.com/anthropics/skills/tree/main/skills/web-artifacts-builder) - 用 React、Tailwind CSS 与 shadcn/ui 打造复杂的 Claude.ai HTML 工件。
- [aws-skills](https://github.com/zxkane/aws-skills) - 提供 AWS CDK 实践、成本优化与无服务器/事件驱动架构建议。
- [Changelog Generator](./changelog-generator/) - 分析 Git 提交并自动生成面向用户的更新日志。
- [Claude Code Terminal Title](https://github.com/bluzername/claude-code-terminal-title) - 每个 Claude Code 终端都有描述当前工作的动态标题。
- [D3.js Visualization](https://github.com/chrisvoncsefalvay/claude-d3js-skill) - 教 Claude 生成 D3 图表与交互可视化。*作者 [@chrisvoncsefalvay](https://github.com/chrisvoncsefalvay)*
- [FFUF Web Fuzzing](https://github.com/jthack/ffuf_claude_skill) - 集成 ffuf 网站模糊测试，并帮助分析潜在漏洞。*作者 [@jthack](https://github.com/jthack)*
- [finishing-a-development-branch](https://github.com/obra/superpowers/tree/main/skills/finishing-a-development-branch) - 提供完成开发分支的清晰选项与执行流程。
- [iOS Simulator](https://github.com/conorluddy/ios-simulator-skill) - 让 Claude 控制 iOS 模拟器以测试与调试应用。*作者 [@conorluddy](https://github.com/conorluddy)*
- [LangSmith Fetch](./langsmith-fetch/) - 自动抓取 LangSmith Studio 的执行追踪，帮助调试 LangChain 与 LangGraph 代理。Claude Code 的首个 AI 可观测性技能。*作者 [@OthmanAdi](https://github.com/OthmanAdi)*
- [MCP Builder](./mcp-builder/) - 指导构建高质量 MCP（Model Context Protocol）服务器，使用 Python 或 TypeScript 调用外部 API 与服务。
- [move-code-quality-skill](https://github.com/1NickPappas/move-code-quality-skill) - 根据 Move 2024 版码质检查表评估 Move 语言包。
- [Playwright Browser Automation](https://github.com/lackeyjb/playwright-skill) - 利用 Playwright 自动化测试与验证 Web 应用。*作者 [@lackeyjb](https://github.com/lackeyjb)*
- [prompt-engineering](https://github.com/NeoLabHQ/context-engineering-kit/tree/master/plugins/customaize-agent/skills/prompt-engineering) - 教授包括 Anthropic 最佳实践在内的提示工程模式与技巧。
- [pypict-claude-skill](https://github.com/omkamal/pypict-claude-skill) - 使用 PICT（Pairwise Independent Combinatorial Testing）生成覆盖 pairwise 的测试方案。
- [reddit-fetch](https://github.com/ykdojo/claude-code-tips/tree/main/skills/reddit-fetch) - 通过 Gemini CLI 获取 Reddit 内容，绕过 WebFetch 限制或 403 错误。
- [Skill Creator](./skill-creator/) - 提供创建 Claude Skills 的流程、结构与工具集。
- [Skill Seekers](https://github.com/yusufkaraaslan/Skill_Seekers) - 几分钟内将任意文档网站转换为 Claude AI 技能。*作者 [@yusufkaraaslan](https://github.com/yusufkaraaslan)*
- [software-architecture](https://github.com/NeoLabHQ/context-engineering-kit/tree/master/plugins/ddd/skills/software-architecture) - 实现设计模式、清晰架构与 SOLID 原则。
- [subagent-driven-development](https://github.com/NeoLabHQ/context-engineering-kit/tree/master/plugins/sadd/skills/subagent-driven-development) - 通过子代理逐步迭代，加入代码审核节点以保证控制与质量。
- [test-driven-development](https://github.com/obra/superpowers/tree/main/skills/test-driven-development) - 在实现前先用测试驱动方法进行开发。
- [using-git-worktrees](https://github.com/obra/superpowers/blob/main/skills/using-git-worktrees/) - 创建隔离的 Git 工作树并自动校验安全性。
- [Connect](./connect/) - 让 Claude 连接任意应用，发邮件、创建 issue、发送消息并更新数据库，支持 Gmail、Slack、GitHub、Notion 等 1000+ 服务。
- [Webapp Testing](./webapp-testing/) - 使用 Playwright 测试本地 Web 应用，验证 UI 行为并捕获截图。

### 数据与分析
- [CSV Data Summarizer](https://github.com/coffeefuelbump/csv-data-summarizer-claude-skill) - 自动分析 CSV 并生成带可视化的洞察，无需额外提示。*作者 [@coffeefuelbump](https://github.com/coffeefuelbump)*
- [postgres](https://github.com/sanjay3290/ai-skills/tree/main/skills/postgres) - 面向 PostgreSQL 的安全只读查询，支持多连接与纵深防御。*作者 [@sanjay3290](https://github.com/sanjay3290)*
- [root-cause-tracing](https://github.com/obra/superpowers/tree/main/skills/root-cause-tracing) - 当执行出现深层错误时，帮助追溯根本原因。

### 商务与营销
- [Brand Guidelines](./brand-guidelines/) - 套用 Anthropic 官方品牌色与排版，确保视觉一致性。
- [Competitive Ads Extractor](./competitive-ads-extractor/) - 抽取并分析广告库中的竞品广告，理解有效的创意与文案。
- [Domain Name Brainstormer](./domain-name-brainstormer/) - 生成富有创意的域名并检查 .com/.io/.dev/.ai 等后缀可用性。
- [Internal Comms](./internal-comms/) - 撰写内部公告、通讯、常见问题与进展报告，适配公司格式。
- [Lead Research Assistant](./lead-research-assistant/) - 研究并筛选高价值潜在客户，给出可执行的外联策略。

### 沟通与写作
- [article-extractor](https://github.com/michalparkola/tapestry-skills-for-claude-code/tree/main/article-extractor) - 提取网页文章正文与元数据。
- [brainstorming](https://github.com/obra/superpowers/tree/main/skills/brainstorming) - 通过结构化提问与替代方案完善概念。
- [Content Research Writer](./content-research-writer/) - 进行内容研究、补充引用、强化开头并逐段反馈。
- [family-history-research](https://github.com/emaynard/claude-family-history-research-skill) - 协助进行家族史与族谱研究规划。
- [Meeting Insights Analyzer](./meeting-insights-analyzer/) - 分析会议记录，识别行为模式（冲突避免、发言比例、填充词、领导风格）。
- [NotebookLM Integration](https://github.com/PleasePrompto/notebooklm-skill) - 让 Claude Code 与 NotebookLM 直接对话，基于上传文档提供有据可依的答案。*作者 [@PleasePrompto](https://github.com/PleasePrompto)*

### 创意与多媒体
- [Canvas Design](./canvas-design/) - 用设计理念与美学原则生成 PNG/PDF 视觉作品（海报、静态图）。
- [imagen](https://github.com/sanjay3290/ai-skills/tree/main/skills/imagen) - 使用 Google Gemini 图像 API 创造 UI 草图、图标与插画。*作者 [@sanjay3290](https://github.com/sanjay3290)*
- [Image Enhancer](./image-enhancer/) - 提升图像与截图分辨率、清晰度与锐利度。
- [Slack GIF Creator](./slack-gif-creator/) - 为 Slack 优化动画 GIF，并进行大小校验与动画拼接。
- [Theme Factory](./theme-factory/) - 为幻灯片、文档与网页应用 10 套主题配色和排版。
- [Video Downloader](./video-downloader/) - 下载 YouTube 与其他平台视频，支持多格式与画质选项。
- [youtube-transcript](https://github.com/michalparkola/tapestry-skills-for-claude-code/tree/main/youtube-transcript) - 获取 YouTube 字幕并生成摘要。

### 生产力与组织
- [File Organizer](./file-organizer/) - 理解上下文智能整理文件夹、查重并建议更优结构。
- [Invoice Organizer](./invoice-organizer/) - 自动整理发票与收据，提取信息并统一命名。
- [kaizen](https://github.com/NeoLabHQ/context-engineering-kit/tree/master/plugins/kaizen/skills/kaizen) - 运用 Kaizen 精益哲学与多种分析方法推进持续改进。
- [n8n-skills](https://github.com/haunchen/n8n-skills) - 让 AI 助手直接理解并操作 n8n 工作流。
- [Raffle Winner Picker](./raffle-winner-picker/) - 从列表/表格/Google Sheet 随机选出获奖者，并使用密码学安全随机性。
- [Tailored Resume Generator](./tailored-resume-generator/) - 分析职位描述，生成突出相关经验与技能的定制简历。
- [ship-learn-next](https://github.com/michalparkola/tapestry-skills-for-claude-code/tree/main/ship-learn-next) - 根据反馈回路判断下一个产品或学习方向。
- [tapestry](https://github.com/michalparkola/tapestry-skills-for-claude-code/tree/main/tapestry) - 将相关文档串联成知识网络并生成摘要。

### 协作与项目管理
- [git-pushing](https://github.com/mhattingpete/claude-skills-marketplace/tree/main/engineering-workflow-plugin/skills/git-pushing) - 自动化 git 操作与仓库交互。
- [review-implementing](https://github.com/mhattingpete/claude-skills-marketplace/tree/main/engineering-workflow-plugin/skills/review-implementing) - 评估实现计划，并与规范对齐。
- [test-fixing](https://github.com/mhattingpete/claude-skills-marketplace/tree/main/engineering-workflow-plugin/skills/test-fixing) - 诊断失败测试并建议修复。

### 安全与系统
- [computer-forensics](https://github.com/mhattingpete/claude-skills-marketplace/tree/main/computer-forensics-skills/skills/computer-forensics) - 数字取证分析与调查。
- [file-deletion](https://github.com/mhattingpete/claude-skills-marketplace/tree/main/computer-forensics-skills/skills/file-deletion) - 安全删除文件与数据清理。
- [metadata-extraction](https://github.com/mhattingpete/claude-skills-marketplace/tree/main/computer-forensics-skills/skills/metadata-extraction) - 提取与分析文件元数据用于取证。
- [threat-hunting-with-sigma-rules](https://github.com/jthack/threat-hunting-with-sigma-rules-skill) - 利用 Sigma 规则侦测威胁并分析安全事件。

## 上手指南

### 在 Claude.ai 中使用技能
1. 点击聊天界面中的技能图标（🧩）。
2. 从市场添加技能或上传自定义技能。
3. Claude 会根据任务自动激活相关技能。

### 在 Claude Code 中使用技能
1. 将技能拷贝到 `~/.config/claude-code/skills/`：
```bash
mkdir -p ~/.config/claude-code/skills/
cp -r skill-name ~/.config/claude-code/skills/
```

2. 检查技能元数据：
```bash
head ~/.config/claude-code/skills/skill-name/SKILL.md
```

3. 启动 Claude Code：
```bash
claude
```

4. 技能会自动加载并在适用时激活。

### 通过 API 使用技能
用 Claude Skills API 编程方式加载与管理技能：
```python
import anthropic

client = anthropic.Anthropic(api_key="your-api-key")

response = client.messages.create(
    model="claude-3-5-sonnet-20241022",
    skills=["skill-id-here"],
    messages=[{"role": "user", "content": "Your prompt"}]
)
```
详情参阅 [Skills API 文档](https://docs.claude.com/en/api/skills-guide)。

## 创建技能

### 技能结构
每个技能是一个包含 YAML 头信息的文件夹：
```
skill-name/
├── SKILL.md          # 必需：技能说明与元数据
├── scripts/          # 可选：辅助脚本
├── templates/        # 可选：文档模板
└── resources/        # 可选：参考文件
```

### 基础技能模板
```markdown
---
name: my-skill-name
description: 清晰描述技能作用与适用场景
---

# My Skill Name

详细说明技能用途与能力。

## 使用时机

- 场景 1
- 场景 2
- 场景 3

## 执行步骤

[Claude 执行该技能的具体步骤]

## 示例

[真实示例展示技能效果]
```

### 技能最佳实践
- 聚焦具体、可重复的任务
- 提供清晰示例与边界情况
- 面向 Claude 而非终端用户编写说明
- 在 Claude.ai、Claude Code 与 API 中均做测试
- 说明前置条件与依赖
- 包含异常处理建议

## 贡献指南
欢迎贡献！请先阅读 [贡献指南](CONTRIBUTING.md)，了解：
- 如何提交新技能
- 技能质量标准
- Pull request 流程
- 行为准则

### 快速贡献步骤
1. 保证你的技能基于真实用例
2. 检查现有技能避免重复
3. 遵循技能结构模板
4. 在多个平台测试技能
5. 提交清晰文档的 PR

## 资源

### 官方文档
- [Claude Skills 概览](https://www.anthropic.com/news/skills) - 官方发布与功能介绍
- [Skills 用户指南](https://support.claude.com/en/articles/12512180-using-skills-in-claude) - 如何在 Claude 中使用技能
- [创建自定义技能](https://support.claude.com/en/articles/12512198-creating-custom-skills) - 技能开发指导
- [Skills API 文档](https://docs.claude.com/en/api/skills-guide) - API 集成说明
- [Agent Skills 博客](https://anthropic.com/engineering/equipping-agents-for-the-real-world-with-agent-skills) - 工程实践深度解读

### 社区资源
- [Anthropic Skills 仓库](https://github.com/anthropics/skills) - 官方示例技能
- [Claude 社区](https://community.anthropic.com) - 与其他用户交流
- [Skills Marketplace](https://claude.ai/marketplace) - 发现与分享技能

### 灵感与应用
- [Lenny's Newsletter](https://www.lennysnewsletter.com/p/everyone-should-be-using-claude-code) - 50 种 Claude Code 的使用方式
- [Notion Skills](https://www.notion.so/notiondevs/Notion-Skills-for-Claude-28da4445d27180c7af1df7d8615723d0) - Notion 集成技能

## 加入社区
- [加入 Discord](https://discord.com/invite/composio) - 与开发者讨论 Claude Skills
- [关注 Twitter/X](https://x.com/composio) - 获取最新技能与功能消息
- 有问题？写信至 [support@composio.dev](mailto:support@composio.dev)

---

<p align="center">
  <b>超过 20,000 名开发者正在打造可交付的智能代理</b>
</p>

<p align="center">
  <a href="https://platform.composio.dev/?utm_source=Github&utm_content=AwesomeSkills">
    <img src="https://img.shields.io/badge/Get_Started_Free-4F46E5?style=for-the-badge" alt="Get Started"/>
  </a>
</p>

## 许可证
本仓库采用 Apache 2.0 协议。

各技能可能另有授权，请查看各技能文件夹中的许可说明。

---

**说明**：Claude Skills 可跨 Claude.ai、Claude Code 与 Claude API 使用。创建技能后，可在所有平台复用，保持工作流一致性。

- [AgentsKB](https://agentskb.com) - 给你的 AI 提供经过研究验证的答案。

---

## 🇺🇸 English

<h1 align="center">Awesome Claude Skills</h1>

<p align="center">
<a href="https://platform.composio.dev/?utm_source=Github&utm_medium=Youtube&utm_campaign=2025-11&utm_content=AwesomeSkills">
  <img width="1280" height="640" alt="Composio banner" src="https://github.com/user-attachments/assets/e91255af-e4ba-4d71-b1a8-bd081e8a234a">
</a>


</p>

<p align="center">
  <a href="https://awesome.re">
    <img src="https://awesome.re/badge.svg" alt="Awesome" />
  </a>
  <a href="https://makeapullrequest.com">
    <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="PRs Welcome" />
  </a>
  <a href="https://www.apache.org/licenses/LICENSE-2.0">
    <img src="https://img.shields.io/badge/License-Apache_2.0-blue.svg?style=flat-square" alt="License: Apache-2.0" />
  </a>
</p>
<div>
<p align="center">
  <a href="https://twitter.com/composio">
    <img src="https://img.shields.io/badge/Follow on X-000000?style=for-the-badge&logo=x&logoColor=white" alt="Follow on X" />
  </a>
  <a href="https://www.linkedin.com/company/composiohq/">
    <img src="https://img.shields.io/badge/Follow on LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="Follow on LinkedIn" />
  </a>
  <a href="https://discord.com/invite/composio">
    <img src="https://img.shields.io/badge/Join our Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Join our Discord" />
  </a>
  </p>
</div>

A curated list of practical Claude Skills for enhancing productivity across Claude.ai, Claude Code, and the Claude API.

---

## Quickstart: Connect Claude to 500+ Apps

The **connect-apps** plugin lets Claude perform real actions - send emails, create issues, post to Slack. It handles auth and connects to 500+ apps using Composio under the hood.

### 1. Install the Plugin

```bash
claude --plugin-dir ./connect-apps-plugin
```

### 2. Run Setup

```
/connect-apps:setup
```

Paste your API key when asked. (Get a free key at [platform.composio.dev](https://platform.composio.dev/?utm_source=Github&utm_content=AwesomeSkills))

### 3. Restart & Try It

```bash
exit
claude
```

> **Want skills that do more than generate text?** Claude can send emails, create issues, post to Slack, and take actions across 1000+ apps. [See how →](./connect/)

If you receive the email, Claude is now connected to 500+ apps.

**[See all supported apps →](./connect-apps/)**

---

## Contents

- [What Are Claude Skills?](#what-are-claude-skills)
- [Skills](#skills)
  - [Document Processing](#document-processing)
  - [Development & Code Tools](#development--code-tools)
  - [Data & Analysis](#data--analysis)
  - [Business & Marketing](#business--marketing)
  - [Communication & Writing](#communication--writing)
  - [Creative & Media](#creative--media)
  - [Productivity & Organization](#productivity--organization)
  - [Collaboration & Project Management](#collaboration--project-management)
  - [Security & Systems](#security--systems)
- [Getting Started](#getting-started)
- [Creating Skills](#creating-skills)
- [Contributing](#contributing)
- [Resources](#resources)
- [License](#license)

## What Are Claude Skills?

Claude Skills are customizable workflows that teach Claude how to perform specific tasks according to your unique requirements. Skills enable Claude to execute tasks in a repeatable, standardized manner across all Claude platforms.

## Skills

### Document Processing

- [docx](https://github.com/anthropics/skills/tree/main/skills/docx) - Create, edit, analyze Word docs with tracked changes, comments, formatting.
- [pdf](https://github.com/anthropics/skills/tree/main/skills/pdf) - Extract text, tables, metadata, merge & annotate PDFs.
- [pptx](https://github.com/anthropics/skills/tree/main/skills/pptx) - Read, generate, and adjust slides, layouts, templates.
- [xlsx](https://github.com/anthropics/skills/tree/main/skills/xlsx) - Spreadsheet manipulation: formulas, charts, data transformations.
- [Markdown to EPUB Converter](https://github.com/smerchek/claude-epub-skill) - Converts markdown documents and chat summaries into professional EPUB ebook files. *By [@smerchek](https://github.com/smerchek)*

### Development & Code Tools

- [artifacts-builder](https://github.com/anthropics/skills/tree/main/skills/web-artifacts-builder) - Suite of tools for creating elaborate, multi-component claude.ai HTML artifacts using modern frontend web technologies (React, Tailwind CSS, shadcn/ui).
- [aws-skills](https://github.com/zxkane/aws-skills) - AWS development with CDK best practices, cost optimization MCP servers, and serverless/event-driven architecture patterns.
- [Changelog Generator](./changelog-generator/) - Automatically creates user-facing changelogs from git commits by analyzing history and transforming technical commits into customer-friendly release notes.
- [Claude Code Terminal Title](https://github.com/bluzername/claude-code-terminal-title) - Gives each Claud-Code terminal window a dynamic title that describes the work being done so you don't lose track of what window is doing what.
- [D3.js Visualization](https://github.com/chrisvoncsefalvay/claude-d3js-skill) - Teaches Claude to produce D3 charts and interactive data visualizations. *By [@chrisvoncsefalvay](https://github.com/chrisvoncsefalvay)*
- [FFUF Web Fuzzing](https://github.com/jthack/ffuf_claude_skill) - Integrates the ffuf web fuzzer so Claude can run fuzzing tasks and analyze results for vulnerabilities. *By [@jthack](https://github.com/jthack)*
- [finishing-a-development-branch](https://github.com/obra/superpowers/tree/main/skills/finishing-a-development-branch) - Guides completion of development work by presenting clear options and handling chosen workflow.
- [iOS Simulator](https://github.com/conorluddy/ios-simulator-skill) - Enables Claude to interact with iOS Simulator for testing and debugging iOS applications. *By [@conorluddy](https://github.com/conorluddy)*
- [LangSmith Fetch](./langsmith-fetch/) - Debug LangChain and LangGraph agents by automatically fetching and analyzing execution traces from LangSmith Studio. First AI observability skill for Claude Code. *By [@OthmanAdi](https://github.com/OthmanAdi)*
- [MCP Builder](./mcp-builder/) - Guides creation of high-quality MCP (Model Context Protocol) servers for integrating external APIs and services with LLMs using Python or TypeScript.
- [move-code-quality-skill](https://github.com/1NickPappas/move-code-quality-skill) - Analyzes Move language packages against the official Move Book Code Quality Checklist for Move 2024 Edition compliance and best practices.
- [Playwright Browser Automation](https://github.com/lackeyjb/playwright-skill) - Model-invoked Playwright automation for testing and validating web applications. *By [@lackeyjb](https://github.com/lackeyjb)*
- [prompt-engineering](https://github.com/NeoLabHQ/context-engineering-kit/tree/master/plugins/customaize-agent/skills/prompt-engineering) - Teaches well-known prompt engineering techniques and patterns, including Anthropic best practices and agent persuasion principles.
- [pypict-claude-skill](https://github.com/omkamal/pypict-claude-skill) - Design comprehensive test cases using PICT (Pairwise Independent Combinatorial Testing) for requirements or code, generating optimized test suites with pairwise coverage.
- [reddit-fetch](https://github.com/ykdojo/claude-code-tips/tree/main/skills/reddit-fetch) - Fetches Reddit content via Gemini CLI when WebFetch is blocked or returns 403 errors.
- [Skill Creator](./skill-creator/) - Provides guidance for creating effective Claude Skills that extend capabilities with specialized knowledge, workflows, and tool integrations.
- [Skill Seekers](https://github.com/yusufkaraaslan/Skill_Seekers) - Automatically converts any documentation website into a Claude AI skill in minutes. *By [@yusufkaraaslan](https://github.com/yusufkaraaslan)*
- [software-architecture](https://github.com/NeoLabHQ/context-engineering-kit/tree/master/plugins/ddd/skills/software-architecture) - Implements design patterns including Clean Architecture, SOLID principles, and comprehensive software design best practices.
- [subagent-driven-development](https://github.com/NeoLabHQ/context-engineering-kit/tree/master/plugins/sadd/skills/subagent-driven-development) - Dispatches independent subagents for individual tasks with code review checkpoints between iterations for rapid, controlled development.
- [test-driven-development](https://github.com/obra/superpowers/tree/main/skills/test-driven-development) - Use when implementing any feature or bugfix, before writing implementation code.
- [using-git-worktrees](https://github.com/obra/superpowers/blob/main/skills/using-git-worktrees/) - Creates isolated git worktrees with smart directory selection and safety verification.
- [Connect](./connect/) - Connect Claude to any app. Send emails, create issues, post messages, update databases - take real actions across Gmail, Slack, GitHub, Notion, and 1000+ services.
- [Webapp Testing](./webapp-testing/) - Tests local web applications using Playwright for verifying frontend functionality, debugging UI behavior, and capturing screenshots.

### Data & Analysis

- [CSV Data Summarizer](https://github.com/coffeefuelbump/csv-data-summarizer-claude-skill) - Automatically analyzes CSV files and generates comprehensive insights with visualizations without requiring user prompts. *By [@coffeefuelbump](https://github.com/coffeefuelbump)*
- [postgres](https://github.com/sanjay3290/ai-skills/tree/main/skills/postgres) - Execute safe read-only SQL queries against PostgreSQL databases with multi-connection support and defense-in-depth security. *By [@sanjay3290](https://github.com/sanjay3290)*
- [root-cause-tracing](https://github.com/obra/superpowers/tree/main/skills/root-cause-tracing) - Use when errors occur deep in execution and you need to trace back to find the original trigger.

### Business & Marketing

- [Brand Guidelines](./brand-guidelines/) - Applies Anthropic's official brand colors and typography to artifacts for consistent visual identity and professional design standards.
- [Competitive Ads Extractor](./competitive-ads-extractor/) - Extracts and analyzes competitors' ads from ad libraries to understand messaging and creative approaches that resonate.
- [Domain Name Brainstormer](./domain-name-brainstormer/) - Generates creative domain name ideas and checks availability across multiple TLDs including .com, .io, .dev, and .ai extensions.
- [Internal Comms](./internal-comms/) - Helps write internal communications including 3P updates, company newsletters, FAQs, status reports, and project updates using company-specific formats.
- [Lead Research Assistant](./lead-research-assistant/) - Identifies and qualifies high-quality leads by analyzing your product, searching for target companies, and providing actionable outreach strategies.

### Communication & Writing

- [article-extractor](https://github.com/michalparkola/tapestry-skills-for-claude-code/tree/main/article-extractor) - Extract full article text and metadata from web pages.
- [brainstorming](https://github.com/obra/superpowers/tree/main/skills/brainstorming) - Transform rough ideas into fully-formed designs through structured questioning and alternative exploration.
- [Content Research Writer](./content-research-writer/) - Assists in writing high-quality content by conducting research, adding citations, improving hooks, and providing section-by-section feedback.
- [family-history-research](https://github.com/emaynard/claude-family-history-research-skill) - Provides assistance with planning family history and genealogy research projects.
- [Meeting Insights Analyzer](./meeting-insights-analyzer/) - Analyzes meeting transcripts to uncover behavioral patterns including conflict avoidance, speaking ratios, filler words, and leadership style.
- [NotebookLM Integration](https://github.com/PleasePrompto/notebooklm-skill) - Lets Claude Code chat directly with NotebookLM for source-grounded answers based exclusively on uploaded documents. *By [@PleasePrompto](https://github.com/PleasePrompto)*

### Creative & Media

- [Canvas Design](./canvas-design/) - Creates beautiful visual art in PNG and PDF documents using design philosophy and aesthetic principles for posters, designs, and static pieces.
- [imagen](https://github.com/sanjay3290/ai-skills/tree/main/skills/imagen) - Generate images using Google Gemini's image generation API for UI mockups, icons, illustrations, and visual assets. *By [@sanjay3290](https://github.com/sanjay3290)*
- [Image Enhancer](./image-enhancer/) - Improves image and screenshot quality by enhancing resolution, sharpness, and clarity for professional presentations and documentation.
- [Slack GIF Creator](./slack-gif-creator/) - Creates animated GIFs optimized for Slack with validators for size constraints and composable animation primitives.
- [Theme Factory](./theme-factory/) - Applies professional font and color themes to artifacts including slides, docs, reports, and HTML landing pages with 10 pre-set themes.
- [Video Downloader](./video-downloader/) - Downloads videos from YouTube and other platforms for offline viewing, editing, or archival with support for various formats and quality options.
- [youtube-transcript](https://github.com/michalparkola/tapestry-skills-for-claude-code/tree/main/youtube-transcript) - Fetch transcripts from YouTube videos and prepare summaries.

### Productivity & Organization

- [File Organizer](./file-organizer/) - Intelligently organizes files and folders by understanding context, finding duplicates, and suggesting better organizational structures.
- [Invoice Organizer](./invoice-organizer/) - Automatically organizes invoices and receipts for tax preparation by reading files, extracting information, and renaming consistently.
- [kaizen](https://github.com/NeoLabHQ/context-engineering-kit/tree/master/plugins/kaizen/skills/kaizen) - Applies continuous improvement methodology with multiple analytical approaches, based on Japanese Kaizen philosophy and Lean methodology.
- [n8n-skills](https://github.com/haunchen/n8n-skills) - Enables AI assistants to directly understand and operate n8n workflows.
- [Raffle Winner Picker](./raffle-winner-picker/) - Randomly selects winners from lists, spreadsheets, or Google Sheets for giveaways and contests with cryptographically secure randomness.
- [Tailored Resume Generator](./tailored-resume-generator/) - Analyzes job descriptions and generates tailored resumes that highlight relevant experience, skills, and achievements to maximize interview chances.
- [ship-learn-next](https://github.com/michalparkola/tapestry-skills-for-claude-code/tree/main/ship-learn-next) - Skill to help iterate on what to build or learn next, based on feedback loops.
- [tapestry](https://github.com/michalparkola/tapestry-skills-for-claude-code/tree/main/tapestry) - Interlink and summarize related documents into knowledge networks.

### Collaboration & Project Management

- [git-pushing](https://github.com/mhattingpete/claude-skills-marketplace/tree/main/engineering-workflow-plugin/skills/git-pushing) - Automate git operations and repository interactions.
- [review-implementing](https://github.com/mhattingpete/claude-skills-marketplace/tree/main/engineering-workflow-plugin/skills/review-implementing) - Evaluate code implementation plans and align with specs.
- [test-fixing](https://github.com/mhattingpete/claude-skills-marketplace/tree/main/engineering-workflow-plugin/skills/test-fixing) - Detect failing tests and propose patches or fixes.

### Security & Systems

- [computer-forensics](https://github.com/mhattingpete/claude-skills-marketplace/tree/main/computer-forensics-skills/skills/computer-forensics) - Digital forensics analysis and investigation techniques.
- [file-deletion](https://github.com/mhattingpete/claude-skills-marketplace/tree/main/computer-forensics-skills/skills/file-deletion) - Secure file deletion and data sanitization methods.
- [metadata-extraction](https://github.com/mhattingpete/claude-skills-marketplace/tree/main/computer-forensics-skills/skills/metadata-extraction) - Extract and analyze file metadata for forensic purposes.
- [threat-hunting-with-sigma-rules](https://github.com/jthack/threat-hunting-with-sigma-rules-skill) - Use Sigma detection rules to hunt for threats and analyze security events.

## Getting Started

### Using Skills in Claude.ai

1. Click the skill icon (🧩) in your chat interface.
2. Add skills from the marketplace or upload custom skills.
3. Claude automatically activates relevant skills based on your task.

### Using Skills in Claude Code

1. Place the skill in `~/.config/claude-code/skills/`:
   ```bash
   mkdir -p ~/.config/claude-code/skills/
   cp -r skill-name ~/.config/claude-code/skills/
   ```

2. Verify skill metadata:
   ```bash
   head ~/.config/claude-code/skills/skill-name/SKILL.md
   ```

3. Start Claude Code:
   ```bash
   claude
   ```

4. The skill loads automatically and activates when relevant.

### Using Skills via API

Use the Claude Skills API to programmatically load and manage skills:

```python
import anthropic

client = anthropic.Anthropic(api_key="your-api-key")

response = client.messages.create(
    model="claude-3-5-sonnet-20241022",
    skills=["skill-id-here"],
    messages=[{"role": "user", "content": "Your prompt"}]
)
```

See the [Skills API documentation](https://docs.claude.com/en/api/skills-guide) for details.

## Creating Skills

### Skill Structure

Each skill is a folder containing a `SKILL.md` file with YAML frontmatter:

```
skill-name/
├── SKILL.md          # Required: Skill instructions and metadata
├── scripts/          # Optional: Helper scripts
├── templates/        # Optional: Document templates
└── resources/        # Optional: Reference files
```

### Basic Skill Template

```markdown
---
name: my-skill-name
description: A clear description of what this skill does and when to use it.
---

# My Skill Name

Detailed description of the skill's purpose and capabilities.

## When to Use This Skill

- Use case 1
- Use case 2
- Use case 3

## Instructions

[Detailed instructions for Claude on how to execute this skill]

## Examples

[Real-world examples showing the skill in action]
```

### Skill Best Practices

- Focus on specific, repeatable tasks
- Include clear examples and edge cases
- Write instructions for Claude, not end users
- Test across Claude.ai, Claude Code, and API
- Document prerequisites and dependencies
- Include error handling guidance

## Contributing

We welcome contributions! Please read our [Contributing Guidelines](CONTRIBUTING.md) for details on:

- How to submit new skills
- Skill quality standards
- Pull request process
- Code of conduct

### Quick Contribution Steps

1. Ensure your skill is based on a real use case
2. Check for duplicates in existing skills
3. Follow the skill structure template
4. Test your skill across platforms
5. Submit a pull request with clear documentation

## Resources

### Official Documentation

- [Claude Skills Overview](https://www.anthropic.com/news/skills) - Official announcement and features
- [Skills User Guide](https://support.claude.com/en/articles/12512180-using-skills-in-claude) - How to use skills in Claude
- [Creating Custom Skills](https://support.claude.com/en/articles/12512198-creating-custom-skills) - Skill development guide
- [Skills API Documentation](https://docs.claude.com/en/api/skills-guide) - API integration guide
- [Agent Skills Blog Post](https://anthropic.com/engineering/equipping-agents-for-the-real-world-with-agent-skills) - Engineering deep dive

### Community Resources

- [Anthropic Skills Repository](https://github.com/anthropics/skills) - Official example skills
- [Claude Community](https://community.anthropic.com) - Discuss skills with other users
- [Skills Marketplace](https://claude.ai/marketplace) - Discover and share skills

### Inspiration & Use Cases

- [Lenny's Newsletter](https://www.lennysnewsletter.com/p/everyone-should-be-using-claude-code) - 50 ways people use Claude Code
- [Notion Skills](https://www.notion.so/notiondevs/Notion-Skills-for-Claude-28da4445d27180c7af1df7d8615723d0) - Notion integration skills


## Join the Community

- [Join our Discord](https://discord.com/invite/composio) - Chat with other developers building Claude Skills
- [Follow on Twitter/X](https://x.com/composio) - Stay updated on new skills and features
- Questions? [support@composio.dev](mailto:support@composio.dev)

---

<p align="center">
  <b>Join 20,000+ developers building agents that ship</b>
</p>

<p align="center">
  <a href="https://platform.composio.dev/?utm_source=Github&utm_content=AwesomeSkills">
    <img src="https://img.shields.io/badge/Get_Started_Free-4F46E5?style=for-the-badge" alt="Get Started"/>
  </a>
</p>

## License

This repository is licensed under the Apache License 2.0.

Individual skills may have different licenses - please check each skill's folder for specific licensing information.

---

**Note**: Claude Skills work across Claude.ai, Claude Code, and the Claude API. Once you create a skill, it's portable across all platforms, making your workflows consistent everywhere you use Claude.

- [AgentsKB](https://agentskb.com) - Upgrade your AI with researched answers. We did the research so your AI gets it right the first time.
