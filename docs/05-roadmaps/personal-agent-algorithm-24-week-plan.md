# 个人学习计划：AI Agent 开发 + 算法（24 周逐日版）

> 适用对象：Agent / 大模型零基础，目标是通过跳槽进入 **Agent 开发、LLM 应用开发、RAG / Agent 算法工程**相关岗位。
>
> 计划周期：**2026-06-22 ～ 2026-12-06，共 24 周 / 168 天**。
>
> 路线权重：**Agent 开发与工程 70% + 算法、模型原理与实验 30%**。
>
> 默认投入：工作日 2～3 小时，周六 4～6 小时，周日 2～4 小时；全职学习可将一天内容压缩到半天，但不要跳过产出和验收。
>
> 当前版本：v1.0（2026-06-21）；本文件是后续计划、进度、复盘与调整的唯一事实来源。

---

## 1. 最终目标

24 周后，不以“看完多少资料”为标准，而以以下可验证成果为标准：

- 能独立解释 chatbot、workflow、agent、multi-agent、RAG、memory、context、harness、eval 的边界。
- 能手写最小 Agent Loop，并实现工具注册、结构化输出、超时、重试、trace 和权限确认。
- 能完成一个具备引用、评测、API、Docker 和 README 的 **Paper Agent 主项目**。
- 能完成一个带 Playwright、结构化观察、截图和动作轨迹的 **Web Agent 次项目**。
- 能设计至少 20 条 eval case，统计成功率、检索指标、成本、延迟和失败类型。
- 能理解 Transformer、Embedding、LoRA / QLoRA、SFT、DPO、PPO、GRPO 的核心原理。
- 完成至少 **120 道数据结构与算法题**，能独立写常见题型。
- 形成 1 页中文简历、项目架构图、3～5 分钟项目介绍、失败案例和技术博客。
- 从第 23 周开始真实投递，并根据 JD 和面试反馈迭代项目与简历。

### 建议投递岗位优先级

1. Agent 开发工程师 / LLM 应用开发工程师。
2. RAG 工程师 / 上下文工程开发工程师。
3. Agent 算法工程师 / RAG 算法工程师（项目实验足够深入后）。
4. 大模型算法工程师（若后续继续补训练、论文或相关工作经历）。

---

## 2. 执行规则

### 2.1 每天固定节奏

工作日建议采用 `20 分钟复习 + 60 分钟学习 + 60 分钟编码 + 20 分钟记录`。周末用于项目集成、评测和复盘。

每天结束前必须留下至少一种证据：

- Git commit；
- 可运行代码或测试；
- 一页结构化笔记；
- 一张架构图；
- eval 数据或实验表；
- 一道独立完成并复盘的算法题。

### 2.2 状态标记

后续同步进度时，直接修改每日表格第一列：

| 标记 | 含义 |
|:---:|:---|
| ⬜ | 未开始 |
| 🟡 | 进行中 |
| ✅ | 已完成并通过验收 |
| 🔁 | 做过但未通过验收，需要返工 |
| ⏸ | 主动暂停，必须写明原因 |

### 2.3 防止计划崩盘的规则

- 某天未完成：顺延到下一个“复盘日”，不要同时背两天债。
- 连续落后 3 天：砍掉可选阅读，保留代码、项目、算法题和复盘。
- 连续落后 7 天：本周停止新增知识，只清欠账并恢复节奏。
- 不允许只看视频不写代码；不允许复制代码后把“能运行”当成“已掌握”。
- AI 可以解释、review 和提示，但核心模块至少独立重写一次。
- 任何项目指标必须由固定测试集得到，不得凭感觉或编造。

---

## 3. AgentGuide 核心资源索引

每日计划中的 `Gxx` 均指本仓库内文档。

| 编号 | 资源 |
|:---:|:---|
| G01 | [AgentGuide 快速开始](../00-getting-started/README.md) |
| G02 | [Agent 学习地图](../00-getting-started/01-agent-map.md) |
| G03 | [前 7 天学习计划](../00-getting-started/02-first-7-days.md) |
| G04 | [什么是 AI Agent](../01-theory/01-what-is-agent.md) |
| G05 | [手撕 ReAct 框架](../01-theory/04-react-framework.md) |
| G06 | [Agent 评估指标体系](../01-theory/09-evaluation-metrics.md) |
| G07 | [RAG 全链路实战](../02-tech-stack/20-rag-full-pipeline.md) |
| G08 | [上下文工程实践](../02-tech-stack/11-context-engineering-practices.md) |
| G09 | [Agent Memory](../02-tech-stack/15-agent-memory.md) |
| G10 | [MCP 协议详解](../02-tech-stack/14-mcp-protocol.md) |
| G11 | [Agent Harness Engineering](../02-tech-stack/27-agent-harness-engineering.md) |
| G12 | [Agent 评估完全指南](../02-tech-stack/agent-evaluation-complete-guide.md) |
| G13 | [Evaluation Harness 指南](../02-tech-stack/26-agent-evaluation-harness-guide.md) |
| G14 | [Agent Sandbox 指南](../02-tech-stack/24-agent-sandbox-guide.md) |
| G15 | [SFT 微调实战](../02-tech-stack/16-sft-finetuning.md) |
| G16 | [Post-Training 面试笔记](../02-tech-stack/25-post-training-complete-guide.md) |
| G17 | [如何落地简历级 Agent 项目](../03-practice/05-ship-agent-project.md) |
| G18 | [Paper Agent 蓝图](../../projects/01-paper-agent/README.md) |
| G19 | [Travel Agent 蓝图](../../projects/02-travel-agent/README.md) |
| G20 | [Web Agent 蓝图](../../projects/03-web-agent/README.md) |
| G21 | [Agent 面试题](../04-interview/03-agent-questions.md) |
| G22 | [RAG 面试题](../04-interview/02-rag-questions.md) |
| G23 | [LLM 基础必考题](../04-interview/16-llm-fundamentals.md) |
| G24 | [大模型算法手写题](../04-interview/17-coding-exercises.md) |
| G25 | [简历指南](../04-interview/12-resume-guide.md) |
| G26 | [求职攻略](../04-interview/08-job-hunting-guide.md) |
| G27 | [职业转型指南](../04-interview/07-career-transition.md) |
| G28 | [2026 Agent 求职路线](./agent-job-ready-roadmap-2026.md) |

---

## 4. 24 周里程碑

