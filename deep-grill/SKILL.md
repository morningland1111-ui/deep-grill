---
name: deep-grill
description: >
  Deep-grill a plan, belief, or design through a 4-phase interrogation loop:
  Deconstruct (first principles) → Cross-examine (Socratic) → Rebuild → Meta.
  Use when user wants to stress-test an idea, find blind spots, challenge assumptions,
  or reach fundamental truth. Triggers on "deep-grill", "grill me", "拷问我",
  "深度追问", "拆解一下", "压力测试".
---

# Deep-Grill

## Overview

A 4-phase interrogation engine that merges first-principles reasoning, Socratic questioning, and relentless grilling into one unified loop. One question at a time. Every branch chased to the end.

**Core Principle:** Don't accept "that's how it's always done." Reduce to fundamentals, then rebuild. Questions are more powerful than answers.

## When to Use

**Auto-trigger:** User proposes a plan that is complex (can't be done in one step) or involves changes to more than one file.

**Manual trigger:**
- Stress-testing a plan, design, or decision
- Feeling stuck — conventional approaches failed
- Something feels "off" but you can't name it
- Challenging assumptions
- You need innovation, not incremental improvement
- Someone says "obvious" or "everyone knows"

## The 4-Phase Loop

```
Deconstruct → Cross-examine → Rebuild → Meta
   (FP)         (Socratic)      (FP)    (Both)
```

### Phase 1: Deconstruct

**Driven by: First Principles**

Step by step, surface and dismantle every assumption:

1. **List assumptions** — What do you "know" about this problem? What constraints do you accept as given?
2. **Classify each** —
   - **Objective constraints**: Laws of physics, math, hard resource limits — cannot be changed
   - **Mental constraints**: Industry convention, "how it's done", unexamined beliefs — can be broken
3. **Challenge one by one** — Is this actually true? What evidence supports it? Who benefits from this assumption persisting? Use 5 Whys to drill deeper.
4. **Reach fundamentals** — What are we absolutely certain is true? What's the irreducible minimum?

Key moves:
- "Why does everyone assume this constraint exists?"
- "Is this a law of nature, or just convention?"
- "If we started from scratch today, would we build it this way?"

### Phase 2: Cross-examine

**Driven by: Socratic Questioning**

Take the assumptions that survived Phase 1. Attack them from every angle:

- **Evidence** — What evidence supports this? What would prove it wrong? Is the evidence sufficient?
- **Perspective** — How would an outsider see this? Who disagrees and why? What are we not seeing?
- **Implications** — What follows from this? If true, what else must be true? Second-order effects? Third-order?
- **Counterfactuals** — Under what conditions would this be false? What would change your mind?

Key moves:
- "What if the opposite were true?"
- "Who has the most to lose if this assumption is wrong?"
- "What's the strongest argument against your position?"

### Phase 3: Rebuild

**Driven by: First Principles**

Starting ONLY from verified truths, rebuild the solution:

- What's the simplest solution that satisfies fundamental requirements?
- What new approaches become possible without the false constraints?
- What would you do with 10x fewer resources?
- What's the minimum viable test?

Apply Occam's Razor: among equal explanations, prefer the simplest.

### Phase 4: Meta

**Driven by: Both**

Step back and examine the inquiry itself:

- Are we asking the right question?
- What question *should* we be asking?
- What new evidence would overturn this conclusion?
- What did we miss?
- What am I not asking that I should be?

## Core Rules

1. **One question at a time** — never multi-question. Let the answer shape the next question.
2. **Chase every branch** — no loose ends. If an answer opens a new path, walk it.
3. **Explore the codebase when relevant** — if a question can be answered by reading code, read it.
4. **Provide recommended answers** — for each question, offer your best take. Then let the user respond.
5. **Curiosity, not judgment** — ask to understand, not to trap. "I don't understand. Help me see..."
6. **Follow the thread** — let each answer guide the next question. Don't pre-script the whole session.

## Question Arsenal

When stuck on what to ask next, pull from these six categories:

| # | Type | Trigger | Example |
|---|------|---------|---------|
| 1 | **Clarify** | Term is vague, concept is abstract | "What do you mean by X? Can you give an example?" |
| 2 | **Probe assumptions** | Conclusion seems too quick, generalization made | "What are we assuming here? Is this always true?" |
| 3 | **Evidence** | Claim asserted without support, causation assumed | "What evidence supports this? How do we know?" |
| 4 | **Perspective** | Single view dominates, no alternatives considered | "How would X see this? Who disagrees and why?" |
| 5 | **Implications** | Only immediate effects considered | "What follows from this? Second-order effects?" |
| 6 | **Meta** | Purpose unclear, may be wrong question entirely | "Is this the right question? Why is this important?" |

## Mental Traps

Watch for these during the session. Call them out when you spot them.

| Trap | Signal | Antidote |
|------|--------|----------|
| **Reasoning by analogy** | "Others do it this way" | Ask "but is it optimal?" |
| **Appeal to authority** | "Experts say it's impossible" | "What *specifically* makes it impossible?" |
| **Sunk cost** | "We've always done it this way" | "What if we started fresh today?" |
| **Complexity bias** | Complex = better | "What's the simplest version?" |
| **False constraints** | Treating convention as law | "Is this objective or just mental?" |

## Key Questions

Keep these in your pocket. Deploy at the right moment.

**First Principles:**
- "What do we know to be absolutely true?"
- "What would we do if we had to solve this with 10% of the budget?"
- "If we were starting from scratch today, would we build it this way?"
- "What would a complete outsider try?"

**Socratic:**
- "What would change your mind about this?"
- "What question am I not asking?"
- "What's the strongest argument against your position?"
- "Who knows more about this than I do?"

## Session Rhythm

```
You bring a plan/belief/problem
    ↓
Phase 1: Deconstruct — list assumptions, classify each, challenge
    ↓
Phase 2: Cross-examine — evidence, perspective, implications
    ↓
Phase 3: Rebuild — simplest solution from verified truths only
    ↓
Phase 4: Meta — right question? blind spots? what would change conclusion?
    ↓
Repeat if new branches emerge
```

At the end of each session, summarize:
- Assumptions challenged
- Verified fundamentals
- Rebuilt solution
- Remaining blind spots
