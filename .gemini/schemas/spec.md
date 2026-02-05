# Specification Schema

A valid spec MUST follow this exact format:

```markdown
# Spec: [FEATURE_NAME]

## Status
- **State:** DRAFT | APPROVED | IMPLEMENTED | ARCHIVED
- **Created:** YYYY-MM-DD
- **Author:** [who requested]

## Requirements
1. [MUST] Required behavior
2. [SHOULD] Preferred behavior
3. [MAY] Optional behavior

## Technical Design
- **Approach:** How it will be built
- **Files:** List of files to create/modify
- **Dependencies:** External packages or internal modules needed

## Acceptance Criteria
- [ ] Criterion 1
- [ ] Criterion 2

## Edge Cases
- What happens when X?
- What happens when Y?
```

## Rules
1. MUST/SHOULD/MAY follow RFC 2119 semantics
2. Every spec needs at least one acceptance criterion
3. Edge cases section cannot be empty for non-trivial features