| 阶段 | 周数 | 核心目标 | 阶段产出 |
|:---:|:---:|:---|:---|
| A | 1～4 | Python、Git、HTTP、LLM API、Agent Loop | CLI 工具、FastAPI 服务、最小 Agent |
| B | 5～8 | RAG、检索、引用、Paper Agent | Paper Agent MVP + 20 条 eval + Docker |
| C | 9～12 | Context、Memory、LangGraph、MCP、Multi-Agent | 可恢复 Agent + Skill / MCP demo |
| D | 13～16 | Harness、Eval、安全、Web Agent | Evaluation Harness + Web Agent MVP |
| E | 17～20 | Transformer、SFT/LoRA、DPO/GRPO、消融实验 | 原理代码 + 小型微调实验 + 算法实验报告 |
| F | 21～24 | 主项目打磨、部署、简历、面试、投递 | 作品集、简历、博客、模拟面试、投递记录 |

---

# 阶段 A：编程与 Agent 最小闭环

## 第 1 周：建立学习环境与 Python 最小基础

**本周验收**：能使用 Git 管理代码；能独立写一个读写 JSON/Markdown 的 Python CLI；累计完成 3 道简单算法题。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 1 / 06-22 | 通读 G01、G02、G28；写《我为什么转 Agent、目标岗位、24 周约束》；安装 Python、Git、VS Code/Cursor、uv 或 venv | 暂不刷题；理解时间/空间复杂度概念 | `notes/day01-career-goal.md` + 环境版本截图/记录 |
| ⬜ | Day 2 / 06-23 | 学 Python 变量、数字、字符串、布尔值、输入输出；写命令行单位换算器 | 数组概念；完成“数组求和” | 脱离教程重写换算器，含输入校验 |
| ⬜ | Day 3 / 06-24 | 学 list、tuple、dict、set 和切片；写联系人增删改查脚本 | 完成“数组最大值” | 联系人保存在内存中，4 个操作可运行 |
| ⬜ | Day 4 / 06-25 | 学 if、for、while、函数、参数和返回值；重构联系人脚本 | 完成“两数之和”并写暴力/哈希两版 | 每个操作均封装为函数；解释哈希为何更快 |
| ⬜ | Day 5 / 06-26 | 学文件读写、JSON、异常处理；让联系人数据持久化 | 复盘前三题，写复杂度 | 程序重启后数据仍在；坏 JSON 有可读错误 |
| ⬜ | Day 6 / 06-27 | 学 Git：init/add/commit/status/log/branch/diff；为练习项目写 README | 字符串反转、有效回文 | 至少 3 个语义清晰的 commit |
| ⬜ | Day 7 / 06-28 | 周复盘：整理本周错误、命令和 Python 语法；录 3 分钟自述“我学会了什么” | 独立重做“两数之和” | 周报包含完成率、卡点、下周调整 |

## 第 2 周：Python 工程、HTTP、FastAPI 与测试

**本周验收**：完成一个带参数校验、日志、测试的 FastAPI Todo API；累计算法题达到 10 道。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 8 / 06-29 | 学模块、包、虚拟环境、依赖文件；把联系人项目拆成包 | 哈希表：有效的字母异位词 | `src/`、`tests/`、`pyproject.toml` 或 requirements 齐全 |
| ⬜ | Day 9 / 06-30 | 学类、对象、dataclass、类型注解；定义 `Contact` 数据模型 | 哈希表：两个数组的交集 | mypy/IDE 无明显类型错误 |
| ⬜ | Day 10 / 07-01 | 学 HTTP 请求/响应、JSON、状态码、REST；用 `requests/httpx` 调公开 API | 双指针：移动零 | 保存一次完整请求、响应和错误分析 |
| ⬜ | Day 11 / 07-02 | FastAPI 路由、Pydantic、Swagger；创建 Todo API | 双指针：合并有序数组 | GET/POST 可通过 Swagger 调用 |
| ⬜ | Day 12 / 07-03 | 增加 PUT/DELETE、异常处理、日志和配置 | 滑动窗口：最大连续 1 的个数 | 404/422/500 行为清楚，日志可定位请求 |
| ⬜ | Day 13 / 07-04 | 学 pytest、fixture、参数化；给 Todo API 写测试 | 字符串：最长公共前缀 | 至少 8 个测试，含正常和异常路径 |
| ⬜ | Day 14 / 07-05 | 学基础 SQL/SQLite；将 Todo 从内存迁到 SQLite；周复盘 | 本周错题重做 2 道 | API 重启数据不丢，测试全部通过 |

## 第 3 周：LLM 应用基础与结构化输出

**本周验收**：完成一个可切换 mock/真实模型的 LLM CLI 与 FastAPI 服务；理解 token、temperature、system prompt、结构化输出。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 15 / 07-06 | 学 LLM、token、上下文窗口、生成、幻觉基本概念；浏览 G23 第一部分 | 栈：有效的括号 | 写一页“LLM 如何从输入生成输出” |
| ⬜ | Day 16 / 07-07 | 封装 `LLMClient` 接口；实现 `MockLLMClient`，有 API Key 再接真实模型 | 栈：最小栈 | mock 和真实实现使用同一调用接口 |
| ⬜ | Day 17 / 07-08 | 学 system/user/assistant 消息、temperature、max tokens；做参数对比实验 | 队列：用栈实现队列 | 固定 5 个问题，记录不同参数输出差异 |
| ⬜ | Day 18 / 07-09 | 学 prompt 的目标、约束、示例、输出格式；实现摘要器和分类器 | 链表：反转链表 | 两个任务均有 10 个固定输入测试 |
| ⬜ | Day 19 / 07-10 | 学 Pydantic 结构化输出、JSON 解析和重试；做信息抽取 API | 链表：合并两个有序链表 | 非法 JSON 能重试或返回明确失败 |
| ⬜ | Day 20 / 07-11 | 增加限流、超时、重试、日志、token/成本估算 | 二分查找 | 服务连续处理 20 个请求且错误可追踪 |
| ⬜ | Day 21 / 07-12 | 周复盘；写《Prompt Engineering 与普通字符串模板的区别》 | 独立重做有效括号、二分查找 | 输出实验表，不用“感觉更好”作为结论 |

## 第 4 周：Agent 概念、Tool Use 与最小 Agent Loop

