# 个人学习计划：AI Agent 开发 + 算法（24 周，每天 1 小时）

> 适用对象：Agent / 大模型零基础，目标岗位为 Agent 开发、LLM 应用开发、RAG / Agent 算法工程。
>
> 计划周期：**2026-06-22 ～ 2026-12-06，共 24 周 / 168 天 / 约 168 小时**。
>
> 时间约束：**工作日和周末均按每天约 1 小时设计**。
>
> 路线权重：Agent 开发与工程约 70%，算法与模型原理约 30%。
>
> 当前版本：v1.1（2026-06-21）；本文件是后续计划、进度、复盘与调整的唯一事实来源。

## 1. 24 周后的现实目标

每天只有 1 小时时，不追求“大而全”，而追求能够持续完成、可验证、可用于求职的成果：

- 掌握 Python、Git、HTTP、FastAPI、测试等最低工程基础。
- 能解释 chatbot、workflow、agent、RAG、context、memory、harness、eval 的边界。
- 能手写一个带工具注册、最大步数、错误处理和 trace 的最小 Agent Loop。
- 完成一个 **Paper Agent 主项目**：论文检索、PDF 解析、证据引用、CLI、15 条 eval case、测试和 README。
- 完成一个小型浏览器自动化体验，不要求再做完整 Web Agent 项目。
- 理解 Transformer、Attention、Embedding、SFT、LoRA、DPO、PPO、GRPO 的核心直觉。
- 完成约 **40 道核心数据结构与算法题**，并重复练习高频错题。
- 形成一页简历、项目介绍、架构图、评测报告、模拟面试记录和首轮投递记录。

暂不纳入 24 周硬目标：

- 大规模预训练、分布式训练和完整 RLHF 训练。
- 同时精通多个 Agent 框架。
- 完整开发第二个大型 Agent 项目。
- 只为追求数量而完成 100～120 道算法题。

## 2. 每天 60 分钟怎么用

普通学习日：

| 环节 | 时间 | 要求 |
|:---|:---:|:---|
| 回忆昨天 | 5 分钟 | 不看资料说出 3 个要点 |
| 阅读指定资源 | 20 分钟 | 只读当天标注的文档或章节 |
| 动手练习 | 30 分钟 | 写代码、画图、做题或跑测试 |
| 记录证据 | 5 分钟 | 更新本计划，留下 commit、笔记或结果 |

算法日采用 `5 分钟复习 + 45 分钟做题 + 10 分钟写复杂度与错因`。周复盘日采用 `20 分钟回顾 + 25 分钟补缺 + 15 分钟更新计划`。

每天只要求完成一个核心任务。超过 60 分钟仍未完成时标记为 `🔁`，下一周复盘日继续，不通过熬夜追赶。

### 状态标记

| 标记 | 含义 |
|:---:|:---|
| ⬜ | 未开始 |
| 🟡 | 进行中 |
| ✅ | 已完成并通过当日验收 |
| 🔁 | 已投入时间但未通过验收 |
| ⏸ | 主动暂停，必须写明原因 |

## 3. 学习资源索引

每日表格的“学习资源”列会引用以下编号，并尽量标明阅读章节。看到 `Gxx` 或 `Rxx` 时，从本节直接打开链接。

### 3.1 AgentGuide 仓库内资源

| 编号 | 文档 |
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
| G18 | [Paper Agent 项目蓝图](../../projects/01-paper-agent/README.md) |
| G19 | [Web Agent 项目蓝图](../../projects/03-web-agent/README.md) |
| G20 | [Agent 面试题](../04-interview/03-agent-questions.md) |
| G21 | [RAG 面试题](../04-interview/02-rag-questions.md) |
| G22 | [LLM 基础必考题](../04-interview/16-llm-fundamentals.md) |
| G23 | [大模型算法手写题](../04-interview/17-coding-exercises.md) |
| G24 | [简历指南](../04-interview/12-resume-guide.md) |
| G25 | [求职攻略](../04-interview/08-job-hunting-guide.md) |
| G26 | [职业转型指南](../04-interview/07-career-transition.md) |
| G27 | [2026 Agent 求职路线](./agent-job-ready-roadmap-2026.md) |
| G28 | [Transformer 架构详解](../01-theory/03-transformer.md) |
| G29 | [思维链与规划](../01-theory/05-cot-and-planning.md) |
| G30 | [Agent Benchmark](../01-theory/08-agent-bench.md) |
| G31 | [多 Agent 框架](../02-tech-stack/06-multi-agent-frameworks.md) |

### 3.2 外部基础资源

