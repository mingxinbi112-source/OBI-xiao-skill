# OBI-xiao-skill · 我的 AI 技能库

> OBI 的开源技能库，中文名「**我的 AI 技能库**」。
> 首发阵容:**卡兹克 12 核心 Prompt 技能化**——把「可粘贴的提示词」升级为「可安装、可复用、可沉淀」的 Agent 技能。
> 别人给模板，我们给系统——5 大场景 12 个剖析动作 + 1 套认知操作系统，覆盖从混沌到行动的整条链路。

**状态:v1.0 稳定版(2026-08-29)。15 个技能 + 黑洞可视化官网，一条命令装全家。**

## 命名三层

```
OBI-xiao-skill / 我的AI技能库   ← 总库(本仓库)
└── 12 个思考框架              ← 系列(问清问题/学习/解决问题/决策/认识自己 5 大场景)
    └── socratic-questioning    ← 件:具体技能
```

以后新的系列进同一个库，安装命令永远不变。对你的 agent 说「苏格拉底式提问」，或直接粘一个场景，即可唤起。

## 为什么有这套技能

市面的 Prompt 收藏夹有一个根病:**收藏即遗忘**——模板躺在收藏夹里，遇到问题想不起来用。这套库把 12 个核心 Prompt 技能化，每个技能都是「触发信号 → 思考动作 → 输出格式」的完整闭环：

- **场景前置**：每个技能写清「何时触发」，任务进来先定位场景，再选对应动作
- **反方辩手**：先质疑假设、找盲区、压力测试，不当 yes-man
- **先验证再构建**：问清问题排第一——一切执行从澄清开始
- **沉淀闭环**：用过的剖析动作遇到新坑 → 回写 pitfalls；发现新模式 → 新增技能

## 十五件套(v1.0)

| 场景 | Skill | 干什么 |
|---|---|---|
| 启动 | `core-framework` | 核心工作框架：四条铁律 + 12 动作索引，每次会话的启动协议 |
| 问清问题 | `socratic-questioning` | 苏格拉底式问诊：≤6 个追问，把表层问题收敛为真正值得回答的问题 |
| 学习 | `dual-layer-explanation` | 双层解释法：小白层给直觉、专业层给机制，杜绝「好像懂了」 |
| 学习 | `reverse-decomposition` | 反向拆解：从优秀成品逆向学「为什么有效」，提炼可迁移规律 |
| 学习 | `cross-axis-research` | 横纵分析法：历史演化 ✕ 横向对比，半小时搞懂陌生领域 |
| 学习 | `fact-check` | 事实核查：先怀疑一切，再分级标记可信度 |
| 解决问题 | `expert-panel` | 专家会诊：3 个互补视角互相挑战，真正的信息在分歧里 |
| 解决问题 | `first-principles` | 第一性原理：抛开惯例，从基本事实/目标/约束重新推导 |
| 解决问题 | `cross-domain-solution` | 跨领域借解：你的问题可能在其他行业已被解决十几年 |
| 决策 | `steelman-argument` | 双向钢人论证：摆全双方最强论证，找到真正分歧与关键变量 |
| 决策 | `minimal-experiment` | 最小实验：纸上谈兵不会更清晰时，用现实反馈验证最关键假设 |
| 认识自己 | `talent-mining` | 天赋挖掘：天赋藏在怪癖/缺点/嫉妒/能量模式里，反宿命论 |
| 认识自己 | `life-design` | 人生设计术：看清位置 → 指南针 → 三个五年版本 → 原型行动 |
| 合集 | `prompt-dozen` | 12 个 Prompt 模板合集：全部可直接复制粘贴给任意 AI |
| 企业级 | `fde-ai-b2b-delivery` | AI 企业级 FDE 交付方法论：四阶段工作流 + Go/Hold/No-Go 关卡 + 14 个 references playbook |

## 仓库结构

```text
.
├── README.md                    # 本文件(总览)
├── index.html                   # GitHub Pages 官网(黑洞可视化)
├── assets/                      # 官网星空背景图
├── docs/
│   ├── 12-prompt-methods.md     # 12 个剖析动作详解(内化手册)
│   ├── core-agent.md            # Agent 工作协议
│   ├── core-soul.md             # Agent 核心灵魂(四条铁律)
│   └── format-spec.md           # SKILL.md 格式规范(贡献者必读)
└── skills/                      # 15 个技能(每个一个 SKILL.md)
    ├── core-framework/
    ├── socratic-questioning/
    ├── ...                      # 详见上表
    └── fde-ai-b2b-delivery/
        └── references/          # 14 个深入 playbook
```

## 两种用法

**方式一:直接复制(零依赖)**
打开任意技能的 `SKILL.md`，把 `【】` 占位符换成你的信息，复制 `## Prompt 模板` 里的整段代码块，粘贴给任意 AI 即可。

**方式二:装成 Agent 技能(推荐)**

```bash
npx -y skills add mingxinbi112-source/OBI-xiao-skill -g --all
```

装好后对你的 agent 说「苏格拉底式提问」「帮我拆解这个」或「做个最小实验」，它会自动加载对应技能。

## 在线页面

黑洞可视化官网:https://mingxinbi112-source.github.io/OBI-xiao-skill/

## Roadmap

- 更多场景:写作 / 沟通 / 项目管理方向的剖析动作
- 与 Hermes 等 Agent 环境深度打通(触发词自动路由)
- 英文版 README 与技能说明
- 每个技能沉淀个人实践 pitfalls(用过的坑回写)

## License

12 个核心 Prompt 版权归原作者卡兹克(公众号「卡兹克」)所有，本文库为整理与技能化改编，仅供个人学习使用；仓库代码(官网)MIT，文档与方法论 CC BY-NC 4.0。详见 [LICENSE.md](LICENSE.md)。

---

*来源:卡兹克《都 Agent 时代了，我还是想分享给你这12个我最常用的Prompt》(2026-08，公众号「卡兹克」)。这套技能不是设计出来的，是 obi_xiao 在真实工作里一次次被纠偏调出来的——每条铁律都来自一次翻车。*