**本周验收**：手写 50～150 行最小 Agent，可调用 3 个工具，具备最大步数、trace 和错误处理；累计算法题达到 25 道。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 22 / 07-13 | 精读 G04；对比 chatbot/workflow/agent/multi-agent | 二叉树：前序遍历 | 画一张 5 类系统边界图 |
| ⬜ | Day 23 / 07-14 | 精读 G05 的基本模式与最小实现；手写 observe-act-observe 伪代码 | 二叉树：最大深度 | 不看文档解释 Agent Loop 停止条件 |
| ⬜ | Day 24 / 07-15 | 设计 `calculator`、`search_notes`、`write_summary` 三个工具及 schema | 二叉树：翻转二叉树 | 每个工具有名称、描述、参数、返回、错误码 |
| ⬜ | Day 25 / 07-16 | 实现工具 dispatch 表和结构化 tool call 解析 | BFS：二叉树层序遍历 | 不使用长 if-elif；未知工具有明确错误 |
| ⬜ | Day 26 / 07-17 | 实现最大 5 步、timeout、重试、停止条件 | 递归：对称二叉树 | 故意制造失败，Agent 不崩溃、不死循环 |
| ⬜ | Day 27 / 07-18 | 按 G03 为每步写 JSONL trace；准备 10 条任务 | DFS：路径总和 | trace 含 step/tool/args/observation/duration |
| ⬜ | Day 28 / 07-19 | 跑 10 条任务，分类工具失败、模型误判、格式错误；写 README | 本周错题重做 3 道 | 最小 Agent 可 clone 运行；周报给出成功率 |

---

# 阶段 B：RAG 与 Paper Agent

## 第 5 周：Naive RAG 全链路

**本周验收**：实现 Markdown/PDF 文档问答，回答带 chunk/source 引用；累计算法题达到 32 道。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 29 / 07-20 | 阅读 G07；画 `load→chunk→embed→retrieve→generate` 流程 | 排序：冒泡、选择、插入排序 | 能解释 RAG 解决什么、不解决什么 |
| ⬜ | Day 30 / 07-21 | 用 PyMuPDF/Docling 解析 Markdown 与 PDF，保留页码和标题 | 排序：合并两个有序数组复盘 | 输出统一 `Document/Chunk` 数据结构 |
| ⬜ | Day 31 / 07-22 | 实现固定长度、递归、按标题三种 chunk；比较结果 | 排序：排序数组 | 记录 chunk 数量、平均长度和断句问题 |
| ⬜ | Day 32 / 07-23 | 学 Embedding、余弦相似度；手写向量相似度检索 | Top K：数组中的第 K 大元素 | 不依赖框架实现 top-k 检索 |
| ⬜ | Day 33 / 07-24 | 使用 FAISS/Chroma 保存向量和元数据 | 堆：最后一块石头的重量 | 索引可持久化并重新加载 |
| ⬜ | Day 34 / 07-25 | 完成检索→提示→回答；每条回答附 source/page/chunk | 堆：前 K 个高频元素 | 10 个文档问题中引用可点击/可定位 |
| ⬜ | Day 35 / 07-26 | 分析 10 条失败；区分检索失败和生成失败 | 错题重做 2 道 | 写 `rag_baseline_report.md` |

## 第 6 周：Advanced RAG、检索指标与实验

**本周验收**：实现 BM25 + dense hybrid + rerank，对固定测试集报告 Recall@k、MRR、延迟。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 36 / 07-27 | 学 lexical vs dense retrieval；实现 BM25 baseline | 区间：合并区间 | 同一 query 展示两种检索结果差异 |
| ⬜ | Day 37 / 07-28 | 实现 BM25+dense 加权或 RRF 混合检索 | 区间：插入区间 | 权重可配置，结果可复现 |
| ⬜ | Day 38 / 07-29 | 加 cross-encoder/reranker；记录前后排序变化 | 贪心：买卖股票最佳时机 | 至少展示 3 个 rerank 改善/恶化案例 |
| ⬜ | Day 39 / 07-30 | 实现 query rewrite、multi-query，限制扩展次数 | 贪心：跳跃游戏 | 无结果和重复查询有停止策略 |
| ⬜ | Day 40 / 07-31 | 构建 30 条 query-ground-truth 测试集 | 前缀和：区域和检索 | 数据集含简单、改写、多跳、无答案 |
| ⬜ | Day 41 / 08-01 | 实现 Recall@k、Precision@k、MRR、平均延迟 | 前缀和：和为 K 的子数组 | 自动输出 CSV/Markdown 指标表 |
| ⬜ | Day 42 / 08-02 | 做 chunk size、top-k、hybrid、rerank 四组消融 | 本周错题重做 3 道 | 只基于实验数据选择最终配置 |

## 第 7 周：Paper Agent MVP

**本周验收**：根据 G18 完成论文搜索、去重、排序、摘要、引用和 Markdown 输出的 MVP。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 43 / 08-03 | 精读 G18；写用户、范围、非目标、成功标准和目录结构 | 回溯：子集 | 完成 `SPEC.md`，明确不绕过付费墙 |
| ⬜ | Day 44 / 08-04 | 接 arXiv API；实现 query/year/limit 与缓存 | 回溯：组合 | 返回结构化论文元数据并处理超时 |
| ⬜ | Day 45 / 08-05 | 接 OpenAlex 或 Semantic Scholar；按 DOI/title 去重 | 回溯：全排列 | 两源结果合并且重复项可解释 |
| ⬜ | Day 46 / 08-06 | 设计 Paper Ranker：相关性、年份、引用、来源质量 | 回溯：组合总和 | 对 5 个 query 人工检查 top-5 |
| ⬜ | Day 47 / 08-07 | 下载公开 PDF、校验 hash、解析 page/section | 回溯：电话号码组合 | 解析失败不阻断整个任务 |
| ⬜ | Day 48 / 08-08 | 抽取贡献、方法、数据集、指标、局限；每条 claim 绑定证据 | 矩阵：旋转图像 | 任何结论都能回溯到 paper/page/section |
| ⬜ | Day 49 / 08-09 | 生成 `review.md`、`papers.bib`、`evidence.jsonl`、trace | 本周错题复盘 | 一条命令完成端到端主题综述 |

## 第 8 周：Paper Agent 评测、服务化与发布

**本周验收**：Paper Agent 具备 20 条 eval、FastAPI、Docker、README、失败报告和可演示流程。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 50 / 08-10 | 阅读 G06；为 Paper Agent 定义相关性、引用准确率、覆盖率、幻觉率 | 图：岛屿数量 | 指标定义可计算、无模糊词 |
| ⬜ | Day 51 / 08-11 | 编写 20 条 eval：检索、单篇、多篇、失败、安全 | 图：省份数量 | 每条含输入、期望、禁止行为、grader |
| ⬜ | Day 52 / 08-12 | 实现 code grader：URL、引用字段、篇数、文件完整性 | 图：克隆图 | 确定性规则可自动跑 |
| ⬜ | Day 53 / 08-13 | 设计 rubric grader；人工抽查 5 条校准 | 图：课程表 | rubric 拆成相关性/证据/覆盖三个维度 |
| ⬜ | Day 54 / 08-14 | FastAPI 封装任务创建、状态查询、结果下载 | 图：腐烂的橘子 | 长任务不阻塞请求；失败状态可查询 |
| ⬜ | Day 55 / 08-15 | Docker 化；补配置示例、日志、超时、缓存、测试 | 最短路概念：BFS vs Dijkstra | 新环境按 README 能启动 |
| ⬜ | Day 56 / 08-16 | 录 demo；写 eval 报告和第一版简历 bullet；阶段复盘 | 前 50 天错题抽查 5 道 | 项目达到“别人能 clone 运行”最低线 |

