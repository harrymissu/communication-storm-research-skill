 Communication STORM Research Skill / 传播学 STORM 论文前期研究 Skill

面向传播学、新闻传播学、媒介研究、广告与品牌传播、健康传播、文旅传播、计算传播等方向的硕士论文前期研究 Skill 包。

它基于 Stanford STORM 方法论，将论文写作前的“选题—文献—问题—证据—方法—答辩”整理成一套可执行工作流，帮助学生从一个模糊选题，逐步形成可开题、可检索、可答辩的研究设计。

> 本项目不是论文代写工具，而是论文前期研究训练工具。
> 核心目标：让学生在写作前，先知道该问什么、查什么、如何判断证据、如何设计方法。

---

适用对象

* 传播学 / 新闻传播学硕士生
* 本科毕业论文高阶训练
* 论文开题准备
* 文献综述训练
* 研究方法课程
* 导师组论文工作坊
* ChatGPT / Claude 学术研究 Skill 配置

---

核心能力

本 Skill 包支持以下任务：

1. **选题逆向工程**
   从近年论文的 Introduction、Discussion、Limitations 中反推可执行选题。

2. **多视角问题生成**
   从媒介效果、受众研究、平台传播、文化研究、品牌传播、计算传播等视角提出研究问题。

3. **深度文献检索**
   设计 Web of Science、Scopus、CNKI、EBSCO CMMC、Google Scholar 等检索式。

4. **Gap 类型判断**
   判断选题属于理论缺口、情境缺口、方法缺口、对象缺口还是争议缺口。

5. **证据卡片与综述矩阵**
   将文献从“摘要堆砌”整理为理论、对象、方法、变量、发现、局限和对话关系。

6. **研究方法设计**
   辅助设计问卷、内容分析、实验、访谈、文本/话语分析、计算传播和混合方法。

7. **开题答辩预审**
   模拟导师追问，检查文献深度、gap 真实性、方法可行性和学术诚信风险。

---

 完整工作流

```text
Topic
→ Topic Reverse Engineering
→ Perspectives
→ Question Storm
→ Deep Retrieval
→ Evidence Cards
→ Synthesis Grid
→ Gap Typology
→ Theory / Variable Map
→ Method Design
→ Proposal Outline
→ Defense Review
```

---

文件结构

```text
communication-storm-research-skill/
├── SKILL.md
├── README.md
├── prompts/
├── templates/
├── examples/
├── docs/
├── rubrics/
└── CHANGELOG.md
```

建议重点阅读：

```text
SKILL.md
docs/deep-research-engine.md
docs/method-design-deep.md
docs/gap-typology.md
templates/evidence-card-template.md
templates/synthesis-grid.md
rubrics/proposal-quality-rubric.md
```

---

## 最简单使用方式

### 1. 在 ChatGPT 中使用

推荐使用 **Project**：

1. 新建 ChatGPT Project；
2. 上传本 Skill 包中的 Markdown 文件；
3. 将 `SKILL.md` 或 `prompts/master-prompt.md` 的内容放入项目指令；
4. 开启联网检索；
5. 输入你的论文选题或研究兴趣。

也可以用 **Custom GPT**：

1. Create GPT；
2. 将 `SKILL.md` 放入 Instructions；
3. 将 `docs/`、`templates/`、`examples/` 上传到 Knowledge；
4. 测试输出是否遵守“零编造”和“文献核验”要求。

---

### 2. 在 Claude 中使用

推荐使用 **Claude Project** 或 **Claude Code Skills**。

Claude Project：

1. 新建 Project；
2. 上传 `SKILL.md`、`docs/`、`templates/`、`examples/`；
3. 将 `prompts/master-prompt.md` 作为项目指令；
4. 输入论文选题，让 Claude 按 STORM 工作流输出研究准备报告。

Claude Code：

