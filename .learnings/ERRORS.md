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
- Related Files: docs/05-roadmaps/personal-agent-algorithm-24-week-plan.md

### Resolution
- **Resolved**: 2026-06-21T18:12:00+08:00
- **Notes**: 改用 PowerShell 原生正则完成校验。

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
- Related Files: docs/05-roadmaps/personal-agent-algorithm-24-week-plan.md

### Resolution
- **Resolved**: 2026-06-21T19:16:00+08:00
- **Notes**: 使用 `${day}` 重新执行校验。

---
