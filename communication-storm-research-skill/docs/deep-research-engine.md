# 深度文献调研引擎（Deep Research Engine）

> 编纂：**西南交通大学 传播系 黄昕恺，Ph.D in Communication from University of Utah**
>
> 本文件把 `SKILL.md` 第 4 步"检索计划"从口号升级为可操作的检索工程。配合 `docs/hot-topics-2024-2026.md`（热点坐标）与 `docs/method-design-deep.md`（方法落地）使用。**凡涉及具体期刊收录/分区，须联网核实，不得凭记忆罗列。**

---

## 1. 分层期刊地图（传播学本体 + 六个交叉学科）

下表是**检索起点清单**，不是权威认定。`收录` 与 `分区` 一栏标注的是"通常归属"，**学生必须以 Web of Science Master Journal List、CSSCI 来源期刊目录、中科院文献情报中心分区表的当年版本核实**后使用。

| 学科域 | 代表期刊（需核实收录/分区） | 通常收录 | 传播学硕士的切入价值 |
|---|---|---|---|
| 传播学本体（国际） | Journal of Communication; Communication Research; New Media & Society; Journal of Computer-Mediated Communication; Human Communication Research; Information, Communication & Society; Political Communication; Social Media + Society; International Journal of Communication | SSCI（多为 Q1） | 理论与方法标杆，看 gap 与对话 |
| 传播学本体（中文） | 《新闻与传播研究》《国际新闻界》《现代传播》《新闻大学》《新闻记者》《编辑之友》 | CSSCI | 本土议题、可投稿坐标 |
| 社会学 | American Journal of Sociology; Social Forces; Sociology;《社会学研究》《社会》 | SSCI / CSSCI | 身份、社群、不平等、结构 |
| 心理学（社会/媒介） | Computers in Human Behavior; Cyberpsychology, Behavior, and Social Networking; Journal of Social and Personal Relationships;《心理学报》 | SSCI / CSSCI | 量表、机制、中介调节模型 |
| AI / 计算传播 / HCI | Big Data & Society; CHI / CSCW Proceedings; Journal of Quantitative Description: Digital Media; New Media & Society（计算专题） | SSCI / 顶会 | 平台数据、文本挖掘、网络分析 |
| 市场营销 / 消费者 | Journal of Consumer Research; Journal of Advertising; Journal of Interactive Advertising; Journal of Marketing | SSCI（多 Q1/FT50） | 品牌关系、说服、购买意愿 |
| 文旅 / 旅游 | Tourism Management; Annals of Tourism Research; Journal of Travel Research; Mobilities | SSCI（多 Q1） | 城市形象、目的地营销、流动性 |
| 教育学 | Computers & Education; British Journal of Educational Technology;《电化教育研究》 | SSCI / CSSCI | 学习行为、知识传播、素养 |

> 建议：每个核心概念至少在**本体刊 + 1 个交叉学科刊**各找到高质量来源；交叉学科文献用于借理论与方法，本体刊用于定位对话。

---

## 2. 数据库高级检索语法速查（以示范主题"短视频 + 怀旧 + 认同"为例）

- **Web of Science**：`TS=(("short video" OR TikTok OR Douyin) AND (nostalgia OR "collective memory") AND (identif* OR identity))`。用 `Citing Articles / Cited References` 做前/后向滚雪球。
- **Scopus**：`TITLE-ABS-KEY(("short video") AND (nostalgia) AND (identity))`，可按 `Subject area` 限定到 SOCI/PSYC/BUSI。
- **CNKI 高级检索**：主题/篇关摘 = `短视频 * (怀旧 + 集体记忆) * 认同`；用"来源类别"勾选 CSSCI；用"引证文献/参考文献"追链。
- **EBSCO Communication & Mass Media Complete (CMMC)**：`(short video) AND (nostalg*) AND (identity)`，限定 `Scholarly (Peer Reviewed)`。
- **Google Scholar**：`"short video" nostalgia identity`，用 `Cited by` 与年份过滤近两年；用 `允许引用格式` 导出但仍需回原库核实。
- **语义检索（找邻近文献）**：Semantic Scholar、Connected Papers、Research Rabbit、Litmaps——输入一篇种子论文，自动给出引用网络，**用于发现遗漏的关键文献，不能替代正式检索**。

---

## 3. 选题逆向工程（从已发表论文反推可执行选题）

这是本引擎价值最高的部分。不要先拍脑袋想题目，而是从近 2–3 年高质量论文里反推：

**四步法**
1. **锁定**：在目标期刊找 3–5 篇高相关近作。
2. **拆 Introduction 末段**：它加入了哪个**理论对话**？它声称的 **gap** 是什么（"然而，鲜有研究……"）？
3. **拆 Discussion / Limitations / Future Research**：它**自己留了什么口子**——对象、情境/平台、方法、变量、机制？
4. **增量四问**生成候选题：换**对象**？换**情境/平台**？补**缺失的证据端**（只做文本→补用户端）？把**现象拆成机制**？

**走查示例（用本包既有案例"年代剧共情"演示动作；不引用具体文献）**：
- 检索 *New Media & Society* / 《国际新闻界》近年关于"怀旧、媒介记忆、叙事共情"的实证文。
- 观察它们**怎么操作化"共情"**（共情量表 vs 评论情感编码），**留了什么口子**（多做文本少做用户端；多欧美剧少中国年代剧）。
- 学生的增量随即清晰：对象增量（中国年代剧）+ 证据增量（补弹幕/评论用户端）+ 机制增量（把"共情"拆成叙事触发点→用户表达→认同）。
- 这比"年代剧为什么让人共情"执行力强一个量级。

> 配合 `docs/hot-topics-2024-2026.md`：先用热点库选领域，再用本节四步在该领域内逆向出题。

---

## 4. 两个评分 rubric

**来源质量（沿用"来源等级 1–4"）**

| 等级 | 类型 | 识别特征 | 可用于论文 | 边界 |
|---|---|---|---|---|
| 1 | 同行评议论文/专著 | 有方法、有同行评议 | 理论、方法、发现 | 主力，越近越好 |
| 2 | 官方/平台透明度报告 | 政府、平台官方 | 背景、政策、数据 | 不可替代理论文献 |
| 3 | 行业报告/数据平台 | 咨询机构、数据库 | 行业背景、量级 | 注意立场与口径 |
| 4 | 媒体报道/社媒文本 | 新闻、帖子、弹幕 | 现象佐证、研究对象 | 仅作语境/对象，不作论据 |

**选题可执行性（0–100，建议维度与权重）**：对象具体度(15)、问题可回答性(20)、概念可操作化(20)、方法可行性(15)、数据可获得性(15)、相对已有研究的增量(10)、伦理风险(5)。每维度给优秀/及格/不及格判据，低于 60 分先缩小再做。

---

## 5. 引文链滚雪球协议

- **后向**（读参考文献找经典）：从 1–2 篇高相关近作的参考文献里，找被反复引用的奠基理论与量表。
- **前向**（用"被引"找最新）：用 WoS/Scopus/Scholar 的"被引"功能，找引用了奠基作的近两年新作。
- **停止判据**：新检索不再带来新概念、新理论、新方法时，视为饱和。

> 一般硕士前期：核心文献 ≥ 30 篇，中英文兼有，每篇做证据卡。
