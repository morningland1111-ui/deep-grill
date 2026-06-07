# deep-grill / deep-grill-cn Changelog

## 2026-06-07 — v2: 第一性原理从"阶段"变成"可注射模式" / FP from phase-locked to injectable mode

### 问题 / Problem

旧版将第一性原理锁定在阶段一（解构）和阶段三（重建），是一个线性流水线。实际会话中，AI 在阶段二、阶段四、甚至阶段三"重建"时，可能正在复用未经审视的假设——而旧版没有给 AI 切回第一性原理的机制。

The old design locked first-principles thinking to Phase 1 (Deconstruct) and Phase 3 (Rebuild), forming a linear pipeline. In practice, the AI may be reusing unexamined assumptions during Phase 2, Phase 4, or even Phase 3 "Rebuild" — and there was no mechanism to switch back to first principles.

### 变更 / Changes

| 旧 (Old) | 新 (New) |
|---|---|
| 4 个线性阶段，FP 专属阶段一和阶段三 | 4 段弧线作为方向，FP 可在任意点注射 |
| "阶段一：解构（第一性原理）" | "模式 B：第一性原理拆解"——不锁在任何阶段 |
| 无切换机制 | 6 个 FP 注射触发条件，AI 自行判断 |
| 对话节奏图是单向箭头 | 网状可回跳结构 |
| 5 条核心规则 | 8 条——新增 #7 & #8 |

### 新增的 6 个 FP 触发条件 / 6 New FP Injection Triggers

1. 拿旧框架的零件拼新东西 / Rebuilding with old-framework parts
2. 结论下得太快 / Conclusion reached too fast
3. "显然""大家都知道"出现 / "Obviously" / "everyone knows" appears
4. 用户说"我没看懂"或"为什么" / User says "I don't get it" or "why"
5. AI 复用了上一阶段的结论而不加验证 / AI reuses a prior conclusion without re-verifying
6. 苏格拉底审问转了三轮没进展 / Socratic rounds produce no progress after 3 attempts
