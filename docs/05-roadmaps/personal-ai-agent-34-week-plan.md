# 个人 AI Agent 开发与模型基础学习计划（34 周，每天 1 小时）

> 适用对象：AI Agent / 大模型应用零基础，目标岗位为 Agent 开发、LLM 应用开发、RAG / Agent 相关岗位。
>
> 计划周期：**2026-06-22 ～ 2027-02-14，共 34 周 / 238 天 / 约 238 小时**。
>
> 时间约束：**工作日和周末均按每天约 1 小时设计**。
>
> 范围约束：**LeetCode 式数据结构与算法学习由你单独安排，不占用这里的每天 1 小时，也不在本文件统计。Transformer、Embedding、LoRA、SFT、DPO/GRPO、Agent 规划与检索等模型和 Agent 算法属于本计划。**
>
> 当前版本：v1.3（2026-06-21）；本文件是后续计划、进度、复盘与调整的唯一事实来源。

## 1. 34 周后的目标

- 掌握 Python、Git、HTTP、FastAPI、测试等 Agent 工程最低基础。
- 能解释 chatbot、workflow、agent、RAG、context、memory、harness、eval、MCP、multi-agent 的边界。
- 能手写带工具注册、最大步数、错误处理、权限确认和 trace 的 Agent Loop。
- 完成一个可写入简历的 **Paper Agent 主项目**：论文搜索、PDF 解析、证据引用、RAG、CLI/API、评测、测试、Docker 和 README。
- 完成一个受控的 **Web Agent 次项目**：公开网页、结构化观察、Playwright、截图、trace、安全边界和固定评测。
- 能使用 LangGraph 或等价状态机实现暂停、恢复、重试和 human-in-the-loop。
- 能设计 Agent Harness、Evaluation Harness、Context、Memory、Observability 和安全边界。
- 能完成一个 MCP Server、一个可复用 Skill 和一个有对照实验的 multi-agent 小流程。
- 理解 Transformer、Attention、Embedding、SFT、LoRA、DPO、PPO、GRPO 的核心原理及其与 Agent 能力的关系。
- 理解 ReAct、Plan-and-Execute、Reflection、Tree Search、检索和 Memory 策略的算法取舍，并完成最小实验。
- 形成一页简历、作品集入口、项目架构图、评测报告、3～5 分钟项目介绍、模拟面试和投递反馈台账。

本计划不包含：

- LeetCode、数据结构与通用算法训练。
- 大规模预训练、分布式训练和完整 RLHF 训练。

LeetCode 式算法可以平行学习，但不得挤占本计划每天 1 小时的 Agent 时间。

## 2. 每天 60 分钟的执行方式

| 环节 | 时间 | 要求 |
|:---|:---:|:---|
| 回忆 | 5 分钟 | 不看资料回忆昨天 3 个要点 |
| 阅读 | 20 分钟 | 只读当天指定的文档或章节 |
| 实作 | 30 分钟 | 写代码、测试、图、评测或文档 |
| 记录 | 5 分钟 | 更新状态，保存 commit、笔记或结果 |

周复盘日采用 `15 分钟回顾 + 30 分钟补缺 + 15 分钟更新计划`。

每天只要求完成一个核心任务。60 分钟后仍未通过验收，标记为 `🔁`，放到后续复盘日继续，不挤占独立的 LeetCode 学习时间，也不熬夜追赶。

### 状态标记

| 标记 | 含义 |
|:---:|:---|
| ⬜ | 未开始 |
| 🟡 | 进行中 |
| ✅ | 已完成并通过当日验收 |
| 🔁 | 已投入时间但未通过验收 |
| ⏸ | 主动暂停，必须写明原因 |

## 3. 学习资源索引

每日表格中的 `Gxx` 指 AgentGuide 仓库文档，`Rxx` 指外部官方资料。资源列会尽量标明当天应阅读的章节。

### 3.1 AgentGuide 仓库内资源

| 编号 | 文档 |
|:---:|:---|
| G01 | [AgentGuide 快速开始](../00-getting-started/README.md) |
| G02 | [Agent 学习地图](../00-getting-started/01-agent-map.md) |
| G03 | [前 7 天学习计划](../00-getting-started/02-first-7-days.md) |
| G04 | [什么是 AI Agent](../01-theory/01-what-is-agent.md) |
| G05 | [Agent 历史](../01-theory/02-agent-history.md) |
| G06 | [手撕 ReAct 框架](../01-theory/04-react-framework.md) |
| G07 | [思维链与规划](../01-theory/05-cot-and-planning.md) |
| G08 | [Agent Benchmark](../01-theory/08-agent-bench.md) |
| G09 | [Agent 评估指标体系](../01-theory/09-evaluation-metrics.md) |
| G10 | [RAG 全链路实战](../02-tech-stack/20-rag-full-pipeline.md) |
| G11 | [上下文工程实践](../02-tech-stack/11-context-engineering-practices.md) |
| G12 | [Agent Memory](../02-tech-stack/15-agent-memory.md) |
| G13 | [MCP 协议详解](../02-tech-stack/14-mcp-protocol.md) |
| G14 | [多 Agent 框架](../02-tech-stack/06-multi-agent-frameworks.md) |
| G15 | [Agent Harness Engineering](../02-tech-stack/27-agent-harness-engineering.md) |
| G16 | [Agent 评估完全指南](../02-tech-stack/agent-evaluation-complete-guide.md) |
| G17 | [Evaluation Harness 指南](../02-tech-stack/26-agent-evaluation-harness-guide.md) |
| G18 | [Agent Sandbox 指南](../02-tech-stack/24-agent-sandbox-guide.md) |
| G19 | [如何落地简历级 Agent 项目](../03-practice/05-ship-agent-project.md) |
| G20 | [Paper Agent 项目蓝图](../../projects/01-paper-agent/README.md) |
| G21 | [Web Agent 项目蓝图](../../projects/03-web-agent/README.md) |
| G22 | [Agent Workflow 项目](../../projects/05-agent-workflows/README.md) |
| G23 | [Agent 面试题](../04-interview/03-agent-questions.md) |
| G24 | [RAG 面试题](../04-interview/02-rag-questions.md) |
| G25 | [开发岗专项](../04-interview/06-development-specialized.md) |
| G26 | [简历指南](../04-interview/12-resume-guide.md) |
| G27 | [求职攻略](../04-interview/08-job-hunting-guide.md) |
| G28 | [职业转型指南](../04-interview/07-career-transition.md) |
| G29 | [2026 Agent 求职路线](./agent-job-ready-roadmap-2026.md) |
| G30 | [Transformer 架构详解](../01-theory/03-transformer.md) |
| G31 | [SFT 微调实战](../02-tech-stack/16-sft-finetuning.md) |
| G32 | [Post-Training 面试笔记](../02-tech-stack/25-post-training-complete-guide.md) |
| G33 | [大模型算法手写题](../04-interview/17-coding-exercises.md) |
| G34 | [Agent Reinforcement Learning](../02-tech-stack/21-agent-reinforcement-learning.md) |