---

# 阶段 C：Context、Memory、LangGraph 与协议

## 第 9 周：Context Engineering

**本周验收**：实现五层 Context Builder、预算控制、压缩和引用；对比优化前后的成本与成功率。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 57 / 08-17 | 精读 G08 核心概念；区分 prompt engineering 与 context engineering | 动态规划：爬楼梯 | 写一页对比表并结合 Paper Agent 举例 |
| ⬜ | Day 58 / 08-18 | 把 context 分为 system/task/memory/evidence/recent trace | DP：打家劫舍 | 输出结构稳定、每层来源清楚 |
| ⬜ | Day 59 / 08-19 | 实现 token budget 和优先级裁剪 | DP：最小路径和 | 超预算时按策略裁剪，不随机截断 |
| ⬜ | Day 60 / 08-20 | 实现工具结果摘要、原文引用和 artifact offload | DP：不同路径 | 大结果写文件，模型只收摘要+定位符 |
| ⬜ | Day 61 / 08-21 | 学 retrieve/compress/isolate/write；各做一个最小例子 | DP：最长递增子序列 | 说明每种策略适用条件 |
| ⬜ | Day 62 / 08-22 | 在 Paper Agent 中接 Context Builder，记录 token/延迟 | DP：最长公共子序列 | 同一测试集跑优化前后对比 |
| ⬜ | Day 63 / 08-23 | 分析 context pollution 与信息遗漏；周复盘 | 错题重做 3 道 | 输出成本、成功率、失败类型变化 |

## 第 10 周：Agent Memory

**本周验收**：实现工作记忆、会话记忆、长期记忆；有写入、检索、更新、遗忘规则和评测。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 64 / 08-24 | 精读 G09 的三层架构与五个问题 | DP：零钱兑换 | 画 memory 生命周期图 |
| ⬜ | Day 65 / 08-25 | 用内存/SQLite 实现工作记忆和会话摘要 | DP：完全平方数 | 重启前后会话状态行为明确 |
| ⬜ | Day 66 / 08-26 | 用向量库实现长期记忆 add/search | DP：单词拆分 | 记忆含 owner/source/time/importance |
| ⬜ | Day 67 / 08-27 | 设计何时写入：事实、偏好、任务状态；过滤敏感信息 | DP：乘积最大子数组 | 10 条样例中不保存密码/无关闲聊 |
| ⬜ | Day 68 / 08-28 | 设计检索排序：相关性+新鲜度+重要性 | DP：最长回文子串 | 排序公式可配置、可解释 |
| ⬜ | Day 69 / 08-29 | 实现冲突更新、TTL、遗忘和用户删除 | DP：编辑距离（理解即可） | 修改偏好后不同时返回冲突旧值 |
| ⬜ | Day 70 / 08-30 | 写 20 条 memory eval，统计 recall/污染/延迟 | 错题复盘 | 输出 `memory_eval_report.md` |

## 第 11 周：LangGraph、有状态执行与 HITL

**本周验收**：将最小 Agent 或 Paper Agent 改造成可暂停、恢复、重试、人工确认的状态图。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 71 / 08-31 | 学 node/edge/state/conditional edge；画现有 Agent 状态图 | 并查集：冗余连接 | 图中有开始、分支、失败、结束 |
| ⬜ | Day 72 / 09-01 | 实现最小 LangGraph：plan→tool→verify→answer | 并查集：省份数量复盘 | 每个节点输入输出有类型 |
| ⬜ | Day 73 / 09-02 | 增加 checkpoint/persistence；中断后恢复 | 拓扑排序：课程表复盘 | 杀掉进程后可从 checkpoint 继续 |
| ⬜ | Day 74 / 09-03 | 增加 retry、fallback、max steps、idempotency | 拓扑排序：课程表 II | 重跑不产生重复副作用 |
| ⬜ | Day 75 / 09-04 | 增加 human-in-the-loop：下载、写文件等动作确认 | 单调栈：每日温度 | 未确认前不执行高风险工具 |
| ⬜ | Day 76 / 09-05 | 保存 state transition trace；给每个节点写测试 | 单调栈：接雨水（理解思路） | 至少 12 个节点/路由测试 |
| ⬜ | Day 77 / 09-06 | 对比手写 loop 与 LangGraph 的优缺点；周复盘 | 错题重做 3 道 | 能回答“何时不需要框架” |

## 第 12 周：MCP、Skills 与 Multi-Agent

**本周验收**：完成一个最小 MCP/工具协议 demo、一个可复用 Skill，以及 research→write→review 小型多 Agent 流程。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 78 / 09-07 | 精读 G10；区分 function calling、tool、MCP、Skill | 位运算：只出现一次的数字 | 画 host/client/server 调用链 |
| ⬜ | Day 79 / 09-08 | 将 `search_papers` 封装为最小 MCP Server 或等价协议 demo | 位运算：比特位计数 | 客户端能发现并调用工具 |
| ⬜ | Day 80 / 09-09 | 为工具增加权限、超时、分页、错误码和不可信输出标记 | 数学：快乐数 | 工具描述对模型友好，返回不过载 |
| ⬜ | Day 81 / 09-10 | 写一个 `paper-review` Skill：触发条件、步骤、模板、验收 | 数学：多数元素 | 新会话按 Skill 可复现流程 |
| ⬜ | Day 82 / 09-11 | 学 planner/executor/reviewer/router；判断何时单 Agent 更好 | 设计：LRU Cache（理解） | 写 multi-agent 采用/拒绝决策表 |
| ⬜ | Day 83 / 09-12 | 实现 research→write→review→revise，限制轮数与 schema | 设计：实现 Trie | 各角色上下文隔离、最多修订 2 轮 |
| ⬜ | Day 84 / 09-13 | 对比单/多 Agent 的质量、token、延迟；阶段复盘 | 84 天错题抽查 6 道 | 有实验结论，不默认多 Agent 更强 |

---

# 阶段 D：Harness、Evaluation、安全与 Web Agent

## 第 13 周：Agent Harness Engineering

