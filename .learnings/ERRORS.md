# Errors

## [ERR-20260621-001] node-stdin-validation

**Logged**: 2026-06-21T18:10:00+08:00
**Priority**: low
**Status**: resolved
**Area**: tests

### Summary
PowerShell 通过管道向 Node 传递含中文字符的正则时，中文被替换为问号并导致正则语法错误。

### Error

```text
SyntaxError: Invalid regular expression: /??\s+(\d+)?/g: Nothing to repeat
```

### Context
- 使用 Node stdin 脚本统计计划中的“算法 N”条目。
- Windows PowerShell 管道编码改变了脚本中的中文字符。

### Suggested Fix
在 Windows PowerShell 环境中对此类中文文本校验使用 PowerShell 原生 `[regex]`，或避免在 stdin JavaScript 源码中嵌入中文正则。

### Metadata
- Reproducible: yes
- Related Files: docs/05-roadmaps/personal-ai-agent-34-week-plan.md

### Resolution
- **Resolved**: 2026-06-21T18:12:00+08:00
- **Notes**: 改用 PowerShell 原生正则完成校验。

---

## [ERR-20260623-002] apply-patch-large-context

**Logged**: 2026-06-23T11:05:00+08:00
**Priority**: low
**Status**: resolved
**Area**: docs

### Summary
包含多个远距离修改的大补丁因变更记录中的一个术语不一致而整体校验失败。

### Error

```text
apply_patch verification failed: Failed to find expected lines
```

### Context
- 同一补丁同时修改资源索引、多个周计划和变更记录。
- 补丁预期为 `PPO/GRPO`，原文实际为 `DPO/GRPO`。
- 补丁校验失败，目标计划文件未发生部分写入。

### Suggested Fix
对长文档按资源索引、阶段表格和变更记录拆分小补丁；提交前先读取尾部精确文本。

### Metadata
- Reproducible: yes
- Related Files: docs/05-roadmaps/personal-ai-agent-34-week-plan.md
- See Also: ERR-20260623-001

### Resolution
- **Resolved**: 2026-06-23T11:07:00+08:00
- **Notes**: 改用多个小范围补丁，降低单处文本漂移导致整体失败的风险。

---

## [ERR-20260623-001] powershell-foreach-pipeline

**Logged**: 2026-06-23T10:30:00+08:00
**Priority**: low
**Status**: resolved
**Area**: tests

### Summary
PowerShell 中将 `foreach` 语句块直接连接到管道，导致三个仓库的规模统计命令解析失败。

### Error

```text
An empty pipe element is not allowed.
```

### Context
- 尝试使用 `foreach (...) { ... } | Format-Table`。
- PowerShell 语句形式的 `foreach` 不能像表达式一样直接接管道。

### Suggested Fix
先将 `foreach` 输出赋值给数组，再对数组执行 `Format-Table`；或使用 `ForEach-Object` 管道。

### Metadata
- Reproducible: yes
- Related Files: docs/05-roadmaps/personal-ai-agent-34-week-plan.md

### Resolution
- **Resolved**: 2026-06-23T10:32:00+08:00
- **Notes**: 改用数组收集后再格式化输出。

---

## [ERR-20260621-003] powershell-foreach-spacing

**Logged**: 2026-06-21T20:15:00+08:00
**Priority**: low
**Status**: resolved
**Area**: tests

### Summary
为缩短 PowerShell 校验命令而移除关键空格，导致 `foreach` 语句无法解析。

### Error

```text
Missing 'in' after variable in foreach loop.
```

### Context
- 将 `foreach ($m in $rows)` 压缩成了 `foreach($m in$rows)`。
- 三个并行校验命令均在解析阶段失败，未修改任何文件。

### Suggested Fix
复杂 PowerShell 校验脚本保持可读格式，不压缩关键语法空格。

### Metadata
- Reproducible: yes
- Related Files: docs/05-roadmaps/personal-ai-agent-34-week-plan.md

### Resolution
- **Resolved**: 2026-06-21T20:16:00+08:00
- **Notes**: 使用标准 `foreach ($x in $items)` 语法重跑校验。

---

## [ERR-20260621-002] powershell-variable-interpolation

**Logged**: 2026-06-21T19:15:00+08:00
**Priority**: low
**Status**: resolved
**Area**: tests

### Summary
PowerShell 双引号字符串中的 `$day:` 被解析为带作用域的变量名，导致计划日期校验脚本无法运行。

### Error

```text
Variable reference is not valid. ':' was not followed by a valid variable name character.
```

### Context
- 在错误信息中拼接 `"Day $day:$shown/$expected"`。
- PowerShell 将变量名后的冒号解释为作用域语法。

### Suggested Fix
变量后紧接冒号时使用 `${day}:` 或格式化字符串。

### Metadata
- Reproducible: yes
- Related Files: docs/05-roadmaps/personal-ai-agent-34-week-plan.md

### Resolution
- **Resolved**: 2026-06-21T19:16:00+08:00
- **Notes**: 使用 `${day}` 重新执行校验。

---
