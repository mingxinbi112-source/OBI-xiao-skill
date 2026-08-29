# SKILL.md 格式规范

> 本文件供贡献者/维护者阅读。所有技能统一为**标准 Markdown**，结构如下:

```
---
name: skill-name                 # frontmatter(元信息)
description: 一句话描述此技能用途(含场景)
whenToUse: 何时使用此技能
---

# 技能中文名

> 一句话简介

## 何时使用
(何时触发)

## 使用方法
(怎么用)

## Prompt 模板

```text
(完整 Prompt，可直接复制给 AI，用【】占位符)
```
```

**统一要点**:

- 所有技能都有 `frontmatter`(name / description / whenToUse)
- 所有技能正文都有 `## 何时使用` 分节
- Prompt 模板一律用 ` ```text ` 代码块包裹(方便一键复制)
- 长技能(life-design / talent-mining)用完整角色指令，多轮对话式
- 合集(prompt-dozen)内含 12 个模板，每个模板都是独立代码块
- 例外:`fde-ai-b2b-delivery` 是**方法论型技能**(不是填空式 Prompt)，正文是四阶段交付工作流 + Go/No-Go 关卡，并带 `references/` 子目录存放 14 个深入 playbook，用相对路径在正文引用

## 如何更新 / 新增技能

```bash
# 新增:在 skills/ 下新建文件夹，里面放 SKILL.md(遵循上面的格式规范)
mkdir -p skills/my-new-skill

# 编辑 skills/my-new-skill/SKILL.md，然后提交推送
git add -A
git commit -m "添加新技能:my-new-skill"
git push
```