**本周验收**：把已有 Agent 重构为包含模型、循环、工具、记忆、通道和可靠性组件的轻量 harness。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 85 / 09-14 | 精读 G11；标注七层模型在现有项目中的对应模块 | 综合：数组/哈希限时 2 题 | 产出 harness 架构图和缺口表 |
| ⬜ | Day 86 / 09-15 | 抽象 Model Adapter，支持 mock 和至少一个真实 provider | 综合：字符串/双指针 2 题 | provider 切换不改业务代码 |
| ⬜ | Day 87 / 09-16 | 抽象 loop、stop policy、retry policy、budget policy | 综合：链表 2 题 | 每种策略可独立测试/替换 |
| ⬜ | Day 88 / 09-17 | 抽象 Tool Registry、permission gate、result sanitizer | 综合：树 2 题 | 高风险动作拦截；工具输出先清洗 |
| ⬜ | Day 89 / 09-18 | 抽象 session store、artifact store、memory store | 综合：图 2 题 | 状态、产物、记忆不混在 messages 中 |
| ⬜ | Day 90 / 09-19 | 增加 CLI/API channel；统一事件流和日志 | 综合：DP 2 题 | 两个入口复用同一核心 |
| ⬜ | Day 91 / 09-20 | 做故障注入：超时、限流、坏 JSON、工具空结果 | 错题重做 3 道 | 每类故障都有预期恢复或终止行为 |

## 第 14 周：Evaluation Harness 与回归测试

**本周验收**：实现配置驱动、可重复运行、可聚合结果的 Mini Evaluation Harness，并接入项目。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 92 / 09-21 | 精读 G13 第 1 章；区分 task/trial/grader/transcript/outcome | 二分答案：搜索插入位置 | 画 evaluation harness 组件图 |
| ⬜ | Day 93 / 09-22 | 定义 `EvalCase/EvalResult/Trial/Grader` 数据结构 | 二分答案：寻找峰值 | schema 支持 component/trajectory/e2e |
| ⬜ | Day 94 / 09-23 | 实现 exact/rule/JSON schema grader | 堆：数据流中位数（理解） | grader 单测覆盖边界值 |
| ⬜ | Day 95 / 09-24 | 实现 rubric/LLM-as-judge 接口和人工复核字段 | 堆：合并 K 个升序链表（理解） | judge prompt 有逃生门和分维度评分 |
| ⬜ | Day 96 / 09-25 | 支持同一 case 多 trial；计算 pass@k/pass^k | 概率基础：均值、方差、置信意识 | 不再以单次运行判断改动好坏 |
| ⬜ | Day 97 / 09-26 | 实现 YAML/JSON 配置、并发、缓存、结果聚合 | SQL：SELECT/JOIN/GROUP BY 练习 | 一条命令运行整套 eval |
| ⬜ | Day 98 / 09-27 | 接 CI 或本地质量门禁；对 Paper Agent 跑回归 | 错题重做 3 道 | 指标低于阈值时返回失败状态 |

## 第 15 周：安全、Sandbox、Observability 与生产基础

**本周验收**：项目具备威胁模型、权限分级、审计日志、敏感信息保护、成本/延迟观测和安全测试。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 99 / 09-28 | 阅读 G14；学习 prompt injection、tool injection、数据泄露 | 操作系统：进程/线程/协程概念 | 写项目 threat model |
| ⬜ | Day 100 / 09-29 | 建立 read/write/network/execute 四级权限与 allowlist | 网络：TCP、HTTP、DNS 概念 | 默认最小权限，拒绝路径可测试 |
| ⬜ | Day 101 / 09-30 | 工具输出视为不可信；实现 prompt-injection 标记与隔离 | 数据库：索引与事务概念 | 恶意网页/PDF 文本不能直接变系统指令 |
| ⬜ | Day 102 / 10-01 | 学 sandbox 思路；为文件/命令工具限制工作区、超时和资源 | Linux：文件权限、进程、常用命令 | 越界路径和危险命令被阻止 |
| ⬜ | Day 103 / 10-02 | 实现 API Key 从环境变量读取、日志脱敏、配置模板 | 工程：缓存、限流、幂等 | 仓库和日志中无密钥 |
| ⬜ | Day 104 / 10-03 | 增加 trace_id、span、token、cost、latency、error_type | 工程：P50/P95/P99 | 一次任务可追踪到每个工具调用 |
| ⬜ | Day 105 / 10-04 | 编写 20 条安全 eval；阶段复盘 | 综合限时 3 题 | 输出安全通过率与未解决风险 |

## 第 16 周：Web Agent MVP

**本周验收**：完成只操作公开网页的 Web Agent，具备结构化观察、动作工具、截图、trace、10 个本地任务和 5 个公开网页任务。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 106 / 10-05 | 精读 G20；写安全边界、动作空间、观察空间和任务定义 | Hot100：哈希 2 题 | 完成 Web Agent `SPEC.md` |
| ⬜ | Day 107 / 10-06 | 学 Playwright：open、locator、click、type、wait | Hot100：双指针 2 题 | 自动打开本地页面并完成点击/填写 |
| ⬜ | Day 108 / 10-07 | 实现 observe：URL/title/visible text/interactive elements | Hot100：滑动窗口 2 题 | 不把完整 DOM 直接塞给模型 |
| ⬜ | Day 109 / 10-08 | 封装 open/observe/click/type/extract/screenshot 工具 | Hot100：栈 2 题 | 每个动作有前后页面状态 |
| ⬜ | Day 110 / 10-09 | 实现 planner→executor→verifier loop、最大步数和恢复 | Hot100：链表 2 题 | 元素失效/超时可重试或换路径 |
| ⬜ | Day 111 / 10-10 | 建本地测试页与 10 个任务；自动 verifier | Hot100：二叉树 2 题 | 输出任务成功率、平均步数、恢复率 |
| ⬜ | Day 112 / 10-11 | 跑 5 个官方文档/GitHub 公开任务；写报告和 demo | Hot100：图 2 题 | 保存 URL、截图、动作 trace 和最终证据 |

---

# 阶段 E：模型算法、Post-Training 与实验

## 第 17 周：Transformer 与 Embedding 原理

