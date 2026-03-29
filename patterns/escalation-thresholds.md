# Pattern: Escalation Thresholds

## Problem
Teams say incidents will be escalated, but no one knows exactly when escalation becomes mandatory.

## Pattern
Define escalation thresholds using measurable indicators:
- confidence below threshold
- abnormal output rate above threshold
- complaint count above threshold
- fallback activation rate above threshold
- policy or safety rule violation

## Example threshold table

| Signal | Threshold | Action |
|---|---:|---|
| Low-confidence rate | > 12% over 1 hour | Escalate to product + ops |
| Harmful response category | > 0.5% | Trigger immediate review |
| Fallback invocation rate | > 20% | Hold wider rollout |
| Critical incident | 1 event | Immediate disablement decision |

## Design rule
Escalation thresholds should be:
- observable,
- owned,
- reviewable,
- tied to real actions.