| 编号 | 资源 |
|:---:|:---|
| R01 | [Python 官方教程](https://docs.python.org/3/tutorial/) |
| R02 | [Pro Git 中文版](https://git-scm.com/book/zh/v2) |
| R03 | [MDN：HTTP 概览](https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Guides/Overview) |
| R04 | [FastAPI 官方教程](https://fastapi.tiangolo.com/zh/tutorial/) |
| R05 | [pytest 入门](https://docs.pytest.org/en/stable/getting-started.html) |
| R06 | [Pydantic 官方文档](https://docs.pydantic.dev/latest/) |
| R07 | [arXiv API 手册](https://info.arxiv.org/help/api/index.html) |
| R08 | [PyMuPDF 文档](https://pymupdf.readthedocs.io/en/latest/tutorial.html) |
| R09 | [LangGraph 官方概览](https://docs.langchain.com/oss/python/langgraph/overview) |
| R10 | [MCP 官方入门](https://modelcontextprotocol.io/docs/getting-started/intro) |
| R11 | [Playwright Python 入门](https://playwright.dev/python/docs/intro) |
| R12 | [Docker Get Started](https://docs.docker.com/get-started/) |
| R13 | [NumPy 快速入门](https://numpy.org/doc/stable/user/quickstart.html) |
| R14 | [PyTorch：Transformer 组件](https://pytorch.org/docs/stable/nn.html#transformer-layers) |
| R15 | [Hugging Face LLM Course](https://huggingface.co/learn/llm-course/chapter1/1) |
| R16 | [LeetCode 热题 100](https://leetcode.cn/studyplan/top-100-liked/) |
| R17 | [Anthropic：Building Effective Agents](https://www.anthropic.com/engineering/building-effective-agents) |
| R18 | [Semantic Scholar API](https://api.semanticscholar.org/api-docs/) |

## 4. 24 周逐日计划

# 阶段 A：编程基础与 Agent 最小闭环

## 第 1 周：建立地图与 Python 最小基础

**本周验收**：环境可用；能写并运行一个带输入校验的 Python 小程序。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 1 / 06-22 | 浏览路线，写目标岗位、每天 1 小时约束和不做事项；检查 Python、Git | G01；G02；G27「适合谁」 | `notes/day01-goal.md` 有目标、时间和边界 |
| ⬜ | Day 2 / 06-23 | 学变量、数字、字符串和 `print/input`；写温度换算器 | R01「3. Python 速览」 | 程序可运行并处理非法输入 |
| ⬜ | Day 3 / 06-24 | 学 list、tuple、dict、set；写联系人数据结构 | R01「5. 数据结构」 | 能增、查联系人 |
| ⬜ | Day 4 / 06-25 | 学 `if/for/while`；给联系人增加菜单循环 | R01「4. 控制流工具」 | 菜单可重复操作并正常退出 |
| ⬜ | Day 5 / 06-26 | 学函数、参数和返回值；重构联系人脚本 | R01「4.8 Defining Functions」 | 至少拆成 3 个职责清楚的函数 |
| ⬜ | Day 6 / 06-27 | 学文件读写、JSON 和异常；保存联系人 | R01「7. 输入和输出」「8. 错误和异常」 | 重启程序后数据仍在 |
| ⬜ | Day 7 / 06-28 | 按模板复盘第一周，脱离资料重写一个核心函数 | G03「Day 7」 | 写出完成率、卡点和下周动作 |

## 第 2 周：Python 工程、Git、HTTP

**本周验收**：小项目受 Git 管理；能解释 HTTP 请求和响应；累计算法题 2 道。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 8 / 06-29 | 学模块、包、`venv`；整理联系人项目目录 | R01「6. 模块」「12. 虚拟环境和包」 | 有 `src/`、README、依赖说明 |
| ⬜ | Day 9 / 06-30 | 学类、对象、`dataclass` 和类型注解 | R01「9. 类」 | 定义带类型的 `Contact` 模型 |
| ⬜ | Day 10 / 07-01 | 学 Git 工作区、暂存区、提交和 diff | R02「Git 基础」 | 完成 3 个语义清楚的 commit |
| ⬜ | Day 11 / 07-02 | 学 HTTP 方法、状态码、头和 JSON | R03「HTTP 概览」 | 用自己的话画一次请求/响应 |
| ⬜ | Day 12 / 07-03 | 用 Python 请求公开 API，打印成功和失败结果 | R03；R01「标准库简介」 | 保存状态码、响应体和异常处理 |
| ⬜ | Day 13 / 07-04 | 算法 1：数组求和 | R16「数组」 | 独立写出循环解法并标注复杂度 |
| ⬜ | Day 14 / 07-05 | 算法 2：两数之和；最后 15 分钟做周复盘 | R16「哈希」；第 5 节复盘模板 | 解释暴力法与哈希法差异 |

## 第 3 周：FastAPI、测试与 LLM 基础

**本周验收**：完成最小 Todo API 和测试；累计算法题 4 道。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 15 / 07-06 | 跑通 FastAPI Hello World 和 Swagger | R04「第一步」 | `/docs` 可调用接口 |
| ⬜ | Day 16 / 07-07 | 学路径参数、请求体和 Pydantic 模型 | R04「路径参数」「请求体」；R06「Models」 | Todo POST 可校验输入 |
| ⬜ | Day 17 / 07-08 | 增加 GET/POST/DELETE 三个 Todo 接口 | R04「教程」 | 三个接口均可手动调用 |
| ⬜ | Day 18 / 07-09 | 学 pytest 基本断言与 fixture；写 3 个测试 | R05「Get Started」 | `pytest` 全部通过 |
| ⬜ | Day 19 / 07-10 | 算法 3：有效括号 | R16「栈」 | 独立写栈解法和复杂度 |
| ⬜ | Day 20 / 07-11 | 算法 4：二分查找 | R16「二分查找」 | 能说清循环不变量 |
| ⬜ | Day 21 / 07-12 | 阅读 LLM、token、上下文、幻觉基础并周复盘 | G22「适用对象」「Transformer 基础」 | 写 10 条 LLM 基础问答卡 |

## 第 4 周：Agent 概念与最小循环

**本周验收**：手写可运行的 mock Agent Loop；累计算法题 6 道。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 22 / 07-13 | 区分 chatbot、workflow、agent、multi-agent | G04「Agent 不等于 Chatbot」；G02「5 个概念」 | 画一张边界表 |
| ⬜ | Day 23 / 07-14 | 学 Agent 最小闭环与 8 个组成部分 | G04「Agent 的最小闭环」「8 个组成部分」 | 不看文档口述闭环 |
| ⬜ | Day 24 / 07-15 | 学 ReAct 基本模式，写 observe-act-observe 伪代码 | G05「基本模式」「最小实现」 | 伪代码含停止条件 |
| ⬜ | Day 25 / 07-16 | 用 Mock 模型实现最多 3 步的循环 | G05「最小实现」 | 可执行工具请求并返回最终结果 |
| ⬜ | Day 26 / 07-17 | 算法 5：反转链表 | R16「链表」 | 迭代解法通过测试 |
| ⬜ | Day 27 / 07-18 | 算法 6：合并两个有序数组 | R16「双指针」 | 写出原地或新数组解法 |
| ⬜ | Day 28 / 07-19 | 周复盘；用 3 分钟讲清最小 Agent | G03「Day 2」；G04「面试怎么回答」 | 录音或逐字稿可复述 |

## 第 5 周：工具设计、错误处理与 Trace

**本周验收**：Agent 可调用 2 个工具并保存 trace；累计算法题 8 道。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 29 / 07-20 | 学 Tool Card：名称、描述、参数、返回、错误 | G05「Tool Card 很重要」 | 写 `calculator` 工具卡 |
| ⬜ | Day 30 / 07-21 | 实现 `calculator` 和 `search_notes` | G03「Day 2～3」 | 两个工具有统一返回结构 |
| ⬜ | Day 31 / 07-22 | 用 dispatch 表替代长 `if-elif` | G11「L3：工具层」 | 新增工具只需注册一项 |
| ⬜ | Day 32 / 07-23 | 增加最大步数、未知工具错误和异常捕获 | G05「常见失败模式」 | 错误不会导致死循环 |
| ⬜ | Day 33 / 07-24 | 算法 7：二叉树最大深度 | R16「二叉树」 | 递归解法通过 |
| ⬜ | Day 34 / 07-25 | 算法 8：二叉树层序遍历 | R16「二叉树」 | BFS 解法通过 |
| ⬜ | Day 35 / 07-26 | 为每一步保存 JSONL trace；周复盘 | G06「Trace 是评测前提」 | trace 含 step/tool/args/result/error |

# 阶段 B：RAG 与 Paper Agent 主项目

## 第 6 周：RAG 基础与文档切分

**本周验收**：能将 Markdown 文档切成带来源的 chunk；累计算法题 10 道。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 36 / 07-27 | 理解 `load→chunk→embed→retrieve→generate` | G07「概述」；G21「RAG 基础题」 | 画 RAG 流程图 |
| ⬜ | Day 37 / 07-28 | 定义 `Document`、`Chunk` 数据结构 | G07；G18「MVP 范围」 | 结构含 source、page、text |
| ⬜ | Day 38 / 07-29 | 实现固定长度切分 Markdown | G07 | chunk 可保留来源 |
| ⬜ | Day 39 / 07-30 | 对比两种 chunk size，记录边界问题 | G07；G21「Chunk 相关题」 | 输出一张对比表 |
| ⬜ | Day 40 / 07-31 | 算法 9：有效的字母异位词 | R16「哈希」 | 哈希计数解法通过 |
| ⬜ | Day 41 / 08-01 | 算法 10：无重复字符的最长子串 | R16「滑动窗口」 | 能解释窗口何时移动 |
| ⬜ | Day 42 / 08-02 | 周复盘；回答“RAG 能和不能解决什么” | G21「RAG 面试题」 | 写 5 条边界结论 |

## 第 7 周：Embedding、检索与基础评测

**本周验收**：实现小型向量检索 baseline 和 10 条检索测试；累计算法题 12 道。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 43 / 08-03 | 学向量、点积和余弦相似度 | R13「基础与数组运算」；G22「Embedding」 | 手算一个余弦相似度 |
| ⬜ | Day 44 / 08-04 | 用 NumPy 实现余弦相似度 | R13 | 有 3 个单元测试 |
| ⬜ | Day 45 / 08-05 | 用 mock embedding 或小模型做 top-k 检索 | G07；R15「Transformers 基础」 | 查询返回 chunk 和分数 |
| ⬜ | Day 46 / 08-06 | 写 10 条 query-ground-truth 检索 case | G06「Eval Case 格式」 | 测试集保存为 JSONL |
| ⬜ | Day 47 / 08-07 | 算法 11：前 K 个高频元素 | R16「堆」 | 至少完成一种解法 |
| ⬜ | Day 48 / 08-08 | 算法 12：数组中的第 K 个最大元素 | R16「堆」 | 堆解法通过 |
| ⬜ | Day 49 / 08-09 | 计算 Recall@k，分析 3 个失败 case | G06「核心指标」 | 输出 baseline 指标 |

## 第 8 周：Paper Agent 规格与论文检索

**本周验收**：项目 spec 完成；可从 arXiv 搜索并保存论文元数据；累计算法题 14 道。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 50 / 08-10 | 阅读 Paper Agent 蓝图，明确用户、输入、输出、非目标 | G18「为什么值得做」「MVP 范围」 | 完成 `docs/spec.md` |
| ⬜ | Day 51 / 08-11 | 设计 `search_papers` 工具 schema | G18「核心工具设计」；R07 | 工具卡含错误和数量上限 |
| ⬜ | Day 52 / 08-12 | 调用 arXiv API 搜索 5 篇论文 | R07「API User's Manual」 | 保存标题、作者、摘要、URL |
| ⬜ | Day 53 / 08-13 | 实现标题/DOI 去重和简单排序 | G18「论文检索」 | 重复输入不会产生重复论文 |
| ⬜ | Day 54 / 08-14 | 算法 13：合并区间 | R16「区间」 | 排序扫描解法通过 |
| ⬜ | Day 55 / 08-15 | 算法 14：插入区间 | R16「区间」 | 写出边界 case |
| ⬜ | Day 56 / 08-16 | 周复盘；补 README 的项目目标和运行方式 | G17「Step 4：先写 Spec」 | 陌生人能理解项目范围 |

## 第 9 周：PDF 解析与证据结构

**本周验收**：可解析公开 PDF，并按页保存证据；累计算法题 16 道。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 57 / 08-17 | 学 PyMuPDF 打开文档、读取页数和文本 | R08「Opening a File」「Extracting Text」 | 打印一篇 PDF 前两页文本 |
| ⬜ | Day 58 / 08-18 | 定义 `Evidence`：paper、page、section、text | G18「证据引用」 | 数据结构可序列化 |
| ⬜ | Day 59 / 08-19 | 将 PDF 按页或段落切块 | R08；G18「PDF 解析」 | 每个 chunk 保留页码 |
| ⬜ | Day 60 / 08-20 | 实现关键词搜索，返回相关证据 | G18「Evidence Store」 | 输入关键词可定位原页 |
| ⬜ | Day 61 / 08-21 | 算法 15：岛屿数量 | R16「图论」 | DFS 或 BFS 解法通过 |
| ⬜ | Day 62 / 08-22 | 算法 16：课程表 | R16「图论」 | 能解释拓扑排序 |
| ⬜ | Day 63 / 08-23 | 周复盘；抽查 5 条证据是否能回到原文 | G06「证据与事实性」 | 记录证据准确率 |

## 第 10 周：摘要、引用与 Paper Agent MVP

**本周验收**：输入主题后能输出带论文链接和页码证据的 Markdown；累计算法题 18 道。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 64 / 08-24 | 设计贡献、方法、实验、局限四字段输出 | G18「输出格式」 | Pydantic schema 可验证 |
| ⬜ | Day 65 / 08-25 | 用 mock 或真实 LLM 生成结构化摘要 | G05「Prompt 结构」；R06 | 非法输出会明确失败 |
| ⬜ | Day 66 / 08-26 | 将摘要结论绑定 evidence id | G18「证据引用」 | 每条结论有来源 |
| ⬜ | Day 67 / 08-27 | 串联 search→download→parse→summarize | G18「推荐架构」 | CLI 跑通 1 个主题 |
| ⬜ | Day 68 / 08-28 | 算法 17：爬楼梯 | R16「动态规划」 | 写递推式和空间优化 |
| ⬜ | Day 69 / 08-29 | 算法 18：打家劫舍 | R16「动态规划」 | 状态定义清楚 |
| ⬜ | Day 70 / 08-30 | MVP 复盘；记录最严重的 3 类失败 | G17「Step 5：评测、归因」 | `failure-analysis.md` 有实例 |

# 阶段 C：Context、Memory、协议与评测

## 第 11 周：Context Engineering 与简单 Memory

**本周验收**：上下文分层，项目可保存会话或任务状态；累计算法题 20 道。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 71 / 08-31 | 区分 Prompt Engineering 与 Context Engineering | G08「核心概念」 | 写一页对比 |
| ⬜ | Day 72 / 09-01 | 将 context 分成 task、evidence、trace、history | G08「上下文工程的组成部分」 | 画 context builder 输入输出 |
| ⬜ | Day 73 / 09-02 | 实现只保留必要 evidence 的 context builder | G08「长上下文问题」 | 输出含长度统计 |
| ⬜ | Day 74 / 09-03 | 学 working/episodic/semantic memory | G09「三层记忆架构」；G11「L4」 | 给项目标注三类信息 |
| ⬜ | Day 75 / 09-04 | 算法 19：零钱兑换 | R16「动态规划」 | 完成 DP 解法 |
| ⬜ | Day 76 / 09-05 | 算法 20：最长递增子序列 | R16「动态规划」 | 完成 O(n²) 解法 |
| ⬜ | Day 77 / 09-06 | 用 JSONL/SQLite 保存运行摘要；周复盘 | G09「5 大核心问题」 | 可写入并读取一次任务记录 |

## 第 12 周：LangGraph、MCP 与 Multi-Agent 边界

**本周验收**：完成最小 LangGraph 或状态机 demo、理解 MCP 调用链；累计算法题 22 道。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 78 / 09-07 | 理解 state、node、edge、conditional edge | R09「Overview」 | 画现有 Agent 状态图 |
| ⬜ | Day 79 / 09-08 | 实现 plan→tool→answer 三节点 demo | R09「Graph API」 | 每个节点输入输出明确 |
| ⬜ | Day 80 / 09-09 | 学 checkpoint、暂停、恢复的用途 | R09；G11「L2」 | 写恢复流程伪代码 |
| ⬜ | Day 81 / 09-10 | 区分 function calling、tool、Skill、MCP | G10「MCP 与 Function Calling」；R10 | 画 host/client/server 图 |
| ⬜ | Day 82 / 09-11 | 算法 21：多数元素 | R16「技巧」 | Boyer-Moore 或哈希解法通过 |
| ⬜ | Day 83 / 09-12 | 算法 22：只出现一次的数字 | R16「位运算」 | 异或解法通过 |
| ⬜ | Day 84 / 09-13 | 阅读 Multi-Agent 边界并周复盘 | G31；G27「Stage 4」 | 写“采用/不采用”决策表 |

## 第 13 周：Evaluation Harness

**本周验收**：Paper Agent 有 15 条固定 eval case 和可重复运行的结果表；累计算法题 24 道。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 85 / 09-14 | 理解 component、trajectory、end-to-end 三层评测 | G06「三层评估」 | 为项目各写 1 个例子 |
| ⬜ | Day 86 / 09-15 | 定义 `EvalCase` 和 `EvalResult` schema | G13「Task/Trial/Grader」 | JSONL 可加载 |
| ⬜ | Day 87 / 09-16 | 扩充到 15 条：正常、边界、失败、安全 | G06「最小评测集」 | 四类 case 均覆盖 |
| ⬜ | Day 88 / 09-17 | 实现规则 grader：是否有来源、页码、必要字段 | G12「Code-based Grader」 | grader 有单测 |
| ⬜ | Day 89 / 09-18 | 算法 23：LRU Cache | R16「设计」 | 完成或写出完整数据结构设计 |
| ⬜ | Day 90 / 09-19 | 算法 24：实现 Trie | R16「字典树」 | insert/search 通过 |
| ⬜ | Day 91 / 09-20 | 跑 baseline，统计通过率、延迟、失败类型 | G06「核心指标」 | 生成 Markdown 表格 |

## 第 14 周：Harness、可靠性与安全

**本周验收**：项目有超时、重试、成本/步数限制、权限边界和安全 case；累计算法题 26 道。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 92 / 09-21 | 理解 Model + Harness 和七层模型 | G11「什么是 Harness」「七层模型」 | 在项目图上标出现有层 |
| ⬜ | Day 93 / 09-22 | 增加 timeout、retry、max steps | G11「可靠性六件套」 | 故障注入不死循环 |
| ⬜ | Day 94 / 09-23 | 增加 token/请求次数预算和错误分类 | G11「Cost Guard」「Observability」 | trace 有 cost/error_type |
| ⬜ | Day 95 / 09-24 | 写 threat model：不可信 PDF、路径、网络、密钥 | G14「核心结论」「实践建议」 | 至少列 5 个风险及措施 |
| ⬜ | Day 96 / 09-25 | 算法 25：搜索二维矩阵 | R16「二分查找」 | 二分解法通过 |
| ⬜ | Day 97 / 09-26 | 算法 26：寻找峰值 | R16「二分查找」 | 解释为何可二分 |
| ⬜ | Day 98 / 09-27 | 增加 5 条安全 eval 并周复盘 | G06「安全与治理」 | 危险输入不会触发写操作 |

## 第 15 周：Paper Agent 集成与回归

**本周验收**：形成可演示的 v1；累计算法题 28 道。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 99 / 09-28 | 对照项目清单检查缺口 | G17「最终标准」；G18「实现里程碑」 | 生成 P0/P1 缺口表 |
| ⬜ | Day 100 / 09-29 | 修复最高优先级功能缺口 | 上一日缺口表；G18 | P0 功能可运行 |
| ⬜ | Day 101 / 09-30 | 修复最高频 eval 失败 | G17「Step 5」 | 固定测试集通过率提升或有解释 |
| ⬜ | Day 102 / 10-01 | 完善 CLI 参数、错误提示和输出目录 | G18「输出格式」 | 一条命令完成一次任务 |
| ⬜ | Day 103 / 10-02 | 算法 27：每日温度 | R16「单调栈」 | 单调栈解法通过 |
| ⬜ | Day 104 / 10-03 | 算法 28：最小栈 | R16「栈」 | 所有操作满足要求 |
| ⬜ | Day 105 / 10-04 | 跑完整回归并记录 v1 指标 | G13；G06 | 保存 eval 报告和失败样本 |

## 第 16 周：算法阶段复习与浏览器 Agent 体验

**本周验收**：累计算法题 32 道；完成一个只读网页信息提取脚本。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 106 / 10-05 | 算法 29：移动零 | R16「双指针」 | 原地解法通过 |
| ⬜ | Day 107 / 10-06 | 算法 30：盛最多水的容器 | R16「双指针」 | 解释移动规则 |
| ⬜ | Day 108 / 10-07 | 算法 31：最大子数组和 | R16「动态规划」 | 写出状态转移 |
| ⬜ | Day 109 / 10-08 | 算法 32：除自身以外数组的乘积 | R16「数组」 | 不使用除法通过 |
| ⬜ | Day 110 / 10-09 | 学 Playwright open、locator、读取文本 | R11「Installation」「Writing tests」；G19「MVP 范围」 | 读取公开页面标题 |
| ⬜ | Day 111 / 10-10 | 保存 URL、文本摘要和截图，不执行写入动作 | G19「安全边界」「观察层」 | 输出一个只读网页报告 |
| ⬜ | Day 112 / 10-11 | 阶段复盘：为什么本路线不做完整 Web Agent | G19；第 1 节暂不纳入目标 | 写出时间收益取舍 |

# 阶段 D：模型与算法基础

## 第 17 周：Transformer 直觉

**本周验收**：能解释 token、embedding、attention、残差和 LayerNorm；累计算法题 34 道。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 113 / 10-12 | 理解 token id、embedding 和向量形状 | G28「概述」；G22「Tokenization」 | 画输入到 embedding |
| ⬜ | Day 114 / 10-13 | 学 Q/K/V 和 scaled dot-product attention | G22「Transformer 架构基础」；R14 | 用自己的话解释 Q/K/V |
| ⬜ | Day 115 / 10-14 | 用小矩阵手算一次 attention | G23「Attention 机制核心」 | 保存完整计算过程 |
| ⬜ | Day 116 / 10-15 | 理解 multi-head、mask、残差、LayerNorm | G22「Transformer 架构基础」 | 画 Transformer Block |
| ⬜ | Day 117 / 10-16 | 算法 33：颜色分类 | R16「双指针」 | 完成一种解法 |
| ⬜ | Day 118 / 10-17 | 算法 34：数组中的第 K 个最大元素，重做限时版 | R16「堆」 | 30 分钟内完成 |
| ⬜ | Day 119 / 10-18 | 口述 10 个 Transformer 高频问题并复盘 | G22「第一部分」 | 标出不会的 3 题 |

## 第 18 周：Embedding 与 Attention 最小代码

**本周验收**：手写 softmax 和单头 attention；累计算法题 36 道。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 120 / 10-19 | 用 NumPy 手写稳定版 softmax | R13；G23「激活函数」 | 极端输入不溢出 |
| ⬜ | Day 121 / 10-20 | 手写单头 attention 前向计算 | G23「Softmax Attention」 | shape 注释清楚 |
| ⬜ | Day 122 / 10-21 | 增加 causal mask | G23「Causal Attention」 | 未来位置权重为 0 |
| ⬜ | Day 123 / 10-22 | 对比 embedding 检索和 attention 的作用 | G07；G28；G22 | 写一页对比 |
| ⬜ | Day 124 / 10-23 | 算法 35：全排列 | R16「回溯」 | 回溯解法通过 |
| ⬜ | Day 125 / 10-24 | 算法 36：组合总和 | R16「回溯」 | 能解释剪枝 |
| ⬜ | Day 126 / 10-25 | 周复盘；脱离资料重写 softmax | G23「第一阶段」 | 独立实现通过测试 |

## 第 19 周：SFT、LoRA 与数据

**本周验收**：理解何时用 Prompt、RAG、SFT、LoRA；只做最小代码，不要求真实训练；累计算法题 38 道。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 127 / 10-26 | 对比 Prompt、RAG、SFT、RL 的适用边界 | G15「基础概念篇」 | 写技术选型表 |
| ⬜ | Day 128 / 10-27 | 学 SFT 数据格式、chat template、labels mask | G15「数据构建篇」；G16「2.1」 | 标出一条样本的 loss token |
| ⬜ | Day 129 / 10-28 | 理解 LoRA 的 `W'=W+BA`、rank、alpha | G22「PEFT」；G15「LoRA、PEFT」 | 画 LoRA 旁路 |
| ⬜ | Day 130 / 10-29 | 手写最小 `LoRALinear` 或伪代码 | G23「训练优化技术」 | 前向 shape 正确 |
| ⬜ | Day 131 / 10-30 | 算法 37：和为 K 的子数组 | R16「前缀和」 | 哈希 + 前缀和通过 |
| ⬜ | Day 132 / 10-31 | 算法 38：最长连续序列 | R16「哈希」 | O(n) 解法通过 |
| ⬜ | Day 133 / 11-01 | 周复盘；回答“何时不该微调” | G15「SFT 前提条件」「风险防控」 | 写 5 条拒绝微调理由 |

## 第 20 周：Post-Training 直觉与小型实验

**本周验收**：能区分 SFT、PPO、DPO、GRPO，并完成一次 Paper Agent 小消融；累计算法题 40 道。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 134 / 11-02 | 浏览 Post-Training 完整地图 | G16「1.2 完整链路」 | 画 SFT→偏好优化路线 |
| ⬜ | Day 135 / 11-03 | 理解 reward model、PPO、KL 的直觉 | G16「强化学习与对齐」；G22「第七部分」 | 写 5 个概念卡 |
| ⬜ | Day 136 / 11-04 | 理解 DPO 与 GRPO 的输入、目标和差异 | G16；G22「强化学习与对齐」 | 完成对比表 |
| ⬜ | Day 137 / 11-05 | 设计 Paper Agent 消融：有/无 context 压缩或不同 top-k | G17「消融实验」；G06「核心指标」 | 写假设、变量和指标 |
| ⬜ | Day 138 / 11-06 | 算法 39：最小路径和 | R16「动态规划」 | DP 解法通过 |
| ⬜ | Day 139 / 11-07 | 算法 40：单词拆分 | R16「动态规划」 | 写状态定义和转移 |
| ⬜ | Day 140 / 11-08 | 跑一次消融并记录真实结果 | G17「Step 5」 | 有 baseline、对照和限制 |

# 阶段 E：作品、面试与求职

## 第 21 周：项目可靠性与文档

**本周验收**：Paper Agent 可从 README 启动，测试和 eval 可重复运行。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 141 / 11-09 | 重读简历级项目标准并列最终缺口 | G17「最终标准」 | P0 缺口不超过 5 项 |
| ⬜ | Day 142 / 11-10 | 修复最高风险错误路径 | G11「可靠性六件套」 | 超时/空结果有明确行为 |
| ⬜ | Day 143 / 11-11 | 补关键单元测试 | R05；G17 | 核心工具有测试 |
| ⬜ | Day 144 / 11-12 | 整理配置模板和密钥说明 | G14「实践建议」 | 仓库无真实密钥 |
| ⬜ | Day 145 / 11-13 | 写 README：目标、架构、安装、运行 | G17「最终标准」；G18 | 新读者能按步骤运行 |
| ⬜ | Day 146 / 11-14 | 写 eval 报告：数据、指标、失败、局限 | G06；G13 | 所有数字可复现 |
| ⬜ | Day 147 / 11-15 | 画架构图并录 3 分钟 demo | G18「推荐架构」 | 图与代码一致 |

## 第 22 周：简历与项目讲述

**本周验收**：完成一页简历和 3～5 分钟项目介绍。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 148 / 11-16 | 阅读简历指南，收集教育、技能、项目素材 | G24「简历指南」 | 建立素材清单 |
| ⬜ | Day 149 / 11-17 | 写 Agent 开发方向一页简历初稿 | G24；G17「简历写法」 | 每条 bullet 有动作和结果 |
| ⬜ | Day 150 / 11-18 | 写算法方向项目 bullet：问题、baseline、实验 | G24；G17「消融实验」 | 不编造指标 |
| ⬜ | Day 151 / 11-19 | 写 30 秒自我介绍 | G26「职业转型」 | 录音不超过 45 秒 |
| ⬜ | Day 152 / 11-20 | 写 3 分钟 Paper Agent 项目介绍 | G17；G18 | 包含背景、架构、指标、失败 |
| ⬜ | Day 153 / 11-21 | 准备 5 个深挖问题和答案 | G20；G21 | 答案绑定自己的项目 |
| ⬜ | Day 154 / 11-22 | 找一位朋友或 AI 做简历 review 并修改 | G24「检查清单」 | 形成 v1 简历 |

## 第 23 周：面试题与模拟面试

**本周验收**：完成两次模拟面试和个人错题清单。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 155 / 11-23 | 回答 Agent 基础 10 题 | G20「第一部分」 | 每题控制在 2 分钟 |
| ⬜ | Day 156 / 11-24 | 回答 Tool、Memory、框架 10 题 | G20「第二～四部分」 | 标记不会的题 |
| ⬜ | Day 157 / 11-25 | 回答 RAG 10 题 | G21 | 至少 5 题结合项目 |
| ⬜ | Day 158 / 11-26 | 回答 Transformer、LoRA、SFT 10 题 | G22「第一～三部分」 | 形成概念错题本 |
| ⬜ | Day 159 / 11-27 | 45 分钟算法模拟：抽 2 道旧题 | R16；算法错题记录 | 至少完整通过 1 题 |
| ⬜ | Day 160 / 11-28 | 模拟面试 1：Agent 开发与项目 | G20；G17 | 按知识/表达/证据评分 |
| ⬜ | Day 161 / 11-29 | 模拟面试 2：RAG、模型基础与算法 | G21；G22；G23 | 列出最高优先级 5 个缺口 |

## 第 24 周：投递、反馈与下一轮计划

**本周验收**：开始真实投递，建立反馈台账，并生成下一阶段 4 周计划。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 162 / 11-30 | 阅读求职攻略，建立岗位筛选标准 | G25「求职攻略」；G27「求职路线」 | 明确岗位优先级 |
| ⬜ | Day 163 / 12-01 | 收集 10 个 JD，提取共同技能和缺口 | G25 | 形成能力矩阵 |
| ⬜ | Day 164 / 12-02 | 针对 2 个 JD 调整简历关键词 | G24；上一日矩阵 | 生成 2 个简历版本 |
| ⬜ | Day 165 / 12-03 | 完成首批 3～5 个有效投递 | G25 | 记录岗位、版本、日期、状态 |
| ⬜ | Day 166 / 12-04 | 根据首轮反馈补一个最高频缺口 | G20～G23 对应章节 | 产出可验证补强记录 |
| ⬜ | Day 167 / 12-05 | 整理作品集入口、README、demo 和联系方式 | G17「最终标准」 | 所有链接可访问 |
| ⬜ | Day 168 / 12-06 | 24 周总复盘，制定下一阶段 4 周计划 | G27；第 5 节模板 | 写成果、缺口、投递数据和下步 |

## 5. 每周复盘模板

```markdown
## Week N 周报（YYYY-MM-DD）

- 本周完成：x / 7 天
- 实际投入：x / 7 小时
- 新增算法题：x；累计：x / 40
- 本周最重要产出：
- 已掌握：
- 仍然模糊：
- 最大阻塞：
- 一个失败案例及原因：
- 下周保留：
- 下周删减：
- 是否需要调整未来日期：
```

## 6. Paper Agent 最终验收清单

- [ ] 有明确用户、输入、输出、非目标和成功标准。
- [ ] 能从 arXiv 搜索论文并保存结构化元数据。
- [ ] 能解析公开 PDF，并保留 paper/page/text 证据。
- [ ] 每条核心结论带可追溯来源，不把无证据内容写成事实。
- [ ] Agent Loop 有最大步数、错误处理和 trace。
- [ ] 有 15 条以上固定 eval case，覆盖正常、边界、失败和安全。
- [ ] 报告成功率、延迟和失败类型，数字均可复现。
- [ ] 核心工具有单元测试。
- [ ] README 能让陌生人从零运行最小 demo。
- [ ] 有架构图、demo、eval report、失败分析和限制说明。

## 7. 当前进度仪表盘

| 项目 | 当前值 |
|:---|:---|
| 当前日期 | 2026-06-21 |
| 当前周 / Day | Week 0 / Day 0 |
| 完成天数 | 0 / 168 |
| 累计学习小时 | 0 / 168 |
| 累计算法题 | 0 / 40 |
| 最小 Agent | 未开始 |
| Paper Agent | 未开始 |
| Eval Case | 0 / 15+ |
| 一页简历 | 未开始 |
| 模拟面试 | 0 / 2 |
| 有效投递 | 0 / 3+ |
| 当前最大阻塞 | 无 |
| 下一步 | 执行 Day 1 |

## 8. Git 生命周期与同步规则

### 8.1 单一事实来源

- 后续安排、完成状态、延期、删减、周报和求职进度全部维护在本文件。
- 不另建“最新版计划”；历史通过 Git commit、tag 和 diff 保留。
- 已完成日期不改写历史；只调整尚未开始的任务。

### 8.2 提交约定

| 场景 | commit 示例 |
|:---|:---|
| 完成一天 | `learn(day-001): finish environment setup` |
| 完成一周 | `learn(week-01): review python basics` |
| 调整计划 | `plan(week-05): reduce scope for one-hour schedule` |
| 修正文档 | `docs(plan): fix resource link` |
| 更新求职反馈 | `career: record interview feedback` |

每天通过验收后更新状态和仪表盘，再提交一次。每周复盘后提交周快照。阶段完成可创建 tag。

### 8.3 调整规则

- 单日未完成：标记 `🔁`，放到最近周复盘日处理。
- 连续 3 天未完成：删除可选阅读，不压缩实践和复盘。
- 连续 7 天未完成：暂停新增知识一周，只恢复节奏。
- 中断 7～21 天：保留已完成记录，重排未来日期并提升次版本号。
- 中断超过 21 天或目标岗位变化：重新做能力盘点，建立 v2.0。

## 9. 变更记录

| 版本 | 日期 | 变更 | 原因 |
|:---:|:---:|:---|:---|
| v1.0 | 2026-06-21 | 建立 24 周、168 天初版计划 | 建立 Agent 开发 + 算法求职路线 |
| v1.1 | 2026-06-21 | 将每天投入统一为约 1 小时；为 Day 1～168 增加学习资源；将目标收敛为一个 Paper Agent、40 道算法题和必要求职产出 | 用户确认真实时间预算，并指出每日任务缺少明确学习链接或文档 |