**本周验收**：能手写并解释 softmax、attention、multi-head attention、position encoding、LayerNorm 和 Transformer Block 的最小版本。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 113 / 10-12 | 学向量、矩阵、点积、矩阵乘；用 NumPy 做形状练习 | G24：ReLU、Sigmoid、Softmax | 手算一个 2×2 矩阵乘法和 softmax |
| ⬜ | Day 114 / 10-13 | 学 tokenization、embedding、position encoding | G24：Embedding、Sinusoidal PE | 解释 token id 与 embedding 向量区别 |
| ⬜ | Day 115 / 10-14 | 推导 scaled dot-product attention 的 Q/K/V | G24：Softmax Attention | 用小矩阵手算一次 attention |
| ⬜ | Day 116 / 10-15 | 实现 causal mask 和 multi-head attention | G24：Causal Attention、MHA | 单元测试验证 shape 和 mask |
| ⬜ | Day 117 / 10-16 | 学 residual、LayerNorm、FFN、GELU/SwiGLU | G24：LayerNorm、SwiGLU | 解释 Pre-LN 与 Post-LN |
| ⬜ | Day 118 / 10-17 | 拼装最小 Transformer Block；跑前向传播 | G24：GPT-2 Block | forward 可运行，参数和张量形状有注释 |
| ⬜ | Day 119 / 10-18 | 复习 G23 Transformer 高频题；口述 10 题 | Hot100 综合限时 3 题 | 录 10 分钟白板讲解并列出薄弱点 |

## 第 18 周：SFT、LoRA / QLoRA 与数据工程

**本周验收**：理解 SFT 数据、labels mask、LoRA 原理和训练指标；用小模型/Colab 完成一次可复现微调，资源不足则完成 mock 实验与代码审查。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 120 / 10-19 | 精读 G15 基础概念；对比 prompt/RAG/SFT/RL | G24：Cross Entropy、Perplexity | 写技术选型决策树 |
| ⬜ | Day 121 / 10-20 | 学 chat template、input_ids、attention mask、labels=-100 | G24：KL、Label Smoothing | 手工构造一条训练样本并标出 loss token |
| ⬜ | Day 122 / 10-21 | 准备 200～500 条 tool-use 或结构化输出数据；划分 train/val/test | 数据：去重、分层划分 | 数据有来源、版本、质量检查 |
| ⬜ | Day 123 / 10-22 | 推导 LoRA `W'=W+BA`；理解 rank/alpha/dropout/target modules | G24：LoRA | 手写最小 `LoRALinear` 并测试 |
| ⬜ | Day 124 / 10-23 | 学 QLoRA、NF4、显存估算、packing；制定实验配置 | G24：QLoRA、INT8 Linear | 说明为什么 B 零初始化 |
| ⬜ | Day 125 / 10-24 | 用 Qwen 小模型 + PEFT/LLaMA-Factory/Unsloth 跑小型 SFT | Hot100：DP 2 题 | 保存配置、seed、loss 曲线、模型产物 |
| ⬜ | Day 126 / 10-25 | 比较 base vs fine-tuned 的固定测试集；分析过拟合和回退 | 错题重做 3 道 | 只报告真实结果；失败也写原因 |

## 第 19 周：偏好优化、PPO、DPO、GRPO 与 Agent RL

**本周验收**：能解释 SFT→RM→PPO、DPO 与 GRPO 的差异；手写关键 loss；为 Tool Use 任务设计奖励。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 127 / 10-26 | 阅读 G16 第 1～4 章摘要；画 Post-Training 全链路 | G24：Bradley-Terry Loss | 解释为何只做 SFT 不等于对齐 |
| ⬜ | Day 128 / 10-27 | 学 reward model、pairwise preference、reward hacking | G24：KL Penalty | 设计 10 对 chosen/rejected 数据 |
| ⬜ | Day 129 / 10-28 | 学 policy gradient、advantage、PPO clip、KL | G24：PPO Clipped Loss | 手写 PPO loss 伪代码并解释 clip |
| ⬜ | Day 130 / 10-29 | 学 DPO 推导直觉、beta、reference model、分布偏移 | G24：DPO Loss | 实现 DPO loss 最小函数和数值测试 |
| ⬜ | Day 131 / 10-30 | 学 GRPO 组内相对优势、无 critic、梯度真空问题 | G24：GRPO Loss | 对比 PPO/DPO/GRPO 表格 |
| ⬜ | Day 132 / 10-31 | 为 Agent Tool Use 设计 format/outcome/process/efficiency/safety reward | MCTS 基础概念 | 5 类奖励均给出可计算示例 |
| ⬜ | Day 133 / 11-01 | 回答 G23 对齐高频题；做一次 30 分钟算法模拟面试 | 综合限时 3 题 | 复盘答不出的概念并建补漏清单 |

## 第 20 周：算法实验与 Paper Agent 消融

**本周验收**：完成一份像算法项目的实验报告：问题、假设、数据、baseline、指标、消融、误差分析和结论。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 134 / 11-02 | 从检索/排序/context/memory 选一个问题；写可证伪假设 | 统计：均值、分位数、方差复习 | 问题必须能由指标回答 |
| ⬜ | Day 135 / 11-03 | 固定数据集、随机种子、baseline、变量和实验矩阵 | Hot100：数组 2 题 | 实验配置可复现，避免一次改多项 |
| ⬜ | Day 136 / 11-04 | 跑 baseline；记录成功率、Recall@k、引用准确率、成本、延迟 | Hot100：树 2 题 | 原始结果完整保存 |
| ⬜ | Day 137 / 11-05 | 实验 A：chunk/top-k/hybrid/rerank 之一 | Hot100：图 2 题 | 输出与 baseline 对比表 |
| ⬜ | Day 138 / 11-06 | 实验 B：context compression 或 memory 策略 | Hot100：DP 2 题 | 至少跑 3 次，记录波动 |
| ⬜ | Day 139 / 11-07 | 逐条分析失败：数据、检索、规划、工具、生成、评测 | Hot100：回溯 2 题 | 每类失败给出代表 case |
| ⬜ | Day 140 / 11-08 | 写实验报告、图表、局限和下一步；阶段复盘 | 140 天错题抽查 8 道 | 形成算法岗可讲的实验故事 |

---

# 阶段 F：旗舰项目、作品集与求职

## 第 21 周：旗舰项目重构与产品化

**本周验收**：以 Paper Agent 为旗舰项目，完成 v2 Spec、架构重构、核心功能和生产可靠性。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 141 / 11-09 | 重读 G17；收敛目标用户、核心任务、非目标、成功标准 | Hot100 限时 2 题 | `SPEC-v2.md` 不超过必要范围 |
| ⬜ | Day 142 / 11-10 | 画系统架构、数据流、状态图、权限图、部署图 | Hot100 限时 2 题 | 5 张图与实际代码一致 |
| ⬜ | Day 143 / 11-11 | 重构 tool registry、context builder、state store、artifact store | Hot100 限时 2 题 | 核心模块依赖方向清晰 |
| ⬜ | Day 144 / 11-12 | 完成多源检索、证据存储、引用验证 | Hot100 限时 2 题 | 断言无证据时不输出确定结论 |
| ⬜ | Day 145 / 11-13 | 完成 planner/reviewer、最大轮数、人工确认 | Hot100 限时 2 题 | reviewer 不可无限循环 |
| ⬜ | Day 146 / 11-14 | 增加队列/后台任务、缓存、重试、幂等、限流 | 系统设计：任务队列 | 重复请求不重复下载/处理 |
| ⬜ | Day 147 / 11-15 | 全量测试和故障注入；修复 P0/P1 问题 | 本周错题重做 | 单测、集成测试、关键 eval 全通过 |

