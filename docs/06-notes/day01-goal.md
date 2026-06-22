# Day 1：职业目标与学习边界

> 日期：2026-06-22
>
> 当前基础：AI Agent / 大模型应用零基础
>
> 固定投入：每天约 1 小时 Agent 学习；LeetCode 式数据结构与算法另行安排，不占用这 1 小时。

## 1. 求职目标

### 岗位优先级

1. **Agent 开发工程师 / LLM 应用开发工程师**
2. **RAG 工程师 / Context Engineering 相关岗位**
3. **Agent 算法工程师 / RAG 算法工程师**
4. 大模型算法工程师：作为长期方向，需要继续补充训练、论文和模型算法经历

现阶段以工程落地能力建立求职基本盘，再逐步增加模型基础、检索、记忆、规划和评测实验的算法深度。

## 2. 学习路线

### 主线 A：工程落地，约 60%

- Python、Git、HTTP、FastAPI、测试和 Docker
- Agent Loop、Tool Use、状态管理和错误恢复
- RAG、Context、Memory、MCP 和 LangGraph
- Harness、Evaluation、Observability、安全和部署

### 主线 B：研究与算法，约 25%

- Transformer、Attention、Embedding
- SFT、LoRA、DPO / GRPO 的核心原理
- ReAct、Plan-and-Execute、Reflection、Tree Search
- 检索、排序、Memory 和 Agent trajectory 的对照与消融实验

### 主线 C：求职作品，约 15%，贯穿全程

求职作品不能完全弱化。它不是额外负担，而是把 A、B 两条路线转化为可验证证据：

- Paper Agent 主项目
- Web Agent 次项目
- 固定评测集、失败分析和实验报告
- README、架构图、演示视频和简历表达

前期不为了包装而包装；每完成一个阶段，就同步保留代码、指标和失败案例。后期再集中整理简历与作品集。

## 3. 34 周核心产出

- 一个带工具、trace、权限和评测的最小 Agent
- 一个可运行、可评测、可部署的 Paper Agent 主项目
- 一个受控的 Web Agent 次项目
- 一个 MCP Server 和一个可复用 Skill
- 一套 Agent Evaluation Harness
- 一份 Context / Memory / Multi-Agent 对照实验
- Transformer、LoRA、SFT、DPO / GRPO 等模型基础笔记与最小实现
- 一页简历、项目逐字稿、作品集入口和模拟面试记录

## 4. 明确不做什么

- 不把 LeetCode 刷题计入 Agent 每天 1 小时
- 不一开始同时学习多个 Agent 框架
- 不追求“通用、全自动、什么都能做”的 Agent
- 不进行大规模预训练、分布式训练或完整 RLHF 训练
- 不只看视频和收藏链接；每天必须留下代码、笔记、图或评测结果
- 不为了简历编造指标；所有数字必须能由测试或日志复现

## 5. 学习原则

1. 先做简单 workflow，固定流程不能覆盖任务分支时再引入 Agent。
2. 先手写最小 Agent Loop，再学习 LangGraph、Agents SDK 等框架。
3. Tool、Context、Trace、Eval 和权限边界与 Agent 功能同步设计。
4. 每天只完成一个核心任务，超过 60 分钟则标记返工，不通过熬夜追赶。
5. AI 可以解释、提示和 review，但核心模块至少独立重写一次。
6. 学习成果以“能解释、能运行、能测试、能复盘”为准，而不是以阅读数量为准。

## 6. 阅读队列

### 当前阶段优先阅读

- [AgentGuide 快速开始](../00-getting-started/README.md)
- [Agent 学习地图](../00-getting-started/01-agent-map.md)
- [2026 Agent 求职路线](../05-roadmaps/agent-job-ready-roadmap-2026.md)
- [Building Effective Agents - Anthropic](https://www.anthropic.com/engineering/building-effective-agents)
- [A Practical Guide to Building Agents - OpenAI](https://openai.com/business/guides-and-resources/a-practical-guide-to-building-ai-agents/)

### 到对应阶段再阅读

- [Writing Effective Tools for Agents - Anthropic](https://www.anthropic.com/engineering/writing-tools-for-agents)
- [OpenAI Agents SDK](https://developers.openai.com/api/docs/guides/agents)
- [LangGraph](https://github.com/langchain-ai/langgraph)
- [Model Context Protocol](https://github.com/modelcontextprotocol/modelcontextprotocol)
- [OWASP Top 10 for LLM Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/)

> 这些链接是阅读队列，不是 Day 1 必须全部读完的任务。

## 7. Day 1 验收

- [x] 明确目标岗位和优先级
- [x] 明确每天 1 小时的 Agent 时间边界
- [x] 明确 LeetCode 学习独立安排
- [x] 明确工程、算法与求职作品三条路线的权重
- [x] 明确 34 周核心产出与非目标
- [x] 建立分阶段阅读队列

下一步：执行 Day 2，检查 Python、Git、编辑器和虚拟环境，并保存版本记录。
