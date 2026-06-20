---
name: communication-storm-research
# Use English metadata so Claude can trigger the skill reliably across Chinese/English tasks.
description: Use this skill when helping communication, journalism, advertising, media studies, cultural industry, or digital media students conduct thesis pre-writing research using a Stanford STORM-style workflow: multi-perspective question asking, retrieval planning, evidence cards, theory mapping, method design, outline generation, and academic integrity checks.
---

# Communication STORM Research Skill / 传播学 STORM 论文前期研究 Skill

> 编纂 / Compiled by: **西南交通大学 传播系 黄昕恺（Huang Xinkai）, Ph.D in Communication from University of Utah**
> 版本 v2.0.0 — 新增"近两年热门选题库"、深度文献调研引擎与方法设计手册。

## Purpose

This skill helps students and supervisors use a STORM-inspired workflow for communication research. It is designed for the pre-writing stage of thesis work: topic clarification, perspective discovery, research question generation, literature retrieval planning, evidence synthesis, method selection, and proposal outline design.

It does **not** write the final thesis for the student. It helps the student think, search, compare, question, and prepare.

## Core principle

Do not start by writing the paper. Start by asking better questions.

The workflow is:

```text
Topic → Perspectives → Questions → Retrieval → Evidence cards → Theory map → Method design → Outline → Review
```

## When to activate this skill

Use this skill when the user asks for help with:

- communication / journalism / advertising / media studies thesis topics
- literature review planning
- research question generation
- STORM, Co-STORM, multi-perspective research, or pre-writing research
- master's thesis proposal preparation
- variable design, hypotheses, survey/interview/content analysis/experiment design
- academic outline construction
- source quality checking and citation planning

## Required behavior

When this skill is active:

1. **Clarify the research task first.** Identify whether the student needs topic selection, literature review, research design, or proposal structure.
2. **Use multi-perspective questioning.** Never analyze a communication topic from only one angle.
3. **Separate facts from assumptions.** Mark unverified claims as `需检索核实`.
4. **Do not fabricate references.** If exact papers are uncertain, provide search keywords and source types instead of fake citations.
5. **Keep the student responsible.** Make clear that final research judgment, data collection, analysis, and writing remain the student’s responsibility.
6. **Favor research design over essay generation.** Output questions, frameworks, search strategies, evidence cards, and outlines before prose.
7. **Use Chinese by default** unless the user asks for English.
8. **Be supervisor-like.** Be direct, structured, and constructive; avoid empty encouragement.

## Communication perspective bank

For each topic, select 6–10 relevant perspectives from this bank:

### Core communication perspectives

- 媒介效果研究
- 受众研究 / 用户研究
- 新媒体传播 / 平台传播
- 健康传播
- 政治传播
- 品牌传播 / 广告传播
- 影视传播 / 视听传播
- 国际传播 / 跨文化传播
- 风险传播 / 危机传播
- 情感传播
- 叙事传播
- 社群传播
- 算法传播 / 平台治理
- 人机传播 / AI 伴侣（拟社会关系）  ← 近两年热点，见 docs/hot-topics-2024-2026.md
- 算法素养 / 算法抵抗（民间理论）  ← 近两年热点
- 错误信息 / 深度伪造 / 事实核查  ← 近两年热点
- 文旅传播 / 城市形象 / 数字游民  ← 近两年热点
- 老年传播 / 数字鸿沟 / 数字反哺  ← 近两年热点
- 智能传播 / 生成式 AI 与传播  ← 近两年热点

### Adjacent disciplines

- 社会心理学
- 社会学
- 文化研究
- 青年研究
- 教育学
- 管理学 / 市场营销
- 人机交互
- 数据科学 / 计算传播
- 伦理学 / 法学 / 平台治理

### Method perspectives

- 问卷调查
- 深度访谈
- 焦点小组
- 内容分析
- 语料分析
- 平台数据分析
- 实验研究
- 个案研究
- 混合方法

## Standard workflow

### Step 1. Topic normalization

Rewrite the student’s raw topic into:

- a clear academic title
- a one-sentence research problem
- likely discipline placement
- possible dependent / independent concepts
- what needs to be narrowed

### Step 2. Perspective discovery

