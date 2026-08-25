# OBI Skill Hub · 我的 AI 技能库

> 作者：obi_xiao（OBI）· GitHub: [mingxinbi112-source](https://github.com/mingxinbi112-source)
> 一句话：我反复使用、真正帮我解决问题的 12 个思考框架，整理成 14 个思考技能 + 1 个 FDE 企业级交付方法论（共 15 个可复用技能）。

## 📦 这是什么

15 个可复用技能：14 个思考框架覆盖 **5 大场景**（问清问题 · 学习 · 解决问题 · 决策 · 认识自己），另有 1 个 **FDE 企业级 AI 交付方法论**（AI 在企业/B 端怎么真正落地、Go/No-Go 评估、权限禁区、决策闭环）。
每个技能是独立的 `SKILL.md`，**全部用标准 Markdown 书写**，Prompt 模板用 ``` 代码块包裹（一键复制、不丢格式）。

## 🗂 目录结构

```
.
├── README.md              # 本文件（总览 + 格式规范）
├── index.html             # GitHub Pages 官网首页（黑洞可视化）
├── assets/                # 背景图等资源
├── docs/                  # 核心文档
│   ├── 12-prompt-methods.md   # 12 个剖析动作详解
│   ├── core-agent.md          # Agent 工作协议
│   └── core-soul.md           # Agent 核心灵魂
└── skills/                # 15 个技能（每个一个 SKILL.md）
    ├── core-framework/        # 核心思考与工作框架（启动协议）
    ├── socratic-questioning/  # 苏格拉底式提问
    ├── dual-layer-explanation/# 双层解释法
    ├── cross-axis-research/   # 横纵分析法
    ├── reverse-decomposition/ # 反向拆解
    ├── fact-check/            # 事实核查
    ├── expert-panel/          # 专家会诊
    ├── first-principles/      # 第一性原理
    ├── cross-domain-solution/ # 跨领域借解
    ├── steelman-argument/     # 双向钢人论证
    ├── minimal-experiment/    # 最小实验
    ├── talent-mining/         # 深度天赋挖掘
    ├── life-design/           # 人生设计术
    ├── prompt-dozen/          # 12 个 Prompt 模板合集
    └── fde-ai-b2b-delivery/   # AI 企业级 FDE 交付方法论（SKILL.md + references/）
```

## 📝 格式规范（所有 SKILL.md 统一）

每个技能都是**标准 Markdown**，结构如下：

```markdown
---
name: skill-name                 # frontmatter（元信息）
description: 一句话描述此技能用途（含场景）
whenToUse: 何时使用此技能
---

# 技能中文名

> 一句话简介

## 何时使用
（何时触发）

## 使用方法
（怎么用）

## Prompt 模板

```text
（完整 Prompt，可直接复制给 AI，用【】占位符）
```
```

**统一要点**：
- 所有技能都有 `frontmatter`（name / description / whenToUse）
- 所有技能正文都有 `## 何时使用` 分节
- Prompt 模板一律用 ` ```text ` 代码块包裹（方便一键复制）
- 长技能（life-design / talent-mining）用完整角色指令，多轮对话式
- 合集（prompt-dozen）内含 12 个模板，每个模板都是独立代码块
- 例外：`fde-ai-b2b-delivery` 是**方法论型技能**（不是填空式 Prompt），正文是四阶段交付工作流 + Go/No-Go 关卡，并带 `references/` 子目录存放 15 个深入 playbook，用相对路径在正文引用。

## 🚀 如何使用

1. 打开任意技能的 `SKILL.md`；
2. 把 `【】` 里的占位符换成你自己的信息；
3. 复制 `## Prompt 模板` 里的整段（代码块），粘贴给任意 AI 使用。

## 🛠 如何更新 / 新增技能

```bash
# 新增：在 skills/ 下新建文件夹，里面放 SKILL.md（遵循上面的格式规范）
mkdir -p skills/my-new-skill
# 编辑 skills/my-new-skill/SKILL.md

# 提交并推送
git add -A
git commit -m "添加新技能：my-new-skill"
git push
```

## 🌐 在线页面

GitHub Pages 官网（黑洞可视化首页）：https://mingxinbi112-source.github.io/OBI-xiao-skill/

## 📄 许可证

个人学习使用。
