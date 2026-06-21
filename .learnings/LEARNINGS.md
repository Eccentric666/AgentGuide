# Learnings

## [LRN-20260621-001] correction

**Logged**: 2026-06-21T18:00:00+08:00
**Priority**: high
**Status**: resolved
**Area**: docs

### Summary
个人学习计划必须先确认真实的每日时间预算，并为每一天提供可直接定位的学习资源。

### Details
首版计划按工作日 2～3 小时、周末 2～6 小时设计，但用户实际每天只能投入约 1 小时，因此任务密度、项目数量和算法题量均不现实。首版每日表格还缺少独立的资源列，部分任务无法直接判断应阅读哪份文档。

### Suggested Action
将计划统一改为每天 60 分钟，压缩目标和每日任务；为 Day 1～168 增加“学习资源”列，使用带链接的资源编号并尽量标明章节。

### Metadata
- Source: user_feedback
- Related Files: docs/05-roadmaps/personal-agent-algorithm-24-week-plan.md
- Tags: learning-plan, time-budget, daily-resources

### Resolution
- **Resolved**: 2026-06-21T18:20:00+08:00
- **Commit/PR**: 6376654c
- **Notes**: 已将计划统一为每天 60 分钟，为 168 天逐日增加资源列，并收敛项目和算法目标。

---

## [LRN-20260621-002] correction

**Logged**: 2026-06-21T19:00:00+08:00
**Priority**: high
**Status**: resolved
**Area**: docs

### Summary
Agent 专项计划不得混入用户另行安排的算法学习，计划周期应由能力目标决定，而不是机械限制为 24 周。

### Details
v1.1 仍将 40 道算法题和 Transformer、LoRA、Post-Training 等模型算法内容计入每天 1 小时。用户明确说明算法练习与算法学习会独立进行，不占 Agent 学习时间；同时学习周期可以适当延长。

### Suggested Action
将文件重构为纯 Agent 专项路线，移除算法练习和模型算法章节；根据 Agent 工程、项目、评测、安全和求职产出重新估算周期，并保持逐日资源和验收。

### Metadata
- Source: user_feedback
- Related Files: docs/05-roadmaps/personal-agent-algorithm-24-week-plan.md
- Tags: scope, agent-only, duration, planning
- See Also: LRN-20260621-001

### Resolution
- **Resolved**: 2026-06-21T19:30:00+08:00
- **Commit/PR**: 505bea9e
- **Notes**: 已移除全部算法练习与模型算法日程，扩展为 30 周、210 天纯 Agent 专项计划。

---
