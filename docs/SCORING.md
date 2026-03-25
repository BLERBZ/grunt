# Grunt Scientific Scoring Framework

## Overview

The Grunt Scoring Framework measures the effectiveness of agent persona templates at eliminating human grunt work. Each template receives a composite score (0.0–1.0) across four dimensions.

## Dimensions

### 1. Grunt Units Eliminated (GUE) — 40% weight

**Definition**: The number of human-hours of grunt work automated per cycle.

**Measurement**: Compare task completion time with agent vs. without agent across a standard 30-day cycle.

**Scoring scale**:
- 0.0–0.3: < 5 hours eliminated/month
- 0.3–0.6: 5–20 hours eliminated/month
- 0.6–0.8: 20–50 hours eliminated/month
- 0.8–1.0: 50+ hours eliminated/month

### 2. Autonomy Rate (AR) — 25% weight

**Definition**: The percentage of tasks completed without human intervention.

**Measurement**: (Fully automated tasks) / (Total tasks attempted)

**Scoring scale**:
- 0.0: All tasks require human intervention
- 0.5: 50% fully automated
- 1.0: 100% fully automated (no human in the loop)

### 3. Error Rate (ER) — 20% weight

**Definition**: Inverse of the error rate per 100 tasks.

**Measurement**: 1 - (errors / 100 tasks). Capped at 1.0.

**Scoring scale**:
- 0.0: > 50 errors per 100 tasks
- 0.5: 5 errors per 100 tasks
- 1.0: 0 errors per 100 tasks

### 4. Iteration Delta (ID) — 15% weight

**Definition**: Improvement in composite score vs. the prior generation.

**Measurement**: (Current GUE score - Prior GUE score). First-generation templates start at 0.5.

**Scoring scale**:
- 0.0: Regression (score decreased)
- 0.5: No change
- 1.0: Significant improvement (≥ 0.2 delta)

## Composite Score Formula

```
Composite = (GUE × 0.40) + (AR × 0.25) + (ER × 0.20) + (ID × 0.15)
```

## Thresholds

| Composite Score | Status | Action |
|----------------|--------|--------|
| ≥ 0.80 | ⭐ Gold | Promoted to Featured Templates |
| 0.60–0.79 | ✅ Pass | Retained for next generation |
| 0.40–0.59 | ⚠️ Review | Flagged for improvement |
| < 0.40 | ❌ Fail | Retired (or returned for major revision) |

## Self-Iteration Rules

1. Templates below threshold are automatically queued for revision
2. Each revision cycle produces a new generation (v1, v2, v3...)
3. A template is retired after 3 consecutive failing generations
4. The top 10% of templates are featured in the README

---

_Last updated: 2026-03-25 by AI CEO (bootstrapping)_
_Owner: Grunt PM_