## 第 22 周：评测、部署、文档与公开展示

**本周验收**：旗舰项目有可靠评测、在线或本地一键 demo、完整文档、技术博客和可复现指标。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 148 / 11-16 | 扩充 eval 到 30～50 条，含正常/边界/安全/无答案 | Hot100 模拟 2 题 | case 分布和来源写入数据说明 |
| ⬜ | Day 149 / 11-17 | 跑 component/trajectory/e2e 三层评测 | Hot100 模拟 2 题 | 报告成功率、成本、延迟、失败类型 |
| ⬜ | Day 150 / 11-18 | 做最终消融：无 rerank/无 reviewer/无 compression | Hot100 模拟 2 题 | 每个模块的收益或负收益有数据 |
| ⬜ | Day 151 / 11-19 | 增加 Docker Compose、健康检查、配置模板、启动脚本 | 系统设计：缓存与降级 | 新机器可按 README 启动 |
| ⬜ | Day 152 / 11-20 | 部署到可承受成本的平台；若不部署则录完整本地 demo | 系统设计：API 限流 | Demo 链接或视频可访问 |
| ⬜ | Day 153 / 11-21 | 完善 README：问题、架构、运行、评测、限制、安全 | SQL/网络高频题复习 | 面试官 5 分钟能看懂项目价值 |
| ⬜ | Day 154 / 11-22 | 写技术博客《从 Demo 到可评测 Paper Agent》 | 本周错题重做 | 博客包含真实失败案例和数据 |

## 第 23 周：简历、面试题、项目讲述与投递准备

**本周验收**：完成开发岗/算法岗两版简历、项目逐字稿、面试题答案、目标公司与 JD 能力矩阵。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 155 / 11-23 | 阅读 G25、G26、G27；整理教育/经历/技能/项目素材 | Hot100 模拟：45 分钟 2 题 | 所有简历素材可证明、可追问 |
| ⬜ | Day 156 / 11-24 | 写 Agent 开发岗一页简历：系统、可靠性、指标、部署 | Hot100 高频错题 3 道 | 每个 bullet 有动作、难点、结果 |
| ⬜ | Day 157 / 11-25 | 写 Agent 算法岗一页简历：问题、baseline、实验、消融 | G24 高频手写 3 题 | 不把普通调参包装成算法创新 |
| ⬜ | Day 158 / 11-26 | 准备 30 秒自我介绍、3 分钟项目介绍、10 分钟深挖 | Hot100 模拟：45 分钟 2 题 | 录音回听，删除术语堆砌 |
| ⬜ | Day 159 / 11-27 | 回答 G21 Agent 题 20 道；整理不会题 | 手写最小 Agent Loop | 答案必须结合自己的项目 |
| ⬜ | Day 160 / 11-28 | 回答 G22 RAG 题 20 道、G23 LLM 题 15 道 | 手写 attention/LoRA/DPO 之一 | 建立个人面试错题本 |
| ⬜ | Day 161 / 11-29 | 收集 30 个 JD；提取共性技能、缺口、关键词和优先级 | 本周错题重做 | 形成 10 家重点 + 20 家练手机会 |

## 第 24 周：模拟面试、真实投递与下一轮迭代

**本周验收**：完成至少 3 次模拟面试、首批 20～30 个有效投递、反馈台账和后续 4 周迭代计划。

| 状态 | Day / 日期 | 当日学习与实作 | 算法训练 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 162 / 11-30 | 模拟面试 1：Python/FastAPI/RAG/Agent 基础 | 45 分钟算法模拟 2 题 | 按知识/表达/项目证据三维评分 |
| ⬜ | Day 163 / 12-01 | 修补模拟 1 最弱的 3 个知识点；更新简历 | 重做模拟失败题 | 补漏后重新口述并通过 |
| ⬜ | Day 164 / 12-02 | 模拟面试 2：系统设计、Harness、Eval、安全、部署 | 45 分钟算法模拟 2 题 | 画出完整 Agent 系统设计 |
| ⬜ | Day 165 / 12-03 | 模拟面试 3：Transformer、RAG 算法、SFT/LoRA、DPO/GRPO | 手写 attention + DPO loss | 算法回答含公式直觉、工程取舍、实验 |
| ⬜ | Day 166 / 12-04 | 针对 10 家重点公司定制简历与开场消息；开始投递 | 高频错题 3 道 | 10 个定制投递，不海投同一版 |
| ⬜ | Day 167 / 12-05 | 扩展至 20～30 个有效投递；记录岗位、版本、状态、反馈 | 高频错题 3 道 | 建立投递看板和跟进日期 |
| ⬜ | Day 168 / 12-06 | 24 周总复盘：成果、短板、作品、题量、面试反馈；制定下一阶段 | 随机抽查 5 道旧题 | 发布总结；生成下一轮 4 周计划 |

---

## 5. 每周复盘模板

每周日复制并填写，后续与 AI 同步时优先提供这一段：

```markdown
## Week N 周报（YYYY-MM-DD）

- 本周计划完成：x / 7 天
- 实际投入：x 小时
- 新增代码提交：x 次
- 新增算法题：x 道；累计：x 道
- 本周最重要产出：
- 已掌握：
- 仍然模糊：
- 最大阻塞：
- 失败案例及原因：
- 下周需要保留：
- 下周需要删减：
- 当前求职信心（1～5）：
```

## 6. 项目验收清单

Paper Agent 与 Web Agent 至少满足：

- [ ] 明确目标用户、输入、输出、非目标和成功标准。
- [ ] 工具 schema、返回结构、错误码、timeout 和权限清楚。
- [ ] 有最大步数、停止条件、重试、fallback 和成本上限。
- [ ] 有结构化 state、context builder、artifact 和 trace。
- [ ] 有 20 条以上 eval case，覆盖正常、边界、失败、安全。
- [ ] 指标至少包含成功率、成本、延迟和失败类型。
- [ ] 有单元测试、集成测试和固定回归测试。
- [ ] README 可让陌生人从零运行。
- [ ] 有架构图、demo、eval report、失败分析和限制说明。
- [ ] 简历描述中的每个数字都能由报告或日志复现。

