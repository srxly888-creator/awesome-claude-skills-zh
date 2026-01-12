# Contributing to Awesome Claude Skills

## 🇨🇳 中文

# 贡献 Awesome Claude Skills

感谢你愿意为这个 Claude Skills 的精选集合贡献力量！本指南帮你按照社区标准创建有价值的新技能。

## 开始前
- 确保你的技能基于**真实场景**而非理论假想。
- 查找已有技能以防重复。
- 如有原始人员或来源，请尽量注明出处。

## 技能要求
所有技能必须：

1. **解决真实问题** - 基于实际使用场景而非假设。
2. **文档完备** - 提供清晰说明、示例与使用场景。
3. **易于访问** - 尽可能为非技术用户提供友好语言。
4. **附带示例** - 展示真实、可实践的使用方式。
5. **经过测试** - 在 Claude.ai、Claude Code 与/或 API 中验证功能。
6. **安全可靠** - 进行破坏性操作前需二次确认。
7. **跨平台可移植** - 在适用时应兼容所有 Claude 平台。

## 技能结构
创建以技能名命名的新文件夹（使用小写与短横线）：

```
skill-name/
└── SKILL.md
```

## SKILL.md 模板
请使用下列模板提供技能说明：

```markdown
---
name: skill-name
description: 简短说明技能的作用与适用场景。
---

# Skill Name

详细描述技能帮助用户完成的工作。

## 何时使用

- 使用场景 1
- 使用场景 2
- 使用场景 3

## 本技能能做什么

1. **能力 1**：描述
2. **能力 2**：描述
3. **能力 3**：描述

## 如何使用

### 基础用法

```
简单示例提示
```

### 高级用法

```
更复杂的示例提示与选项
```

## 示例

**用户**：“示例提示”

**输出**：
```
展示技能生成的内容
```

**灵感来自：** [如适用，注明来源或人物]

## 小贴士

- 提示 1
- 提示 2
- 提示 3

## 常见使用场景

- 场景 1
- 场景 2
- 场景 3
```

## 将技能加入 README
1. 选择合适的分类（商务与营销 / 沟通与写作 / 创意与多媒体 / 开发 / 生产力与组织）。
2. 在该分类中按字母顺序添加词条：

```markdown
- [Skill Name](./skill-name/) - 一句话说明技能作用。灵感来源 [Person/Source]。
```

3. 严格遵循现有格式（无表情符号、统一标点）。

## Pull Request 流程
1. Fork 本仓库
2. 创建分支：`git checkout -b add-skill-name`
3. 添加技能文件夹与 `SKILL.md`
4. 在 `README.md` 中对应分类添加技能
5. 提交更改：`git commit -m "Add [Skill Name] skill"`
6. 推送到 Fork：`git push origin add-skill-name`
7. 提交 Pull Request

## PR 指南
你的 PR 应包含：
- **标题**：“Add [Skill Name] skill”
- **说明**：解释真实用例，并包括以下信息：
  - 解决了什么问题
  - 谁在使用此工作流
  - 出处/灵感来源
  - 示例用法

## 行为准则
- 保持尊重与建设性
- 认可原作者与灵感来源
- 聚焦实用、有帮助的技能
- 撰写清晰、易懂的文档
- 在提交前测试技能

## 有问题？
如需贡献指导或结构建议，请提交 Issue 询问。

## 归属说明
基于他人物的流程时，请在说明中指出：

```markdown
**灵感来自：** [Person Name] 的工作流
```

或

```markdown
**致谢：** 基于 [Company/Team] 的流程
```

例如：
- **灵感来自：** Dan Shipper 的会议分析流程
- **灵感来自：** Teresa Torres 的内容调研过程
- **致谢：** 基于 Notion 的文档工作流

## 技能分类
### 商务与营销
面向客户开发、竞争研究、品牌与商务拓展的技能。

### 沟通与写作
改善沟通、分析对话与创作内容的技能。

### 创意与多媒体
处理图像、视频、音频等创意内容的技能。

### 开发
涵盖软件开发、文档与技术工作流的技能。

