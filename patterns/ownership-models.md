# Pattern: Ownership Models

## Problem
Many AI systems have distributed responsibility and unclear accountability.

## Pattern
Separate ownership into a small number of clear layers:
- release ownership
- runtime monitoring ownership
- incident response ownership
- post-release improvement ownership

## Example model

| Decision area | Accountable | Contributors |
|---|---|---|
| Release decision | Product lead | Engineering, quality |
| Monitoring readiness | Ops lead | Engineering, data |
| Incident disablement | Ops lead | Engineering on-call |
| Policy exception approval | Governance lead | Product, legal |
| Corrective action closure | Product lead | Engineering, ops |

## Anti-pattern
Everyone contributes, but nobody is accountable.
