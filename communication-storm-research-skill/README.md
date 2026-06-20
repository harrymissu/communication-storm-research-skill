# Communication STORM Research Skill / 传播学 STORM 论文前期研究 Skill

> 编纂 / Compiled by: **西南交通大学 传播系 黄昕恺（Huang Xinkai）, Ph.D in Communication from University of Utah**
> **v2.0.0** — 新增近两年热门选题库、深度文献调研引擎与方法设计手册。

一个面向传播学、新闻学、广告学、新媒体、文化产业与数字媒体方向硕士生的论文前期研究 Skill。

它借鉴 Stanford STORM 的核心思路：**先从多视角生成好问题，再进行资料检索、证据整理和大纲建构**。本 Skill 的目标不是替学生写论文，而是帮助学生更快完成选题澄清、文献综述准备、研究问题生成、方法设计和开题报告结构化。

## 适用对象

- 传播学 / 新闻传播学 / 广告学 / 网络与新媒体硕士生
- 正在准备开题报告的学生
- 需要训练学生论文前期研究能力的导师
- 需要把 AI 用于学术研究准备，而不是代写论文的课程团队

## 核心工作流

```text
Topic → Perspectives → Questions → Retrieval → Evidence Cards → Theory Map → Method Design → Outline → Review
```

## 文件结构

```text
communication-storm-research-skill/
├── SKILL.md
├── README.md
├── prompts/
│   ├── master-prompt.md
│   ├── chatgpt-project-instructions.md
│   └── proposal-defense-prompt.md
├── templates/
│   ├── input-brief.md
│   ├── storm-output-template.md
│   ├── evidence-card-template.md
│   └── thesis-prep-checklist.md
├── examples/
│   ├── social-media-loneliness.md
│   ├── xiaohongshu-community-identity.md
│   ├── period-drama-user-identity.md
│   ├── ai-companion-loneliness.md            (v2.0.0 热点)
│   ├── digital-nomad-city-tourism.md         (v2.0.0 热点)
│   └── algorithm-literacy-resistance.md      (v2.0.0 热点)
├── docs/
│   ├── hot-topics-2024-2026.md               (v2.0.0 近两年热门选题库)
│   ├── deep-research-engine.md               (v2.0.0 深度文献调研引擎)
│   ├── method-design-deep.md                 (v2.0.0 方法设计手册)
│   ├── upload-guide-chatgpt-claude.md
│   └── references.md
└── rubrics/
    └── proposal-quality-rubric.md
```

## 最简单安装路径

### Claude Code

1. 解压本文件夹。
2. 放入：`~/.claude/skills/communication-storm-research/`
3. 重启 Claude Code。
4. 输入：`请用 communication-storm-research skill 分析我的论文题目：……`

### Claude.ai / Claude 项目

如果账号界面支持 Skills，可在 Skills / Customize 中安装该文件夹。  
如果没有 Skills 入口，最简单路径是：创建一个 Claude Project → 上传本文件夹中的 `SKILL.md`、`README.md`、`templates` 和 `prompts` → 把 `prompts/master-prompt.md` 作为项目指令使用。

### ChatGPT Projects

1. 新建 Project。
2. 将 `prompts/chatgpt-project-instructions.md` 粘贴为项目指令。
3. 上传 `SKILL.md`、`README.md`、`templates`、`examples` 和 `docs/references.md`。
4. 在项目中输入论文题目开始使用。

### Custom GPT

1. 打开 GPTs → Create。
2. Instructions 粘贴 `prompts/chatgpt-project-instructions.md`。
3. Knowledge 上传本文件夹中的 Markdown 文件。
4. 开启 Web Search（用于检索最新文献线索）和 Code Interpreter（如需数据分析）。
5. 在 Preview 中测试。

## 重要边界

- 不生成虚假文献。
- 不替学生完成最终论文。
- 不替代导师判断。
- 不替代真实文献阅读、数据采集和伦理审查。

## 推荐使用方式

```text
请用传播学 STORM 方法，帮我对以下硕士论文题目做前期研究设计：
【题目】

请输出：多视角矩阵、研究问题、文献检索关键词、理论框架、方法建议、开题报告大纲和风险提示。
```
