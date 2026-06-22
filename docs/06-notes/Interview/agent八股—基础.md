# Agent 八股：基础概念

## 目录

- [Agent 是什么](#agent-是什么)
- [五类系统的区别](#五类系统的区别)
- [分类维度说明](#分类维度说明)
- [什么时候不该使用 Agent](#什么时候不该使用-agent)
- [Agent 的 7 个核心模块](#agent-的-7-个核心模块)
- [单 Agent 与 Multi-Agent 的选择](#单-agent-与-multi-agent-的选择)
- [面试回答模板](#面试回答模板)
- [脱稿自测](#脱稿自测)

## Agent 是什么

Agent 不是一个库名，而是一类系统设计：模型在受控环境中观察状态、选择动作、调用工具、接收反馈，并在达到目标、触发停止条件或需要人类介入时结束当前循环。

最小闭环：

```text
Goal
  -> Observe State
  -> Select Action
  -> Execute Tool
  -> Receive Observation
  -> Update State
  -> Continue or Stop
```

一个系统是否算 Agent，关键不在于是否使用了某个框架，而在于模型是否拥有受约束的动作选择权。

## 五类系统的区别

| 概念 | 核心特征 | 自己的例子 | 什么时候用 |
|:---|:---|:---|:---|
| Chatbot | 单轮或多轮对话，主要输出文本 | 回答 AgentGuide 中的概念问题 | 任务只需要回答，不需要执行动作 |
| Workflow | 执行预先定义的固定步骤，LLM 是其中的组件 | 上传文档后固定执行解析→切分→检索→生成 | 流程稳定、分支有限、成功标准明确 |
| Agent | 模型根据当前状态自主选择下一步动作 | Paper Agent 自主决定继续搜索、读取 PDF 或开始总结 | 任务开放，需要多步探索和动态决策 |
| Multi-Agent | 多个相对独立的 Agent 分工协作 | researcher 搜索、writer 写作、reviewer 检查引用 | 子任务可独立完成，需要上下文隔离或并行 |
| Computer-Use Agent | Agent 通过浏览器、桌面或终端进入真实软件环境 | Web Agent 打开官方文档、点击导航并提取安装命令 | 任务必须操作图形界面或真实软件 |

Anthropic 的核心建议是：从能够解决问题的最简单方案开始。固定 workflow 足够时，不要为了“更智能”而引入 Agent；只有任务分支无法预先穷举时，才逐步增加自主性。

## 分类维度说明

上表中的概念并不完全位于同一维度：

- Chatbot、Workflow、Agent：描述系统具有多大的决策自主权。
- Single-Agent、Multi-Agent：描述决策主体的数量和协作方式。
- Computer-Use Agent、Coding Agent、Research Agent：描述 Agent 所处的环境或任务类型。

因此，Computer-Use Agent 也可以是单 Agent 或 Multi-Agent；Multi-Agent 系统内部也可以同时包含 workflow。

## 什么时候不该使用 Agent

以下情况优先使用普通代码或 workflow：

- 步骤固定并且可以穷举
- 输出必须严格确定、可证明正确
- 延迟、成本或稳定性要求非常严格
- 只有一个简单 API 调用
- 高风险动作无法建立人工确认和权限边界
- 没有固定测试集，无法判断系统是否真的变好

### 例子

需求：用户上传发票后，提取固定字段并写入数据库。

- 如果字段和流程固定：使用 OCR + 结构化抽取 workflow。
- 如果还要自动发现缺失材料、查询多个系统、处理异常并请求人工补充：才考虑 Agent。

判断问题：

> 下一步动作是否能够由开发者提前可靠地写死？

如果答案是“能”，优先 workflow；如果答案是“不能，且需要根据环境反馈动态选择”，再考虑 Agent。

## Agent 的 7 个核心模块

| 模块 | 核心问题 | 常见坑 | Paper Agent 示例 |
|:---|:---|:---|:---|
| Goal | 成功、失败和非目标分别是什么？ | 只有模糊目标，没有验收标准 | 找到相关论文并输出带引用的综述 |
| State | 当前进度、历史和产物存在哪里？ | 只依赖聊天历史 | 保存候选论文、已读论文、证据和草稿 |
| Context | 哪些信息以什么顺序进入模型？ | 把完整 PDF 和日志全部塞入上下文 | 只提供任务、相关证据、最近 trace |
| Tools | 有哪些动作？schema、权限和错误是什么？ | 工具含义重叠，返回过长 | 搜索论文、下载 PDF、解析、读取证据 |
| Loop | 最大步数、停止、重试和恢复如何设计？ | 无限循环或过早停止 | 最多搜索 3 轮，证据足够后停止 |
| Guardrails | 哪些输入不可信？哪些动作需要确认？ | 让模型自行决定安全边界 | 拒绝绕过付费墙，写入前要求确认 |
| Eval | 如何证明任务真的完成？ | 只看演示，没有回归测试 | 检索相关率、引用准确率、幻觉率 |

七个模块之间不是独立的。例如，Goal 决定 Eval；Tools 和 State 决定 Loop 能做什么；Context 决定模型能看到什么；Guardrails 约束 Tools 和 Loop。

## 单 Agent 与 Multi-Agent 的选择

优先使用单 Agent，除非满足以下至少一项：

- 子任务可以相对独立地完成，最后只需要汇总结果
- 不同角色需要明显不同的上下文或工具权限
- 子任务可以并行，且并行收益高于协调成本
- 单 Agent 的职责过宽，导致提示冲突或上下文污染

不适合 Multi-Agent 的信号：

- 各角色需要频繁交换细粒度中间状态
- 任务很短，角色切换成本高于收益
- reviewer 和 writer 无限争论，没有明确停止条件
- 只是给同一个模型换了几个人设，没有职责、schema 和评测差异

### Paper Agent 示例

先实现单 Agent baseline。只有当“搜索、写作、引用检查”三个环节能够独立评测，并且 reviewer 确实提升引用准确率时，才拆成 researcher、writer、reviewer。

## 面试回答模板

### 如何解释 Agent 与 Workflow 的区别

> Workflow 的执行路径主要由开发者预先定义，模型只负责其中的局部步骤；Agent 则让模型在受控动作空间内，根据状态和工具反馈动态选择下一步。我的选择原则是先用 workflow，只有任务分支难以穷举时才引入 Agent，同时必须补上最大步数、trace、权限和 eval。

### 如何解释 Multi-Agent

> Multi-Agent 的价值不是角色越多越强，而是任务分解、上下文隔离和并行执行。只有子任务相对独立、角色工具或上下文差异明显，并且实验能证明收益大于 token、延迟和协调成本时，我才会采用。

### 如何解释一个完整 Agent

回答时依次说明：

1. Goal：要完成什么任务
2. State / Context：模型掌握哪些状态和信息
3. Tools：可以执行哪些动作
4. Loop：如何持续观察与行动
5. Guardrails：如何限制风险
6. Eval：如何证明完成效果

## 脱稿自测

不看笔记，用自己的话回答：

1. Agent 和普通 LLM 调用的本质区别是什么？
2. Workflow 与 Agent 的边界是什么？
3. 为什么 Computer-Use Agent 与 Multi-Agent 不是同一分类维度？
4. 举出两个不应该使用 Agent 的场景。
5. Agent 的 Goal 为什么必须与 Eval 同时设计？
6. Tool schema 设计差会导致哪些失败？
7. Context 与 State 有什么区别？
8. 为什么没有 trace 的 Agent 很难调试？
9. 什么条件下 Multi-Agent 才可能优于单 Agent？
10. 用 Paper Agent 举例说明七个核心模块。

自测标准：

- 能在 2 分钟内回答单个问题
- 至少给出一个自己的项目例子
- 不只背定义，还能说明取舍、失败模式和验证方法