### 生产力与组织
整理文件、任务管理与个人效率的技能。

---

## 🇺🇸 English

# Contributing to Awesome Claude Skills

Thank you for your interest in contributing to the premier collection of Claude Skills! This guide will help you add new skills that benefit the entire Claude community.

## Before You Start

- Ensure your skill is based on a **real use case**, not a hypothetical scenario.
- Search existing skills to avoid duplicates.
- If possible, attribute the use case to the original person or source.

## Skill Requirements

All skills must:

1. **Solve a real problem** - Based on actual usage, not theoretical applications.
2. **Be well-documented** - Include clear instructions, examples, and use cases.
3. **Be accessible** - Written for non-technical users when possible.
4. **Include examples** - Show practical, real-world usage.
5. **Be tested** - Verify the skill works across Claude.ai, Claude Code, and/or API.
6. **Be safe** - Confirm before destructive operations.
7. **Be portable** - Work across Claude platforms when applicable.

## Skill Structure

Create a new folder with your skill name (use lowercase and hyphens):

```
skill-name/
└── SKILL.md
```

## SKILL.md Template

Use this template for your skill:

```markdown
---
name: skill-name
description: One-sentence description of what this skill does and when to use it.
---

# Skill Name

Detailed description of the skill and what it helps users accomplish.

## When to Use This Skill

- Bullet point use case 1
- Bullet point use case 2
- Bullet point use case 3

## What This Skill Does

1. **Capability 1**: Description
2. **Capability 2**: Description
3. **Capability 3**: Description

## How to Use

### Basic Usage

```
Simple example prompt
```

### Advanced Usage

```
More complex example prompt with options
```

## Example

**User**: "Example prompt"

**Output**:
```
Show what the skill produces
```

**Inspired by:** [Attribution to original source, if applicable]

## Tips

- Tip 1
- Tip 2
- Tip 3

## Common Use Cases

- Use case 1
- Use case 2
- Use case 3
```

## Adding Your Skill to README

1. Choose the appropriate category:
   - Business & Marketing
   - Communication & Writing
   - Creative & Media
   - Development
   - Productivity & Organization

2. Add your skill in alphabetical order within the category:

```markdown
- [Skill Name](./skill-name/) - One-sentence description. Inspired by [Person/Source].
```

3. Follow the existing format exactly - no emojis, consistent punctuation.

## Pull Request Process

1. Fork the repository
2. Create a branch: `git checkout -b add-skill-name`
3. Add your skill folder with SKILL.md
4. Update README.md with your skill in the appropriate category
5. Commit your changes: `git commit -m "Add [Skill Name] skill"`
6. Push to your fork: `git push origin add-skill-name`
7. Open a Pull Request

## Pull Request Guidelines

Your PR should:

- **Title**: "Add [Skill Name] skill"
- **Description**: Explain the real-world use case and include:
  - What problem it solves
  - Who uses this workflow
  - Attribution/inspiration source
  - Example of how it's used

## Code of Conduct

- Be respectful and constructive
- Credit original sources and inspirations
- Focus on practical, helpful skills
- Write clear, accessible documentation
- Test your skills before submitting

## Questions?

Open an issue if you have questions about contributing or need help structuring your skill.

## Attribution

When adding a skill based on someone's workflow or use case, include proper attribution:

```markdown
**Inspired by:** [Person Name]'s workflow
```

or

```markdown
**Credit:** Based on [Company/Team]'s process
```

Examples:
- **Inspired by:** Dan Shipper's meeting analysis workflow
- **Inspired by:** Teresa Torres's content research process
- **Credit:** Based on Notion's documentation workflow

## Skill Categories

### Business & Marketing
Skills for lead generation, competitive research, branding, and business development.

### Communication & Writing
Skills for improving communication, analyzing conversations, and creating content.

### Creative & Media
Skills for working with images, videos, audio, and creative content.

### Development
Skills for software development, documentation, and technical workflows.

### Productivity & Organization
Skills for organizing files, managing tasks, and personal productivity.

---

Thank you for contributing to Awesome Claude Skills!
