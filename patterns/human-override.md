# Pattern: Human Override

## Problem
A system allows human intervention on paper, but the human does not have enough authority, speed, or context to reduce risk in practice.

## Forces
- fast-moving operational conditions
- uncertain model outputs
- safety, compliance, or customer-harm concerns
- ambiguity over who can stop or redirect the system

## Pattern
Design a human override path with:
1. explicit trigger conditions,
2. named authorized actors,
3. permitted actions,
4. expected response time,
5. decision logging.

## Minimal design
- Trigger: low confidence, policy violation, abnormal behavior spike, or critical user complaint
- Actor: named operator or accountable lead
- Action: pause, reroute, fallback, disable, or approve continuation
- Evidence: reason for intervention logged with timestamp and context

## Anti-patterns
- "A human can always step in" with no actual tooling
- override exists but requires too many approvals
- no logged reason, so learning is impossible
