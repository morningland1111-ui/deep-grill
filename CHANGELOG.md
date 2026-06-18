# deep-grill / deep-grill-cn Changelog

## 2026-06-18 — 加入「前提认知」一句，从源头防止 AI 越界为老师 / Add a "going-in stance" line to prevent the AI from drifting into instructor mode

### 问题 / Problem

实际使用中发现一种失败模式：AI 在 grilling 过程中会反复切到"教学"姿态——列学术名词、画框架表格、自动推送解法。这些行为表面上看像"产出价值"，实质是把"我知道更多 fact"误读成"我对用户的处境更有判断力"。用户被反复打断、被装高姿态对话，违背 skill 设计初衷。

In practice, a failure pattern showed up: the AI repeatedly slips into "instructor" mode while grilling — listing academic terms, drawing frameworks, pushing solutions. These behaviors look like "delivering value" but actually conflate "I know more facts" with "I have better judgment about the user's situation." Users end up being lectured at, which contradicts the skill's intent.

### 变更 / Changes

在「概述」中的「核心原则」下方新增**前提认知**一句，从对话开头就 frame AI 的姿态：你可能对用户的处境一无所知；多知道几个 fact 不代表更懂；拷问不是展示知识的舞台。

Added a **Going-in Stance** line right after the Core Principle in the Overview, framing the AI's posture from the start: you may know nothing about the user's situation; knowing more facts doesn't mean understanding more; grilling is not a stage to display knowledge.

### 为什么放在最前面 / Why up front

这是 posture，不是 procedure。如果埋进核心规则列表里，下次 AI 跑 skill 时会把它当成"也要遵守的一条"被稀释。放在概述顶层、跟核心原则并列，它会先 frame 整段会话的姿态——procedure 才能不偏。

This is posture, not procedure. Buried in the rules list, it would get diluted as "one more rule to follow." Placed at the top of the Overview alongside the Core Principle, it frames the posture of the whole session — only then can the procedure stay on track.

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
