# deep-grill / 深度拷问

A Claude Code skill that merges **first-principles reasoning**, **Socratic questioning**, and **relentless grilling** into one 4-phase interrogation loop.

融合**第一性原理**、**苏格拉底式追问**与**穷追到底的拷问节奏**的四阶段追问引擎。

```
Deconstruct → Cross-examine → Rebuild → Meta
   解构    →   交叉审问   →  重建  → 元审视
```

One question at a time. Every branch chased to the end. / 一次只问一个问题。每条分支追到不可再拆为止。

## Skills / 技能

| 技能名 | 语言 | 触发词 |
|--------|------|--------|
| `deep-grill` | English | `deep-grill`, `grill me` |
| `deep-grill-cn` | 中文 | `拷问我`, `深度追问`, `拆解一下`, `压力测试` |

## Auto-trigger / 自动触发

Automatically activates when the user proposes a plan that is complex (can't be done in one step) or involves changes to more than one file.

用户提出复杂方案（至少一步改不完）或涉及不止一个文件改动时自动激活。

## The 4 Phases / 四阶段

| # | Phase / 阶段 | Engine / 引擎 | What it does / 做什么 |
|---|-------------|---------------|----------------------|
| 1 | **Deconstruct / 解构** | First Principles / 第一性原理 | List assumptions, classify objective vs mental constraints, challenge each one / 列出假设，区分客观约束 vs 思维约束，逐一挑战 |
| 2 | **Cross-examine / 交叉审问** | Socratic / 苏格拉底 | Attack surviving assumptions: evidence, perspective, implications, counterfactuals / 对幸存假设追问证据、换视角、推后果、找反例 |
| 3 | **Rebuild / 重建** | First Principles / 第一性原理 | From verified truths only, what's the simplest solution? / 仅从已验证真理出发，最简方案是什么？ |
| 4 | **Meta / 元审视** | Both / 合流 | Right question? Blind spots? What would overturn the conclusion? / 问对问题了吗？盲点？什么会推翻结论？ |

## Installation / 安装

```bash
# Clone
git clone https://github.com/morningland1111-ui/deep-grill.git

# English only / 只要英文
cp -r deep-grill/deep-grill ~/.claude/skills/

# Chinese only / 只要中文
cp -r deep-grill/deep-grill-cn ~/.claude/skills/

# Both / 两个都要
cp -r deep-grill/deep-grill ~/.claude/skills/
cp -r deep-grill/deep-grill-cn ~/.claude/skills/
```

Or via npx / 或用 npx:

```bash
npx skills@latest add morningland1111-ui/deep-grill
```

## Built upon / 借鉴自

This skill synthesizes three existing skills into one unified loop. / 本技能融合了以下三个既有技能：

- [mattpocock/skills — grill-me](https://github.com/mattpocock/skills) — one-question-at-a-time rhythm, chase every branch / 一问一答节奏，穷追分支
- [tjboudreaux/cc-thinking-skills — thinking-first-principles](https://github.com/tjboudreaux/cc-thinking-skills) — assumption decomposition, objective vs mental constraint classification / 假设拆解，客观约束 vs 思维约束分类
- [tjboudreaux/cc-thinking-skills — thinking-socratic](https://github.com/tjboudreaux/cc-thinking-skills) — 6-category question arsenal, cross-examination moves / 六类问题武器库，交叉审问动作

## License / 许可

MIT