### 3.2 外部官方资源

| 编号 | 资源 |
|:---:|:---|
| R01 | [Python 官方教程](https://docs.python.org/3/tutorial/) |
| R02 | [Pro Git 中文版](https://git-scm.com/book/zh/v2) |
| R03 | [MDN：HTTP 概览](https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Guides/Overview) |
| R04 | [FastAPI 官方教程](https://fastapi.tiangolo.com/zh/tutorial/) |
| R05 | [pytest 入门](https://docs.pytest.org/en/stable/getting-started.html) |
| R06 | [Pydantic 官方文档](https://docs.pydantic.dev/latest/) |
| R07 | [OpenAI API Quickstart](https://developers.openai.com/api/docs/quickstart) |
| R08 | [OpenAI Function Calling](https://developers.openai.com/api/docs/guides/function-calling) |
| R09 | [Anthropic：Building Effective Agents](https://www.anthropic.com/engineering/building-effective-agents) |
| R10 | [arXiv API 手册](https://info.arxiv.org/help/api/index.html) |
| R11 | [Semantic Scholar API](https://api.semanticscholar.org/api-docs/) |
| R12 | [OpenAlex API](https://docs.openalex.org/) |
| R13 | [PyMuPDF 教程](https://pymupdf.readthedocs.io/en/latest/tutorial.html) |
| R14 | [LangGraph 官方文档](https://docs.langchain.com/oss/python/langgraph) |
| R15 | [MCP 官方入门](https://modelcontextprotocol.io/docs/getting-started/intro) |
| R16 | [OpenAI Agents SDK](https://openai.github.io/openai-agents-python/) |
| R17 | [Playwright Python 入门](https://playwright.dev/python/docs/intro) |
| R18 | [Docker Get Started](https://docs.docker.com/get-started/) |
| R19 | [OWASP LLM Top 10](https://owasp.org/www-project-top-10-for-large-language-model-applications/) |
| R20 | [OpenTelemetry Python](https://opentelemetry.io/docs/languages/python/) |
| R21 | [Prometheus Python Client](https://prometheus.github.io/client_python/) |
| R22 | [NumPy 快速入门](https://numpy.org/doc/stable/user/quickstart.html) |
| R23 | [PyTorch Transformer 组件](https://pytorch.org/docs/stable/nn.html#transformer-layers) |
| R24 | [Hugging Face LLM Course](https://huggingface.co/learn/llm-course/chapter1/1) |
| R25 | [Hugging Face TRL 文档](https://huggingface.co/docs/trl/index) |
| R26 | [ReAct 论文](https://arxiv.org/abs/2210.03629) |
| R27 | [Reflexion 论文](https://arxiv.org/abs/2303.11366) |
| R28 | [Tree of Thoughts 论文](https://arxiv.org/abs/2305.10601) |
| R29 | [LoRA 论文](https://arxiv.org/abs/2106.09685) |

## 4. 34 周逐日计划

# 阶段 A：工程基础与 Agent 最小闭环

## 第 1 周：路线、环境与 Python 入门

**本周验收**：环境可用；理解学习边界；能运行带输入校验的 Python 小程序。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 1 / 06-22 | 浏览路线；写目标岗位、每日 1 小时和算法独立安排 | G01；G02；G29「适合谁」 | `notes/day01-goal.md` 写清目标与边界 |
| ⬜ | Day 2 / 06-23 | 检查 Python、Git、编辑器和虚拟环境 | R01「Using Python」；R02「起步」 | 保存版本与环境记录 |
| ⬜ | Day 3 / 06-24 | 学变量、字符串、数字和输入输出 | R01「3. Python 速览」 | 写可运行的单位换算器 |
| ⬜ | Day 4 / 06-25 | 学 `if/for/while` | R01「4. 控制流工具」 | 换算器有菜单和退出逻辑 |
| ⬜ | Day 5 / 06-26 | 学函数、参数和返回值 | R01「4.8 Defining Functions」 | 拆出至少 3 个函数 |
| ⬜ | Day 6 / 06-27 | 学 list、dict、set | R01「5. 数据结构」 | 写联系人内存模型 |
| ⬜ | Day 7 / 06-28 | 周复盘；不看旧代码重写一个函数 | G03「Day 7」 | 写完成率、卡点、下周动作 |

## 第 2 周：文件、异常与 Python 工程

**本周验收**：联系人 CLI 可持久化；目录和依赖结构清楚。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 8 / 06-29 | 学文件读写和 JSON | R01「7. 输入和输出」 | 联系人可保存到 JSON |
| ⬜ | Day 9 / 06-30 | 学异常处理 | R01「8. 错误和异常」 | 坏 JSON 返回可读错误 |
| ⬜ | Day 10 / 07-01 | 学模块和包 | R01「6. 模块」 | 将脚本拆成 2～3 个模块 |
| ⬜ | Day 11 / 07-02 | 学虚拟环境和依赖文件 | R01「12. 虚拟环境和包」 | 建立 venv 和依赖说明 |
| ⬜ | Day 12 / 07-03 | 学类、dataclass 和类型注解 | R01「9. 类」 | 定义 `Contact` 数据模型 |
| ⬜ | Day 13 / 07-04 | 整理 `src/`、`tests/`、README | G19「Step 2」 | 项目目录职责清楚 |
| ⬜ | Day 14 / 07-05 | 周复盘；从空目录按 README 重建环境 | R01；第 5 节模板 | 环境可重复创建 |

## 第 3 周：Git、HTTP 与 API 调用

**本周验收**：能使用 Git 管理项目；能解释并调试 HTTP 请求。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 15 / 07-06 | 学工作区、暂存区和提交 | R02「Git 基础」 | 完成 3 个语义清楚的 commit |
| ⬜ | Day 16 / 07-07 | 学 branch、diff、log 和恢复思路 | R02「Git 分支」；「撤消操作」 | 创建分支并查看 diff |
| ⬜ | Day 17 / 07-08 | 学 HTTP 方法、状态码、header、body | R03「HTTP 概览」 | 画请求/响应结构 |
| ⬜ | Day 18 / 07-09 | 用 Python 请求公开 API | R03；R01「标准库简介」 | 保存成功响应 |
| ⬜ | Day 19 / 07-10 | 处理超时、非 2xx 和坏 JSON | R03「HTTP 状态码」 | 三类失败均有明确错误 |
| ⬜ | Day 20 / 07-11 | 将 API 调用封装成客户端类 | R01「9. 类」 | 业务代码不直接拼请求 |
| ⬜ | Day 21 / 07-12 | 周复盘；写 HTTP 调试清单 | R03；第 5 节模板 | 清单覆盖 URL、状态码、body、超时 |

## 第 4 周：FastAPI、Pydantic 与测试

**本周验收**：完成有校验和测试的最小 Todo API。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 22 / 07-13 | 跑通 FastAPI Hello World 和 Swagger | R04「第一步」 | `/docs` 可调用 |
| ⬜ | Day 23 / 07-14 | 学路径参数、查询参数和请求体 | R04「路径参数」「查询参数」「请求体」 | GET/POST 可调用 |
| ⬜ | Day 24 / 07-15 | 学 Pydantic 模型与字段校验 | R06「Models」「Fields」 | 非法 Todo 被拒绝 |
| ⬜ | Day 25 / 07-16 | 增加 PUT/DELETE 和异常响应 | R04「处理错误」 | 404/422 行为明确 |
| ⬜ | Day 26 / 07-17 | 学 pytest 基本断言和 fixture | R05「Get Started」 | 写 3 个测试 |
| ⬜ | Day 27 / 07-18 | 扩充正常和异常测试 | R05 | 至少 8 个测试通过 |
| ⬜ | Day 28 / 07-19 | 周复盘；整理 API 的目录与 README | G19「最终标准」 | 陌生人可启动 API |

## 第 5 周：LLM API 与结构化输出

**本周验收**：完成可切换 mock/真实模型的 LLM 客户端和结构化信息抽取。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 29 / 07-20 | 理解 message、token、上下文和生成参数 | R07「Quickstart」 | 写 8 张概念卡 |
| ⬜ | Day 30 / 07-21 | 实现 `LLMClient` 和 `MockLLMClient` | R07 | mock 可稳定返回结果 |
| ⬜ | Day 31 / 07-22 | 接入一个真实 provider，密钥用环境变量 | R07 | 真实调用可运行且仓库无密钥 |
| ⬜ | Day 32 / 07-23 | 比较 system/user 消息与参数变化 | R07 | 保存固定输入实验表 |
| ⬜ | Day 33 / 07-24 | 学 Pydantic 结构化输出 | R06；R07 | 输出可解析为模型 |
| ⬜ | Day 34 / 07-25 | 增加非法 JSON 处理、重试和超时 | R06 | 坏输出不会让程序崩溃 |
| ⬜ | Day 35 / 07-26 | 周复盘；写“LLM 客户端为何需要抽象” | G15「L1：模型层」 | 能解释 provider adapter |

## 第 6 周：Agent、Workflow 与 ReAct

**本周验收**：能判断何时使用 workflow 或 agent，并写出最小 ReAct 伪代码。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 36 / 07-27 | 区分 chatbot、workflow、agent、multi-agent | G04「Agent 不等于 Chatbot」；G02 | 画边界表 |
| ⬜ | Day 37 / 07-28 | 学 Agent 最小闭环和组成部分 | G04「最小闭环」「8 个组成部分」 | 不看资料口述闭环 |
| ⬜ | Day 38 / 07-29 | 学什么时候不该用 Agent | G04「什么时候不该用 Agent」；R09 | 写 5 个反例 |
| ⬜ | Day 39 / 07-30 | 学 ReAct 基本模式 | G06「基本模式」 | 写 observe-act-observe 伪代码 |
| ⬜ | Day 40 / 07-31 | 学 ReAct 常见失败模式 | G06「常见失败模式」 | 为每类失败写一个例子 |
| ⬜ | Day 41 / 08-01 | 对比 ReAct 与 Plan-and-Execute | G06「ReAct vs Plan-and-Execute」；G07 | 写选择表 |
| ⬜ | Day 42 / 08-02 | 周复盘；录 3 分钟 Agent 基础讲解 | G04「面试怎么回答」 | 讲解包含边界和失败 |

## 第 7 周：工具设计与最小 Agent Loop

**本周验收**：Agent 可调用 3 个工具，有最大步数和明确停止条件。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 43 / 08-03 | 学 Function Calling 的工具 schema | R08「Function calling」 | 写 `calculator` schema |
| ⬜ | Day 44 / 08-04 | 设计 `search_notes` 和 `write_summary` 工具卡 | G06「Tool Card 很重要」 | 工具描述语义互斥 |
| ⬜ | Day 45 / 08-05 | 实现 Tool Registry 和 dispatch 表 | G15「L3：工具层」 | 新增工具不改核心循环 |
| ⬜ | Day 46 / 08-06 | 解析结构化 tool call 并执行 | R08 | 单次工具调用跑通 |
| ⬜ | Day 47 / 08-07 | 实现最多 5 步的 Agent Loop | G06「最小实现」 | 多步任务可结束 |
| ⬜ | Day 48 / 08-08 | 增加未知工具、参数错误和异常回传 | G06「常见失败模式」 | 三类错误可读 |
| ⬜ | Day 49 / 08-09 | 周复盘；准备 8 条固定任务 | G03「Day 2～3」 | 任务覆盖成功与失败 |

## 第 8 周：Trace、基础 Eval 与最小 Agent 发布

**本周验收**：最小 Agent 有 trace、固定评测、测试和 README。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 50 / 08-10 | 设计 JSONL trace schema | G09「Trace 是评测前提」 | schema 含 step/tool/result/time |
| ⬜ | Day 51 / 08-11 | 每步写 trace，并生成 run id | G15「Observability」 | 一次运行可完整回放 |
| ⬜ | Day 52 / 08-12 | 定义 10 条 eval case | G09「Eval Case 格式」「最小评测集」 | JSONL 可加载 |
| ⬜ | Day 53 / 08-13 | 实现规则评分和成功率统计 | G09「评分方式」 | 自动输出通过率 |
| ⬜ | Day 54 / 08-14 | 分类工具、格式、规划和模型失败 | G09「常见评测陷阱」 | 每个失败有类别 |
| ⬜ | Day 55 / 08-15 | 补核心测试与 README | G19「最终标准」 | 新环境可运行 |
| ⬜ | Day 56 / 08-16 | 阶段复盘；发布最小 Agent v0.1 | G19「简历写法」 | tag、README、eval 报告齐全 |

# 阶段 B：RAG 与 Paper Agent 主项目

## 第 9 周：RAG 基础与文档模型

**本周验收**：能解释 RAG 边界，并将文档切成带来源的 chunk。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 57 / 08-17 | 理解 RAG 全链路 | G10「概述」；G24「RAG 基础」 | 画 RAG 流程图 |
| ⬜ | Day 58 / 08-18 | 写 RAG 能和不能解决的问题 | G24 | 至少 5 条边界 |
| ⬜ | Day 59 / 08-19 | 定义 `Document` 和 `Chunk` | G20「MVP 范围」 | 含 source/page/text |
| ⬜ | Day 60 / 08-20 | 实现 Markdown 加载器 | G10 | 输出统一 Document |
| ⬜ | Day 61 / 08-21 | 实现固定长度切分 | G10 | chunk 保留来源 |
| ⬜ | Day 62 / 08-22 | 实现按标题切分 | G10 | 记录标题层级 |
| ⬜ | Day 63 / 08-23 | 比较两种切分策略并周复盘 | G24「Chunk 相关题」 | 输出对比表 |

## 第 10 周：Embedding、检索与检索评测

**本周验收**：实现 top-k 检索 baseline 和 15 条固定检索 case。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 64 / 08-24 | 理解 embedding、相似度和 top-k | G10；G24 | 用自己的话解释 |
| ⬜ | Day 65 / 08-25 | 接入 embedding 或可复现 mock | G10 | 文档可向量化 |
| ⬜ | Day 66 / 08-26 | 实现向量 top-k 检索 | G10 | 返回 chunk、score、source |
| ⬜ | Day 67 / 08-27 | 保存和重新加载索引 | G10 | 重启后无需重复构建 |
| ⬜ | Day 68 / 08-28 | 写 15 条 query-ground-truth | G09「Eval Case 格式」 | 覆盖简单、改写、无答案 |
| ⬜ | Day 69 / 08-29 | 计算 Recall@k 与 MRR | G09「证据与事实性」 | 自动输出指标 |
| ⬜ | Day 70 / 08-30 | 分析 5 个检索失败并周复盘 | G24 | 每个失败有改进建议 |

## 第 11 周：Hybrid Retrieval 与 Rerank

**本周验收**：比较 dense、关键词、hybrid 和 rerank 的真实指标。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 71 / 08-31 | 理解 lexical 与 dense retrieval | G10；G24 | 写差异表 |
| ⬜ | Day 72 / 09-01 | 实现简单关键词检索 baseline | G10 | 同一 query 可比较 |
| ⬜ | Day 73 / 09-02 | 实现加权或 RRF hybrid | G10 | 权重可配置 |
| ⬜ | Day 74 / 09-03 | 理解 reranker 的输入输出 | G24 | 画两阶段检索 |
| ⬜ | Day 75 / 09-04 | 接入 rerank 或规则替代版 | G10 | 保存重排前后结果 |
| ⬜ | Day 76 / 09-05 | 跑四组固定测试 | G09「核心指标」 | 指标表可复现 |
| ⬜ | Day 77 / 09-06 | 选择 baseline 配置并周复盘 | G19「消融实验」 | 结论只基于数据 |

## 第 12 周：Paper Agent 规格与论文搜索

**本周验收**：完成项目 spec；可从至少两个来源搜索并去重论文。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 78 / 09-07 | 阅读 Paper Agent 蓝图，明确 MVP | G20「为什么值得做」「MVP 范围」 | 写目标用户与非目标 |
| ⬜ | Day 79 / 09-08 | 写 `SPEC.md`：输入、输出、工具、成功标准 | G19「Step 4」 | spec 可测试 |
| ⬜ | Day 80 / 09-09 | 设计 `search_papers` 工具 | G20「核心工具设计」 | 有 schema、限制和错误 |
| ⬜ | Day 81 / 09-10 | 接入 arXiv API | R10 | 返回 5 篇结构化论文 |
| ⬜ | Day 82 / 09-11 | 接入 Semantic Scholar 或 OpenAlex | R11 或 R12 | 第二来源可查询 |
| ⬜ | Day 83 / 09-12 | 实现标题、DOI、arXiv id 去重 | G20 | 重复结果合并 |
| ⬜ | Day 84 / 09-13 | 写搜索工具测试并周复盘 | R05；G20 | 正常、空结果、限流均覆盖 |

## 第 13 周：PDF 获取、解析与证据

**本周验收**：能解析公开 PDF，并保存 paper/page/section/text 证据。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 85 / 09-14 | 学 PyMuPDF 打开文档和读取页面 | R13「Opening a File」 | 打印前两页文本 |
| ⬜ | Day 86 / 09-15 | 定义 PDF 下载边界与缓存 | G20「download_pdf」 | 只处理公开 PDF |
| ⬜ | Day 87 / 09-16 | 实现下载、hash 和本地缓存 | G20 | 重复 URL 不重复下载 |
| ⬜ | Day 88 / 09-17 | 按页提取文本 | R13「Extracting Text」 | 文本保留页码 |
| ⬜ | Day 89 / 09-18 | 定义 `Evidence` 结构 | G20「证据引用」 | 可序列化为 JSONL |
| ⬜ | Day 90 / 09-19 | 将 PDF 切成带证据的 chunk | G10；G20 | 每个 chunk 可回到原页 |
| ⬜ | Day 91 / 09-20 | 人工抽查 10 条证据并周复盘 | G09「证据与事实性」 | 记录准确与错误原因 |

## 第 14 周：论文结构抽取与摘要

**本周验收**：能输出贡献、方法、实验、局限的结构化摘要。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 92 / 09-21 | 设计论文摘要 schema | G20「输出格式」；R06 | 字段和可空规则清楚 |
| ⬜ | Day 93 / 09-22 | 设计 evidence-first prompt | G06「Prompt 结构」 | prompt 要求无证据不下结论 |
| ⬜ | Day 94 / 09-23 | 抽取贡献与方法 | G20「extract_claims」 | 每条 claim 带 evidence id |
| ⬜ | Day 95 / 09-24 | 抽取数据集、指标与实验 | G20 | 不混淆不同指标 |
| ⬜ | Day 96 / 09-25 | 抽取局限与开放问题 | G20 | 缺失时明确标记 |
| ⬜ | Day 97 / 09-26 | 生成单篇 Markdown 笔记 | G20「review.md 结构」 | 输出可读且可追溯 |
| ⬜ | Day 98 / 09-27 | 用 3 篇论文人工核验并周复盘 | G09 | 记录引用准确率 |

## 第 15 周：多论文比较与综述

**本周验收**：输入主题后能输出带引用的多论文比较与短综述。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 99 / 09-28 | 设计论文比较维度 | G20「compare_papers」 | 维度适合任务 |
| ⬜ | Day 100 / 09-29 | 实现对比表生成 | G20「输出格式」 | 表格含来源 |
| ⬜ | Day 101 / 09-30 | 实现搜索→筛选→解析→抽取 | G20「推荐架构」 | 一条 CLI 跑通 |
| ⬜ | Day 102 / 10-01 | 实现 evidence store | G20 | claim 可通过 id 找原文 |
| ⬜ | Day 103 / 10-02 | 实现综合写作步骤 | G20「Synthesis Agent」 | 结论带 paper/page |
| ⬜ | Day 104 / 10-03 | 增加 reviewer 检查缺失引用 | G20「Review Agent」 | 无证据断言被标记 |
| ⬜ | Day 105 / 10-04 | 跑一个完整主题并周复盘 | G20「Milestone 3」 | 生成 review、evidence、trace |

## 第 16 周：Paper Agent Eval

**本周验收**：建立 20 条固定评测和自动报告。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 106 / 10-05 | 区分 component、trajectory、e2e eval | G09「三层评估」 | 每层写 2 个例子 |
| ⬜ | Day 107 / 10-06 | 定义 Paper Agent eval schema | G17「核心抽象」 | case 可配置 |
| ⬜ | Day 108 / 10-07 | 写 8 条主题检索 case | G20「Eval 设计」 | 有 ground truth |
| ⬜ | Day 109 / 10-08 | 写 6 条单篇精读 case | G20 | 有引用要求 |
| ⬜ | Day 110 / 10-09 | 写 6 条失败与安全 case | G20 | 覆盖搜不到、解析失败、付费墙 |
| ⬜ | Day 111 / 10-10 | 实现规则 grader 和结果聚合 | G16「Code-based Grader」 | 自动输出报告 |
| ⬜ | Day 112 / 10-11 | 跑 baseline 并周复盘 | G09「核心指标」 | 保存通过率、延迟、失败类型 |

## 第 17 周：Paper Agent v1 服务化

**本周验收**：Paper Agent 具备 CLI、API、测试、配置和可重复运行的 v1。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 113 / 10-12 | 对照项目蓝图列 v1 缺口 | G20「实现里程碑」 | P0/P1 缺口表 |
| ⬜ | Day 114 / 10-13 | 整理 CLI 参数和输出目录 | G20「输出格式」 | 一条命令执行 |
| ⬜ | Day 115 / 10-14 | 增加 FastAPI 任务入口 | R04 | 可提交并查询任务 |
| ⬜ | Day 116 / 10-15 | 增加配置模型和环境变量模板 | R06 | 配置校验清楚 |
| ⬜ | Day 117 / 10-16 | 补核心单元与集成测试 | R05；G19 | 关键路径有测试 |
| ⬜ | Day 118 / 10-17 | 完善 README 和示例 | G19「最终标准」 | 新环境可运行 |
| ⬜ | Day 119 / 10-18 | 跑全量回归并发布 v1 | G17 | 指标和 tag 齐全 |

# 阶段 C：Context、Memory、状态图与协议

## 第 18 周：Context Engineering

**本周验收**：实现分层 context builder，并用实验说明取舍。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 120 / 10-19 | 区分 Prompt 与 Context Engineering | G11「核心概念」 | 写对比表 |
| ⬜ | Day 121 / 10-20 | 将 context 分为 task/evidence/history/trace | G11「组成部分」 | 画输入顺序 |
| ⬜ | Day 122 / 10-21 | 实现 context builder | G11「长上下文问题」 | 输出结构稳定 |
| ⬜ | Day 123 / 10-22 | 实现工具结果截断和引用保留 | G15「L3」 | 长结果不过载 |
| ⬜ | Day 124 / 10-23 | 实现 history summary | G11「业界实践」 | 摘要保留关键状态 |
| ⬜ | Day 125 / 10-24 | 比较压缩前后成本与质量 | G09「成本与性能」 | 输出实验表 |
| ⬜ | Day 126 / 10-25 | 周复盘；确定项目 context policy | G11「总结」 | 写 ADR |

## 第 19 周：Agent Memory

**本周验收**：实现简单的任务记忆写入、检索、更新和遗忘规则。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 127 / 10-26 | 理解 working/episodic/semantic memory | G12「三层记忆架构」 | 给项目数据分类 |
| ⬜ | Day 128 / 10-27 | 设计什么值得写入 | G12「什么时候存储」 | 写入规则可测试 |
| ⬜ | Day 129 / 10-28 | 用 JSONL/SQLite 保存 episodic memory | G12「自己实现简单 Memory」 | 可写入读取 |
| ⬜ | Day 130 / 10-29 | 实现关键词或向量检索 | G12「如何检索」 | 查询返回来源 |
| ⬜ | Day 131 / 10-30 | 实现更新、去重和冲突处理 | G12「如何更新」 | 相同事实不重复 |
| ⬜ | Day 132 / 10-31 | 设计遗忘和过期策略 | G12「何时遗忘」 | 过期记录不召回 |
| ⬜ | Day 133 / 11-01 | 跑有/无 memory 对照并周复盘 | G09 | 记录质量与成本差异 |

## 第 20 周：LangGraph 与可恢复执行

**本周验收**：Agent 可暂停、保存 checkpoint、恢复和人工确认。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 134 / 11-02 | 学 state、node、edge、conditional edge | R14「Overview」 | 画 Paper Agent 状态图 |
| ⬜ | Day 135 / 11-03 | 实现最小三节点图 | R14「Graph API」 | plan→tool→answer 跑通 |
| ⬜ | Day 136 / 11-04 | 将 Paper Agent 主流程迁入状态图 | R14 | 节点职责清楚 |
| ⬜ | Day 137 / 11-05 | 增加 checkpoint | R14「Persistence」 | 中断后可继续 |
| ⬜ | Day 138 / 11-06 | 增加 retry、fallback 和 max steps | G15「L2：循环层」 | 故障路径可终止 |
| ⬜ | Day 139 / 11-07 | 增加 human-in-the-loop | R14「Interrupts」 | 未确认不执行写操作 |
| ⬜ | Day 140 / 11-08 | 比较手写 loop 与 LangGraph 并周复盘 | G15「学习顺序」 | 写选型 ADR |

## 第 21 周：MCP 与 Skill

**本周验收**：完成一个 MCP Server 和一个可复用 Paper Review Skill。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 141 / 11-09 | 理解 host/client/server 和 MCP 边界 | G13「核心角色」；R15 | 画调用链 |
| ⬜ | Day 142 / 11-10 | 区分 function calling、tool、Skill、MCP | G13「与 Function Calling 的关系」 | 写对比表 |
| ⬜ | Day 143 / 11-11 | 将 `search_papers` 封装为 MCP 工具 | G13「最小实践路线」；R15 | 客户端可发现并调用 |
| ⬜ | Day 144 / 11-12 | 增加 schema、分页、超时和错误 | G13「Server 应该怎么设计」 | 返回不过载 |
| ⬜ | Day 145 / 11-13 | 增加权限与不可信输出标记 | G13「安全风险」 | 权限路径可测试 |
| ⬜ | Day 146 / 11-14 | 写 `paper-review` Skill | G29「Stage 5」 | 含触发、步骤、模板、验收 |
| ⬜ | Day 147 / 11-15 | 新会话复现 Skill 并周复盘 | G19「Step 3」 | smoke test 通过 |

# 阶段 D：Harness、评测、安全与真实环境

## 第 22 周：Agent Harness 重构

**本周验收**：Paper Agent 的模型、循环、工具、状态、记忆和通道边界清楚。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 148 / 11-16 | 理解 Agent = Model + Harness | G15「什么是 Harness」 | 标出现有模块 |
| ⬜ | Day 149 / 11-17 | 抽象 Model Adapter | G15「L1」 | provider 切换不改业务 |
| ⬜ | Day 150 / 11-18 | 抽象 loop、stop 和 budget policy | G15「L2」 | 策略可独立测试 |
| ⬜ | Day 151 / 11-19 | 抽象 Tool Registry 和 permission gate | G15「L3」 | 高风险工具被拦截 |
| ⬜ | Day 152 / 11-20 | 抽象 session、artifact、memory store | G15「L4」 | 三类数据不混在 messages |
| ⬜ | Day 153 / 11-21 | 统一 CLI/API 事件流 | G15「L6」 | 两入口复用同一 core |
| ⬜ | Day 154 / 11-22 | 故障注入并周复盘 | G15「可靠性六件套」 | 超时、坏 JSON、空结果均可处理 |

## 第 23 周：Evaluation Harness

**本周验收**：评测可配置、多次试验、聚合并作为质量门禁。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 155 / 11-23 | 理解 task/trial/grader/transcript/outcome | G17「核心抽象」 | 画组件图 |
| ⬜ | Day 156 / 11-24 | 定义 `EvalCase/Trial/EvalResult` | G17 | schema 支持三层评测 |
| ⬜ | Day 157 / 11-25 | 实现 exact/rule/schema grader | G16「Code-based Grader」 | grader 有单测 |
| ⬜ | Day 158 / 11-26 | 设计 rubric grader 接口 | G16「Model-based Grader」 | 分维度评分 |
| ⬜ | Day 159 / 11-27 | 支持同一 case 多 trial | G16「多次试验」 | 不以单次判断 |
| ⬜ | Day 160 / 11-28 | 实现配置、缓存和结果聚合 | G17 | 一条命令跑整套 eval |
| ⬜ | Day 161 / 11-29 | 建立质量阈值并周复盘 | G17「质量门禁」 | 低于阈值返回失败 |

## 第 24 周：安全、Sandbox 与权限

**本周验收**：项目有威胁模型、最小权限、敏感信息保护和安全评测。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 162 / 11-30 | 学 prompt/tool injection 与数据泄露 | R19；G18 | 写威胁清单 |
| ⬜ | Day 163 / 12-01 | 工具输出视为不可信数据 | G13「不要信任工具输出」 | 恶意文本不变系统指令 |
| ⬜ | Day 164 / 12-02 | 设计 read/write/network/execute 权限 | G15「Permission Tier」 | 默认最小权限 |
| ⬜ | Day 165 / 12-03 | 限制文件工作区和网络 allowlist | G18「实践建议」 | 越界访问被拒绝 |
| ⬜ | Day 166 / 12-04 | 实现密钥环境变量和日志脱敏 | R19 | 仓库与日志无密钥 |
| ⬜ | Day 167 / 12-05 | 写 15 条安全 eval | G09「安全与治理」 | 覆盖注入、越权、泄露 |
| ⬜ | Day 168 / 12-06 | 跑安全评测并阶段复盘 | G18 | 输出通过率和残余风险 |

## 第 25 周：Observability 与可靠性

**本周验收**：一次任务可追踪到每个模型和工具调用，并具备基本可靠性策略。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 169 / 12-07 | 设计 trace/span/event 字段 | G15「Observability」；R20 | 写 telemetry schema |
| ⬜ | Day 170 / 12-08 | 接入结构化日志和 trace id | R20 | 一次任务全链路可关联 |
| ⬜ | Day 171 / 12-09 | 记录 token、延迟、工具耗时和错误 | G09「成本与性能」 | 自动输出指标 |
| ⬜ | Day 172 / 12-10 | 增加 timeout、指数退避和 jitter | G15「可靠性六件套」 | 临时失败可恢复 |
| ⬜ | Day 173 / 12-11 | 增加幂等 key 和重复请求保护 | G15「Idempotency」 | 重试不重复写入 |
| ⬜ | Day 174 / 12-12 | 导出 Prometheus 指标 | R21 | 可查看计数和延迟 |
| ⬜ | Day 175 / 12-13 | 做故障注入报告并周复盘 | G19「Step 5」 | 每类故障有恢复或终止 |

## 第 26 周：Web Agent 次项目

**本周验收**：完成只操作公开网页的 Web Agent MVP 和 10 条任务评测。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 176 / 12-14 | 写 Web Agent 安全边界和 spec | G21「安全边界」「MVP 范围」 | 不含登录、支付、发布 |
| ⬜ | Day 177 / 12-15 | 学 Playwright open、locator、click | R17「Intro」 | 自动打开并点击本地页 |
| ⬜ | Day 178 / 12-16 | 实现结构化 observe | G21「观察层怎么做」 | 不把完整 DOM 塞给模型 |
| ⬜ | Day 179 / 12-17 | 封装 open/observe/click/type/screenshot | G21「核心工具设计」 | 每个动作有前后状态 |
| ⬜ | Day 180 / 12-18 | 实现 planner→executor→verifier | G21「推荐架构」 | 有最大步数 |
| ⬜ | Day 181 / 12-19 | 写 10 条本地或公开网页任务 | G21「Eval 设计」 | 有自动或规则 verifier |
| ⬜ | Day 182 / 12-20 | 跑评测并周复盘 | G21「指标」 | 保存成功率、步骤、截图、trace |

## 第 27 周：Multi-Agent 与 Orchestration

**本周验收**：用数据判断单 Agent 与 multi-agent 的取舍。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 183 / 12-21 | 理解 planner/executor/reviewer/router | G14；G29「Stage 4」 | 写职责边界 |
| ⬜ | Day 184 / 12-22 | 设计 research→write→review 流程 | G14 | 每个角色有 schema |
| ⬜ | Day 185 / 12-23 | 实现单 Agent baseline | G22 | 保存质量、成本、延迟 |
| ⬜ | Day 186 / 12-24 | 实现双角色版本 | G14 | 上下文隔离 |
| ⬜ | Day 187 / 12-25 | 增加最多两轮 review | G14 | 不无限循环 |
| ⬜ | Day 188 / 12-26 | 对比单/多 Agent | G09「成本与性能」 | 输出实验表 |
| ⬜ | Day 189 / 12-27 | 写采用或拒绝 multi-agent ADR | R09；G14 | 结论有数据支持 |

## 第 28 周：Agents SDK 与框架选型

**本周验收**：用一种成熟 SDK 重做小流程，并能解释框架取舍。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 190 / 12-28 | 阅读 Agents SDK 概览和 Quickstart | R16「Overview」「Quickstart」 | 跑通最小 agent |
| ⬜ | Day 191 / 12-29 | 学 agent definition 与 runner | R16「Agent definitions」「Running agents」 | 最小流程可运行 |
| ⬜ | Day 192 / 12-30 | 接入一个 function tool | R16；R08 | 工具调用有类型 |
| ⬜ | Day 193 / 12-31 | 学 guardrails 和 state | R16「Guardrails」「Results and state」 | 写一个输入护栏 |
| ⬜ | Day 194 / 01-01 | 学 handoff/orchestration | R16「Orchestration」 | 跑通一次 handoff |
| ⬜ | Day 195 / 01-02 | 对比手写 loop、LangGraph、Agents SDK | G02「框架怎么选」；R16 | 形成选型矩阵 |
| ⬜ | Day 196 / 01-03 | 阶段复盘；确定作品集技术栈 | G19 | 写最终 ADR |

# 阶段 E：模型基础与 Agent 算法

## 第 29 周：Transformer、Token 与 Embedding

**本周验收**：能解释 token、embedding、position、Q/K/V、attention 和 Transformer Block 的作用。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 197 / 01-04 | 建立 Transformer 全局结构认知 | G30「概述」；R24「Transformer models」 | 画输入到输出的模块图 |
| ⬜ | Day 198 / 01-05 | 理解 token、token id 与 embedding | R24；G30 | 写三者区别和 shape 示例 |
| ⬜ | Day 199 / 01-06 | 学位置编码和序列位置信息 | G30；G33「位置编码」 | 解释为什么需要位置编码 |
| ⬜ | Day 200 / 01-07 | 理解 Q/K/V 和 scaled dot-product attention | G33「Attention 机制核心」；R23 | 用自己的话解释 Q/K/V |
| ⬜ | Day 201 / 01-08 | 理解 multi-head、causal mask | G33「注意力变体」；R23 | 画 mask 前后注意力矩阵 |
| ⬜ | Day 202 / 01-09 | 理解 residual、LayerNorm、FFN | G33「Transformer 完整模块」；G30 | 画一个 Transformer Block |
| ⬜ | Day 203 / 01-10 | 联系 Agent：模型能力、context、embedding 检索的分工 | G11；G15；G30 | 写一页“模型与 Harness 的边界” |

## 第 30 周：Attention 与 Transformer 最小代码

**本周验收**：能用 NumPy/PyTorch 实现并解释 softmax、单头 attention、causal mask 和最小 Transformer Block。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 204 / 01-11 | 复习向量、矩阵乘法和 shape | R22「基础与数组运算」 | 手算一个小矩阵乘法 |
| ⬜ | Day 205 / 01-12 | 手写数值稳定的 softmax | G33「激活函数」；R22 | 极端输入不溢出 |
| ⬜ | Day 206 / 01-13 | 手写单头 scaled dot-product attention | G33「Softmax Attention」 | 测试输出 shape |
| ⬜ | Day 207 / 01-14 | 为 attention 增加 causal mask | G33「Causal Attention」 | 未来位置权重为 0 |
| ⬜ | Day 208 / 01-15 | 理解并实现 multi-head reshape 流程 | G33「Multi-Head Attention」；R23 | 注释每次 shape 变化 |
| ⬜ | Day 209 / 01-16 | 拼装最小 Transformer Block | G33「完整 Block」；R23 | forward 可运行 |
| ⬜ | Day 210 / 01-17 | 脱离资料讲解代码并周复盘 | G30；G33 | 录 8 分钟白板讲解 |

## 第 31 周：SFT、数据与 LoRA

**本周验收**：能判断 Prompt/RAG/SFT 的边界，理解训练样本、labels mask、LoRA/QLoRA，并完成最小 LoRA 代码。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 211 / 01-18 | 对比 Prompt、RAG、SFT 的适用场景 | G31「基础概念篇」 | 完成技术选型表 |
| ⬜ | Day 212 / 01-19 | 理解 SFT 数据格式和 chat template | G31「数据构建篇」；G32「2.1」 | 构造一条训练样本 |
| ⬜ | Day 213 / 01-20 | 理解 input_ids、attention mask、labels=-100 | G32「Labels 掩码设计」 | 标出计算 loss 的 token |
| ⬜ | Day 214 / 01-21 | 理解 LoRA 的 `W'=W+BA`、rank 和 alpha | R29；G31「LoRA、PEFT」 | 画 LoRA 旁路并解释参数量 |
| ⬜ | Day 215 / 01-22 | 手写最小 `LoRALinear` | G33「训练优化技术」 | forward shape 正确 |
| ⬜ | Day 216 / 01-23 | 理解 QLoRA、量化和显存取舍 | G31「技术实施篇」；G32 | 写 LoRA/QLoRA 对比表 |
| ⬜ | Day 217 / 01-24 | 为 Agent tool-use 设计 10 条 SFT 样本并复盘 | G32「Tool Call 掩码策略」 | 数据有 schema 和质量检查 |

## 第 32 周：Post-Training 与 Agent 推理算法

**本周验收**：能区分 PPO、DPO、GRPO，理解 Agent reward，并比较 ReAct、Reflection、Tree Search 的取舍。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 218 / 01-25 | 浏览 SFT→RM→PPO/DPO/GRPO 完整链路 | G32「1.2 完整链路」 | 画 Post-Training 地图 |
| ⬜ | Day 219 / 01-26 | 理解 reward model、preference data 和 reward hacking | G32「强化学习与对齐」 | 写 5 对 chosen/rejected 示例 |
| ⬜ | Day 220 / 01-27 | 对比 PPO、DPO、GRPO 的输入、目标和成本 | G32；R25 | 完成三者对比表 |
| ⬜ | Day 221 / 01-28 | 为 Agent tool-use 设计 outcome/process/safety reward | G34；G09 | 每类 reward 给出可计算示例 |
| ⬜ | Day 222 / 01-29 | 精读 ReAct 的方法与轨迹结构 | R26；G06 | 画 ReAct 算法流程 |
| ⬜ | Day 223 / 01-30 | 对比 Reflexion 与 Tree of Thoughts | R27；R28；G07 | 写适用场景和成本差异 |
| ⬜ | Day 224 / 01-31 | 设计 ReAct vs ReAct+Reflection 小实验并复盘 | G08；G09 | 明确数据、指标、变量和停止条件 |

# 阶段 F：生产化、作品集与求职

## 第 33 周：部署、作品集与简历

**本周验收**：主项目可用 Docker 启动，作品集和一页简历完成。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 225 / 02-01 | 为 Paper Agent 写 Dockerfile | R18「Get Started」 | 镜像可构建 |
| ⬜ | Day 226 / 02-02 | 增加健康检查和配置模板 | R18；G19 | 容器可启动并检查 |
| ⬜ | Day 227 / 02-03 | 跑最终全量 eval 和安全测试 | G17；G18 | 指标报告归档 |
| ⬜ | Day 228 / 02-04 | 完善 README、架构图、限制说明 | G19「最终标准」 | 新读者能理解并运行 |
| ⬜ | Day 229 / 02-05 | 录 3～5 分钟项目 demo | G20「简历表达」 | 视频覆盖价值、架构、评测 |
| ⬜ | Day 230 / 02-06 | 写 Agent 开发与算法两版项目 bullet | G26；G19「简历写法」 | 每条数字可复现 |
| ⬜ | Day 231 / 02-07 | 组织作品集入口并周复盘 | G26 | Paper/Web Agent 链接完整 |

## 第 34 周：面试、投递与下一阶段

**本周验收**：完成两次模拟面试、首批投递和下一阶段计划。

| 状态 | Day / 日期 | 60 分钟安排 | 学习资源 | 当日验收 |
|:---:|:---|:---|:---|:---|
| ⬜ | Day 232 / 02-08 | 准备 30 秒自我介绍和 3 分钟项目介绍 | G28；G19 | 录音并删掉术语堆砌 |
| ⬜ | Day 233 / 02-09 | 回答 Agent、RAG、Harness、Eval 与安全问题 | G23；G24；G25 | 标记薄弱题 |
| ⬜ | Day 234 / 02-10 | 回答 Transformer、LoRA、SFT、DPO/GRPO 问题 | G30～G34 | 回答包含直觉、取舍和项目联系 |
| ⬜ | Day 235 / 02-11 | 模拟面试 1：Agent 开发与项目 | G23；G25 | 按知识、表达、证据评分 |
| ⬜ | Day 236 / 02-12 | 模拟面试 2：模型基础、Agent 算法与系统设计 | G30～G34；G15 | 列 5 个最高优先级缺口 |
| ⬜ | Day 237 / 02-13 | 收集 10 个 JD，定制简历并首批投递 | G27；G29 | 建立岗位/版本/状态台账 |
| ⬜ | Day 238 / 02-14 | 34 周总复盘；制定下一阶段 4 周计划 | 第 5 节模板；G29 | 写成果、缺口、反馈和下步 |

## 5. 每周复盘模板

```markdown
## Week N 周报（YYYY-MM-DD）

- Agent 学习完成：x / 7 天
- Agent 学习投入：x / 7 小时
- 本周最重要产出：
- 已掌握：
- 仍然模糊：
- 最大阻塞：
- 一个失败案例及原因：
- 下周保留：
- 下周删减：
- 是否需要调整未来日期：

说明：LeetCode 式数据结构与算法学习不在本周报统计；模型基础与 Agent 算法属于本计划。
```

## 6. 项目验收清单

### Paper Agent

- [ ] 有明确用户、输入、输出、非目标和成功标准。
- [ ] 能从至少两个来源搜索论文并去重。
- [ ] 能解析公开 PDF，并保留 paper/page/section/text 证据。
- [ ] 每条核心结论带可追溯来源。
- [ ] Agent Loop 有最大步数、错误处理、预算和 trace。
- [ ] 有 20 条以上固定 eval case。
- [ ] 报告成功率、检索指标、成本、延迟和失败类型。
- [ ] 有单元测试、集成测试和固定回归测试。
- [ ] README 能让陌生人从零运行。
- [ ] 有 Docker、架构图、demo、eval report、失败分析和限制说明。

### Web Agent

- [ ] 只操作公开网页或本地测试页。
- [ ] 有结构化观察，不把完整 DOM 直接交给模型。
- [ ] 每个动作保存 URL、页面摘要、截图和 trace。
- [ ] 有最大步数、超时、恢复和安全边界。
- [ ] 有至少 10 条固定任务和结果报告。

## 7. 当前进度仪表盘

| 项目 | 当前值 |
|:---|:---|
| 当前日期 | 2026-06-21 |
| 当前周 / Day | Week 0 / Day 0 |
| Agent 完成天数 | 0 / 238 |
| Agent 累计学习小时 | 0 / 238 |
| 最小 Agent | 未开始 |
| Paper Agent | 未开始 |
| Paper Agent Eval | 0 / 20+ |
| Web Agent | 未开始 |
| Web Agent Eval | 0 / 10+ |
| MCP / Skill | 未开始 |
| 一页简历 | 未开始 |
| 模拟面试 | 0 / 2 |
| 有效投递 | 0 |
| 当前最大阻塞 | 无 |
| 下一步 | 执行 Day 1 |

> LeetCode 式数据结构与算法学习拥有独立计划和统计，不在本仪表盘出现。

## 8. Git 生命周期与同步规则

### 8.1 单一事实来源

- Agent 安排、完成状态、延期、删减、周报和求职进度全部维护在本文件。
- LeetCode 式数据结构与算法学习使用独立计划，不向本文件添加刷题进度或耗时。
- Transformer、Embedding、SFT/LoRA、Post-Training 和 Agent 推理/检索/记忆算法继续由本文件管理。
- 不另建“Agent 最新版计划”；历史通过 Git commit、tag 和 diff 保留。
- 已完成日期不改写历史，只调整尚未开始的任务。

### 8.2 提交约定

| 场景 | commit 示例 |
|:---|:---|
| 完成一天 | `learn(agent-day-001): finish environment setup` |
| 完成一周 | `learn(agent-week-01): review python basics` |
| 调整计划 | `plan(agent-week-12): extend paper search practice` |
| 修正文档 | `docs(plan): fix resource link` |
| 更新求职反馈 | `career: record interview feedback` |

每天通过验收后更新状态和仪表盘，再提交一次。每周复盘后提交周快照。阶段完成可创建 tag。

### 8.3 调整规则

- 单日未完成：标记 `🔁`，放到最近周复盘日处理。
- 连续 3 天未完成：删除可选阅读，不压缩实作和复盘。
- 连续 7 天未完成：暂停新增知识一周，只恢复节奏。
- 计划可以继续延长，不以 34 周为硬截止；优先保证理解和项目质量。
- 中断 7～21 天：保留已完成记录，重排未来日期并提升次版本号。
- 中断超过 21 天或目标岗位变化：重新做能力盘点，建立 v2.0。

## 9. 变更记录

| 版本 | 日期 | 变更 | 原因 |
|:---:|:---:|:---|:---|
| v1.0 | 2026-06-21 | 建立 24 周、168 天初版计划 | 建立 Agent 开发 + 算法求职路线 |
| v1.1 | 2026-06-21 | 将每天投入统一为约 1 小时；为每日任务增加资源；收敛目标 | 用户确认真实时间预算和资源要求 |
| v1.2 | 2026-06-21 | 从计划中移除全部算法练习和模型算法学习；扩展为 30 周、210 天的纯 Agent 专项路线；增加 Web Agent、Harness、安全、可观测性和框架选型深度 | 用户明确算法独立学习且不占 Agent 每日 1 小时，学习周期无需限制在 24 周 |
| v1.3 | 2026-06-21 | 文件重命名为 `personal-ai-agent-34-week-plan.md`；明确仅排除 LeetCode 式通用算法；重新纳入 Transformer、LoRA、SFT、DPO/GRPO 和 Agent 推理算法；扩展为 34 周、238 天 | 用户澄清“算法学习/练习”特指 LeetCode 考察的算法，并要求同步修改文件名 |