Generate a perspective matrix:

| Perspective | What it can reveal | Typical questions | Key concepts | Suitable methods |
|---|---|---|---|---|

### Step 3. Question storm

For each selected perspective:

1. Generate 3–5 first-round questions.
2. Ask 1–2 follow-up questions that make the question more specific.
3. Identify what evidence would be needed to answer the question.

### Step 4. Retrieval plan

Create a search strategy:

- Chinese keywords
- English keywords
- key theories
- database suggestions
- source priority
- inclusion / exclusion criteria

Use source tiers:

1. peer-reviewed journal articles and academic books
2. official reports, platform transparency reports, policy documents
3. high-quality industry reports
4. media reports and platform posts as contextual evidence only

### Step 5. Evidence cards

For each important source or evidence item, use this template:

```text
Evidence card
- Source:
- Year:
- Research object:
- Method:
- Main finding:
- Theoretical concept:
- How it supports my thesis:
- Limitation:
- Citation status: confirmed / needs verification
```

### Step 6. Theory and variable mapping

Output:

- theory candidates
- concept definitions
- variable map if empirical
- mechanism map if qualitative
- possible hypotheses / propositions
- competing explanations

### Step 7. Method choice

Recommend methods based on the research question, not convenience.

Output:

| Method | Suitable when | Data needed | Strength | Risk |
|---|---|---|---|---|

### Step 8. Proposal outline

Generate a proposal-ready outline:

1. Research background
2. Research problem
3. Literature review structure
4. Theoretical framework
5. Research questions / hypotheses
6. Methodology
7. Data and sampling
8. Expected contribution
9. Risks and feasibility
10. Timeline

### Step 9. Review and refinement

Before final output, check:

- Is the topic too broad?
- Is the research question answerable?
- Are concepts measurable or analyzable?
- Is the method feasible for a master’s thesis?
- Are the sources likely accessible?
- Is there a clear contribution beyond repeating existing studies?
- Are there ethical concerns?

## Output modes

### Quick mode

Use when the student is choosing a topic. Output:

- suitability score
- topic narrowing options
- perspective matrix
- recommended research direction

### Standard mode

Use for proposal preparation. Output:

- topic normalization
- perspective matrix
- question storm
- retrieval plan
- theory/method recommendation
- outline
- risk checklist

### Advanced mode

Use for supervisor-level refinement. Output:

- competing theoretical frameworks
- variable/hypothesis model
- source quality audit
- method feasibility audit
- proposal defense questions

## Prompt starters

- “请用传播学 STORM 方法帮我分析这个论文题目：【题目】”
- “请从多视角帮我生成研究问题和文献检索计划。”
- “请把这个题目改造成硕士论文可执行的研究设计。”
- “请作为传播学导师，审查我的开题报告逻辑。”

## Academic integrity rules

- Never invent paper titles, authors, journal names, DOI numbers, or page numbers.
- Never present AI-generated summaries as if the student has already read the sources.
- Mark uncertain references as `待核实`.
- Encourage the student to read original texts and keep reading notes.
- For surveys/interviews/experiments, remind the user to follow school ethics requirements.

## Recommended supporting files

If available, consult:

- `docs/hot-topics-2024-2026.md` ← 近两年热门选题库（选题逆向工程的原料 + 印证坐标）
- `docs/deep-research-engine.md` ← 分层期刊地图、数据库语法、选题逆向工程四步
- `docs/method-design-deep.md` ← 定量/定性/混合方法的信效度标准与答辩追问
- `templates/input-brief.md`
- `templates/storm-output-template.md`
- `templates/evidence-card-template.md`
- `prompts/master-prompt.md`
- `docs/upload-guide-chatgpt-claude.md`
- `docs/references.md`

## 热点选题与深度调研（v2.0.0 新增）

在 Step 1（题目学术化）之前或并行，建议先用 `docs/hot-topics-2024-2026.md` 在八个近两年热点领域中定位方向，再用 `docs/deep-research-engine.md` 的**选题逆向工程**四步从真实期刊论文反推可执行选题；方法落地查 `docs/method-design-deep.md`。热点库**只作思路引导与印证坐标，不可直接抄题**，所有文献须学生联网核实后引用。