```bash
mkdir -p ~/.claude/skills/communication-storm-research
cp -r communication-storm-research-skill/* ~/.claude/skills/communication-storm-research/
```

然后在 Claude Code 中调用该 Skill 处理论文前期研究任务。

---

 示例输入

```text
我的研究兴趣是：
小红书考研类博主粉丝社群中，社群认同如何影响成员粘性。

请使用传播学 STORM Skill，帮我完成：
1. 选题逆向工程；
2. gap 类型判断；
3. 多视角研究问题；
4. 文献检索式；
5. 证据卡片模板；
6. 综述矩阵；
7. 方法设计；
8. 开题答辩追问。
```

---

## 推荐检索入口

* Stanford STORM Project
  [https://storm-project.stanford.edu/research/storm/](https://storm-project.stanford.edu/research/storm/)

* STORM GitHub
  [https://github.com/stanford-oval/storm](https://github.com/stanford-oval/storm)

* Google Scholar
  [https://scholar.google.com/](https://scholar.google.com/)

* Google Scholar Help
  [https://scholar.google.com/intl/en/scholar/help.html](https://scholar.google.com/intl/en/scholar/help.html)

* Web of Science Master Journal List
  [https://mjl.clarivate.com/](https://mjl.clarivate.com/)

* Journal Citation Reports
  [https://jcr.clarivate.com/](https://jcr.clarivate.com/)

* CNKI 高级检索
  [https://kns.cnki.net/](https://kns.cnki.net/)

* CSSCI / 南京大学中国社会科学研究评价中心
  [https://cssrac.nju.edu.cn/](https://cssrac.nju.edu.cn/)

* EBSCO Communication & Mass Media Complete
  [https://about.ebsco.com/products/research-databases/communication-mass-media-complete](https://about.ebsco.com/products/research-databases/communication-mass-media-complete)

---

## 学术诚信边界

可以使用 AI 做：

* 生成检索式；
* 拆解选题；
* 提出研究问题；
* 整理证据卡片；
* 搭建综述矩阵；
* 模拟答辩追问；
* 检查方法设计漏洞。

必须由学生自己完成：

* 阅读原始文献；
* 核验作者、题名、期刊、DOI、分区；
* 判断文献是否可用；
* 解释理论与变量；
* 收集和分析数据；
* 撰写最终论文；
* 对研究结论负责。

绝对禁止：

* 编造文献；
* 编造 DOI；
* 编造访谈或问卷数据；
* 让 AI 代写正文后直接提交；
* 未核验就引用 AI 给出的文献。

---

## 适合的论文方向

* 社交媒体与用户心理
* 短视频传播
* 平台传播
* 粉丝社群与用户参与
* 品牌传播与消费行为
* 健康传播
* 文旅传播
* 影视传播与用户认同
* AI 生成内容与新闻信任
* 计算传播与平台数据研究

---

 一句话总结

**Communication STORM Research Skill** 不是让 AI 替学生写论文，而是让学生在写作之前，先完成选题、文献、问题、证据和方法的系统训练。

它帮助学生回答五个关键问题：

```text
我研究什么？
我的 gap 从哪里来？
我需要查哪些文献？
我用什么方法回答？
导师会怎样追问我？
```

## Quick Start（3分钟开始）

### ChatGPT

1. New Project
2. 上传：
   - SKILL.md
   - docs/
   - templates/
   - examples/
   - rubrics/
3. 将 SKILL.md 核心规则复制到 Project Instructions
4. 打开联网
5. 开始研究

### Claude

1. New Project
2. 上传全部文件
3. 将 SKILL.md 放入 Project Instructions
4. 开始使用

推荐研究流程：

Topic
→ Reverse Engineering
→ Question Storm
→ Retrieval
→ Evidence Cards
→ Synthesis Grid
→ Gap Typology
→ Method Design
→ Proposal Outline
→ Defense Review

 License

Recommended: MIT License or CC BY-NC 4.0.

For teaching and academic training use.
