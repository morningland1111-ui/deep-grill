# deep-grill / deep-grill-cn Changelog

## 2026-06-07 — v2: FP from phase-locked to injectable mode

### Problem

The old design locked first-principles thinking to Phase 1 (Deconstruct) and Phase 3 (Rebuild), forming a linear pipeline:

```
Deconstruct(FP) → Cross-examine(Socratic) → Rebuild(FP) → Meta
```

In practice, the AI may be reusing unexamined assumptions during Phase 2, Phase 4, or even Phase 3 "Rebuild" — and the old version gave the AI no mechanism to switch back to first principles.

### Changes

| Old | New |
|---|---|
| 4 linear phases, FP exclusive to Phase 1 & 3 | 4 movements as direction, FP injectable at any point |
| "Phase 1: Deconstruct (First Principles)" | "Mode B: First-Principles Deconstruction" — not locked to any phase |
| No switch mechanism | 6 FP injection triggers, AI self-judges |
| Session rhythm diagram: one-way arrows | Mesh structure with loop-backs |
| 5 core rules | 8 — added #7 (Mode B is not a ceremony), #8 (when in doubt, drill deeper) |
| Rebuild movement had no special warning | Rebuild movement explicitly flagged as most prone to Trigger #1 |

### 6 New FP Injection Triggers

1. Rebuilding with old-framework parts
2. Conclusion reached too fast
3. "Obviously" / "everyone knows" appears
4. User says "I don't get it" or "why"
5. AI reuses a conclusion from an earlier phase without re-verifying
6. Socratic rounds produce no progress after 3 attempts