## 7. 面试准备最低线

进入正式投递前，应能不看资料回答：

1. Agent 与 workflow 的区别，何时不该用 Agent。
2. ReAct / Plan-and-Execute 的差异与失败模式。
3. Tool schema、权限、错误处理和幂等如何设计。
4. RAG 的 chunk、embedding、hybrid retrieval、rerank、引用和评测。
5. Context Engineering 与 Prompt Engineering 的区别。
6. 短期、长期、工作记忆的写入、检索、更新、遗忘策略。
7. Agent Harness 与 Evaluation Harness 分别解决什么问题。
8. 如何评测非确定性 Agent，pass@k 与 pass^k 有何区别。
9. 如何防 prompt injection、tool injection、数据泄露和危险动作。
10. Transformer、Attention、LoRA、SFT、DPO、PPO、GRPO 的核心直觉。
11. 项目中最严重的一次失败、如何定位、如何验证修复。
12. 如果数据量、用户量或工具数扩大 10 倍，系统如何调整。

---

## 8. 当前进度仪表盘

> 后续每次同步学习进度时更新此处；不要另建互相冲突的进度文件。

| 项目 | 当前值 |
|:---|:---|
| 当前日期 | 2026-06-21 |
| 当前阶段 | 准备开始 |
| 当前周 / Day | Week 0 / Day 0 |
| 完成天数 | 0 / 168 |
| 累计学习小时 | 0 |
| 累计算法题 | 0 / 120+ |
| Paper Agent | 未开始 |
| Web Agent | 未开始 |
| Eval Case | 0 |
| 技术博客 | 0 / 2+ |
| 模拟面试 | 0 / 3+ |
| 有效投递 | 0 / 20+ |
| 当前最大阻塞 | 无 |
| 下一步 | 执行 Day 1 |

---

## 9. Git 生命周期与后续同步规则

### 9.1 单一事实来源

- 后续学习安排、完成状态、延期、删减、补课、周复盘和求职进度全部维护在本文件。
- 不新建第二份“最新版计划”；需要保留历史时依靠 Git commit、tag 和 diff。
- 学习代码、笔记和项目可以放在独立目录或仓库，但它们在本计划中的状态必须回写到每日表格与进度仪表盘。

### 9.2 提交粒度与 commit 约定

| 场景 | commit 示例 |
|:---|:---|
| 完成一天并通过验收 | `learn(day-001): complete environment and career goal` |
| 完成一周并复盘 | `learn(week-01): finish python foundation review` |
| 调整未来安排 | `plan(week-05): reduce reading and extend rag practice` |
| 修正计划错误 | `docs(plan): fix day 36 resource link` |
| 更新求职反馈 | `career: record interview feedback and next actions` |

- 每次提交只做一类事情，避免把学习代码、计划调整和无关 IDE 配置混在同一个 commit。
- 日常最少在通过当日验收后提交一次；未通过验收时标记为 `🔁`，不要提交虚假的“完成”状态。
- 每周复盘完成后提交一次周快照；每个阶段结束后创建 tag，例如 `learning-stage-a-complete`。

### 9.3 版本号规则

- `v1.x`：目标和 24 周主结构不变，只调整每日内容、资源、节奏或验收标准。
- `v2.0`：目标岗位、总周期、主项目或路线权重发生重大变化。
- 每次修改版本时同步更新文件顶部版本号和第 11 节变更记录。

### 9.4 每日同步流程

1. 将当天状态从 `⬜` 改为 `🟡`。
2. 学习和实作结束后，按“当日验收”逐项核对证据。
3. 通过则改为 `✅`；未通过则改为 `🔁`，并在当日单元格末尾注明阻塞或下一步。
4. 更新第 8 节的当前日期、Day、完成天数、学习小时、算法题数、项目与 eval 数据。
5. 使用 `learn(day-NNN): ...` 提交当天变化。

### 9.5 每周调整流程

1. 按第 5 节模板完成周报，先记录真实完成情况，再讨论调课。
2. 只调整尚未开始的日期；已完成内容保留原记录，不改写历史。
3. 延期内容优先占用下一次周日复盘时间；连续落后时执行第 2.3 节的删减规则。
4. 调整后检查阶段验收目标是否仍可实现，并在第 11 节记录“改了什么、为什么、影响哪些日期”。
5. 使用 `plan(week-NN): ...` 提交调整，并在阶段结束时打 tag。

### 9.6 回滚与恢复

- 误改计划：先用 `git diff` 定位，再通过新的修复 commit 恢复；不要重写已经共享的历史。
- 中断少于 7 天：从最近一个 `🔁` 或未完成日恢复，不整体重排。
- 中断 7～21 天：保留已完成记录，重新计算后续日期，并提升一个次版本号。
- 中断超过 21 天或目标岗位改变：先做能力盘点，再建立 `v2.0`，不要机械补齐所有旧任务。

---

## 10. 路线设计说明

### 共识

- 对零基础跳槽者，先建立工程闭环，再补算法深度，比一开始钻进大模型训练更可执行。
- 求职证据应来自项目、评测、部署、实验和复盘，而不是框架名词列表。
- Agent 开发和 Agent 算法并非两条完全分离的路线：同一项目可以用工程可靠性投开发岗，用检索/上下文/记忆消融投算法岗。
- Paper Agent 适合作为主项目，因为它同时覆盖 RAG、工具、引用、上下文、评测和实验；Web Agent 用来补浏览器、真实环境和失败恢复。

### 主动舍弃

- 前 16 周不做大规模预训练、分布式训练和复杂 Agent RL，避免基础不足时被算力与数学拖垮。
- 不同时深学多个 Agent 框架；先手写 loop，再以 LangGraph 为主。
- 不把低代码平台项目作为主简历项目，但可用于理解 workflow 和快速验证需求。
- 不追求“通用全自动 Agent”，优先做边界清楚、可评测、可复现的垂直项目。

### 收敛检查

1. 否决理由 → ADR：有；已记录在“主动舍弃”。
2. 踩坑教训 → lessons-learned：当前没有，后续每周复盘持续沉淀。
3. 操作规则 → 指引文件：有；已写入“执行规则”和“防止计划崩盘的规则”。

---

## 11. 变更记录

| 版本 | 日期 | 变更 | 原因 |
|:---:|:---:|:---|:---|
| v1.0 | 2026-06-21 | 建立 24 周、168 天逐日计划；确定 Paper Agent 主项目、Web Agent 次项目、120+ 算法题、评测与求职闭环；加入 Git 生命周期规则 | 为 Agent / 大模型零基础转向 Agent 开发 + 算法岗位建立可执行、可验证、可持续调整的路线 |
