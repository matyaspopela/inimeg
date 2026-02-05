# Plan Artifact Schema

A valid plan MUST follow this exact format:

```markdown
# Plan: [TITLE]

## Context
- **Goal:** One sentence describing the objective
- **Scope:** Files/modules affected
- **Risk:** LOW | MEDIUM | HIGH

## Tasks (@tagged)
- @T1 [Action verb] [specific target] [expected outcome]
- @T2 [Action verb] [specific target] [expected outcome]
- @T3 ...

## Verification
- [ ] How to confirm success
- [ ] What tests to run
```

## Rules
1. Each task tag (@T1, @T2...) must be unique and sequential
2. Tasks must be atomic — one action per task
3. Tasks must be ordered by dependency (T2 cannot depend on T3)
4. No vague language ("improve", "fix", "update") without specifics
